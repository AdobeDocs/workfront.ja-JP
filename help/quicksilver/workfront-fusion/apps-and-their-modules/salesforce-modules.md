---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Salesforce モジュール
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2806'
ht-degree: 90%

---

# [!DNL Salesforce] モジュール

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [Salesforce モジュール ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

Adobe Workfront Fusion のシナリオでは、[!DNL Salesforce] を使用するワークフローを自動化したり、複数のサードパーティのアプリケーションやサービスに接続したりすることができます。

Salesforce コネクタの紹介ビデオについては、以下を参照してください。

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

>[!NOTE]
>
>* すべての [!DNL Salesforce] エディションで API にアクセスできるわけではありません。詳しくは、[!DNL Salesforce] コミュニティサイトで、 API にアクセスできる [!DNL Salesforce] エディションについての情報を参照してください。
>* [!DNL Salesforce] API から返された特定のエラーについては、[!DNL Salesforce] API ドキュメントを参照してください。[!DNL Salesforce] API のステータスをチェックして、サービス停止の可能性がないか確認することもできます。
>

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
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] の [!DNL Adobe Workfront] プランがある場合、この記事に記載されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] の購入 [!DNL Adobe Workfront] 必要です。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Salesforce] モジュールを使用するには、[!DNL Salesforce] アカウントが必要です。

## Salesforce API の情報

Salesforce コネクタでは、以下を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ベース URL</td> 
   <td> &lbrace;&lbrace;connection.instanceUrl&rbrace;&rbrace;</td>
  </tr> 
  <tr> 
   <td role="rowheader">API バージョン</td> 
   <td> v46.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API タグ</td> 
   <td>v1.15.14</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Salesforce] オブジェクトの検索について

オブジェクトを検索する際には、個々の検索ワードを入力するか、ワイルドカードや演算子を使用してより複雑なクエリを作成できます。

* アスタリスクのワイルドカード（「*」）は、0 文字以上の文字の代わりに使用します。例えば、「Ca*」と検索すると「Ca」で始まる項目が表示されます
* 疑問符のワイルドカード（?）は、1 つの文字の代わりに使用します。例えば「Jo?n」と検索すると、「John」や「Joan」は見つかりますが、「Jon」は表示されません。
* 完全に一致するフレーズを検索するには、引用符演算子（&quot; &quot;）を使用します。例：&quot;Monday meeting&quot;

検索の可能性について詳しくは、SOQL および SOSL に関する [!DNL Salesforce] 開発者向けドキュメントを参照してください。

## [!DNL Salesforce] モジュールとそのフィールド

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

* [[!UICONTROL レコードの監視]](#watch-for-records)
* [[!UICONTROL アウトバウンドメッセージの監視]](#watch-outbound-messages)
* [[!UICONTROL フィールドの監視]](#watch-a-field)

#### [!UICONTROL レコードの監視]

このトリガーモジュールは、オブジェクト内のレコードが作成または更新されたときにシナリオを実行します。このモジュールは、レコードに関連付けられたすべての標準フィールドと、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>モジュールで監視する [!DNL Salesforce] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Fields]</td> 
   <td>モジュールで監視するフィールドを選択します。使用可能なフィールドは、レコードのタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>選択したタイプの新しいレコードのみをシナリオで監視するか、選択したタイプの新しいレコードと、そのタイプのレコードに対するその他すべての変更をシナリオで監視するかを決定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アウトバウンドメッセージを監視]

このトリガーモジュールは、誰かがメッセージを送信したときにシナリオを実行します。このモジュールは、レコードに関連付けられたすべての標準フィールドと、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールには、追加の設定が必要です。

1. [!DNL Salesforce] 設定ページに移動します。

   設定ページにアクセスするには、[!DNL Salesforce] アカウントの右上隅にある「[!UICONTROL 設定]」というラベルのボタンを見つけてクリックします。[!DNL Salesforce] 設定ページから、左側にある「[!UICONTROL クイック検索／検索]」バーを見つけます。「[!UICONTROL ワークフロールール]」を検索します。

1. 「**[!UICONTROL ワークフロールール]**」をクリックします。
1. 表示される[!UICONTROL ワークフロールール]ページで、「**[!UICONTROL 新規ルール]**」をクリックし、ルールを適用するオブジェクトタイプ（「[!UICONTROL 機会]」など）を選択します（商談レコードの更新を監視している場合）。
1. 「**[!UICONTROL 次へ]**」をクリックします。
1. ルール名、評価基準およびルール基準を設定し、**[!UICONTROL 保存]**／**[!UICONTROL 次へ]**&#x200B;をクリックします。

1. 「**[!UICONTROL 完了]**」をクリックします。
1. 新しく作成したワークフロールールで、「**[!UICONTROL 編集]**」をクリックします。
1. **[!UICONTROL ワークフローアクションを追加]**&#x200B;ドロップダウンリストで、「**[!UICONTROL 新規アウトバウンドメッセージ]**」を選択します。

1. 名前、説明、エンドポイント URL、新しいアウトバウンドメッセージに含めるフィールドを指定し、「**[!UICONTROL 保存]**」をクリックします。

   「**[!UICONTROL エンドポイント URL]**」フィールドには、[!DNL Workfront Fusion] の「[!DNL Salesforce] [!UICONTROL  送信メッセージ]」で提供された URL が含まれています。

1. [!UICONTROL アウトバウンドメッセージ]イベント次で始まるシナリオを設定します。

1. 右下にある **&lt;/>** アイコンをクリックし、提供された URL をコピーします。
1. **[!UICONTROL ワークフロールール]**&#x200B;ページに戻り、新しく作成されたルールを探し、「**[!UICONTROL アクティブ化]**」をクリックします。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>送信メッセージの監視に使用する web フックを選択します。Web フックを追加するには、「<strong>[!UICONTROL Add]</strong>」をクリックして、web フックの名前と接続を入力します。</p> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion] への接続の作成 - 基本的な手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>モジュールでアウトバウンドメッセージを監視する [!DNL Salesforce] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fields]</td> 
   <td> <p>モジュールでアウトバウンドメッセージを監視するフィールドを選択します。使用可能なフィールドは、レコードのタイプによって異なります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL フィールドを監視]*

