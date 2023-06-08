---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Workfrontモジュール
description: Adobe Workfront Fusion Adobe Workfrontコネクタを使用すると、Workfront内でのプロセスを自動化できます。 Work Automation および Integration 用のWorkfront Fusion のライセンスをお持ちの場合は、それを使用してサードパーティのアプリケーションやサービスに接続することもできます。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 2a49e8f1947d39efa85bb8b8bdb7aee5054f8d33
workflow-type: tm+mt
source-wordcount: '5378'
ht-degree: 3%

---

# [!DNL Adobe Workfront] モジュール

以下を使用して、 [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] 内でプロセスを自動化するコネクタ [!DNL Workfront]. 次の場合、 [!UICONTROL [!DNL Workfront Fusion] 作業の自動化と統合] ライセンスを取得する場合は、それを使用してサードパーティのアプリやサービスに接続することもできます。

この [!DNL Workfront] コネクタは、組織で使用可能なアクティブなアプリの数に対してカウントされません。 すべてのシナリオ ( たとえ [!DNL Workfront] アプリの場合、組織の合計シナリオ数に対してカウントします。

組織で使用可能なアプリとシナリオについて詳しくは、 [組織](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] 組織とチーム](../../workfront-fusion/organizations/organizations-and-teams.md).

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>


ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 接続 [!DNL Workfront] から [!DNL Workfront Fusion]

この [!DNL Workfront] コネクタは、OAuth 2.0 を使用して [!DNL Workfront].

次に、 [!DNL Workfront] 内部から直接アカウントを取得する [!DNL Workfront Fusion] モジュール。

1. 任意の [!DNL Workfront] アプリモジュール、 **[!UICONTROL 追加]** の横 [!UICONTROL 接続] ボックス
1. インスタンスの名前を URL に入力します。 例: `https://<your instance>.my.workfront.com`.
1. クリック **[!UICONTROL 次へ]**.
1. クリック **[!UICONTROL SAML ログイン]** 接続を作成し、モジュールに戻ります。

   または

   ユーザー名とパスワードを入力し、「 **[!UICONTROL ログイン]** 接続を作成し、モジュールに戻ります。

   >[!NOTE]
   >
   >* SAML ログインボタンが表示されない場合、組織でシングルサインオン (SSO) が有効になっていません。 ユーザー名とパスワードを使用してログインできます。
   >   
   >   SSO の詳細は、 [シングルサインオンの概要 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* への OAuth 2.0 接続 [!DNL Workfront] API が API キーに依存しなくなりました。

## [!DNL Workfront] モジュールとそのフィールド

設定時に [!DNL Workfront] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Workfront] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

+++ **[!UICONTROL イベントを見る]**

このトリガーモジュールは、Workfrontで特定のタイプのオブジェクトが追加、更新または削除された場合に、シナリオをリアルタイムで実行します

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

1. クリック **[!UICONTROL 追加]** 右 **ウェブフック** ボックス

