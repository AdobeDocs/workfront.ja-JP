---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: イベント購読メッセージのフィルタリング
description: イベント購読メッセージのフィルタリング
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# イベント購読メッセージのフィルタリング

ビジネスに必要なイベント購読メッセージのみをフィルタリングして処理するのに役立つ、中間の処理コンポーネントを構築できます。

イベントの購読について詳しくは、 [イベント購読 API](../../wf-api/general/event-subs-api.md).

## イベントメッセージのフィルタリング

この節には、イベント購読メッセージの負荷を軽減するために実装できるフィルタリングのコードスニペットが含まれています。  様々な言語の構文の違いを示すために、これらのスニペットでは、次の言語で記述されたのと同じフィルターのセットを示します。

フィルタリングの例については、 [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples)では、各言語の構文の違い、およびAWS SDK とのやり取りの方法を確認できます。これらの例は、AWS Lambdas として記述されています。これは、中間のフィルタリングと処理のコンポーネントを使用する一般的な方法です。

次のコードスニペットは、ほとんどデプロイに対応しており、独自の、より複雑な、フィルターおよび処理コンポーネントを記述するのに役立つ出発点として使用できます。

### Java

Java での次の例は、で行ったように、プロジェクトのグループ ID に基づいてプロジェクトペイロードをフィルタリングする方法を示しています。 [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. 探しているグループ ID を設定し、静的定数として作成します。

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   この例では、handleRequest メソッド (AWS Lambda 標準メソッド名 ) は、最初のパラメーターとして Map 型（イベント購読メッセージコンテンツ）を取ります。\
   2 番目のパラメータは、現在の Lambda プロキシリクエストのコンテキストです。\
   Context オブジェクトは、Lambda ロガーを取得するために使用され、CloudWatchLogs にメッセージを書き込むために使用されます。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. handleRequest メソッドの呼び出し時に、リソースの更新済み状態を表すイベント購読メッセージの「newState」属性を取得します。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   newState 形式について詳しくは、 [イベント購読用のアウトバウンドメッセージ形式](../../wf-api/api/message-format-event-subs.md).

3. メッセージから「newState」マップを解析した後、オブジェクトのグループ ID が手順 1 で識別したグループ ID と一致していることを確認します。

4. （条件付き）ID が **しない** 一致する場合は、空の応答を返すようにメッセージをドロップします。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >空の成功した応答を返すことが重要です。 200 レベルの応答以外のすべては、失敗した配信と見なされます。

5. メッセージを処理します。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK は、別の Lambda を呼び出すために使用されます。Lambda は、フィルタリングされたメッセージを目的のエンドポイントに配信します。

   別の Lambda にメッセージを配信する責任を渡す目的は、イベント配信登録サービスからの配信要求のタイムアウトを回避することです。 現在、配信の許容タイムアウトは 5 秒に設定されています。 この設定で許可されている時間を超えるフィルターがある場合は、リクエストを処理できますが、イベント購読サービスはタイムアウトし、タイムアウト期間内に 200 レベルの応答を受け取るまで再試行ループに陥ります。

   メッセージ配信の管理について詳しくは、 [タイムアウトに対応しながらメッセージ配信を改善する](#improving-message-delivery-while-accommodating-timeouts).

### Python

Java と Python の主な違いは、Java の例ではイベント購読メッセージが最初のパラメータとして受け取られ、Python の例では、最初のパラメータが Lambda プロキシ「event」で、AWS Lambda プロキシリクエストに関する情報と共にイベント購読メッセージが含まれます。

Python での次の例は、で行ったように、プロジェクトのグループ ID に基づいてプロジェクトペイロードをフィルタリングする方法を示しています。  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. 探しているグループ ID を設定し、静的定数として作成します。

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   最初のパラメータは Lambda プロキシ「event」です。このプロキシには、イベント購読メッセージと、解析する必要のある追加情報が含まれます。\
   2 番目のパラメータは、現在の Lambda プロキシリクエストのコンテキストです。\
   この例では、Context オブジェクトを使用して Lambda ロガーを取得し、CloudWatchLogs にメッセージを書き込むために使用します。

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. イベントからのメッセージを解析します。

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. イベント購読メッセージの「newState」属性を取得します。\
   newState 属性は、リソースの更新済み状態を表します。

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   newState 形式について詳しくは、 [イベント購読用のアウトバウンドメッセージ形式](../../wf-api/api/message-format-event-subs.md).

1. メッセージから「newState」マップを解析した後、オブジェクトのグループ ID が手順 1 で識別したグループ ID と一致していることを確認します。

1. （条件付き）ID が一致しない場合、空の応答が返されるようにメッセージをドロップします。

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >空の成功した応答を返すことが重要です。 200 レベルの応答以外のすべては、失敗した配信と見なされます。

1. メッセージを処理します。

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK は、別の Lambda を呼び出すために使用されます。Lambda は、フィルタリングされたメッセージを目的のエンドポイントに配信します。

   別の Lambda にメッセージを配信する責任を渡す目的は、イベント配信登録サービスからの配信要求のタイムアウトを回避することです。 現在、配信のタイムアウトは 5 秒に設定されています。 この設定で許可されている時間を超えるフィルターがある場合は、リクエストを処理できますが、イベント購読サービスはタイムアウトし、タイムアウト期間内に 200 レベルの応答を受け取るまで再試行ループに陥ります。


### Node.js

プロジェクトグループ ID フィルタリングの Node.js の例は、Java および Python の例と同様に、次のようになっています。 Python の例と同様に、最初のパラメータは Lambda プロキシイベントで、2 番目のパラメータは Lambda コンテキストです。

Node.js の次の例は、で行ったように、プロジェクトのグループ ID に基づいてプロジェクトペイロードをフィルタリングする方法を示しています。  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. 探しているグループ ID を設定し、静的定数として作成します。

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   最初のパラメータは Lambda プロキシ「event」です。このプロキシには、イベント購読メッセージと、解析する必要のある追加情報が含まれます。\
   2 番目のパラメータは、現在の Lambda プロキシリクエストのコンテキストです。\
   この例では、Context オブジェクトを使用して Lambda ロガーを取得し、CloudWatchLogs にメッセージを書き込むために使用します。

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. イベントからのメッセージを解析します。

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. イベント購読メッセージの「newState」属性から projectGroupID を取得し、手順 1 で識別したグループのグループ ID と照合します。

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   newState 形式について詳しくは、 [イベント購読用のアウトバウンドメッセージ形式](../../wf-api/api/message-format-event-subs.md).

4. （条件付き）ID が一致しない場合、空の応答が返されるようにメッセージをドロップします。\
   以下に、一致するグループ ID の例を示します。

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >空の成功した応答を返すことが重要です。 200 レベルの応答以外のすべては、失敗した配信と見なされます。

5. メッセージを処理します。

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK は、別の Lambda を呼び出すために使用されます。Lambda は、フィルタリングされたメッセージを目的のエンドポイントに配信します。\
   別の Lambda にメッセージを配信する責任を渡す目的は、イベント配信登録サービスからの配信要求のタイムアウトを回避することです。 現在、配信のタイムアウトは 5 秒に設定されています。 この設定で許可されている時間を超えるフィルターがある場合は、リクエストを処理できますが、イベント購読サービスはタイムアウトし、タイムアウト期間内に 200 レベルの応答を受け取るまで再試行ループに陥ります。\
   メッセージ配信の管理について詳しくは、 [タイムアウトに対応しながらメッセージ配信を改善する](#improving-message-delivery-while-accommodating-timeouts).

## タイムアウトに対応しながらメッセージ配信を改善する

イベントサブスクリプションサービスのタイムアウトは次のとおりです： **5 秒** すべての配信リクエストに対して。 メッセージの配信が許容時間を超えた場合、イベント購読サービスはそのメッセージの再試行サイクルを開始します。

例えば、 [イベントメッセージのフィルタリング](#filtering-event-messages) また、メッセージが必要かどうかを判断するために、データベース参照を含めます。 必要な処理に必要な時間と Lambda がコールドスタートに必要な時間と共に、データベース参照が 5 秒以上かかる可能性があり、Event Subscription サービスがメッセージの配信を再試行する可能性があります。

プロセスの時間のかかる部分と、メッセージが処理および配信するメッセージかどうかを判断するロジックを分けることで、再試行を回避できます。 これにより、バックグラウンドでメッセージを処理またはフィルタリングし続けながら、メッセージを受け入れて、イベント購読サービスに 200 レベルの応答を返すことができます ( 手順 5 ( [Java](#java) 例を示します )。


処理やフィルタリングが 5 秒のタイムアウトを超えなくても、メッセージのフィルタリングや処理の最初のタッチポイントを、クライアント側の他の処理や配信の手順から切り離すと便利です。 これにより、イベント購読サービスから宛先へのメッセージの引き渡しが、両者に与える時間とパフォーマンスへの影響を最小限に抑えることができます。

再試行メカニズムについて詳しくは、 [イベント購読の再試行](../../wf-api/api/event-sub-retries.md).

## クラウドレスアーキテクチャでのホストフィルターの実装

イベント購読のフィルタリングにクラウドアーキテクチャを利用できない場合でも、 [イベントメッセージのフィルタリング](#filtering-event-messages) 独自にホストされたフィルターや処理コンポーネントを実装する方法のロードマップとして。

### スタンドアロンサービスのフィルタリング例の調整

クラウドレス環境でフィルタリングの例を使用する前に、次の手順を実行します。

* Context パラメータなど、Lambda 固有の例を省略します。

* 例の中の他の Lambdas の呼び出しを変更し、ホストする他のフィルターや処理コンポーネントに対して追加の非同期 HTTP 要求を行います。

* Python と Node.js の例を参照している場合、最初のイベントパラメーターを、Java の例に示されている最初のペイロードパラメーターに置き換えてください。 詳しくは、 [Java](#java).

* Web ベースの API を使用してフィルターまたはプロセッサーをデプロイします。

### イベント配信登録ミスメッセージの防止

クラウドレスなアーキテクチャでは、イベント購読メッセージの受信を担当するサービスに到達できない場合があります。 このようなイベントでは、メッセージは再試行制限を超え、失われ、メッセージ内の情報を取得できなくなる可能性があります。

サービスの起動中に、ミスされたメッセージに含まれていた可能性のあるすべてのリソースの最新の状態を尋ねるクエリを実装することをお勧めします。 次の例に示すように、フィルタ条件を使用して、条件に一致するリソースをクエリし、そのリソースの現在の状態を処理できます。

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

リソースを照会することで、統合システムに最新バージョンのリソースが含まれていることを確認できます。

### メッセージ配信時の非同期処理の実装

すべての例 ( [イベントメッセージのフィルタリング](#filtering-event-messages) セクションでは、別のAWS Lambda にフィルターを適用したメッセージを配信する責任を渡します。 これは、配信リクエストの 5 秒のタイムアウトを超えないようにするためです。このタイムアウトは、リクエストを発行するイベント購読サービスによって適用されます。

クラウドレスなアーキテクチャでは、AWS SDK が他のAWS Lambdas への非同期呼び出しを許可する方法と同様の非同期処理メカニズムを実装する必要が生じる場合があります。 最新のプログラミング言語のほとんどには、非同期処理を処理するサードパーティまたはコアライブラリがあり、この例で実装されている非同期形式の処理を活用できます。
