---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Acrobat Signモジュール
description: を使用 [!DNL Adobe Acrobat Sign] モジュールを使用する場合、 [!DNL Adobe Workfront Fusion] シナリオに基づいて [!DNL Adobe] Acrobat Signのアカウント、契約およびその他のレコードの作成、読み取り、更新、設定した条件を使用したレコードの検索、ドキュメントのアップロードを行います。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 8bb97b08bb5991fadbf2627f4ebfdaa25ae337ce
workflow-type: tm+mt
source-wordcount: '6579'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] モジュール

を使用 [!DNL Adobe Acrobat Sign] モジュールを使用する場合、 [!DNL Adobe Workfront Fusion] シナリオに基づいて [!DNL Adobe Acrobat Sign] 契約およびその他のレコードのアカウント、作成、読み取り、更新、設定した条件を使用したレコードの検索、ドキュメントのアップロードを行います。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Adobe Acrobat Sign] コネクタ使用の推奨事項

この [!DNL Adobe Sign ]アプリがで eSignature ビジネスプロセスを自動化 [!DNL Fusion] はるかに簡単でより強力な

新規ユーザー [!DNL Adobe Sign] は、契約の更新に関する制約の一部に十分注意する必要があります。 契約は、通常、開始後は変更されません。 の新規ユーザーにお勧めします。 [!DNL Adobe Sign] 契約作成モジュールを使用して新しい契約を作成することに重点を置きます。 これで間に合う [!DNL Fusion] 自動化が容易になり、とより効率的に連携 [!DNL Adobe Sign].

[!DNL Adobe Sign] 契約には、使用するフィールドが必要です。 これを行うオプションはいくつかありますが、最も簡単で一般的な方法は、一時的なドキュメントをアップロードし、そのドキュメントを契約書にマッピングすることです。

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] モジュールとそのフィールド

設定時に [!DNL Adobe Acrobat Sign] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Adobe Acrobat Sign] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL 契約を守る]**

このトリガーモジュールは、契約が作成または更新されると、シナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
<td>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td>新しいレコード、更新されたレコード、またはその両方を監視するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ] </td> 
   <td>レコードを監視するレコードの種類を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テキストを検索 ]</td> 
   <td> <p>検索する用語を入力します。 このモジュールは、これらの用語を含むレコードをフィールド値として返します。</p> <p>でのフィールドの検索の詳細 [!DNL Adobe Acrobat Sign](「テキスト検索の仕組み」( <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign検索 — 仕組み</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返される契約の最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL イベントを見る]**

このトリガーモジュールは、選択したイベントが発生したときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>使用するウェブフックを選択するか、 <b>[!UICONTROL 追加 ]</b> 次のフィールドに入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 名 ]</td> 
   <td> <p>ウェブフックの名前を入力</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スコープ ]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL アカウント ]</p> </li> 
     <li> <p>[!UICONTROL グループ ]</p> </li> 
     <li> <p>[!UICONTROL ユーザー ]</p> </li> 
     <li> <p>[!UICONTROL リソース ]</p> <p>「[!UICONTROL Resource]」を選択した場合は、リソース ID とリソースタイプを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リソースレベル ]</td> 
   <td> <p>監視するリソースのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL 契約 ]</p> </li> 
     <li> <p>[!UICONTROL ウィジェット ]</p> </li> 
     <li> <p>[!UICONTROL Megasings]</p> </li> 
     <li> <p>[!UICONTROL ライブラリドキュメント ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 購読イベント ]</td> 
   <td>を選択します。 [!DNL Adobe Sign] モジュールで監視するイベントです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アプリケーションの表示名 ]</td> 
   <td>Webhook の作成に使用するアプリケーションの表示名。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アプリケーション名 ]</td> 
   <td>Webhook の作成に使用するアプリケーションの表示名。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 問題通知 E メール ]</td> 
   <td> <p>この設定は、管理者アカウントに対してのみ機能します</p> <p>問題通知メールを送信する各メールアドレスに対して、 <b>[!UICONTROL 追加 ]</b> をクリックし、電子メールアドレスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 契約の条件付きパラメーター ]</td> 
   <td>条件付きパラメーターを追加する場合は、「 <b>[!UICONTROL はい ]</b> パラメータを追加するレコードタイプで、「 」を選択します。 <b>[!UICONTROL はい ]</b> を有効にします。</td> 
  </tr> 
 </tbody> 
</table>

+++

### アクション

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL レコードの作成]**

