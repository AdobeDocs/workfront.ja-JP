---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Workfront モジュール
description: Adobe Workfront Fusion Adobe Workfront コネクタを使用すると、Workfront 内でのプロセスを自動化できます。Workfront Fusion for Work Automation and Integration ライセンスをお持ちの場合は、それを使用してサードパーティのアプリケーションやサービスに接続することもできます。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 0558f72fb8a7fc52d06adc0421082e20520c0b8f
workflow-type: tm+mt
source-wordcount: '5935'
ht-degree: 91%

---

# [!DNL Adobe Workfront] モジュール

[!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] コネクタを使用して、[!DNL Workfront] 内のプロセスを自動化できます。[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] ライセンスをお持ちの場合は、それを使用してサードパーティのアプリケーションやサービスに接続することもできます。

[!DNL Workfront] コネクタは、組織で使用可能なアクティブなアプリの数に対してカウントされません。すべてのシナリオは、[!DNL Workfront] アプリのみを使用する場合でも、組織の合計シナリオ数にカウントされます。

組織で使用可能なアプリとシナリオについて詳しくは、[[[!DNL Adobe Workfront Fusion]  の組織とチームの組織](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2)](../../workfront-fusion/organizations/organizations-and-teams.md)を参照してください。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## [!DNL Workfront] を [!DNL Workfront Fusion] に接続

[!DNL Workfront] コネクタは、OAuth 2.0 を使用して [!DNL Workfront] に継続します。

[!DNL Workfront] アカウントへの接続を、[!DNL Workfront Fusion] モジュール内から直接作成できます。

1. 任意のAdobe Authenticatorモジュールで、 **追加** 「接続」フィールドの横に表示されます。
1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>新しい接続の名前を入力します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 環境 ]</td>
        <td>
          <p>実稼動環境と非実稼動環境のどちらに接続するかを選択します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>サービスアカウントと個人アカウントのどちらに接続するかを選択します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>[!DNL Workfront] クライアント ID を入力します。これは、Workfrontの「セットアップ」領域の「OAuth2 Applications」領域にあります。 接続先のアプリケーションを開き、クライアント ID を確認します。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>[!DNL Workfront] クライアント ID を入力します。これは、Workfrontの「セットアップ」領域の「OAuth2 Applications」領域にあります。 接続先のアプリケーションを開き、クライアント ID を確認します。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>これはデフォルト値のままにすることもできますし、Workfrontインスタンスの URL を入力した後に <code>/integrations/oauth2</code>. <p>例： <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ホストプレフィックス ]</td>
        <td>ほとんどの場合、この値は <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* SAML ログインボタンが表示されない場合、組織ではシングルサインオン（SSO）が有効になっていません。ユーザー名とパスワードを使用してログインできます。
>   
>   SSO について詳しくは、[シングルサインオンの概要 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)を参照してください。
>   
>* [!DNL Workfront] API への OAuth 2.0 接続は API キーに依存しなくなりました。

## [!DNL Workfront] モジュールとそのフィールド

[!DNL Workfront] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Workfront] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

>[!NOTE]
>
>Workfrontモジュールに最新のフィールドが表示されない場合は、キャッシュの問題が原因である可能性があります。 1 時間待ってから、もう一度お試しください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL イベントを監視]**

このトリガーモジュールは、Workfront で特定のタイプのオブジェクトが追加、更新、または削除された場合に、シナリオをリアルタイムで実行します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

1. 「**Web フック**」ボックスの右側にある「**[!UICONTROL 追加]**」をクリックします。