1. での Webhook の設定 **[!UICONTROL フックを追加]** ボックスが表示されます。

   このモジュールを設定する際には、次のフィールドが表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook 名 ]</td> 
      <td>（オプション）ウェブフックの新しい名前を入力します</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 接続 ]</td> 
      <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL レコードタイプ ]</td> 
      <td>タイプを選択 [!DNL Workfront] レコードを作成します。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 状態 ]</td> 
      <td>古い状態と新しい状態のどちらを監視するかを選択します。<ul><li><p><b>[!UICONTROL 新しい状態 ]</b></p><p>トリガーレコードが変更されたときのシナリオの変更 <b>から</b> 指定された値。</p><p>例えば、状態が [!UICONTROL New State] に設定され、フィルターが [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] に設定されている場合、Webhook はステータスに関係なく、[!UICONTROL Status] が [!UICONTROL In Progress] に変わるときにシナリオをトリガーします以前の </p></li><li><p><b>[!UICONTROL 古い状態 ]</b></p><p>トリガーレコードが変更されたときのシナリオの変更 <b>から</b> 指定された値。</p><p>例えば、状態が [!UICONTROL Old State] に設定され、フィルターが [!UICONTROL Status] [!UICONTROL Equals] [!UICONTROL In Progress] に設定されている場合、現在 [!UICONTROL Status] が別のステータスに変わると、Webhook はシナリオをトリガーします。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL イベントフィルター ]</p> </td> 
      <td> <p>選択した条件を満たすレコードのみを監視するフィルターを設定できます。</p> <p>各フィルターに対して、フィルターを評価するフィールド、演算子およびフィルターに許可する値を入力します。 AND ルールを追加すると、複数のフィルターを使用できます。</p> <p>注意：既存のフィルターは編集できません [!DNL Workfront] ウェブフック。 別のフィルターを設定するには [!DNL Workfront] イベントの購読、現在の webhook を削除し、新しく作成します。</p> <p>イベントフィルターについて詳しくは、 <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">のイベント購読フィルター [!DNL Workfront] &gt; [!UICONTROL イベントを監視 ] モジュール</a> 」を参照してください。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>この接続でおこなわれたイベントを除外</td> 
      <td>このオプションモジュールで使用するのと同じコネクタを使用して作成または更新されたトリガーを除外するには、このオプションを有効にします。 これにより、シナリオ自体がトリガーし、無限ループで繰り返されることを防ぐことができます。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL レコードの起源 ]</td> 
      <td> <p>シナリオを監視するかどうかを選択します <strong>[!UICONTROL 新しいレコードのみ ]</strong>, <strong>[!UICONTROL 更新済みレコードのみ ]</strong>, <strong>[!UICONTROL 新規レコードと更新されたレコード ]</strong>または <strong>[!DNL Deleted Records Only]</strong>.</p> <p>注意：次を選択した場合： <strong>[!UICONTROL 新規レコードと更新されたレコード ]</strong>Webhook の作成により、（同じ Webhook アドレスに対して）2 つのイベント購読が作成されます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

Webhook を作成したら、イベントの送信先のエンドポイントのアドレスを表示できます。

詳しくは、 [イベントペイロードの例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) 内 [!DNL Workfront] ヘルプ記事 [イベント購読 API](../../wf-api/general/event-subs-api.md).

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 監視フィールド]**

このトリガーモジュールは、指定したフィールドが更新されると、シナリオを実行します。 このモジュールは、指定したフィールドの古い値と新しい値の両方を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td> <p>タイプを選択 [!DNL Workfront] レコードを作成します。</p> <p>例えば、タスク内のレコードフィールドが更新されるたびにシナリオの実行を開始する場合は、「[!UICONTROL タスク ]」を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フィールド ]</td> 
   <td>モジュールで更新を監視するフィールドを選択します。 これらのフィールドは、 [!DNL Workfront] 管理者が追跡用に設定されています。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 出力 ]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを監視]**

このトリガー・モジュールは、特定のタイプのオブジェクトが追加、更新、またはその両方された場合にシナリオを実行します。 このモジュールは、レコードまたはレコードに関連付けられているすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。 出力のモジュールは、各レコードが新規か更新かを示します。

指定した期間に追加および更新されたレコードは、新しいレコードとして返されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>シナリオを監視するかどうかを選択します <strong>[!UICONTROL 新しいレコードのみ ]</strong>, <strong>[!UICONTROL 更新済みレコードのみ ]</strong>または <strong>[!UICONTROL 新規レコードと更新されたレコード ]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>( <strong>フィルター</strong>.) タイプを選択 [!DNL Workfront] レコードを作成します。</p> <p>例えば、新しいプロジェクトが作成されるたびにシナリオを開始する場合は、「[!UICONTROL プロジェクト ]」を選択します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL オプションのフィルター ]</td> 
   <td> <p>（詳細）API コード文字列を入力して、条件を絞り込む追加のパラメーターまたはコードを定義します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

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

+++ **[!UICONTROL オブジェクトを変換]**

このアクションモジュールは、次の変換のいずれかをおこないます。