このアクションモジュールは、選択したタイプの新しいレコードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL グループ ]</b> </p> </li> 
     <li> <p><b>[!UICONTROL ライブラリドキュメント ]</b> </p> </li> 
     <li> <p><b>[!UICONTROL ユーザー ]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Web フォーム ] ([!UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL グループ情報 ]</td> 
   <td> <p>グループの [!UICONTROL Name] と [!UICONTROL ID] を入力またはマッピングし、このグループがアカウントのデフォルトのグループであるかどうかを示します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ライブラリドキュメント情報 ]</td> 
   <td> <p>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 送信するファイル ]</b> </p> <p>追加する各ファイルに対して、 <b>[!UICONTROL 項目を追加 ]</b> 「 」フィールドに入力します。</p> 
      <ul> 
       <li><b>[!UICONTROL 一時的なドキュメント ID]</b> <p>一時的なドキュメントの ID を入力</p> </li> 
       <li> <p><b>[!UICONTROL URL ファイル転送 ]</b> </p> <p>次のフィールドに入力します。</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>元のファイルの MIME タイプを入力します。 多目的インターネットメール拡張 (MIME) タイプは、ソフトウェアがインターネットで共有される様々なタイプのデータを識別できるラベルです。 Web サーバーおよびブラウザーは、MIME タイプを使用して、ファイルに対して何を実行するかを決定します。 例えば、MIME タイプがのファイル <code>text/html</code> は、MIME タイプがのファイルとは異なる方法でブラウザーで処理されます <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>ファイル名を入力します。</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>送信するファイルの URL を入力します。</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL 認証</b> </p> <p>このドキュメントを認証する必要があるかどうかを選択します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL ライブラリテンプレート名 ]</b> </p> <p>ライブラリテンプレートの名前を入力またはマッピング</p> </li> 
     <li> <p><b>[!UICONTROL 共有モード ]</b> </p> <p>ライブラリドキュメントへのアクセス権を持つユーザーを指定します。</p> </li> 
     <li> <p><b>[!UICONTROL ライブラリドキュメントの状態 ]</b> </p> <p>ドキュメントがオーサリング状態かアクティブ状態かを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL ライブラリテンプレートタイプ ]</b> </p> <p>使用するライブラリテンプレートタイプごとに、 <b>[!UICONTROL 項目を追加 ]</b> をクリックし、テンプレートタイプを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL 最終イベント日 ]</b> </p> <p>ライブラリドキュメントでイベントが発生した最後の日付を入力します。</p> <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL ライブラリドキュメントのステータス ]</b> </p> <p>ライブラリドキュメントのステータスを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ユーザー情報 ]</td> 
   <td> <p>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 電子メール ]</b> </p> <p>ユーザーの電子メールアドレスを入力します。</p> </li> 
     <li> <p><b>[!UICONTROL アカウント管理者です ]</b> </p> <p>作成したユーザーがアカウント管理者の場合は、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL User ID]</b> </p> <p>ユーザーの一意の ID を入力</p> </li> 
     <li> <p><b>[!UICONTROL アカウント ID]</b> </p> <p>の一意の ID を入力 [!DNL Adobe Acrobat Sign] このユーザーに関連付けられたアカウント。</p> </li> 
     <li> <p><b>[!UICONTROL 名 ]</b> </p> <p>ユーザーの名を入力します。</p> </li> 
     <li> <p><b>[!UICONTROL 姓 ]</b> </p> <p>ユーザーの姓を入力</p> </li> 
     <li> <p><b>[!UICONTROL 会社 ]</b> </p> <p>ユーザーの会社名を入力します。</p> </li> 
     <li> <p><b>[!UICONTROL イニシャル ]</b> </p> <p>ユーザーのイニシャルを入力します。</p> </li> 
     <li> <p><b>[!UICONTROL ロケール ]</b> </p> <p>ユーザーのロケールを入力します。 UI の言語を決定します。 </p> </li> 
     <li> <p><b>[!UICONTROL Phone]</b> </p> <p>ユーザーの電話番号を入力</p> </li> 
     <li> <p><b>プライマリグループ ID</b> </p> <p>新しいユーザーを追加するグループを入力します。 何も入力しなかった場合、ユーザーはアカウントのデフォルトのグループに追加されます。</p> </li> 
     <li> <p><b>[!UICONTROL ジョブのタイトル ]</b> </p> <p>ユーザーの役職を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Web フォーム情報 ]</td> 
   <td> <p>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL ファイル情報 ]</b> </p> <p>Web フォームに追加するファイルごとに、「追加」をクリックし、次のフィールドに入力します。</p> 
      <ul> 
       <li> <p>[!UICONTROL ファイルタイプ ]</p> <p>[!UICONTROL ドキュメント ]</p> </li> 
       <li> <p>[!UICONTROL 一時的なドキュメント ]</p> </li> 
       <li> <p>[!UICONTROL URL ファイル情報 ]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web フォーム名 ]</b> </p> <p>Web フォームの名前を入力します。 この名前は、電子メールや Web サイトなどの場所で Web フォームを識別するために使用されます。</p> </li> 
     <li> <p><b>[!UICONTROL Web フォームの状態 ]</b> </p> <p>新しい Web フォームを作成する状態を選択します。</p> </li> 
     <li> <p><b>[!UICONTROL Web フォーム参加者セット情報 ]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL メンバー情報 ]</b> </p> <p>参加者セットに追加する各メンバーで、 <b>[!UICONTROL 項目を追加 ]</b>. </p> 
        <ul> 
         <li> <p><b>[!UICONTROL 電子メール ]</b> </p> <p>このオプションは空白のままにします。</p> </li> 
         <li> <p><b>[!UICONTROL セキュリティオプション ]</b> </p> <p>このユーザーを認証するセキュリティオプションを追加する場合は、 <b>[!UICONTROL はい ]</b>をクリックし、セキュリティオプションを選択して、必要なフィールドに入力します。</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL ロール ]</b> </p> <p>役割を選択します。 この参加者セットのすべてのメンバーは、役割を共有します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web フォームの追加参加者セット情報 ]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL メンバー情報 ]</b> </p> <p>参加者セットに追加する各メンバーで、 <b>[!UICONTROL 項目を追加 ]</b>.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 電子メール ]</b> </p> <p>このオプションは空白のままにします。</p> </li> 
         <li> <p><b>[!UICONTROL セキュリティオプション ]</b> </p> <p>このユーザーを認証するセキュリティオプションを追加する場合は、 <b>[!UICONTROL はい ]</b>をクリックし、セキュリティオプションを選択して、必要なフィールドに入力します。</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL ロール ]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Web フォーム参加者 ID] </b> </p> <p>Web フォーム参加者の ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL 順序 ]</b> </p> <p>この参加者セットが Web フォームとやり取りする順序を指定します。 例えば、注文値が 1 の参加者グループは最初に行く必要があり、2 は次に行く必要があります。 注文番号は 1 から始まる必要があり、系列に隙間はありません。 </p> </li> 
       <li> <p><b>[!UICONTROL プロバイダー参加者セット情報 ]</b> </p> <p>参加者が不明な場合は、プロバイダーが参加者の詳細を提供する必要があるかどうかを入力し、不明な参加者に必要な詳細を含むメッセージを入力します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 認証失敗情報 ]</b> </p> <p>ユーザーにエラーまたはエラーページを提供する場合は、 <b>[!UICONTROL はい ]</b>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>エラーページの URL を入力</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Web フォーム内にエラーページを表示する場合は、このオプションを有効にします</p> </li> 
       <li> <p><b>[!UICONTROL 遅延 ]</b> </p> <p>ユーザーがエラーページにリダイレクトされるまでの待ち時間（秒）を入力します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC info]</b> </p> <p>Web フォームに対する最終契約が署名されたときに電子メールを受け取る電子メールアドレスごとに、 <b>[!UICONTROL 項目を追加 ]</b> をクリックし、電子メールアドレスを入力します。</p> </li> 
     <li> <p><b>[!UICONTROL 完了情報 ]</b> </p> <p style="font-style: normal;">ユーザーに成功ページを提供する場合は、 <b>[!UICONTROL はい ]</b>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>成功ページの URL を入力</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>成功ページを Web フォーム内に表示する場合は、このオプションを有効にします</p> </li> 
       <li> <p><b>[!UICONTROL 遅延 ]</b> </p> <p>ユーザーが成功ページにリダイレクトされるまでの遅延時間（秒）を入力します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Group ID]</b> </p> <p>Web フォームが属するグループの ID を入力します。 何も入力しなかった場合、Web フォームはアカウントユーザーのプライマリグループに属します。</p> </li> 
     <li> <p><b>[!UICONTROL 最終イベント日 ]</b> </p> <p>Web フォームで最後のイベントが発生した日付を入力します。 形式を使用 <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL ロケール ]</b> </p> <p>ユーザーのロケールを入力します。 UI の言語を決定します。 </p> </li> 
     <li> <p><b>[!UICONTROL セキュリティオプション ]n</b> </p> <p>ドキュメントの保護に使用するパスワードを入力します。 このパスワードは、関係者に別途伝える必要があります。</p> </li> 
     <li> <p><b>[!UICONTROL Vaulting info]</b> </p> <p>アカウントがドキュメントヴォールティング用に設定され、契約ごとに有効にするオプションがある場合、このオプションを有効にしてこの契約をヴォールトできます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 契約の作成]**