1. 表示される「**[!UICONTROL フックを追加]**」ボックスで Web フックを設定します。

   このモジュールを設定する際には、次のフィールドが表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>（オプション）Web フックの新しい名前を入力します。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>モジュールで監視する [!DNL Workfront] レコードのタイプを選択します。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>古い状態と新しい状態のどちらを監視するかを選択します。<ul><li><p><b>[!UICONTROL New state]</b></p><p>レコードが指定された値<b>に</b>変化したときにシナリオをトリガーします。</p><p>例えば、状態が [!UICONTROL New State] に設定され、フィルターが [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] に設定されている場合、[!UICONTROL Status] が [!UICONTROL In Progress] に変わると、以前のステータスに関係なく、web フックがシナリオをトリガーします。 </p></li><li><p><b>[!UICONTROL Old state]</b></p><p>レコードが指定された値<b>から</b>変化したときにシナリオをトリガーします。</p><p>例えば、状態が [!UICONTROL Old State] に設定され、フィルターが [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] に設定されている場合、現在 [!UICONTROL In Progress] である [!UICONTROL Status] が別のステータスに変わると、web フックがシナリオをトリガーします。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Events filters]</p> </td> 
      <td> <p>選択した条件を満たすレコードのみを監視するフィルターを設定できます。</p> <p>各フィルターに対して、フィルターを評価するフィールド、演算子、およびフィルターに許可する値を入力します。AND ルールを追加すると、複数のフィルターを使用できます。</p> <p>メモ：既存の [!DNL Workfront] web フックのフィルターは編集できません。[!DNL Workfront] イベントのサブスクリプションに別のフィルターを設定するには、現在の web フックを削除し、新しい web フックを作成します。</p> <p>イベントフィルターについて詳しくは、この記事の <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">[!DNL Workfront] のイベントサブスクリプションフィルター／[!UICONTROL Watch Events] モジュール</a>を参照してください。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>このトリガーモジュールが使用するのと同じコネクターを使用して作成または更新されたイベントを除外するには、このオプションを有効にします。これにより、シナリオが自分自身をトリガーし、無限ループが繰り返されることを防ぐことができます。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p><strong>[!UICONTROL New Records Only]</strong>、<strong>[!UICONTROL Updated Records Only]</strong>、<strong>[!UICONTROL New and Updated Records]</strong>、または <strong>[!DNL Deleted Records Only]</strong> をシナリオで監視するかどうかを選択します。</p> <p>メモ： <strong>[!UICONTROL New and Updated Records]</strong> を選択した場合、web フックの作成により 2 つのイベントサブスクリプションが同じ web フックアドレスに対して作成されます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

Web フックを作成した後、イベントの送信先エンドポイントのアドレスを表示できます。

詳しくは、[!DNL Workfront] ヘルプ記事[イベントサブスクリプション API](../../wf-api/general/event-subs-api.md) の[イベントペイロードの例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads)の節を参照してください。

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL フィールドを監視]**

このトリガーモジュールは、指定したフィールドが更新されるとシナリオを実行します。このモジュールは、指定したフィールドの古い値と新しい値の両方を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>モジュールで監視する [!DNL Workfront] レコードのタイプを選択します。</p> <p>例えば、タスクでレコードフィールドが更新されるたびにシナリオの実行を開始する場合は、[!UICONTROL Task] を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>モジュールで更新を監視するフィールドを選択します。これらのフィールドは、[!DNL Workfront] 管理者が追跡用に設定したフィールドを反映しています。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを監視]**

このトリガーモジュールは、特定のタイプのオブジェクトが追加、更新、またはその両方が行われた場合にシナリオを実行します。このモジュールは、レコードに関連付けられたすべての標準フィールドと、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。出力のモジュールは、各レコードが新規か更新かを示します。

指定した期間に追加および更新されたレコードは、新しいレコードとして返されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p><strong>[!UICONTROL New Records Only]</strong>、<strong>[!UICONTROL Updated Records Only]</strong>、<strong>[!UICONTROL New and Updated Records]</strong> をシナリオで監視するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>（<strong>フィルター</strong>を選択後に表示されます）モジュールで監視する [!DNL Workfront] レコードのタイプを選択します。</p> <p>例えば、新しいプロジェクトが作成されるたびにシナリオを開始するには、「[!UICONTROL Project]」を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optional Filter]</td> 
   <td> <p>（詳細）API コード文字列を入力して、条件を絞り込む追加のパラメーターまたはコードを定義します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++


### アクション

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL オブジェクトの変換]**

このアクションモジュールは、次のいずれかの変換を行います。

