---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8 モジュール
description: ' [!DNL Adobe Campaign]  モジュールを使用すると、 [!DNL Adobe Campaign]  アカウント内のイベントに基づいて  [!DNL Adobe Workfront Fusion]  シナリオを開始したり、契約書やその他の記録を作成、読み取り、アップデートしたり、設定した条件を使用して記録を検索したり、ドキュメントをアップロードしたりできます。'
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 33488d46a14dae070083f28f56e1347da3944ca0
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 89%

---

# [!DNL Adobe Campaign] モジュール

[!DNL Adobe Campaign] モジュールを使用すると、[!DNL Adobe Campaign v7/v8] アカウント内のイベントに基づいて [!DNL Adobe Workfront Fusion] シナリオを開始したり、記録を作成、読み取り、アップデートしたり、設定した条件を使用して記録を検索したり、カスタム API 呼び出しを実行したりできます。

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
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Adobe Campaign] を [!DNL Adobe Workfront Fusion] に接続

>[!IMPORTANT]
>
>サーバー間接続を作成することを強くお勧めします。 Adobe Campaignは、サーバー間接続のみを受け入れるように API を更新しました。 Campaign のバージョン 8 以降に接続する場合は、 **必須** サーバー間接続を作成します。
>
>Campaign の新しい接続要件について詳しくは、 [Campaign の技術オペレーターのAdobe Developer Console への移行](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) （ Campaign ドキュメント内）を参照してください。

1. 任意の [!DNL Adobe Campaign] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 次のフィールドに入力します。
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection type]</td>
          <td>
            <p>基本接続を作成するか、サーバー間接続を作成するかを選択します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>この接続の名前を入力します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Base URL]</td>
          <td>[!DNL Adobe Campaign] インスタンスへの接続に使用するベース URL を入力します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Username]</td>
          <td>基本的な接続を作成する場合は、Adobe Campaignユーザー名を入力します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Password]</td>
          <td>基本的な接続を作成する場合は、Adobe Campaignのパスワードを入力します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>サーバー間接続を作成する場合は、 [!DNL Adobe] [!UICONTROL クライアント ID]。 これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>サーバー間接続を作成する場合は、 [!DNL Adobe] [!UICONTROL クライアント秘密鍵 ]。 これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 環境 ]</td>
          <td>実稼動環境と非実稼動環境のどちらに接続するかを選択します。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>サービスアカウントと個人アカウントのどちらに接続するかを選択します。
        </tr>
   </tbody>
    </table>
1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。

## [!DNL Adobe Campaign] モジュールとそのフィールド

[!DNL Adobe Campaign] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Campaign] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) におけるモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL レコードを監視]

このスケジュール済みトリガーモジュールは、レコードが変更されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>新しいレコードや更新されたレコード、またはその両方のどれを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>監視するリソースを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>出力に含めるカスタムフィールドごとに、<b>[!UICONTROL Add]</b>をクリックし、カスタムフィールドの名前を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>


### アクション

* [[!UICONTROL レコードを作成]](#create-a-record)
* [[!UICONTROL カスタム API 呼び出しを実行]](#make-a-custom-api-call)
* [[!UICONTROL レコードを削除]](#delete-record)
* [[!UICONTROL アクションを実行]](#perform-an-action)
* [[!UICONTROL レコードの読み取り]](#-read-a-record)
* [[!UICONTROL 登録または登録解除]](#subscribe-or-unsubscribe)
* [[!UICONTROL レコードを更新]](#update-record)

#### [!UICONTROL レコードを作成]

このアクションモジュールは、[!DNL Adobe Campaign] に新しいレコードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>作成する [!DNL Adobe Campaign] レコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>値を設定するフィールドをレコードの作成時に選択して、それらのフィールドの値を入力します。フィールドは、選択したレコードタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> 新しいレコードに追加するカスタムフィールドごとに、「<b>[!UICONTROL Add item]</b>」をクリックし、フィールドの名前と値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出しの実行]

このモジュールは、[!DNL Adobe Campaign] API に対してカスタム API 呼び出しを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続の作成を参照してください。</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>API 呼び出しで実行するアクションを選択します。</p>
      <p>[!UICONTROL Execute query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Get entity if more recent]</p>
      <p>[!UICONTROL Select all]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例えば、 <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion]  が [!UICONTROL x-security] トークンヘッダーを自動的に追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>API 呼び出しの本文コンテンツを、セッション要素を使用せずに XML で追加します。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、[!DNL Adobe Campaign] から 1 つのレコードを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>削除するリソースのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するリソースの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL アクションの実行]

このアクションモジュールは、[!DNL Adobe Campaign] API で、選択されたアクションをオブジェクトに対して実行します。

特定のアクションとフィールドについては、[[!DNL Adobe Campaign]  API ドキュメント](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続の作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>オブジェクトに対して実行するアクションを選択します。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 使用可能なフィールドについては、この記事の<a href="#search" class="MCXref xref" >[!UICONTROL Search]</a>を参照してください。 </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> 使用可能なフィールドについては、この記事の<a href="#search" class="MCXref xref" >[!UICONTROL Search]</a>を参照してください。 </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> 使用可能なフィールドについては、この記事の<a href="#create-a-record" class="MCXref xref" >[!UICONTROL Create a record]</a>を参照してください。 </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> 使用可能なフィールドについては、この記事の<a href="#update-record" class="MCXref xref" >[!UICONTROL Update a record]</a>を参照してください。 </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> 使用可能なフィールドについては、この記事の<a href="#delete-record" class="MCXref xref" >[!UICONTROL Delete a record]</a>を参照してください。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、[!DNL Adobe Campaign] からレコードを読み取ります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>読み取る [!DNL Adobe Campaign] レコードのタイプを選択します。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>読み取るレコードの ID を入力またはマッピングします。</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output] </td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>出力に含めるカスタムフィールドごとに、「<b>[!UICONTROL Add]</b>」をクリックし、カスタムフィールドの名前を入力します。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 登録または登録解除]

このアクションモジュールは、情報サービスにユーザーを登録したり、情報サービスからユーザーの登録を解除したりします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>への接続の作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe or unsubscribe]</td> 
   <td>情報サービスに登録するか、情報サービスから登録を解除するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>登録または登録解除するサービスを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient email address] </td> 
   <td>情報サービスに登録または情報サービスから登録解除するユーザーのメールアドレスを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは、[!DNL Adobe Campaign] 内の 1 つのレコードを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>作成する [!DNL Adobe Campaign] レコードのタイプを選択します。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>更新するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>値を更新するフィールドを選択して、それらのフィールドの値を入力します。フィールドは、選択したレコードタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> 更新するカスタム フィールドごとに、「<b>[!UICONTROL Add item]</b>」をクリックし、フィールドの名前と値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL 検索]

この検索モジュールは、指定された条件に基づいてレコードを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>作成する [!DNL Adobe Campaign] レコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