このアクションモジュールは、契約を作成し、署名用に送信し、契約 ID を返します。

>[!NOTE]
>
>ドキュメントをアップロードして一時的なドキュメントとして署名し、 [!UICONTROL 送信するファイル] フィールド [!UICONTROL 契約の作成] モジュール。 例については、この記事の「ドキュメントのアップロード」を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
<td>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 送信するファイル ]</td> 
   <td> <p>契約に含める各品目に対して、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL ファイルタイプ ]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL ドキュメント ]</b> </p> <p>次のフィールドに入力します。</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 作成日 ]</b> </p> <p>ドキュメントが作成された日付を形式で入力またはマッピングします <code>yyyy-MM-dd'T'HH:mm:ssZ</code>. 例： <code>2016-02-25T18:46:19Z</code> は UTC 時間を表します。</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>ドキュメントの ID を入力またはマッピングします。</p> </li> 
         <li> <p><b>[!UICONTROL ラベル ]</b> </p> <p>ファイルの一意のラベルを入力またはマッピングします。 カスタムワークフローの場合、これはワークフロー定義内の対応するファイル要素にファイルをマッピングします。 これは、カスタムワークフロー契約書作成リクエストの場合に指定する必要があります。</p> </li> 
         <li> <p><b>[!UICONTROL ページ数 ]</b> </p> <p>ドキュメント内のページ数を入力またはマッピングします。</p> </li> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>元のファイルの MIME タイプを入力またはマッピングします。 多目的インターネットメール拡張 (MIME) タイプは、ソフトウェアがインターネットで共有される様々なタイプのデータを識別できるラベルです。 Web サーバーおよびブラウザーは、MIME タイプを使用して、ファイルに対して何を実行するかを決定します。 例えば、MIME タイプがのファイル <code>text/html</code> は、MIME タイプがのファイルとは異なる方法でブラウザーで処理されます <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>ドキュメントの名前を入力またはマッピングします。<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL ライブラリドキュメント ID]</b> </p> <p>ライブラリドキュメントの ID を入力</p> </li> 
       <li> <p><b>[!UICONTROL 一時的なドキュメント ID]</b> </p> <p>一時的なドキュメントの ID を入力</p> </li> 
       <li> <p><b>[!UICONTROL URL ファイル転送 ]</b> </p> <p>次のフィールドに入力します。</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Mime-Type]</b> </p> <p>元のファイルの MIME タイプを入力します。 多目的インターネットメール拡張 (MIME) タイプは、ソフトウェアがインターネットで共有される様々なタイプのデータを識別できるラベルです。 Web サーバーおよびブラウザーは、MIME タイプを使用して、ファイルに対して何を実行するかを決定します。 例えば、MIME タイプがのファイル <code>text/html</code> は、MIME タイプがのファイルとは異なる方法でブラウザーで処理されます <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>ファイル名を入力します。</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>送信するファイルの URL を入力します。</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL ラベル ]</b> </p> <p>ファイルのラベルを入力します。</p> </li> 
     <li> <p><b>[!UICONTROL 認証</b> </p> <p>ファイルを認証する必要があることを示すには、このオプションを有効にします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 契約名 ]</td> 
   <td>新しい契約の名前を入力します。 この名前は、E メールや Web サイトなどの場所での契約を識別するために使用されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 参加者セット情報 ]</td> 
   <td> <p>追加する各参加者セットに対して、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL メンバー ]</b> </p> <p>参加者セットに追加する各人に対して、 <b>[!UICONTROL 項目を追加 ]</b> ユーザーのメールアドレスを入力します。</p> </li> 
     <li> <p><b>[!UICONTROL 順序 ]</b> </p> <p>この参加者セットが契約に署名する順序を指定します。 例えば、注文値が 1 の参加者グループは最初に署名し、2 は次に署名する必要があります。 注文番号は 1 から始まる必要があり、系列に隙間はありません。 </p> </li> 
     <li> <p><b>[!UICONTROL ロール ]</b> </p> <p>この参加者セットの役割を選択します。 セット内のすべての参加者がこの役割を受け取ります。</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>この参加者セットの ID を入力またはマッピングします。</p> </li> 
     <li> <p><b>[!UICONTROL ラベル ]</b> </p> <p>参加者セットの一意のラベルを入力またはマッピングします。 カスタムワークフローの場合、パーティシペーションセットで指定されたラベルで、カスタムワークフローのパーティシペーションステップにマッピングする必要があります。</p> </li> 
     <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>参加者セットの名前を入力します。 この名前は、契約内で一意である必要があります。</p> </li> 
     <li> <p><b>[!UICONTROL プライベートメッセージ ]</b> </p> <p>この参加者セットのメッセージを入力またはマッピングします。 セット内のすべての参加者がこのメッセージを受け取ります。</p> </li> 
     <li> <p><b>[!UICONTROL 表示されるページ ]</b> </p> <p>この免除承諾に対してドキュメントの表示制限が有効な場合は、この参加者セットに表示するファイルを指定します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 署名タイプ ]</td> 
   <td> <p>契約に必要な署名のタイプを選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-sign]</b> </p> <p>契約は電子署名が必要です。</p> </li> 
     <li> <p><b>[!UICONTROL 書き込み済み ]</b> </p> <p>契約は手動で署名する必要があり、署名済みの契約はスキャンされ、アップロードされる必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 状態 ]</td> 
   <td> <p>この契約の州を選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL オーサリング ]</b> </p> <p>この契約には、フィールドを編集または追加することができます。</p> </li> 
     <li> <p><b>[!UICONTROL 下書き ]</b> </p> <p>この契約は、送信前に段階的に作成できます。</p> </li> 
     <li> <p><b>[!UICONTROL 処理中 ]</b> </p> <p>この契約は直ちに送信されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CCs]</td> 
   <td> <p>関係者など、署名する必要のない関係者に対して、この契約を送信できます。 署名プロセスの開始時に電子メールを受信し、最終署名を受信すると別の電子メールを受信します。 また、契約書のPDFコピーも受け取ります。 </p> <p>この契約に CC する各担当者に対して、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 電子メール ]</b> </p> <p>契約の CC を受け取る電子メールアドレスを入力またはマッピングします。</p> </li> 
     <li> <p><b>[!UICONTROL ラベル ]</b> </p> <p>ワークフローの説明に示すように、この電子メールアドレスのラベルを入力またはマップします</p> </li> 
     <li> <p><b>[!UICONTROL 表示されるページ ]</b> </p> </li> 
     <li> <p>この免除承諾に対してドキュメントの表示制限が有効な場合は、この参加者セットに表示するファイルを指定します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 電子メールオプション ]</td> 
   <td> <p>電子メールのタイプごとに、そのタイプの電子メールをすべての参加者に送信するかどうかを選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 完了電子メール ]</b> </p> <p>この契約が完了、キャンセル、期限切れ、または拒否されたら電子メールを送信します。</p> </li> 
     <li> <p><b>[!UICONTROL インフライトメール ]</b> </p> <p>この契約が委任または置き換えられたときに、電子メールを送信しました。</p> </li> 
     <li> <p><b>[!UICONTROL 契約の開始電子メール ]</b> </p> <p>この契約が作成されたとき、または契約に対するアクションがリクエストされたときに電子メールを送信します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 外部 ID]</td> 
   <td> <p>この契約の ID を入力またはマッピングします。 免除承諾の作成時にこれを指定し、後のモジュールまたは問い合わせで免除承諾を検索する際に使用できます。</p> <p>注意：外部 ID 値は API を通じてすべての参加者に表示されるので、機密トークンを含めるために使用しないでください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド情報を結合 ]</td> 
   <td> <p>デフォルト値を設定する契約の各フィールドで、 <b>[!UICONTROL 項目を追加 ]</b> デフォルト値とフィールド名を入力します。</p> <p>値は、編集可能フィールドの署名者に表示されます。読み取り専用フィールドの場合、指定された値は署名プロセス中に編集できません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 公証情報 ]</td> 
   <td> <p>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 予定 ]</b> </p> <p>この契約を公表する予定の日時を入力またはマッピングします。</p> </li> 
     <li> <p><b>[!UICONTROL メモ ]</b> </p> <p>公証会議に関して含めるメモを入力またはマッピングします。</p> </li> 
     <li> <p><b>[!UICONTROL 支払い ]</b> </p> <p>公証人が署名者に支払われるか、契約の送信者に支払われるかを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL 公証型 ]</b> </p> <p>公証人のタイプを選択</p> 
      <ul> 
       <li> <p>[!UICONTROL プロバイダー公証人 ]</p> <p>公証人は公証人の提供者によって提供される。</p> </li> 
       <li> <p>[!UICONTROL BYON 公証人 ]</p> <p>公証人は顧客から提供される。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 署名後オプション ]</td> 
   <td> <p>契約の署名後に成功ページに署名者を誘導するかどうかを選択します。 次を選択した場合、 <b>[!UICONTROL はい ]</b>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL リダイレクト遅延 ]</b> </p> <p>署名者が成功ページにリダイレクトされるまでの秒数を入力またはマッピングします。 この値が 0 より大きい場合、最初に標準 [!DNL Adobe Sign] 成功メッセージの送信後、遅延後は成功ページにリダイレクトされます。</p> </li> 
     <li> <p><b>[!UICONTROL リダイレクト URL]</b> </p> <p>署名プロセスが正常に完了した後にユーザーが送信する、公開アクセス可能な URL を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL セキュリティオプション ]</td> 
   <td> <p>パスワードドキュメントの保護に使用するセカンダリPDFを入力またはマッピングします。 </p> <p>重要： [!DNL Adobe Sign] ではこのパスワードを共有しないので、関係者に別途伝える必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vaulting info]</td> 
   <td>アカウントがドキュメントヴォールティング用に設定され、契約ごとに有効にするオプションがある場合、このオプションを有効にしてこの契約をヴォールトできます。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 関連レコードの作成]**

