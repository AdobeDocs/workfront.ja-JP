---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: イベント登録メッセージのフィルタリング
description: イベント登録メッセージのフィルタリング
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 94%

---

# イベント登録メッセージのフィルタリング

ビジネスに必要なイベント登録メッセージのみをフィルタリングして処理するのに役立つ、中間の処理コンポーネントを構築できます。

イベント登録について詳しくは、[Event Subscription API](../../wf-api/general/event-subs-api.md) を参照してください。

## イベントメッセージのフィルタリング

この節には、イベント登録メッセージの負荷を軽減するために実装できるフィルタリングのコードスニペットが含まれています。様々な言語の構文の違いを示すために、これらのスニペットでは、次の言語で記述されたのと同じフィルターのセットを示します。

フィルタリングの例について詳しくは、[https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples) を参照して、各言語の構文の違い、およびAWS SDK とのやり取りの方法を確認できます。これらの例は、AWS Lambdas として記述され、中間フィルタリングおよび処理コンポーネントを使用する一般的な方法です。

次のコードスニペットは、ほとんどデプロイに対応しており、独自の、より複雑な、フィルターおよび処理コンポーネントを記述するのに役立つ出発点として使用できます。

### Java

Java での次の例は、[ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java) で行ったように、プロジェクトのグループ ID に基づいてプロジェクトペイロードをフィルタリングする方法を示しています。

1. 探しているグループ ID を確定し、静的定数として作成します。

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   この例では、handleRequest メソッド（AWS Lambda 標準メソッド名）は、最初のパラメーターとして Map タイプ（イベント登録メッセージコンテンツ）を使用します。\
   2 番目のパラメーターは、現在の Lambda プロキシリクエストのコンテキストです。\
   Context オブジェクトは、Lambda ロガーの取得に使用され、CloudWatchLogs にメッセージを書き込むために使用されます。

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

   newState 形式について詳しくは、[イベント登録用のアウトバウンドメッセージ形式](../../wf-api/api/message-format-event-subs.md)を参照してください。

3. メッセージから「newState」マップを解析した後、オブジェクトのグループ ID が手順 1 で識別したグループ ID と一致していることを確認します。