* イシューをプロジェクトに変換
* イシューをタスクに変換
* タスクをプロジェクトに変換

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Workfront] の接続を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Object type]</td> 
   <td> <p>変換するオブジェクトのタイプを選択します。これは、変換前のオブジェクトのタイプです。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convert to]</td> 
   <td>変換先のオブジェクトを選択します。これは、変換後のオブジェクトのタイプです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;Object&gt; ID]</td> 
   <td> <p>オブジェクトの ID を入力します。 </p> <p>メモ：オブジェクトの ID を入力する場合は、オブジェクトの名前を入力していき、目的のオブジェクトがリストに表示されたら、それを選択します。そうすると、モジュールが適切な ID をフィールドに入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Template ID]</td> 
   <td> <p>プロジェクトに変換する場合は、プロジェクトに使用するテンプレートの ID を選択します。</p> <p>メモ：オブジェクトの ID を入力する場合は、オブジェクトの名前を入力していき、目的のオブジェクトがリストに表示されたら、それを選択します。そうすると、モジュールが適切な ID をフィールドに入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom forms]</td> 
   <td>新しく変換されたオブジェクトに追加するカスタムフォームを選択し、カスタムフォームのフィールドに値を入力します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Options]</td> 
   <td> <p>オブジェクトの変換時に必要なオプションを有効にします。変換先または変換元のオブジェクトに応じて、オプションを使用できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL レコードを作成（カスタムフォームを添付）]**

このアクションモジュールで、プロジェクト、タスク、イシューなどのオブジェクトを [!DNL Workfront] に作成し、カスタムフォームを新しいオブジェクトに追加できます。モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

例えば、クライアントが実行する必要のあるタスクの [!DNL Google Sheets] リストに新しい行を追加する際に、このモジュールを使用して [!DNL Workfront] でタスクを作成できます。

このモジュールを設定する際には、次のフィールドが表示されます。

入力フィールドの最小数を指定してください。例えば、イシューを作成する場合は、「プロジェクト ID」フィールドに有効な親プロジェクト ID を指定して、Workfront でイシューの配置先を示す必要があります。マッピングパネルを使用してシナリオ内の別のモジュールからこの情報をマッピングするか、名前を入力してリストから選択し、手動で入力することもできます。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>作成するモジュールの [!DNL Workfront] レコードのタイプを選択します。</p> <p>例えば、プロジェクトを作成する場合は、ドロップダウンリストから「[!UICONTROL Project]」を選択し、プロジェクトに入力されるデータ（シナリオの前のモジュールのもの）にアクセスできることを確認します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td> <p>データ入力に使用するフィールドを選択します。これにより、不要なフィールドをスクロールしなくても、これらのフィールドを使用できます。</p> <p>カスタムフォームのフィールドの場合は、「<b>[!UICONTROL Attach Custom Form]</b>」フィールドを使用します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Attach Custom Form]</td> 
   <td>新しいオブジェクトに追加するカスタムフォームを選択し、それらのフィールドに値を入力します。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。そうすると、モジュールが適切な ID をフィールドに入力します。
>* カスタムフィールドまたは[!UICONTROL メモ]オブジェクト（コメントまたは返信）にテキストを入力する際、「[!UICONTROL メモテキスト]」フィールドで HTML タグを使用して、太字や斜体などのリッチテキストを作成できます。
>
>  更新のリッチテキストについて詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)の[作業項目に更新を追加](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)を参照してください。
>

+++

+++ **[!UICONTROL レコードを作成]**

このアクションモジュールは、Workfront でプロジェクト、タスク、イシューなどのオブジェクトを作成します。モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

例えば、完了させることが必要なタスクの Google Sheets リストにクライアントが新しい行を追加する場合、このモジュールを使用して [!DNL Workfront] でタスクを作成します。

このモジュールを設定する際には、次のフィールドが表示されます。

入力フィールドの最小数を指定してください。例えば、イシューを作成する場合は、「プロジェクト ID」フィールドに有効な親プロジェクト ID を指定して、Workfront でイシューの配置先を示す必要があります。マッピングパネルを使用してシナリオ内の別のモジュールからこの情報をマッピングするか、名前を入力してリストから選択し、手動で入力することもできます。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>作成するモジュールの [!DNL Workfront] レコードのタイプを選択します。</p> <p>例えば、プロジェクトを作成する場合は、ドロップダウンリストから「[!UICONTROL Project]」を選択し、プロジェクトに入力されるデータ（シナリオの前のモジュールのもの）にアクセスできることを確認します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Select fields to map]</td> 
   <td>データ入力に使用するフィールドを選択します。これにより、不要なフィールドをスクロールしなくても、これらのフィールドを使用できます。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。そうすると、モジュールが適切な ID をフィールドに入力します。
>* カスタムフィールドまたは[!UICONTROL メモ]オブジェクト（コメントまたは返信）にテキストを入力する際、「[!UICONTROL メモテキスト]」フィールドで HTML タグを使用して、太字や斜体などのリッチテキストを作成できます。
>
>  更新のリッチテキストについて詳しくは、[作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)の[作業項目に更新を追加](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)を参照してください。
>