このアクションモジュールは、選択したモジュールにリンクされたレコードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>作成したレコードを関連付ける元のレコードのレコードタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>作成したレコードを関連付けるオブジェクトの ID を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 契約関連フィールド ]</td> 
   <td> <p>作成する関連フィールドのタイプを選択します</p> 
    <ul> 
     <li> <p><b>[!UICONTROL フォームフィールド ]</b> </p> <p>作成するフィールドを含むテンプレートのテンプレート ID を入力します</p> </li> 
     <li> <p><b>[!UICONTROL リマインダー ]</b> </p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 受信者参加者 ID]</b> </p> <p>リマインダーを受け取る参加者ごとに、「[!UICONTROL 項目を追加 ]」をクリックし、参加者の ID を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL ステータス ]</b> </p> <p>新しいレコードの場合、ステータスは [!UICONTROL アクティブ ] である必要があります。</p> </li> 
       <li> <p><b>[!UICONTROL 最初のリマインダーの遅延 ]</b> </p> <p>最初のリマインダーを送信するまでの遅延時間を時間単位で入力します。 許可される最小値は 1 時間で、最大値は契約の作成と有効期限の時間の差を超えることはできません（時間単位）。 この遅延を設定しない場合、最初のリマインダーは頻度に基づいておこなわれます。</p> </li> 
       <li> <p><b>[!UICONTROL リマインダーの頻度 ]</b> </p> <p>リマインダーを送信する頻度を設定します。 頻度を指定しない場合、リマインダーは 1 回だけ送信されます。</p> </li> 
       <li> <p><b>[!UICONTROL 最終送信日 ]</b> </p> <p>このフィールドはシステムによって設定されます。</p> </li> 
       <li> <p><b>[!UICONTROL 次回送信日 ]</b> </p> <p>このフィールドは空白にするか、[!UICONTROL ONCE] に設定する必要があります。</p> </li> 
       <li> <p><b>[!UICONTROL メモ ]</b> </p> <p>リマインダーに含めるメモを入力します。 これは、参加が必要な理由を参加者に伝えるのに役立ちます。</p> </li> 
       <li> <p><b>[!UICONTROL リマインダー開始カウンター ]</b> </p> <p>リマインダーを送信するタイミングを、使用可能になった時点で契約が作成されるタイミングに基づいて選択します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL 署名者の ID レポート ]</b> </p> <p>パスワードドキュメントの保護に使用するPDFを入力します。</p> </li> 
     <li> <p><b>[!UICONTROL 表示 ]</b> </p> <p>次のフィールドを入力します</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>作成するビューの名前を選択します。</p> </li> 
       <li> <p><b>[!UICONTROL 自動ログインユーザー ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> を使用して、返された URL にユーザーを自動的にログインします。</p> </li> 
       <li> <p><b>[!UICONTROL フレームの親 ]</b> </p> <p>返された URL をフレーム化できる親ドメイン URL のコンマ区切りリストを入力またはマッピングします。 空白の場合、 [!DNL Adobe Acrobat Sign] iframe でページを表示できません。</p> </li> 
       <li> <p><b>[!UICONTROL ロケール ]</b> </p> <p>ビューを作成する言語を入力します。 </p> </li> 
       <li> <p><b>[!UICONTROL Chrome フラグなし ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ナビゲーションヘッダーやフッターを含めずに埋め込みページを表示する。</p> </li> 
       <li> <p><b>[!UICONTROL ファイルを編集できます ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ファイルを追加または削除して、ファイルのアップロードセクションを編集する場合。 これはアクセス制御マシンではありません。 デフォルト値は [!UICONTROL はい ] です。</p> </li> 
       <li> <p><b>[!UICONTROL ライブラリドキュメント ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ライブラリドキュメントのリンクを表示する場合。 デフォルト値は [!UICONTROL はい ] です。</p> </li> 
       <li> <p><b>[!UICONTROL ローカルファイル ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ローカルファイルのアップロードボタンを表示する場合。 デフォルト値は [!UICONTROL はい ] です。</p> </li> 
       <li> <p><b>[!UICONTROL Web コネクタ ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> web ソースからドキュメントを添付するリンクを表示する場合。 デフォルトははいです。</p> </li> 
       <li> <p><b>[!UICONTROL プレビューが選択されています ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> 「構成」ページを「オーサリング」モードに設定する場合。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL メンバー共有 ]</b> </p> <p>契約を共有する各メンバーに対して、 <b>[!UICONTROL 項目を追加 ]</b> メンバーのメールアドレスと、そのメンバーに対するメッセージを入力します。</p> </li> 
     <li> <p>[!UICONTROL 参加者セットを委任 ]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 参加者セット ID]</b> </p> <p>参加者セットの ID を入力</p> </li> 
       <li> <p><b>[!UICONTROL メンバー情報 ]</b> </p> <p>追加する各メンバーに対して、[!UICONTROL 項目の追加 ] をクリックし、そのメンバーの電子メールアドレスと電話情報を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL プライベートメッセージ ]</b> </p> <p>メッセージを入力します。 このメッセージは、参加者セットのすべてのメンバーが受け取ります。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ライブラリビュー情報 ]</td> 
   <td> <p>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>ライブラリテンプレートの名前を入力します。 この名前は、E メールや Web サイトで使用されます。</p> </li> 
     <li> <p><b>[!UICONTROL 自動ログインユーザー ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> を使用して、返された URL にユーザーを自動的にログインします。</p> </li> 
     <li> <p><b>[!UICONTROL フレームの親 ]</b> </p> <p>返された URL をフレーム化できる親ドメイン URL のコンマ区切りリストを入力またはマッピングします。 空白の場合、 [!DNL Adobe Acrobat Sign] iframe でページを表示できません。</p> </li> 
     <li> <p><b>[!UICONTROL ロケール ]</b> </p> <p>ビューを作成する言語を入力します。 </p> </li> 
     <li> <p><b>[!UICONTROL Chrome フラグなし ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ナビゲーションヘッダーやフッターを含めずに埋め込みページを表示する。</p> </li> 
     <li> <p><b>[!UICONTROL ビュー設定を送信 ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> [!UICONTROL 送信 ] ビューを設定する場合は、次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 契約名 ]</b> </p> <p>作成ページでライブラリドキュメントの契約名を入力またはマッピングします。</p> </li> 
       <li> <p><b>[!UICONTROL ファイルを編集できます ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ファイルを追加または削除して、ファイルのアップロードセクションを編集する場合。 これはアクセス制御マシンではありません。 デフォルト値は [!UICONTROL はい ] です。</p> </li> 
       <li> <p><b>[!UICONTROL ローカルファイル ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ライブラリドキュメントのリンクを表示する場合。 デフォルト値は [!UICONTROL はい ] です。</p> </li> 
       <li> <p><b>[!UICONTROL Web コネクタ ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> web ソースからドキュメントを添付するリンクを表示する場合。 デフォルト値は [!UICONTROL はい ] です。</p> </li> 
       <li> <p><b>プレビューが選択されている</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> 「構成」ページを「オーサリング」モードに設定する場合。</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ユーザー表示情報 ]</td> 
   <td> <p>次のフィールドに入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>要求したユーザービューの名前を選択します。</p> </li> 
     <li> <p><b>[!UICONTROL 自動ログインユーザー ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> をクリックして、ユーザーを自動的にログインします。 選択 <b>[!UICONTROL いいえ ]</b> 認証情報が必要です。 デフォルト値は [!UICONTROL No] です。</p> </li> 
     <li> <p><b>[!UICONTROL フレームの親 ]</b> </p> <p>返された URL をフレーム化できる親ドメイン URL のコンマ区切りリストを入力またはマッピングします。 空白の場合、 [!DNL Adobe Acrobat Sign] iframe でページを表示できません。</p> </li> 
     <li> <p><b>クロムフラグなし</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ナビゲーションヘッダーやフッターを含めずに埋め込みページを表示する。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ウィジェット関連のフィールド ]</td> 
   <td> <p>作成する関連レコードを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL 表示 ]</p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>要求する Web フォームビューの名前を選択</p> </li> 
       <li> <p><b>[!UICONTROL 自動ログインユーザー ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> をクリックして、ユーザーを自動的にログインします。 選択 <b>[!UICONTROL いいえ ]</b> 認証情報が必要です。 デフォルト値は [!UICONTROL No] です。</p> </li> 
       <li> <p><b>[!UICONTROL フレームの親 ]</b> </p> <p>返された URL をフレーム化できる親ドメイン URL のコンマ区切りリストを入力またはマッピングします。 空白の場合、 [!DNL Adobe Acrobat Sign] iframe でページを表示できません。</p> </li> 
       <li> <p><b>[!UICONTROL ロケール ]</b> </p> <p>ビューを作成する言語を入力します。 </p> </li> 
       <li> <p><b>[!UICONTROL Chrome フラグなし ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> ナビゲーションヘッダーやフッターを含めずに埋め込みページを表示する。</p> </li> 
       <li> <p>[!UICONTROL パーソナライズされた署名表示設定 ]</p> <p>パーソナライズされた署名表示を設定する場合は、 <b>[!UICONTROL はい ]</b> 次のフィールドに入力します。</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 電子メール ]</b> </p> <p>新しく作成された Web フォームを受け取る人の電子メールアドレスを入力</p> </li> 
         <li> <p><b>[!UICONTROL コメント ]</b> </p> <p>API 呼び出し元が署名者の ID を確立した方法を説明するコメントを入力します。 この情報は、 [!DNL Adobe Acrobat Sign] 監査証跡。</p> </li> 
         <li> <p><b>[!UICONTROL の有効期限 ]</b> </p> <p>この Web フォームのパーソナライゼーションの有効期限を入力します。 </p> <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL 再利用可能 ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> 署名者が複数回フォームに署名できるようにする場合。</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL メンバー共有 ]</b> </p> <p>契約を共有する各メンバーに対して、 <b>[!UICONTROL 項目を追加 ]</b> メンバーのメールアドレスと、そのメンバーに対するメッセージを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL カスタム API 呼び出し]**
このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力 <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>注意：使用可能なエンドポイントの一覧については、 [!DNL Adobe Sign] API リファレンス。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ] </td> 
   <td> <p>リクエストクエリ文字列を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 一時的なドキュメントのアップロード ]</td> 
   <td> <p>一時的なドキュメントをアップロードする場合は、アップロードするドキュメントのソースファイルを入力します。</p> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL レコードのリスト]**

このアクションモジュールは、アカウントがアクセスできる選択したタイプのすべてのレコードを一覧表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>関連レコードを取得するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ロケール ]</td> 
   <td> <p>ユーザーのロケールを入力します。 UI の言語を決定します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 外部 ID]</td> 
   <td>外部 ID( [!DNL Adobe Acrobat Sign]) を使用して、返信する契約に使用します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group ID]</td> 
   <td>リストするレコードに関連付けられたグループの ID を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 非表示（レコード）を表示 ]</td> 
   <td>結果に非表示のレコードを含める場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Start index]</td> 
   <td> <p>モジュールが返す最初のレコードの数を入力します。 </p> <p>注意：このフィールドは、ページネーション用に「返されるレコードの最大数」フィールドと組み合わされます。 例えば、[!UICONTROL 返されるイベントの最大数 ] が 100 で、[!UICONTROL 開始インデックス ] が 101 の場合、モジュールはレコード 101 ～ 200、または結果の 2 ページ目を返します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返されるレコードの最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが [action] に設定するレコードの最大数を入力またはマッピングします。</p> <p>注意：このフィールドは、ページネーション用に [!UICONTROL Cursor] または [!UICONTROL Start Index] フィールドと組み合わせられます。 例えば、[!UICONTROL 返されるイベントの最大数 ] が 100 で、[!UICONTROL 開始インデックス ] が 101 の場合、モジュールはレコード 101 ～ 200、または結果の 2 ページ目を返します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 親ドメイン URL]</td> 
   <td> <p>返された URL をフレーム化できる親ドメイン URL のコンマ区切りリストを入力またはマッピングします。 空白の場合、 [!DNL Adobe Acrobat Sign] iframe でページを表示できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL レコードを読み取る]**

