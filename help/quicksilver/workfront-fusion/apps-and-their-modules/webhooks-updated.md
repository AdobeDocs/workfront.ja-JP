---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Web フック
description: Web フックは、イベントによってトリガーされる HTTP 呼び出しです。Web フックを使用して、インスタントトリガーモジュールをアクティベートできます。インターネットに接続しており、HTTP リクエストを許可するアプリケーションは、Adobe Workfront Fusion に web フックを送信できます。
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 34d7edb6a3f9cb1e818f6c234a8dda88d01c5fc4
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 99%

---

# Web フック



<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

Web フックは、イベントによってトリガーされる HTTP 呼び出しです。Web フックを使用して、インスタントトリガーモジュールをアクティベートできます。インターネットに接続しており、HTTP リクエストを許可するアプリケーションは、Adobe Workfront Fusion に web フックを送信できます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

&#42;&#42;[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Workfront Fusion] で web フックを使用

>[!NOTE]
>
>サードパーティの web フック（送信 web フック）を呼び出すには、いずれかの HTTP モジュールを使用します。詳しくは、[HTTP モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)を参照してください。

Web フックを使用してアプリを [!DNL Workfront Fusion] に接続するには、次の手順に従います。

1. **[!UICONTROL Web フック]**／**[!UICONTROL カスタム web フック]**&#x200B;インスタントトリガーモジュールを、シナリオに追加します。

1. Web フックフィールドの横にある「**[!UICONTROL 追加]**」をクリックして、新規 web フックの名前を入力します。
1. （オプション）「**[!UICONTROL 詳細設定]**」をクリックします。
1. **[!UICONTROL IP 制限]**&#x200B;フィールドに、モジュールがデータを受け入れることができる IP アドレスのカンマ区切りのリストを入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

Web フックを作成すると、一意の URL が表示されます。これは、web フックがデータを送信するアドレスです。Workfront Fusion は、このアドレスに送信されたデータを検証し、そのデータをシナリオでの処理に渡します。

>[!NOTE]
>
>Web フックを作成したら、一度に複数のシナリオで使用できます。

### Web フックのデータ構造を設定 {#configure-the-webhook-s-data-structure}

受信ペイロードのデータ構造を認識するために、[!DNL Workfront Fusion] は、表示されているアドレスに送信するサンプルデータを解析します。サンプルデータを指定するには、そのサービスまたはアプリを変更して、サービスまたはアプリが web フックを呼び出すようにします。例えば、ファイルを削除できます。

または、次の手順に従って、[!UICONTROL HTTP]／[!UICONTROL リクエストを実行]モジュールを使用してサンプルデータを送信できます。

1. **[!UICONTROL HTTP]**／**[!UICONTROL リクエストを実行]**&#x200B;モジュールを使用して、新しいシナリオを作成します。

1. 次の値を使用してモジュールを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>Web フックの URL を入力します。この URL は、web フックの設定に使用した [!UICONTROL Webhooks] モジュールに含まれています。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method] </td> 
      <td><p>[!UICONTROL POST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td><p> JSON（application/json）</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request content]</td> 
      <td><p>Web フックには生の JSON が必要です。</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. 別のブラウザーのタブまたはウィンドウで、[!UICONTROL Webhooks] モジュールを使用してシナリオを開きます。
1. Webhooks モジュールで、「**[!UICONTROL データ構造を再決定]**」をクリックします。

   Webhooks モジュールから他のモジュールのリンクを解除する必要はありません。

1. [!UICONTROL HTTP] モジュールを使用してシナリオに切り替え、実行します。
1. Webhooks モジュールを使用してシナリオに戻ります。

   「[!UICONTROL 正常に決定されました]」というメッセージは、モジュールがデータ構造を正常に決定したことを意味します。

   ![](assets/successfully-determined-350x175.png)

1. 「**[!UICONTROL OK]**」をクリックして、データ構造を保存します。

   これで、web フックの項目がマッピングパネルに表示され、シナリオの後続モジュールで使用できるようになりました。