* 問題をプロジェクトに変換
* 問題をタスクに変換
* タスクをプロジェクトに変換

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL オブジェクトタイプ ]</td> 
   <td> <p>変換するオブジェクトの種類を選択します。 これは、変換前にオブジェクトに含まれるタイプです。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 変換先 ]</td> 
   <td>変換先のオブジェクトを選択します。 これは、変換後にオブジェクトに含まれるタイプです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>オブジェクトの ID を入力します。 </p> <p>注意：オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。 次に、モジュールは、フィールドに適切な ID を入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL テンプレート ID]</td> 
   <td> <p>プロジェクトに変換する場合は、プロジェクトに使用するテンプレート ID を選択します。</p> <p>注意：オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。 次に、モジュールは、フィールドに適切な ID を入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL カスタムフォーム ]</td> 
   <td>新しく変換されたオブジェクトに追加するカスタムフォームを選択し、カスタムフォームのフィールドに値を入力します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL オプション ]</td> 
   <td> <p>オブジェクトの変換時に必要なオプションを有効にします。 変換元または変換元のオブジェクトに応じて、オプションを使用できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL レコードの作成（カスタムフォームの添付）]**

このアクションモジュールは、プロジェクト、タスク、イシューなどのオブジェクトを [!DNL Workfront]をクリックし、新しいオブジェクトにカスタムフォームを追加できます。 モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

例えば、このモジュールを使用して、 [!DNL Workfront] クライアントが [!DNL Google Sheets] 実行する必要があるタスクのリスト。

このモジュールを設定する際には、次のフィールドが表示されます。

入力フィールドの最小数を指定してください。 例えば、イシューを作成する場合は、「プロジェクト ID」フィールドに有効な親プロジェクト ID を指定して、イシューのWorkfrontでの配置先を示す必要があります。 マッピングパネルを使用して、シナリオ内の別のモジュールからこの情報をマッピングするか、名前を入力し、リストから選択して、手動で入力することもできます。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td> <p>タイプを選択 [!DNL Workfront] を記録します。</p> <p>例えば、プロジェクトを作成する場合は、ドロップダウンリストから「 [!UICONTROL プロジェクト ] 」を選択し、プロジェクトに入力されるデータ（シナリオの前のモジュールのもの）にアクセスできることを確認します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL マッピングするフィールドを選択 ]</td> 
   <td> <p>データ入力に使用するフィールドを選択します。 これにより、不要なフィールドをスクロールしなくても、これらのフィールドを使用できます。</p> <p>カスタムフォームのフィールドの場合、 <b>[!UICONTROL カスタムフォームを添付 ]</b> フィールドに入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL カスタムフォームを添付 ]</td> 
   <td>新しいオブジェクトに追加するカスタムフォームを選択し、それらのフィールドに値を入力します。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。 次に、モジュールは、フィールドに適切な ID を入力します。
>* カスタムフィールドまたは [!UICONTROL 注意] オブジェクト（コメントまたは返信）の場合、 [!UICONTROL メモテキスト] 太字や斜体などのリッチテキストを作成するためのフィールドです。
>
>  更新のリッチテキストについて詳しくは、 [作業項目に更新を追加する](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL レコードを作成]**

このアクションモジュールは、Workfrontでプロジェクト、タスク、問題などのオブジェクトを作成します。 モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

例えば、このモジュールを使用して、 [!DNL Workfront] 必要なタスクのGoogle Sheets リストにクライアントが新しい行を追加したとき。

このモジュールを設定する際には、次のフィールドが表示されます。

入力フィールドの最小数を指定してください。 例えば、イシューを作成する場合は、「プロジェクト ID」フィールドに有効な親プロジェクト ID を指定して、イシューのWorkfrontでの配置先を示す必要があります。 マッピングパネルを使用して、シナリオ内の別のモジュールからこの情報をマッピングするか、名前を入力し、リストから選択して、手動で入力することもできます。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td> <p>タイプを選択 [!DNL Workfront] を記録します。</p> <p>例えば、プロジェクトを作成する場合は、ドロップダウンリストから「 [!UICONTROL プロジェクト ] 」を選択し、プロジェクトに入力されるデータ（シナリオの前のモジュールのもの）にアクセスできることを確認します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL マッピングするフィールドを選択 ]</td> 
   <td>データ入力に使用するフィールドを選択します。 これにより、不要なフィールドをスクロールしなくても、これらのフィールドを使用できます。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。 次に、モジュールは、フィールドに適切な ID を入力します。