このアクションモジュールは、1 つのレコードから情報を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>関連レコードを取得するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコード ID]</td> 
   <td>取得するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 関連レコードの読み取り]**

1 つのレコードに関する追加情報を読み取ります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>関連レコードを取得するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコード ID] ( 例：[!UICONTROL アカウント ID])</td> 
   <td>関連レコードを取得するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL その他のフィールド ]</td> 
   <td>レコードタイプおよび関連するフィールドに基づいて、特定のフィールドに情報を入力します。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL レコードの更新]**

このアクションモジュールは、 [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* ベストプラクティスとして、契約に大幅な変更を予想する場合は、既存の契約を更新するのではなく、新しい契約を作成することをお勧めします。
>* 一部の更新では、必須フィールドが使用されます。 更新を設定する際は、必ずすべての必須フィールドに入力してください。 必須フィールドは太字で示されています。 [!DNL Workfront Fusion] モジュール。
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコード ID] </td> 
   <td>更新するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>更新するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL その他のフィールド ]</td> 
   <td> <p>レコードタイプおよび関連するフィールドに基づいて、特定のフィールドに情報を入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 契約 ]</b> </p> <p>ベストプラクティスとして、契約に大幅な変更を予想する場合は、既存の契約を更新するのではなく、新しい契約を作成することをお勧めします。</p> </li> 
     <li> <p><b>[!UICONTROL ライブラリドキュメント ]</b> </p> <p>更新するフィールドを選択し、選択したフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL ステータス ]</b> </p> <p>ライブラリドキュメントの新しいステータスを選択します。</p> </li> 
       <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>ライブラリテンプレートの名前を入力またはマッピング</p> </li> 
       <li> <p><b>[!UICONTROL 共有モード ]</b> </p> <p>ライブラリドキュメントへのアクセス権を持つユーザーを指定します。</p> </li> 
       <li> <p><b>[!UICONTROL ライブラリテンプレートタイプ ]</b> </p> <p>使用するライブラリテンプレートタイプごとに、 <b>[!UICONTROL 項目を追加 ]</b> をクリックし、テンプレートタイプを選択します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL ユーザー ]</b> </p> <p>更新するフィールドを選択し、選択したフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 名 ]</b> </p> <p>ユーザーの名を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL 姓 ]</b> </p> <p>ユーザーの姓を入力</p> </li> 
       <li> <p><b>[!UICONTROL 会社 ]</b> </p> <p>ユーザーの会社名を入力します。</p> </li> 
       <li> <p><b>[!UICONTROL Phone]</b> </p> <p>ユーザーの電話番号を入力</p> </li> 
       <li> <p><b>[!UICONTROLプライマリグループ ID]</b> </p> <p>新しいユーザーを追加するグループを入力します。 何も入力しなかった場合、ユーザーはアカウントのデフォルトのグループに追加されます。</p> </li> 
       <li> <p><b>[!UICONTROL ジョブのタイトル ]</b> </p> <p>ユーザーの役職を入力します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web フォーム ] （[!UICONTROL ウィジェット ]）</b> </p> <p>レコードタイプおよび関連するフィールドに基づいて、特定のフィールドに情報を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 関連レコードを更新]**