4. （条件付き）ID が一致&#x200B;**しない**&#x200B;場合は、空の応答が返されるようにメッセージをドロップします。

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
   >空の正常な応答を返すことが重要です。200 レベルの応答以外のすべては、配信失敗と見なされます。

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

   AWS SDK は、別の Lambda を呼び出すために使用され、Lambda は、フィルタリングされたメッセージを目的のエンドポイントに配信します。

   メッセージの配信を別の Lambda に任せる目的は、イベント登録サービスからの配信リクエストのタイムアウトを回避することです。現在、配信の許容タイムアウトは 5 秒に設定されています。この設定で許可されている時間を超えるフィルターがある場合は、リクエストを処理できますが、イベント登録サービスはタイムアウトし、タイムアウト期間内に 200 レベルの応答を受け取るまで再試行ループに陥ります。

   メッセージ配信の管理について詳しくは、[タイムアウトに対応しながらメッセージ配信を改善する](#improving-message-delivery-while-accommodating-timeouts)を参照してください。

### Python

Java と Python の例における主な違いは、Java ではイベント登録メッセージが最初のパラメーターとして受け取られ、Python では、最初のパラメーターが Lambda プロキシ「event」で、AWS Lambda プロキシリクエストに関する情報と共にイベント登録メッセージが含まれます。

Python での次の例は、[projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py) で行ったように、プロジェクトのグループ ID に基づいてプロジェクトペイロードをフィルタリングする方法を示しています。

1. 探しているグループ ID を確定し、静的定数として作成します。

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   最初のパラメーターは Lambda プロキシ「event」です。このプロキシには、イベント登録メッセージと、解析する必要のある追加情報が含まれます。\
   2 番目のパラメーターは、現在の Lambda プロキシリクエストのコンテキストです。\
   この例では、コンテキストオブジェクトは、CloudWatchLogs にメッセージを書き込むために使用される Lambda Logger を取得するために使用されます。

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

   newState 形式について詳しくは、[イベント登録用のアウトバウンドメッセージ形式](../../wf-api/api/message-format-event-subs.md)を参照してください。

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
   >空の正常な応答を返すことが重要です。200 レベルの応答以外のすべては、配信失敗と見なされます。

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

   AWS SDK は、別の Lambda を呼び出すために使用され、Lambda は、フィルタリングされたメッセージを目的のエンドポイントに配信します。

   メッセージの配信を別の Lambda に任せる目的は、イベント登録サービスからの配信リクエストのタイムアウトを回避することです。現在、配信のタイムアウトは 5 秒に設定されています。この設定で許可されている時間を超えるフィルターがある場合は、リクエストを処理できますが、イベント登録サービスはタイムアウトし、タイムアウト期間内に 200 レベルの応答を受け取るまで再試行ループに陥ります。


### Node.js

プロジェクトグループ ID フィルタリングの Node.js の例は、Java および Python の例と同様に、以下のようになっています。Python の例と同様に、最初のパラメーターは Lambda プロキシイベントで、2 番目のパラメーターは Lambda コンテキストです。

Node.js の次の例は、[projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js) で行われたように、プロジェクトのグループ ID に基づいてプロジェクトペイロードをフィルタリングする方法を示しています。

1. 探しているグループ ID を確定し、静的定数として作成します。

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   最初のパラメーターは Lambda プロキシ「event」です。このプロキシには、イベント登録メッセージと、解析する必要のある追加情報が含まれます。\
   2 番目のパラメーターは、現在の Lambda プロキシリクエストのコンテキストです。\
   この例では、コンテキストオブジェクトは、CloudWatchLogs にメッセージを書き込むために使用される Lambda Logger を取得するために使用されます。

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

   newState 形式について詳しくは、[イベント登録用のアウトバウンドメッセージ形式](../../wf-api/api/message-format-event-subs.md)を参照してください。

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
   >空の正常な応答を返すことが重要です。200 レベルの応答以外のすべては、配信失敗と見なされます。

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

   AWS SDK は、別の Lambda を呼び出すために使用され、Lambda は、フィルタリングされたメッセージを目的のエンドポイントに配信します。\
   メッセージの配信を別の Lambda に任せる目的は、イベント登録サービスからの配信リクエストのタイムアウトを回避することです。現在、配信のタイムアウトは 5 秒に設定されています。この設定で許可されている時間を超えるフィルターがある場合は、リクエストを処理できますが、イベント登録サービスはタイムアウトし、タイムアウト期間内に 200 レベルの応答を受け取るまで再試行ループに陥ります。\
   メッセージ配信の管理について詳しくは、[タイムアウトに対応しながらメッセージ配信を改善](#improving-message-delivery-while-accommodating-timeouts)を参照してください。

## タイムアウトに対応しながらメッセージ配信を改善

イベント登録サービスには、すべての配信リクエストに対して、厳格に **5 秒**&#x200B;のタイムアウトが規定されています。メッセージの配信が許容時間を超えた場合、イベント登録サービスはそのメッセージの再試行サイクルを開始します。

例えば、[イベントメッセージのフィルタリング](#filtering-event-messages)にある例のうちの 1 つに似たプロジェクトグループ ID フィルターを作成し、メッセージが必要かどうかを判断するためのデータベースのルックアップを組み込みます。必要なプロセスおよび Lambda のコールドスタートに必要な時間と合わせたデータベースのルックアップに 5 秒以上かかり、イベント登録サービスがメッセージの配信を再試行する可能性があります。

プロセスの時間のかかる部分を、メッセージが処理して配信するメッセージであるかどうかを判断するロジックから分離することにより、再試行を回避できます。これにより、バックグラウンドでメッセージを処理またはフィルタリングし続けながら、メッセージを承認して、イイベント登録サービスに 200 レベルの応答を返すことができます（例については [Java](#java) の手順 5 を参照）。


処理またはフィルタリングが 5 秒のタイムアウトを超えない場合でも、メッセージのフィルタリングや処理の最初のタッチポイントを、クライアント側の他の処理または配信手順から切り離すと便利です。これにより、イベント登録サービスから宛先へのメッセージの引き渡しが、両者に与える時間とパフォーマンスへの影響を最小限に抑えることができます。

再試行のメカニズムについて詳しくは、[イベント登録の再試行](../../wf-api/api/event-sub-retries.md)を参照してください。

## クラウドレスアーキテクチャでのホストされているフィルターの実装

イベント登録のフィルタリングにクラウドアーキテクチャを利用できない場合でも、[イベントメッセージのフィルタリング](#filtering-event-messages)にある例を、独自にホストされたフィルターや処理コンポーネントを実装する方法のロードマップとして使用できます。

### スタンドアロンサービス向けのフィルタリング例の調整

クラウドレス環境でフィルタリングの例を使用する前に、以下を行う必要があります。

* コンテキストパラメータなど、Lambda 固有の例を省略します。

* 例の中の他の Lambdas の呼び出しを変更し、ホストしている他のフィルターまたは処理コンポーネントに対して追加の非同期 HTTP リクエストを作成します。

* Python と Node.js の例を参照している場合、最初のイベントパラメーターを、Java の例に示されている最初のペイロードパラメーターに置き換えます。[Java](#java) の手順 1 を参照してください。

* Web ベースの API を使用してフィルターまたはプロセッサーをデプロイします。

### イベント登録メッセージの見逃し防止

クラウドレスアーキテクチャでは、イベント登録メッセージの受信を担当するサービスに到達できない場合があります。このようなイベントでは、メッセージは再試行の制限回数を超え、失われ、メッセージ内の情報を取得できなくなる可能性があります。

サービスの起動中に、見逃されたメッセージに含まれていた可能性のある、すべてのリソースの最新の状態を尋ねるクエリを実装することをお勧めします。次の例に示すように、フィルタ条件を使用して、条件に一致するリソースをクエリし、そのリソースの現在の状態を処理できます。

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

リソースをクエリすることで、統合システムに最新バージョンのリソースが含まれていることが確認できます。

### メッセージ配信時の非同期処理の実装

[イベントメッセージのフィルタリング](#filtering-event-messages)セクションのすべての例では、フィルターを適用したメッセージを配信する責任を、別の AWS Lambda に渡します。これは、配信リクエストの 5 秒のタイムアウトを超えないようにするためで、このタイムアウトは、リクエストを発行するイベント登録サービスによって適用されます。

クラウドレスなアーキテクチャでは、AWS SDK が他の AWS Lambdas への非同期呼び出しを許可する方法と同様の非同期処理メカニズムを実装する必要が生じる場合があります。最新のプログラミング言語のほとんどには、非同期処理を処理するサードパーティまたはコアライブラリがあり、この例で実装されている非同期形式の処理を活用できます。