+++

+++ **[!UICONTROL カスタム API 呼び出し]**

このアクションモジュールは、[!DNL Workfront] API に対して認証済みのカスタム呼び出しを実行します。これにより、他の [!DNL Workfront] モジュールで達成できないデータフローの自動化を構築できます。

このモジュールは、次の情報を返します。

* **[!UICONTROL ステータスコード]**（数値）：HTTP リクエストの成功または失敗を示します。これらはインターネット上で検索できる標準コードです。
* **[!UICONTROL ヘッダー]**（オブジェクト）：出力本文に関連しない応答／ステータスコードのより詳細なコンテキスト。応答ヘッダーに表示されるすべてのヘッダーが応答ヘッダーではないので、不要なヘッダーも含まれている可能性があります。

  応答ヘッダーは、モジュールの設定時に選択した HTTP リクエストによって異なります。

* **[!UICONTROL 本文]**（オブジェクト）：モジュールの設定時に選択した HTTP リクエストによっては、データの一部を受け取る場合があります。GET リクエストからのデータなどは、このオブジェクトに含まれます。

この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事の「<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p><code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code> への相対パスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>モジュールで使用する [!DNL Workfront] APIのバージョンを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。これにより、リクエストのコンテンツタイプが決まります。</p> <p>例：<code> {"Content-type":"application/json"}</code></p> <p>メモ：エラーが表示され、エラーの発生元を特定するのが困難な場合は、[!DNL Workfront] ドキュメントを基に、ヘッダーを変更することを考慮してください。カスタム API 呼び出しで 422 HTTP リクエストエラーが返される場合は、<code>"Content-Type":"text/plain"</code> ヘッダーを使用してみてください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> <p>ヒント：情報は、クエリパラメーターではなく、JSON 本文を使用して送信することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件文を JSON で使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを削除]**

このアクションモジュールは、Workfront のプロジェクト、タスクまたはイシューなどのオブジェクトを削除します。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Force delete]</td> 
   <td>このオプションを有効にすると、[!DNL Workfront] UI が削除の確認をリクエストした場合でも、確実にレコードは削除されます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>モジュールで削除するレコードの一意の [!DNL Workfront] IDを入力します。</p> <p>ID を取得するには、ブラウザーで [!DNL Workfront] オブジェクトを開いて、URL の末尾の「ID=」の後のテキストをコピーします。例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>モジュールで削除する [!DNL Workfront] レコードのタイプを選択します。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>非同期操作によってレコードが削除されない可能性を回避するために、次のシナリオ設定をお勧めします。
>
>1. レコードを同期的に削除します。
>1. レコードの削除モジュールにエラー処理を追加し、40 秒のタイムアウトによるエラーを無視します。


+++

+++ **[!UICONTROL ドキュメントのダウンロード]**

このアクションモジュールは、Workfront からドキュメントをダウンロードします。

レコードの ID を指定します。

このモジュールは、ドキュメントの内容、ファイル名、ファイル拡張子、ファイルサイズを返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document ID]</td> 
   <td> <p>モジュールがダウンロードするドキュメントの一意の [!DNL Workfront] ID をマッピングするか、手動で入力します。</p> <p>ID を取得するには、ブラウザーで [!DNL Workfront] オブジェクトを開き、URL の末尾の「ID=」の後のテキストをコピーします。例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL その他のアクション]**