このアクションモジュールは、特定のオブジェクトに関連するレコードを更新します。

>[!IMPORTANT]
>
>* ベストプラクティスとして、契約に大幅な変更を予想する場合は、既存の契約を更新するのではなく、新しい契約を作成することをお勧めします。
>* 一部の更新では、必須フィールドが使用されます。 更新を設定する際は、必ずすべての必須フィールドに入力してください。 必須フィールドは太字で示されています。 [!DNL Workfront Fusion] モジュール。
>




<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>関連するフィールドが関連付けられているレコードのレコードタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>作成したレコードを関連付けるオブジェクトの ID を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL その他のフィールド ]</td> 
   <td> <p>レコードタイプおよび関連するフィールドに基づいて、特定のフィールドに情報を入力します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 契約 ]</b> </p> <p>ベストプラクティスとして、契約に大幅な変更を予想する場合は、既存の契約を更新するのではなく、新しい契約を作成することをお勧めします。</p> </li> 
     <li> <p><b>[!UICONTROL ライブラリドキュメント ]</b> </p> <p>更新するフィールドを選択し、選択したフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL 状態 ]</b> </p> <p>ライブラリドキュメントの新しいステータスを選択します。</p> </li> 
       <li> <p><b>[!UICONTROL メモ ]</b> </p> <p>注記のテキストを入力またはマッピングします。</p> </li> 
       <li> <p><b>[!UICONTROL 表示 ]</b> </p> <p>ライブラリドキュメントを表示するか、ガイダーするかを選択します。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL ユーザー ]</b> </p> <p>更新するフィールドを選択し、選択したフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL グループ情報リスト ]</b> </p> <p>次のフィールドに入力します。</p> 
        <ul> 
         <li> <p><b>[!UICONTROL ステータス ]</b> </p> <p>ユーザーの新しいステータスを選択します。</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>グループの一意の ID を入力</p> </li> 
         <li> <p><b>[!UICONTROL はグループ管理者です ]</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> このユーザーをグループ管理者にします。</p> </li> 
         <li> <p><b>プライマリグループ</b> </p> <p>選択 <b>[!UICONTROL はい ]</b> をクリックして、このグループをユーザーのプライマリグループに更新します。</p> </li> 
         <li> <p><b>[!UICONTROL 作成日 ]</b> </p> <p>グループの作成日を入力します。</p> <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion] での型強制</a>.</p> </li> 
         <li> <p><b>[!UICONTROL 名前 ]</b> </p> <p>グループの名前を入力またはマッピングします。</p> </li> 
         <li> <p><b>[!UICONTROL ライブラリドキュメントの作成が表示される ]</b> </p> <p>これらの設定は、ユーザーがライブラリドキュメントを作成できるかどうかを決定します</p> 
          <ul> 
           <li> <p>[!UICONTROL 値 ]</p> <p>許可</p> </li> 
           <li> <p>[!UICONTROL 継承 ]</p> <p>グループまたはアカウントからグループ設定を継承</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL 送信はワークフローに制限されます ]</b> </p> <p>これらの設定は、ユーザーがワークフローを使用してのみ契約を作成できるかどうかを決定します。</p> 
          <ul> 
           <li> <p>[!UICONTROL 値 ]</p> <p>許可</p> </li> 
           <li> <p>[!UICONTROL 継承 ]</p> <p>グループまたはアカウントからグループ設定を継承</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL ユーザーが送信可能 ]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL 値 ]</p> <p>許可</p> </li> 
           <li> <p>[!UICONTROL 継承 ]</p> <p>グループまたはアカウントからグループ設定を継承</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL 状態 ]</b> </p> <p>ユーザーの新しい状態を選択し、ユーザーをアクティベートまたはアクティベート解除する理由に関するコメントを入力します。</p> </li> 
       <li> <p><b>[!UICONTROL ロケール ]</b> </p> <p>ユーザーのロケールを入力します。 UI の言語を決定します。 </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Web フォーム ] （[!UICONTROL ウィジェット ]）</b> </p> <p>レコードタイプおよび関連するフィールドに基づいて、特定のフィールドに情報を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL ドキュメントをアップロード]**