## Webhook キュー

Web フックがデータを受け取り、そのデータを期待するアクティブなシナリオがない場合、データはキューに格納されます。シナリオをアクティベートすると、キューで待機しているすべてのバンドルが順番に処理されます。

>[!IMPORTANT]
>
>Web フックのキューは、同じ web フックを使用するシナリオ間で共有されます。いずれかのシナリオが無効な場合、すべての受信データはキューに保持されます。

## サポートされる受信データ形式

[!DNL Workfront Fusion] は、[!UICONTROL クエリ文字列]、[!UICONTROL フォームデータ]、[!UICONTROL JSON] の 3 つの受信データ形式をサポートします。

[!DNL Workfront Fusion] は、選択したデータ構造に対するすべての受信データを検証します。次に、シナリオの設定に応じて、データは処理用のキューに格納されるか、すぐに処理されます。

データのいずれかの部分が検証に合格しない場合、[!DNL Workfront Fusion] は 400 HTTP ステータスコードを返し、HTTP 応答の本文で、受信データが検証チェックに失敗した理由を指定します。受信データの検証が成功した場合、Workfront Fusion は「[!UICONTROL 200 受理]」ステータスを返します。

* [[!UICONTROL クエリ文字列]](#query-string)
* [[!UICONTROL フォームデータ]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL クエリ文字列]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL フォームデータ]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### マルチパートフォームデータ

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

`multipart/form-data` でエンコードされたファイルを受信するには、ネストされたフィールド `name`、`mime`、`data` を含む `collection` タイプのフィールドを使用してデータ構造を設定する必要があります。フィールド `name` は `text` タイプで、アップロードされたファイルの名前が含まれます。`mime` は `text` タイプで、MIME 形式のファイルが含まれます。フィールド `data` は `buffer` タイプで、転送中のファイルのバイナリデータが含まれます。

MIME 形式について詳しくは、[MIME モジュール](../../workfront-fusion/apps-and-their-modules/mime.md)を参照してください。

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>元の JSON にアクセスする場合は、web フックの設定時に JSON パススルーを有効にします。
>
>1. 「**[!UICONTROL 追加]**」をクリックして、新しい web フックを追加します。
>1. 「**[!UICONTROL 詳細設定を表示]**」をクリックします。
>1. 「**[!UICONTROL JSON パススルー]**」をクリックします。
>

## Web フックヘッダー

Web フックのヘッダーにアクセスするには、web フックの設定時に GET リクエストヘッダーを有効にします。

1. 「**[!UICONTROL 追加]**」をクリックして、新しい web フックを追加します。
1. 「**[!UICONTROL 詳細設定を表示]**」をクリックします。
1. 「**[!UICONTROL リクエストヘッダーを取得]**」をクリックします。

`map()` 関数と `get()` 関数を組み合わせて、特定のヘッダー値を抽出することができます。