このアクションモジュールを使用すると、API に対してアクションを実行できます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>モジュールがインタラクトする [!DNL Workfront] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Action]</td> 
   <td> <p>モジュールで実行するアクションを選択します。</p> <p>選択した [!UICONTROL Record Type] と [!UICONTROL Action] に応じて、追加のフィールドに入力する必要がある場合があります。この 2 つの設定の組み合わせによっては、レコード ID しか必要ないものもあれば、追加情報（オブジェクト ID やテンプレート ID など）を必要とするもの（<strong>[!UICONTROL Record Type]</strong> のプロジェクトや <strong>[!UICONTROL Action]</strong> の [!UICONTROL Attach Template] など）もあります。</p> <p>個々のフィールドについて詳しくは、<a href="http://developer.workfront.com/">Workfront 開発者ドキュメント</a>を参照してください。 <p><strong>注意</strong>：開発者ドキュメントサイトには、API バージョン 14 を通じた情報のみが含まれていますが、API 呼び出しに関する有用な情報がまだ含まれています。 </p> 
    <ol> 
     <li value="1"> <p>[!DNL Workfront] 開発者ドキュメントページの左側のナビゲーションからレコードタイプを選択します。以下のタイプには、独自のページがあります。</p> 
      <ul> 
       <li> <p>[!UICONTROL Projects]</p> </li> 
       <li> <p>[!UICONTROL Tasks]</p> </li> 
       <li> <p>[!UICONTROL Issues]</p> </li> 
       <li> <p>[!UICONTROL Users]</p> </li> 
       <li> <p>[!UICONTROL Documents]</p> </li> 
      </ul> <p>その他のすべてのレコードタイプに対して、<b>[!UICONTROL Other objects and endpoints]</b> を選択し、アルファベット順に並べ替えられたページでレコードタイプを探します。</p> </li> 
     <li value="2"> <p>適切なレコードタイプのページで、アクションを検索（Ctrl + F キーまたは Command + F キー）します。</p> </li> 
     <li value="3"> <p>選択したアクションで使用可能なフィールドの説明を表示します。</p> </li> 
    </ol> <p>メモ：  <p>[!DNL Workfront] [!UICONTROL Misc Action] モジュールを使用してプルーフを作成する場合、詳細オプションを使用せずにプルーフを作成し、[!DNL Workfront Proof] SOAP API を使用してプルーフを更新するのがベストプラクティスです。</p> <p>[!DNL Workfront]（このモジュールが使用する）API を使用したプルーフの作成について詳しくは、<a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">[!DNL Adobe Workfront] API を使用したプルーフの作成時に高度なプルーフオプションを追加</a>を参照してください。</p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>モジュールがインタラクトするレコードの一意の [!DNL Workfront] ID を入力またはマッピングします。<p>ID を取得するには、ブラウザーで [!DNL Workfront] オブジェクトを開き、URL の末尾の「ID=」の後のテキストをコピーします。例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを読み取り]**

このアクションモジュールは、1 つのレコードからデータを取得します。

レコードの ID を指定します。また、モジュールで読み取る関連レコードを指定することもできます。

例えば、モジュールが読み取っているレコードがプロジェクトの場合、プロジェクトのタスクを読み込むように指定できます。

モジュールは、指定した出力の標準フィールドからデータの配列を返します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>

<td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>モジュールが読み取る [!DNL Workfront] オブジェクトタイプを選択します。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>

<td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL References]</td>
   <td>出力に含める参照フィールドを選択します。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Collections]</td>
   <td>出力に含める参照フィールドを選択します。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>モジュールが読み取るレコードの一意の [!DNL Workfront] ID を入力します。</p> <p>ID を取得するには、ブラウザーで [!DNL Workfront] オブジェクトを開き、URL の末尾の「ID=」の後のテキストをコピーします。例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを更新]**

このアクションモジュールは、プロジェクト、タスク、イシューなどのオブジェクトを更新します。モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。

レコードの ID を指定します。

このモジュールは、オブジェクトの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront]アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>モジュールが更新するレコードの一意の [!DNL Workfront] ID を入力します。</p> <p>ID を取得するには、ブラウザーで [!DNL Workfront] オブジェクトを開き、URL の末尾の「ID=」の後のテキストをコピーします。例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>モジュールで更新する [!DNL Workfront] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>データ入力に使用するフィールドを選択します。これにより、不要なフィールドをスクロールしなくても、これらのフィールドを使用できます。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。そうすると、モジュールが適切な ID をフィールドに入力します。
>* カスタムフィールドまたは[!UICONTROL メモ]オブジェクト（コメントまたは返信）にテキストを入力する際、「[!UICONTROL メモテキスト]」フィールドで HTML タグを使用して、太字や斜体などのリッチテキストを作成できます。
>
>  更新のリッチテキストについて詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)の[作業アイテムへの更新の追加](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)を参照してください。
>

+++

+++ **[!UICONTROL ドキュメントをアップロード]**

このアクションモジュールは、プロジェクト、タスク、イシューなどの [!DNL Workfront] オブジェクトにドキュメントをアップロードします。

ドキュメントの場所、アップロードするファイル、およびオプションで新しいファイル名を指定します。