一時的なドキュメントをアップロードします。 一時的なドキュメントは、アップロード後 7 日間使用できます。

>[!NOTE]
>
>ドキュメントをアップロードして一時的なドキュメントとして署名し、そのドキュメントを「契約の作成」モジュールの「送信するファイル」フィールドにマッピングすることをお勧めします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコード ID]</td> 
   <td>更新するレコードの ID を入力またはマッピングします</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td>元のファイルの MIME タイプを入力します。 多目的インターネットメール拡張 (MIME) タイプは、ソフトウェアがインターネットで共有される様々なタイプのデータを識別できるラベルです。 Web サーバーおよびブラウザーは、MIME タイプを使用して、ファイルに対して何を実行するかを決定します。 例えば、MIME タイプがのファイル <code>text/html</code> は、MIME タイプがのファイルとは異なる方法でブラウザーで処理されます <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**例：** このワークフローでは、( 以前にWorkfrontからダウンロードした ) 署名するドキュメントが一時的なドキュメントとしてアップロードされます。

![](assets/sign-example-1-350x308.png)

この [!UICONTROL ドキュメントをアップロード] モジュールは、ドキュメントに [!DNL Adobe Acrobat Sign] 後のモジュールで参照できる ID。 契約が作成されると、アップロードされたドキュメントの ID が [!UICONTROL 送信するファイル] フィールドに入力します。