>* カスタムフィールドまたは [!UICONTROL 注意] オブジェクト（コメントまたは返信）の場合、 [!UICONTROL メモテキスト] 太字や斜体などのリッチテキストを作成するためのフィールドです。
>
>  更新のリッチテキストについて詳しくは、 [作業項目に更新を追加する](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL カスタム API 呼び出し]**

このアクションモジュールを使用すると、 [!DNL Workfront] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Workfront] モジュール。

モジュールは、次の情報を返します。

* **[!UICONTROL ステータスコード]** （数値）:HTTP リクエストの成功または失敗を示します。 これらはインターネット上で検索できる標準コードです。
* **[!UICONTROL ヘッダー]** （オブジェクト）:出力本文に関連しない応答/ステータスコードのより詳細なコンテキスト。 応答ヘッダーに表示されるすべてのヘッダーが応答ヘッダーではないので、役に立たないヘッダーも含まれている可能性があります。

  応答ヘッダーは、モジュールの設定時に選択した HTTP リクエストによって異なります。

* **[!UICONTROL 本文]** （オブジェクト）:モジュールの設定時に選択した HTTP リクエストに応じて、一部のデータを受け取る場合があります。 このデータ ( データリクエストからのGETなど ) は、このオブジェクトに含まれます。

この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>相対パスを入力<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API バージョン ]</td> 
   <td>のバージョンを選択 [!DNL Workfront] モジュールで使用する API。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。 これにより、リクエストのコンテンツタイプが決まります。</p> <p>以下に例を挙げます。<code> {"Content-type":"application/json"}</code></p> <p>注意：エラーが発生し、エラーの発生元を特定するのが困難な場合は、 [!DNL Workfront] ドキュメント。 カスタム API 呼び出しで 422 HTTP リクエストエラーが返される場合は、 <code>"Content-Type":"text/plain"</code> ヘッダー。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> <p>ヒント：情報は、クエリパラメーターではなく JSON の本文を使用して送信することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを削除]**

このアクションモジュールは、Workfrontのプロジェクト、タスク、問題などのオブジェクトを削除します。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 削除を強制 ]</td> 
   <td>このオプションを有効にすると、 [!DNL Workfront] UI が削除の確認を要求します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>一意の [!DNL Workfront] モジュールで削除するレコードの ID。</p> <p>ID を取得するには、 [!DNL Workfront] オブジェクトを使用し、URL の末尾の「ID=」の後のテキストをコピーします。 例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td>タイプを選択 [!DNL Workfront] を記録します。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL ドキュメントのダウンロード]**

このアクションモジュールは、Workfrontからドキュメントをダウンロードします。

レコードの ID を指定します。

このモジュールは、ドキュメントの内容、ファイル名、ファイル拡張子、およびファイルサイズを返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドキュメント ID]</td> 
   <td> <p>マッピングするか、一意の [!DNL Workfront] モジュールをダウンロードするドキュメントの ID。</p> <p>ID を取得するには、 [!DNL Workfront] オブジェクトを使用し、URL の末尾の「ID=」の後のテキストをコピーします。 例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL その他のアクション]**

