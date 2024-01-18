---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classicモジュール
description: を使用 [!DNL Adobe Campaign Classic] モジュールを使用する場合は、 [!DNL Adobe Workfront Fusion] シナリオに基づいて [!DNL Adobe Campaign Classic] 契約およびその他のレコードのアカウント、作成、読み取り、更新、設定した条件を使用したレコードの検索、ドキュメントのアップロードを行います。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 455d439ec2a9034043cac2570851ab2f9fecc276
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Adobe Campaign Classic] モジュール

を使用 [!DNL Adobe Campaign Classic] モジュールを使用する場合は、 [!DNL Adobe Workfront Fusion] シナリオに基づいて [!DNL Adobe Campaign Classic] アカウント、レコードの作成、読み取り、更新、設定した条件を使用したレコードの検索、カスタム API 呼び出しの実行を行います。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 接続 [!DNL Adobe Campaign Classic] から [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>サーバー間接続を作成することを強くお勧めします。 Adobe Campaignは、サーバー間接続のみを受け入れるように API を更新しました。 Campaign のバージョン 8 以降に接続する場合は、 **必須** サーバー間接続を作成します。
>
>Campaign の新しい接続要件について詳しくは、 [Campaign の技術オペレーターのAdobe Developer Console への移行](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) （ Campaign ドキュメント内）を参照してください。

1. 任意の [!DNL Adobe Campaign Classic] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 次のフィールドに入力します。
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL 接続タイプ ]</td>
          <td>
            <p>基本接続を作成するか、サーバー間接続を作成するかを選択します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 接続名 ]</td>
          <td>
            <p>この接続の名前を入力します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ベース URL]</td>
          <td>の接続に使用するベース URL を入力します [!DNL Adobe Campaign Classic] インスタンス。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ユーザー名 ]</td>
          <td>基本的な接続を作成する場合は、Adobe Campaignユーザー名を入力します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL パスワード ]</td>
          <td>基本的な接続を作成する場合は、Adobe Campaignのパスワードを入力します。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL クライアント ID]</td>
          <td>サーバー間接続を作成する場合は、 [!DNL Adobe] [!UICONTROL クライアント ID]。 これは、 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
          <td>サーバー間接続を作成する場合は、 [!DNL Adobe] [!UICONTROL クライアント秘密鍵 ]。 これは、 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 環境 ]</td>
          <td>実稼動環境と非実稼動環境のどちらに接続するかを選択します。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL の種類 ]</td>
          <td>サービスアカウントと個人アカウントのどちらに接続するかを選択します。
        </tr>
   </tbody>
    </table>
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Adobe Campaign Classic] モジュールとそのフィールド

設定時に [!DNL Adobe Campaign Classic] モジュール、 [!DNL Workfront Fusion] に、以下のフィールドを示します。 これらと共に、 [!DNL Adobe Campaign Classic] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [であるモジュールから別のモジュールに情報をマッピングします。 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td>新しいレコード、更新されたレコード、またはその両方を監視するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソース ]</td> 
   <td>監視するリソースを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力に含めるフィールド ]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力に含めるカスタムフィールド ]</td> 
   <td>出力に含めるカスタムフィールドごとに、 <b>[!UICONTROL 追加 ]</b> カスタムフィールドの名前を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返される結果の最大数 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>


### アクション

* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL カスタム API 呼び出しをおこなう]](#make-a-custom-api-call)
* [[!UICONTROL レコードの削除]](#delete-record)
* [[!UICONTROL アクションの実行]](#perform-an-action)
* [[!UICONTROL レコードを読み取る]](#-read-a-record)
* [[!UICONTROL 購読または購読解除]](#subscribe-or-unsubscribe)
* [[!UICONTROL レコードの更新]](#update-record)

#### [!UICONTROL レコードの作成]

このアクションモジュールは、に新しいレコードを作成します。 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソース ]</td> 
   <td>次のタイプを選択： [!DNL Adobe Campaign Classic] レコードを作成します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ] </td> 
   <td>レコードの作成時に値を設定するフィールドを選択し、それらのフィールドの値を入力します。 フィールドは、選択したレコードのタイプに応じて異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カスタムフィールド ]</td> 
   <td> 新しいレコードに追加する各カスタムフィールドで、 <b>[!UICONTROL 項目を追加 ]</b> フィールドの名前と値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出しをおこなう]

このモジュールは、 [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アクション ]</td>
      <td><p>API 呼び出しで実行するアクションを選択します。</p>
      <p>[!UICONTROL クエリを実行 ]</p>
      <p>[!UICONTROL 書き込み ]</p>
      <p>[!UICONTROL より新しい場合はエンティティを取得する ]</p>
      <p>[!UICONTROL すべて選択 ]</p>
      <p>[!UICONTROL プッシュイベント ]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p>
        <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] [!UICONTROL x-security] トークンヘッダーを自動的に追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML 本文 ]</td>
   <td> <p>セッション要素を含めずに、XML での API 呼び出しの本文コンテンツを追加します。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、次の場所から 1 つのレコードを削除します： [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソース ]</td> 
   <td>削除するリソースのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>削除するリソースの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL アクションの実行]

このアクションモジュールは、 [!DNL Adobe Campaign Classic] API.

特定のアクションおよびフィールドについて詳しくは、 [[!DNL Adobe Campaign] - API ドキュメント](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アクション ]</td> 
   <td><p>オブジェクトに対して実行するアクションを選択します。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 使用可能なフィールドについては、 <a href="#search" class="MCXref xref" >[!UICONTROL 検索 ]</a> 」を参照してください。 </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> 使用可能なフィールドについては、 <a href="#search" class="MCXref xref" >[!UICONTROL 検索 ]</a> 」を参照してください。 </p></li> 
   <li><p><b>[!UICONTROL 作成 ]</b></p><p> 使用可能なフィールドについては、 <a href="#create-a-record" class="MCXref xref" >[!UICONTROL レコードの作成 ]</a> 」を参照してください。 </p></li>
   <li><p><b>[!UICONTROL 更新 ]</b></p><p> 使用可能なフィールドについては、 <a href="#update-record" class="MCXref xref" >[!UICONTROL レコードの更新 ]</a> 」を参照してください。 </p></li>
   <li><p><b>[!UICONTROL 削除 ]</b></p><p> 使用可能なフィールドについては、 <a href="#delete-record" class="MCXref xref" >[!UICONTROL レコードの削除 ]</a> 」を参照してください。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、次からレコードを読み取ります： [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソース ]</td> 
   <td>次のタイプを選択： [!DNL Adobe Campaign Classic] レコードを読み取ります。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>読み取るレコードのマップの ID を入力します。</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL 出力に含めるフィールド ] </td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力に含めるカスタムフィールド ]</td> 
   <td>出力に含めるカスタムフィールドごとに、 <b>[!UICONTROL 追加 ]</b> カスタムフィールドの名前を入力します。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 購読または購読解除]

このアクションモジュールは、ユーザーを情報サービスに登録または登録解除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 購読または購読解除 ]</td> 
   <td>情報サービスを購読するか、購読解除するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>購読または購読解除するサービスを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 受信者の電子メールアドレス ] </td> 
   <td>情報サービスを購読または購読解除するユーザーの電子メールアドレスを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを更新]

このアクションモジュールは、 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソース ]</td> 
   <td>次のタイプを選択： [!DNL Adobe Campaign Classic] レコードを作成します。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>更新するレコードの ID マップの ID を入力します。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL フィールド ] </td> 
   <td>値を更新するフィールドを選択し、それらのフィールドの値を入力します。 フィールドは、選択したレコードのタイプに応じて異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL カスタムフィールド ]</td> 
   <td> 更新する各カスタムフィールドに対して、 <b>[!UICONTROL 項目を追加 ]</b> フィールドの名前と値を入力またはマッピングします。 </td> 
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
   <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td>への接続を作成する手順については、 [!DNL Adobe Campaign Classic]を参照してください。 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >への接続の作成 [!DNL Adobe Campaign Classic]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソース ]</td> 
   <td>次のタイプを選択： [!DNL Adobe Campaign Classic] レコードを作成します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