![](assets/sign-example-2-350x356.png)

+++

### 検索

+++ **[!UICONTROL 契約を検索]**

この検索モジュールでは、指定した基準に基づいて基本契約が検索されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Adobe Acrobat Sign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テキストフィルター ]</td> 
   <td> <p>契約メタデータ内のテキストを検索します。 </p> 
    <ul> 
     <li> <p><b>[!UICONTROL テキストを検索 ]</b> </p> <p>契約メタデータで検索するテキストを入力します。 各単語は、別々のテキスト項目として扱われます。 </p> </li> 
     <li> <p><b>[!UICONTROL [!UICONTROL] でのテキストの検索</b> </p> <p>テキストを検索するメタデータフィールドを選択します。 何も選択しない場合、モジュールはすべてのメタデータを検索します。</p> </li> 
    </ul> <p>モジュールは、選択したフィールドのいずれかに入力されたテキストを含む契約を返します。 例：「春のキャンペーン」を入力し、「タイトル」および「メモ」オプションを選択すると、「タイトル」または「メモ」で「春」または「キャンペーン」という単語を含む契約が返されます。</p> <p>でのフィールドの検索の詳細 [!DNL Adobe Acrobat Sign](「テキスト検索の仕組み」( <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] 検索 — 仕組み</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 作成日 ]</td> 
   <td>日付を選択します。 このモジュールは、作成された日付がこの条件と一致するレコードのみを返します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 有効期限 ]</td> 
   <td>日付を選択します。 このモジュールは、有効期限がこの条件と一致するレコードのみを返します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL 変更日 ]</p> </td> 
   <td>日付を選択します。 このモジュールは、変更された日付がこの条件と一致するレコードのみを返します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 外部 ID]</td> 
   <td> <p> 外部 ID は、契約に送信者が割り当てた ID で、どの形式でもかまいませんが、通常は「&lt;groupid&gt;:&lt;id&gt;".</p> <p>追加する外部 ID ごとに、 <b>[!UICONTROL 追加 ]</b> 外部 ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group ID]</td> 
   <td> <p>グループ ID は、グループの作成時に割り当てられた識別子です。</p> <p>追加する外部 ID ごとに、 <b>[!UICONTROL 追加 ]</b> 外部 ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>これは、特定の契約に割り当てられた ID です。 </p> <p>追加する外部 ID ごとに、 <b>[!UICONTROL 追加 ]</b> 外部 ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 親 ID]</td> 
   <td> <p>これは、免除承諾の親オブジェクトに割り当てられる ID です。 </p> <p>追加する外部 ID ごとに、 <b>[!UICONTROL 追加 ]</b> 外部 ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 参加者電子メール ]</td> 
   <td> <p>参加者の電子メールアドレス。 </p> <p>追加する外部 ID ごとに、 <b>[!UICONTROL 追加 ]</b> 外部 ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ロール ]</td> 
   <td>返された結果に含めるロールを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td> 
   <td>モジュールで結果を並べ替える場合は、結果の並べ替えに使用するフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え順序 ]r</td> 
   <td>モジュールで結果を並べ替える場合は、昇順と降順のどちらで並べ替えるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ステータス ]</td> 
   <td>返された結果に含めるステータスを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ]</td> 
   <td>返された結果に含める基本契約タイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サブタイプ ]</td> 
   <td>返された結果に含める基本契約サブタイプを選択します。 ライブラリテンプレート協定機能のサブタイプのみ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User ID]</td> 
   <td> <p>契約の共有先となるユーザーのユーザー ID。</p> <p>追加する各ユーザー ID に対して、 <b>[!UICONTROL 追加 ]</b> ユーザー ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示 ]</td> 
   <td>返された結果に含める表示レベルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始インデックス ]</td> 
   <td> <p>返す最初の結果の位置を入力します。 これを [!UICONTROL 返される結果の最大数 ] と組み合わせて、結果をページ番号付けします</p> <p>例：一度に 100 個の結果を返す場合は、100 と入力して結果 100-200 を返します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返される結果の最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが [action] に設定するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