このトリガーモジュールは、[!DNL Salesforce] でフィールドがアップデートされたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>モジュールで監視するフィールドが含まれているレコードのタイプを選択します。[!DNL Salesforce] 設定で [!UICONTROL Field History] がオンになっているレコードタイプを選択する必要があります。詳しくは、[!DNL Salesforce] ドキュメントで<a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">フィールド履歴のトラッキング</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>モジュールで変更を監視するフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すフィールドの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL レコードを読み取り]](#read-a-record)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL 添付ファイル／ドキュメントをアップロード]](#upload-attachmentdocument)
* [[!UICONTROL 添付ファイル／ドキュメントをダウンロード]](#download-attachmentdocument)

#### [!UICONTROL レコードの作成]

このアクションモジュールは、オブジェクトに新しいレコードを作成します。

モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。これにより、モジュールを設定する際にスクロールしなければならないフィールドの数が減ります。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>モジュールで作成する [!DNL Salesforce] レコードのタイプを選択します。フィールドは、「[!UICONTROL Record Type]」フィールドで選択したレコードのタイプに基づいて使用できるようになります。これらのフィールドは [!DNL Salesforce] API に基づいています。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>新しいレコードを作成する際にモジュールで設定するフィールドを選択します。必須フィールドはリストの上部にあります。 </p> <p>選択したフィールドがこのフィールドの下に開きます。これらのフィールドに値を入力できるようになります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、[!DNL Salesforce] の単一オブジェクトからデータを読み取ります。

レコードの ID を指定します。

このモジュールは、レコードの ID および関連するフィールドと共に、接続を介してアクセスされるカスタムフィールドとその値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>モジュールで [action] 読み取る [!DNL Salesforce] レコードのタイプを選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Record Fields]</td>
    <td>モジュールで読み取るフィールドを選択します。少なくとも 1 つのフィールドを選択する必要があります。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>モジュールが読み取るレコードの一意の [!DNL Salesforce] ID を入力またはマッピングします。</p> <p>ID を取得するには、ブラウザーで [!DNL Salesforce] オブジェクトを開いて、URL の末尾のフォワードスラッシュ（/）の後のテキストをコピーします。例： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、オブジェクト内の既存のレコードを削除します。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>モジュールで削除する [!DNL Salesforce] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>モジュールが削除するレコードの一意の [!DNL Salesforce] ID を入力またはマッピングします。</p> <p>ID を取得するには、ブラウザーで [!DNL Salesforce] オブジェクトを開いて、URL の末尾のフォワードスラッシュ（/）の後のテキストをコピーします。例： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールは、[!DNL Salesforce] API に対して認証済みのカスタム呼び出しを実行します。これにより、他の [!DNL Salesforce] モジュールでは不可能なデータフロー自動処理を実現できます。

このモジュールは、次の値を返します。

* **[!UICONTROL ステータスコード]**（数値）：HTTP リクエストの成功または失敗を示します。これらはインターネット上で検索できる標準コードです。
* **[!UICONTROL ヘッダー]**（オブジェクト）：出力本文に関連しない応答／ステータスコードのより詳細なコンテキスト。応答ヘッダーに表示されるすべてのヘッダーが応答ヘッダーではないので、不要なヘッダーも含まれている可能性があります。

  応答ヘッダーは、モジュールの設定時に選択した HTTP リクエストによって異なります。