このモジュールは、ドキュメントの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>ドキュメントをアップロードするレコードの一意の [!DNL Workfront] ID を入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Related Record Type]</td> 
   <td>モジュールでドキュメントをアップロードする [!DNL Workfront] レコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

### 検索

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 関連レコードを読み取る]**

この検索モジュールは、特定の親オブジェクト内で、指定した検索クエリに一致するレコードを読み取ります。

出力に含めるフィールドを指定します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>読み取る関連レコードの親レコード（Workfront オブジェクト）のタイプを選択します。</p> <p>このモジュールを使用できる [!DNL Workfront] オブジェクトタイプのリストについては、この記事にある各 [!DNL Workfront] モジュール</a>で利用できる <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] オブジェクトタイプを参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Parent Record ID]</td> 
   <td> <p>読み取る関連レコードの親レコードの ID を入力またはマッピングします。</p> <p>ID を取得するには、ブラウザーで [!DNL Workfront] オブジェクトを開き、URL の末尾の「ID=」の後のテキストをコピーします。例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>モジュールが読み取る子レコードのタイプを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 検索]**

この検索モジュールは、指定された検索クエリに一致するレコードを [!DNL Workfront] のオブジェクト内で検索します。

この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>モジュールで検索する [!DNL Workfront] レコードのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Result Set]</td> 
   <td>モジュールが検索条件に一致する最初の結果を取得するか、一致するすべての結果を取得するかを指定するオプションを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>検索するフィールド、クエリで使用する演算子、およびそのフィールドで検索する値を入力します。</p> <p>メモ：検索条件に <code>username </code> を使用しないでください。[!DNL Workfront] への API クエリに <code>username </code> を含めると、そのユーザーが Workfront に記録され、検索は成功しません。</p> <p>メモ：<code>In</code> と <code>NotIn</code> は配列で動作します。入力は配列形式である必要があります。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL References]</td> 
   <td>検索に含める参照フィールドを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Collections]</td> 
   <td>検索に追加するコレクションを選択します。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] 各オブジェクトタイプで使用可能 [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

## 各 [!DNL Workfront] モジュールで使用可能な [!DNL Workfront] オブジェクトタイプ

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**各 [!DNL Workfront] トリガーモジュールで使用可能なオブジェクトタイプ**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Watch Record]</th> 
   <th>[!UICONTROL Watch Field]</th> 
   <th>[!UICONTROL Watch Events]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>承認プロセス</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>割り当て</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ベースライン</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 請求記録 </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>請求レート</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>会社</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ダッシュボード</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメント</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメントフォルダー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ドキュメントリクエスト</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ドキュメントのバージョン</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>費用タイプ</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時間</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時間タイプ</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>イシュー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>イテレーション</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>担当業務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ジャーナルエントリ</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーン</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーンパス</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>メモ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>メモタグ</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プロジェクトユーザー</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>プルーフの承認</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>予約済み時間* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>レポート</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>リスク</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスクタイプ</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ステップ承認者</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>チーム</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレート</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>テンプレートタスク</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>タイムシート</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>アップデート</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**各 [!DNL Workfront] アクションモジュールで使用可能なオブジェクトタイプ**

>[!NOTE]
>
>[!UICONTROL ドキュメントをダウンロード]モジュールは、その設定に [!DNL Workfront] オブジェクトタイプがないため、この表には含まれていません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Create a record]</th> 
   <th>[!UICONTROL Update a record]</th> 
   <th>[!UICONTROL Delete a record]</th> 
   <th>[!UICONTROL Upload Document]</th> 
   <th>[!UICONTROL Read a record]</th> 
   <th>[!UICONTROL Custom API Call]</th> 
   <th>[!UICONTROL Misc Action]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>承認プロセス</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>割り当て</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>請求記録</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>請求レート</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>会社</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメント</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメントフォルダー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメントのバージョン</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>費用タイプ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時間</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時間タイプ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>イシュー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>イテレーション</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>担当業務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ジャーナルエントリ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>マイルストーン</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーンパス</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>メモ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>メモタグ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プロジェクトユーザー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予約済み時間* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスク</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスクタイプ</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ステップ承認者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>チーム</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレート</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレートタスク</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>タイムシート</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>アップデート</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**各 [!DNL Workfront] 検索モジュールで使用可能なオブジェクトタイプ**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Search]</th> 
   <th>[!UICONTROL Read Related Records]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>承認プロセス</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>割り当て</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>請求記録</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>請求レート</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>会社</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメント</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメントフォルダー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメントのバージョン</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用タイプ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時間</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時間タイプ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>イシュー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>イテレーション</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>担当業務</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ジャーナルエントリ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーン</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーンパス</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>メモ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>メモタグ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>プロジェクトユーザー</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予約済み時間* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスク</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスクタイプ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ステップ承認者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>チーム</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレート</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレートタスク</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>タイムシート</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ユーザーの委任</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