このアクションモジュールを使用すると、API に対してアクションを実行できます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td> <p>タイプを選択 [!DNL Workfront] を記録します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL アクション ]</td> 
   <td> <p>モジュールで実行するアクションを選択します。</p> <p>選択した [!UICONTROL レコードタイプ ] および [!UICONTROL アクション ] に応じて、追加のフィールドの入力が必要になる場合があります。 これら 2 つの設定の組み合わせによっては、レコード ID しか必要ない場合もあれば、レコード ID しか必要ない場合もあります ( 例えば、 <strong>[!UICONTROL レコードタイプ ]</strong> および <strong>[!UICONTROL アクション ]</strong>) には、追加の情報（オブジェクト ID やテンプレート ID など）が必要です。</p> <p>個々のフィールドについて詳しくは、 <a href="http://developer.workfront.com/">Workfront開発者ドキュメント</a>. </p> 
    <ol> 
     <li value="1"> <p>左側のナビゲーションからレコードタイプを選択します。 [!DNL Workfront] 開発者向けドキュメントページ 次のタイプには、独自のページがあります。</p> 
      <ul> 
       <li> <p>[!UICONTROL プロジェクト ]</p> </li> 
       <li> <p>[!UICONTROL タスク ]</p> </li> 
       <li> <p>[!UICONTROL の問題 ]</p> </li> 
       <li> <p>[!UICONTROL ユーザー ]</p> </li> 
       <li> <p>[!UICONTROL ドキュメント ]</p> </li> 
      </ul> <p>その他のすべてのレコードタイプに対して、 <b>[!UICONTROL その他のオブジェクトおよびエンドポイント ]</b>をクリックし、アルファベット順に並べ替えられたページでレコードタイプを探します。</p> </li> 
     <li value="2"> <p>適切なレコードタイプのページで、アクションを検索（Ctrl + F または Command + F）します。</p> </li> 
     <li value="3"> <p>選択したアクションの下にある使用可能フィールドの説明を表示します。</p> </li> 
    </ol> <p>メモ:  <p>次の手順で配達確認を作成する場合： [!DNL Workfront] [!UICONTROL その他のアクション ] モジュールでは、高度なオプションを使用せずに配達確認を作成し、 [!DNL Workfront Proof] SOAP API</p> <p>を使用した配達確認の作成について詳しくは、 [!DNL Workfront] API（このモジュールで使用）（を参照） <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">で配達確認を作成する際に、高度な校正オプションを追加する [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>一意の [!DNL Workfront] モジュールとやり取りするレコードの ID。<p>ID を取得するには、 [!DNL Workfront] オブジェクトを使用し、URL の末尾の「ID=」の後のテキストをコピーします。 例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを読み取る]**

このアクションモジュールは、1 つのレコードからデータを取得します。

レコードの ID を指定します。 また、モジュールで読み取る関連レコードを指定することもできます。

例えば、モジュールが読み取っているレコードがプロジェクトの場合、プロジェクトのタスクを読み取るように指定できます。

モジュールは、指定した出力の標準フィールドからのデータの配列を返します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL 接続 ]</td>

<td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL レコードタイプ ]</td>

<td>を選択します。 [!DNL Workfront] モジュールが読み取るオブジェクトタイプです。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL 出力 ]</td>

<td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL 参照 ]</td>
   <td>出力に含める参照フィールドを選択します。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL コレクション ]</td>
   <td>出力に含める参照フィールドを選択します。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>一意の [!DNL Workfront] モジュールが読み取るレコードの ID。</p> <p>ID を取得するには、 [!DNL Workfront] オブジェクトを使用し、URL の末尾の「ID=」の後のテキストをコピーします。 例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL レコードを更新]**

このアクションモジュールは、プロジェクト、タスク、イシューなどのオブジェクトを更新します。 モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。

レコードの ID を指定します。

このモジュールは、オブジェクトの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>一意の [!DNL Workfront] モジュールを更新するレコードの ID。</p> <p>ID を取得するには、 [!DNL Workfront] オブジェクトを使用し、URL の末尾の「ID=」の後のテキストをコピーします。 例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>タイプを選択 [!DNL Workfront] を記録します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>データ入力に使用するフィールドを選択します。 これにより、不要なフィールドをスクロールしなくても、これらのフィールドを使用できます。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* オブジェクトの ID を入力する際に、オブジェクトの名前を入力し、リストから選択できます。 次に、モジュールは、フィールドに適切な ID を入力します。
>* カスタムフィールドまたは [!UICONTROL 注意] オブジェクト（コメントまたは返信）の場合、 [!UICONTROL メモテキスト] 太字や斜体などのリッチテキストを作成するためのフィールドです。
>
>  更新のリッチテキストについて詳しくは、 [作業項目に更新を追加する](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL ドキュメントをアップロード]**

このアクションモジュールは、ドキュメントを [!DNL Workfront] オブジェクト（プロジェクト、タスク、イシューなど）。

ドキュメントの場所、アップロードするファイル、およびオプションで新しいファイル名を指定します。

このモジュールは、ドキュメントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 関連レコード ID]</td> 
   <td>一意の [!DNL Workfront] ドキュメントをアップロードするレコードの ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 関連レコードタイプ ]</td> 
   <td>タイプを選択 [!DNL Workfront] モジュールでドキュメントをアップロードする場所を記録します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

### 検索

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 関連レコードの読み取り]**