* **[!UICONTROL 本文]**（オブジェクト）：モジュールの設定時に選択した HTTP リクエストに応じて、一部のデータを受け取る場合があります。このデータ（[!UICONTROL GET] リクエストからのデータなど）は、このオブジェクトに含まれます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p><code> &lt;Instance URL&gt;/services/data/v46.0/</code> への相対パスを入力します。</p> <p>使用可能なエンドポイントの一覧について詳しくは、<a href="https://developer.salesforce.com/docs/atlas.ja-jp.246.0.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API 開発者ガイド</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>例えば <code>{"Content-type":"application/json"}</code> のように、標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。Workfront Fusion は認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。次に例を示します。 <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**&#x200B;次の API 呼び出しは、[!DNL Salesforce] アカウントのすべてのユーザーのリストを返します。
>
>* **URL**：`query`
>
>* **メソッド**：[!UICONTROL GET]
>
>* **クエリ文字列**：
>
>* **キー**：`q`
>
>* **値**：`SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>一致した検索結果は、**[!UICONTROL バンドル]／[!UICONTROL 本文]／[!UICONTROL レコード]**&#x200B;下のモジュールの出力に表示されます。
>
>この例では、6 人のユーザーが返されました。
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 添付ファイル／ドキュメントをアップロード]

このアクションモジュールは、ファイルをアップロードして指定したレコードに添付するか、ドキュメントをアップロードします。

このモジュールは、添付ファイルまたはドキュメントの ID、および関連するフィールドを返すほか、接続がアクセスするカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type of Upload]</td> 
   <td>モジュールが添付ファイルまたはドキュメントのどちらをアップロードするかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>添付ファイルのアップロード先のオブジェクトの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>モジュールがアップロードするファイルを含むフォルダーを選択します。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source File]</td> 
   <td>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイル／ドキュメントをダウンロード]

このアクションモジュールは、レコードからドキュメントまたは添付ファイルをダウンロードします。

レコードの ID および必要なダウンロードのタイプを指定します。

このモジュールは、添付ファイルまたはドキュメントの ID、および関連するフィールドを返すほか、接続がアクセスするカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Connection]</td>
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Type of Download]</td>
    <td> <p>Salesforce からダウンロードするファイルのタイプを指定します。</p> 
     <ul> 
      <li>[!UICONTROL Attachment]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument]（これは、[!DNL Saleforce CRM Content] または [!DNL Salesforce Files] のライブラリにアップロードされたドキュメントです）</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>モジュールがダウンロードするレコードの一意の [!DNL Salesforce] ID を入力またはマッピングします。</p> <p>ID を取得するには、ブラウザーで [!DNL Salesforce] オブジェクトを開き、URL の末尾のフォワードスラッシュ（/）の後のテキストをコピーします。例： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL レコードを更新]

このアクションモジュールは、オブジェクト内のレコードを編集します。

モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。これにより、モジュールを設定する際にスクロールしなければならないフィールドの数が減ります。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>更新するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>モジュールが更新する [!DNL Salesforce] レコードのタイプを選択します。フィールドは、「レコードタイプ」フィールドで選択されたレコードタイプに基づいて使用可能になります。これらのフィールドは [!DNL Salesforce] API に基づいています。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>新しいレコードを作成する際にモジュールで設定するフィールドを選択します。必須フィールドはリストの上部にあります。 </p> <p>選択したフィールドがこのフィールドの下に開きます。これらのフィールドに値を入力できるようになります。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL クエリによる検索]

この検索モジュールは、指定された検索クエリに一致するレコードを [!DNL Salesforce] 内のオブジェクトで検索します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 – 基本手順 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search Type]</td> 
   <td> <p>モジュールで実行する検索のタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Using SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>「シンプル」検索タイプを選択した場合は、モジュールで検索する [!DNL Salesforce] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]／[!UICONTROL SOSL Query]／[!UICONTROL SOQL Query]</td> 
   <td> <p>検索に使用するクエリを入力します。</p> <p>SOSL について詳しくは、[!DNL Salesforce] ドキュメントの <a href="https://developer.salesforce.com/docs/atlas.ja-jp.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language（SOSL）</a>を参照してください。</p> <p>SOQL について詳しくは、[!DNL Salesforce] ドキュメントの <a href="https://developer.salesforce.com/docs/atlas.ja-jp.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language（SOQL）</a>を参照してください。</p> <p>メモ：モジュールの出力は、パラメーター <code>RETURNING </code> の値に左右されます。<code>LIMIT</code> を使用する場合、[!DNL Fusion] は「[!UICONTROL Maximal count of records]」フィールドの設定を無視します。制限を設定しない場合、Fusion は [!UICONTROL LIMIT = Maximal count of records] という値を挿入します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal count of records]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 検索]

このアクションモジュールは、指定された条件を満たすすべてのレコードを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL Salesforce] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL  Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td> <p>検索するオブジェクトのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>検索条件となるフィールド、クエリで使用する演算子およびそのフィールドで検索する値を選択します。AND または OR を使用してクエリを結合できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>モジュールで条件に一致するすべてのレコードを返すか、条件に一致する最初のレコードのみを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>シナリオの実行サイクルごとにモジュールが取得するレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