これが期待どおりに機能することを再確認することをお勧めします。

+++

## [!DNL Workfront]／[!UICONTROL イベントの監視]モジュールのイベント登録フィルター

>[!NOTE]
>
>[!UICONTROL イベントの監視]モジュールでは、イベント登録フィルターを使用することを強くお勧めします。

[!DNL Workfront][!UICONTROL イベントの監視]モジュールは、[!DNL Workfront] API でイベント登録を作成する web フックに基づいてシナリオをトリガーします。イベント登録は、web フックに送信されるイベントを決定する一連のデータです。例えば、イシューを監視する[!UICONTROL イベントの監視]モジュールを設定した場合、イベント登録はイシューに関連するイベントのみを送信します。

Fusion ユーザーは、イベント登録フィルターを使用して、ユースケースに適したイベント登録を作成できます。例えば、[!DNL Workfront] API でイベント登録を設定すると、特定のプロジェクトのイシューだけを web フックに送信して、[!UICONTROL イベントの監視]モジュールがそのプロジェクトのイシューに対してのみトリガーされるようにすることができます。より範囲の狭いトリガーを作成できるので、無関係なトリガーの数が減り、シナリオの設計を改善できます。

これは、[!DNL Workfront Fusion] シナリオでのフィルターの設定とは異なります。イベント登録フィルターを使用しない場合、web フックは、選択されたオブジェクトタイプに関連するすべてのイベントを受信します。これらのイベントのほとんどはシナリオとは無関係と思われるので、シナリオを続行する前に除外する必要があります。

Workfront／イベントの監視フィルターで使用できる演算子は、次のとおりです。

* が次と等しい
* 等しくない
* より大きい
* より小さい
* が次よりも大きいか等しい
* が次よりも小さいか等しい
* が次を含む
* 存在する
   * この演算子には値は必要ありません。また、値フィールドは存在しません。
* が存在しません
   * この演算子には値は必要ありません。また、値フィールドは存在しません。
* 変更済み
   * この演算子には値は必要ありません。また、値フィールドは存在しません。
   * この演算子では、「状態」フィールドを無視します。
   * `Changed` を使用する際は、「**レコード元**」フィールドで「**更新されたイベントのみ**」を選択します。

>[!IMPORTANT]
>
>既存の [!DNL Workfront] web フックのフィルターは編集できません。[!DNL Workfront] イベント登録に異なるフィルターを設定するには、現在の web フックを削除し、新しく作成します。

>[!INFO]
>
>**例：** 特定のユーザー Ana に割り当てられた新規イシューを処理するシナリオについて考えます。
>
>### イベント登録フィルターを使用したイベントのフィルタリング（推奨）
>
>イベントフィルターを使用すると、イシューが Ana に割り当てられている場合のシナリオをイシューの作成時にトリガーする web フックを設定できます。Ana の ユーザー IDは、b378489d8f7cd3cee0539260720a84b7 です。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>1 日に 100 件のイシューが作成され、そのうち 2 件のみが Ana に割り当てられている場合、シナリオは 2 回実行されます。
>
>### シナリオ内でのイベントのフィルタリング（非推奨）
>
>Ana に割り当てられたイシューのみを処理するようにイベントをフィルタリングするには、[!UICONTROL イベントを監視]モジュールの後にフィルターを作成できます。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>1 日に 100 件のイシューが作成され、そのうち 2 件のみが Ana に割り当てられている場合、シナリオは 100 回実行されます。98 回の実行はフィルターで停止しますが、トリガーモジュールは引き続きデータを消費し、すべての実行で操作が実行されます。

イベント登録について詳しくは、[FAQ - イベント登録](../../wf-api/general/event-subs-faq.md)を参照してください。

Web フックについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) のインスタントトリガー（web フック）を参照してください

シナリオでのフィルターについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md) でのシナリオへのフィルターの追加を参照してください。