この検索モジュールは、指定した検索クエリ（特定の親オブジェクト内）に一致するレコードを読み取ります。

出力に含めるフィールドを指定します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td> <p>読み取る関連レコードの親レコード (Workfrontオブジェクト ) のタイプを選択します。</p> <p>以下のリストを参照してください： [!DNL Workfront] このモジュールを <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] 各 [!DNL Workfront] モジュール</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 親レコード ID]</td> 
   <td> <p>読み取る関連レコードの親レコードの ID を入力またはマップします。</p> <p>ID を取得するには、 [!DNL Workfront] オブジェクトを使用し、URL の末尾の「ID=」の後のテキストをコピーします。 例：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL コレクション ]</td> 
   <td>モジュールが読み取る子レコードのタイプを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 検索]**

この検索モジュールは、 [!DNL Workfront] 指定した検索クエリに一致する

この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Workfront] 次のアプリ： [!DNL Workfront Fusion]を参照してください。 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">接続 [!DNL Workfront] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ]</td> 
   <td> <p>タイプを選択 [!DNL Workfront] を記録します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 結果セット ]</td> 
   <td>オプションを選択して、検索条件に一致する最初の結果を取得するか、一致するすべての結果を取得するかを指定します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最大 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索条件 ]</td> 
   <td> <p>検索するフィールド、クエリで使用する演算子、および「 」フィールドで検索する値を入力します。</p> <p>注意：使用しない <code>username </code>」と入力します。 次を含む <code>username </code>を [!DNL Workfront] ユーザーをWorkfrontに記録すると、検索に失敗します。</p> <p>注意： <code>In</code> および <code>NotIn</code>は配列を使用します。 入力は配列形式である必要があります。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 参照 ]</td> 
   <td>検索に含める参照フィールドを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL コレクション ]</td> 
   <td>検索に追加するコレクションを選択します。</td> 
  </tr> 
 </tbody> 
</table>

以下のリストを参照してください： [!DNL Workfront] このモジュールを [[!DNL Workfront] object types available for each [!DNL Workfront] モジュール](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] 各 [!DNL Workfront] モジュール

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**各 [!DNL Workfront] トリガーモジュール**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL ウォッチレコード ]</th> 
   <th>[!UICONTROL 監視フィールド ]</th> 
   <th>[!UICONTROL ウォッチイベント ]</th> 
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
   <td>請求率</td> 
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
   <td>ドキュメント フォルダー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ドキュメント要求</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ドキュメント バージョン</td> 
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
   <td>問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>反復</td> 
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
   <td>ジャーナル エントリ</td> 
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
   <td>マイルストーン パス</td> 
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
   <td>メモ タグ</td> 
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
   <td>プロジェクト ユーザー</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予約時間* </td> 
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
   <td>危険</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>危険タイプ</td> 
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
   <td>テンプレート タスク</td> 
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
   <td>更新</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**各 [!DNL Workfront] アクションモジュール**

>[!NOTE]
>
>この [!UICONTROL ドキュメントをダウンロード] モジュールはこのテーブルに含まれていません。 [!DNL Workfront] オブジェクトタイプは設定に含まれていません。

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
   <th>[!UICONTROL レコードの作成 ]</th> 
   <th>[!UICONTROL レコードの更新 ]</th> 
   <th>[!UICONTROL レコードの削除 ]</th> 
   <th>[!UICONTROL ドキュメントをアップロード ]</th> 
   <th>[!UICONTROL レコードの読み取り ]</th> 
   <th>[!UICONTROL カスタム API 呼び出し ]</th> 
   <th>[!UICONTROL その他のアクション ]</th> 
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
   <td>請求率</td> 
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
   <td>ドキュメント フォルダー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメント バージョン</td> 
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
   <td>問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>反復</td> 
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
   <td>ジャーナル エントリ</td> 
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
   <td>マイルストーン パス</td> 
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
   <td>メモ タグ</td> 
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
   <td>プロジェクト ユーザー</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予約時間* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>危険</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>危険タイプ</td> 
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
   <td>テンプレート タスク</td> 
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
   <td>更新</td> 
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