>[!INFO]
>
>**例：**
>
>以下の例は、`Headers[]` 配列から `authorization` ヘッダーの値を抽出する式を示しています。この式は、抽出された値と指定されたテキストを比較し、一致する場合に web フックのみを渡すフィルターで使用されます。
>
>![](assets/set-up-a-filter-350x169.png)
>
>特定のキーを使用して配列の要素を取得する方法について詳しくは、[Adobe Workfront Fusion でのモジュール間の情報のマッピング](../../workfront-fusion/mapping/map-information-between-modules.md)の記事にある、[指定されたキーを使用した配列の要素のマッピング](../../workfront-fusion/mapping/map-information-between-modules.md#mapping)を参照してください。

## Web フックへの応答

Web フック呼び出しに対するデフォルトの応答は、「受理」というテキストです。応答は、カスタム web フックモジュールの実行中に web フックを呼び出したアプリに返されます。

* [Web フックへの応答のテスト](#test-the-response-to-a-webhook)
* [HTML 応答の例](#html-response-example)
* [リダイレクトの例](#redirect-example)

### Web フックへの応答をテスト

1. **[!UICONTROL カスタム web フック]**&#x200B;モジュールを含めます。
1. モジュールに新しい web フックを追加します。
1. Web フックの URL をクリップボードにコピーします。
1. シナリオを実行します。

   [!UICONTROL カスタム web フック]モジュールの稲妻アイコンが回転する点に変わります。これは、モジュールが web フック呼び出しを待機していることを示しています。

1. 新しいブラウザーウィンドウを開き、コピーした URL をアドレスバーにペーストして、**[!UICONTROL Enter]** キーを押します。

   [!UICONTROL カスタム web フック]モジュールがトリガーされ、ブラウザーに新しいページが表示されます。

Web フックの応答をカスタマイズする場合は、web フックの応答モジュールを使用します。

モジュールの設定には、[!UICONTROL ステータス]および[!UICONTROL 本文]の 2 つのフィールドが含まれます。

* [!UICONTROL ステータス]フィールドには、成功の 2xx（OK の `200` など）、リダイレクトの 3xx（一時リダイレクトの `307` など）、4xx のクライアントエラー（例えば、無効なリクエストの `400`）などの HTTP 応答ステータスコードが含まれます。

* [!UICONTROL 本文]フィールドには、web フックの呼び出しで受け入れられるすべてが含まれます。シンプルなテキスト、HTML、XML、JSON などが含まれます。

  >[!TIP]
  >
  >`Content-Type` ヘッダーを対応する MIME タイプに設定することをお勧めします。プレーンテキストの場合は `text/plain`、HTMLの場合は `text/html`、JSON の場合は `application/json`、XML の場合は `application/xml` などです。MIME タイプについて詳しくは、[MIME モジュール](../../workfront-fusion/apps-and-their-modules/mime.md)を参照してください。

応答の送信のタイムアウトは 40 秒です。その期間内に応答が利用できない場合、Workfront Fusion は「200 受理」ステータスを返します。

### HTML 応答の例

>[!INFO]
>
>**例：**
>
>[!UICONTROL Web フック応答]モジュールを次のように設定します。
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>2xx 成功 HTTP ステータスコード（例：200）</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Body] </td> 
&gt;   <td> <p>HTML コード</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>キー</strong>：Content-type</li> 
&gt;     <li><strong>値</strong>：text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>これにより、web ブラウザーに表示される HTML 応答が生成されます。
>
>![](assets/html-response-350x70.png)

### リダイレクトの例

>[!INFO]
>
>**例：**[!UICONTROL web フック応答]モジュールを次のように設定します。
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL Status] </td> 
&gt;   <td> <p>3xx リダイレクト HTTP ステータスコード（例：303）</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL Custom headers]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL Key]</strong>：場所</li> 
&gt;     <li><strong>[!UICONTROL Value]</strong>：リダイレクト先の URL。</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook の無効化

次のいずれかに該当する場合、Web フックは自動的に非アクティブ化されます。

* Web フックが 6 日以上どのシナリオにも接続されていない
* Web フックが、非アクティブなシナリオ（非アクティブになってから 30 日を超えたシナリオ）でのみ使用される。

非アクティブ化された web フックは、いかなるシナリオにも接続されておらず、非アクティブ状態となって 30 日が経過した場合、自動的に削除され、登録解除されます。


## トラブルシューティング

### マッピングパネルに項目がありません

[!UICONTROL Web フック]／[!UICONTROL カスタム web フック]モジュールに続くモジュールの設定でマッピングパネルに一部の項目が欠落している場合は、**[!UICONTROL Web フック]／[!UICONTROL カスタム web フック]**&#x200B;モジュールを選択して設定を開き、「**[!UICONTROL データ構造を再決定]**」をクリックします。

![](assets/redetermine-data-structure-btn-350x195.png)

次に、この記事の [web フックのデータ構造の設定](#configure-the-webhook-s-data-structure)の節で説明されている手順に従います。