+++**各 [!DNL Workfront] 検索モジュール**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL 検索 ]</th> 
   <th>[!UICONTROL 関連レコードの読み取り ]</th> 
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
   <td>請求率</td> 
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
   <td>ドキュメント フォルダー</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>ドキュメント バージョン</td> 
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
   <td>問題</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>反復</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>担当業務</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ジャーナル エントリ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーン</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーン パス</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>メモ</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>メモ タグ</td> 
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
   <td>プロジェクト ユーザー</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予約時間* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>危険</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>危険タイプ</td> 
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
   <td>テンプレート タスク</td> 
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

この機能が期待どおりに動作することを確認するために、再度チェックすることをお勧めします。

+++

## のイベント購読フィルター [!DNL Workfront] > [!UICONTROL イベントを見る] モジュール

>[!NOTE]
>
>イベント購読フィルターを [!UICONTROL イベントを見る] モジュール。

この [!DNL Workfront] [!UICONTROL イベントを見る] モジュールトリガーシナリオ： [!DNL Workfront] API イベント購読は、Webhook に送信するイベントを決定する一連のデータです。 例えば、 [!UICONTROL イベントを見る] モジュールで問題を監視している場合、イベント購読は問題に関連するイベントのみを送信します。

Fusion ユーザーは、イベントサブスクリプションフィルタを使用して、自分の使用例に適したイベントサブスクリプションを作成できます。 例えば、 [!DNL Workfront] 特定のプロジェクトにある問題のみを Webhook に送信する API。 [!UICONTROL イベントを見る] モジュールは、そのプロジェクトでの問題に対してのみトリガーします。 より狭いトリガーを作成する機能により、無関係なトリガーの数を減らし、シナリオのデザインを改善します。

これは、 [!DNL Workfront Fusion] シナリオ。 イベント購読フィルターがない場合、Webhook は選択したオブジェクトタイプに関連するすべてのイベントを受け取ります。 これらのイベントのほとんどはシナリオとは無関係で、シナリオを続行する前に除外する必要があります。

Workfront/イベントを監視フィルターでは、次の演算子を使用できます。

* が次と等しい
* 等しくない
* より大きい
* 未満
* 次よりも大きいか等しい
* 次よりも小さいか等しい
* が次を含む
* 存在
   * この演算子には値は必要ありません。また、値フィールドは存在しません。
* 存在しない
   * この演算子には値は必要ありません。また、値フィールドは存在しません。
* 変更済み
   * この演算子には値は必要ありません。また、値フィールドは存在しません。
   * この演算子は、「状態」フィールドを無視します。
   * を使用する場合 `Changed`を選択します。 **更新されたイベントのみ** 内 **レコードの起源** フィールドに入力します。

>[!IMPORTANT]
>
>既存のフィルターは編集できません [!DNL Workfront] ウェブフック。 別のフィルターを設定するには [!DNL Workfront] イベントの購読、現在の webhook を削除し、新しく作成します。

>[!INFO]
>
>**例：** 特定のユーザー Ana に割り当てられた新しい問題を処理するシナリオを検討します。
>
>### イベント購読フィルターを使用してイベントをフィルタリングする（推奨）
>
>イベントフィルターを使用すると、問題の作成時に問題が Ana に割り当てられた場合のシナリオをトリガーする Webhook を設定できます。 Ana は userID b378489d8f7cd3cee0539260720a84b7 を持っています。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>1 日に 100 個の問題が作成され、そのうち 2 個のみが Ana に割り当てられている場合、シナリオは 2 回実行されます。
>
>### シナリオ内のイベントをフィルター（非推奨）
>
>Ana に割り当てられた問題のみを処理するようにイベントをフィルタリングするには、 [!UICONTROL イベントを見る] モジュール。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>1 日に 100 個の問題が作成され、そのうち 2 個のみが Ana に割り当てられている場合、シナリオは 100 回実行されます。 実行の 98 回がフィルターで停止しますが、トリガーモジュールは引き続きデータを消費し、すべての実行で操作を実行しています。

イベントの購読について詳しくは、 [FAQ — イベント購読](../../wf-api/general/event-subs-faq.md).

ウェブフックの詳細については、 [のインスタントトリガー（Web フック） [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

シナリオでのフィルターの詳細については、 [のシナリオにフィルターを追加する [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
