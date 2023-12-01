---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Devtool でのシナリオのデバッグ
description: Adobe Workfront Fusion Devtool を使用すると、シナリオを理解し、トラブルシューティングできます。 開発ツールは、Chrome Developer Tools にパネルを追加します。 このデバッガーパネルを使用すると、シナリオのすべての手動実行を確認し、実行されたすべての操作を確認し、実行されたすべての API 呼び出しの詳細を確認できます。 エラーが発生したモジュール、操作、または単一の応答を確認し、その知識を使用してシナリオを絞り込むことができます。
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 82ff5d2731c981c89eb02c86d6d6eddc5d87dec7
workflow-type: tm+mt
source-wordcount: '1799'
ht-degree: 1%

---

# でのシナリオのデバッグ [!DNL Adobe Workfront Fusion] 開発者ツール

The [!DNL Adobe Workfront Fusion] 開発者ツールを使用すると、シナリオを理解し、トラブルシューティングできます。 開発ツールは、 [!DNL Chrome Developer Tools]. このデバッガーパネルを使用すると、シナリオのすべての手動実行を確認し、実行されたすべての操作を確認し、実行されたすべての API 呼び出しの詳細を確認できます。 エラーが発生したモジュール、操作、または単一の応答を確認し、その知識を使用してシナリオを絞り込むことができます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td>    </tr> 
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

## Workfront Fusion Devtool へのアクセス

Devtool へのアクセスは、Fusion を [!DNL Adobe Unified Experience].

* [の開発ツールにアクセスします。 [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [クラシックの開発ツールにアクセスする [!DNL Fusion] エクスペリエンス](#access-the-devtool-in-the-classic-fusion-experience)

### の開発ツールにアクセスします。 [!DNL Adobe Unified Experience]

統合シェルAdobeで Fusion を使用する場合は、シナリオエディタから開発ツールにアクセスできます。

1. デバッグするシナリオのシナリオエディターに移動します。

   シナリオエディタを見つけるには、 [シナリオエディター](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. ページの空の領域（モジュール上ではなく）を右クリックします。
1. 選択 **開発者ツールを開く**.

### クラシックの開発ツールにアクセスする [!DNL Fusion] エクスペリエンス

クラシックの開発ツールを使用するには [!DNL Fusion] エクスペリエンスの場合は、 [!DNL Chrome] 拡張子。 その後、この拡張機能は、 [!DNL Chrome] 開発者ツール。

* [インストール [!DNL Chrome] Devtool 拡張機能](#install-the-chrome-devtool-extension)
* [次を見つけます。 [!DNL Workfront Fusion] 開発者ツール](#locate-the-workfront-fusion-devtool)

#### をインストールします。 [!DNL Chrome] Devtool 拡張機能

次の項目を追加できます。 [!DNL Workfront Fusion] 開発ツール [!DNL Chrome] から [!UICONTROL [!DNL Chrome] Web ストア].

1. クリック [このリンク](https://chrome.google.com/webstore/detail/workfront-fusion-Devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn/related) に行く [!DNL Workfront Fusion] の開発ツール [!UICONTROL [!DNL Chrome] Web ストア].
1. クリック **[!UICONTROL 追加先[!DNL Chrome]]**.
1. 表示されるウィンドウで、権限を確認します。 権限に同意する場合は、 **[!UICONTROL 拡張機能を追加]**.

The [!DNL Workfront Fusion] Devtool 拡張機能が [!DNL Chrome] 拡張機能。


#### 次を見つけます。 [!DNL Workfront Fusion] 開発者ツール

次の手順で [!DNL Workfront Fusion] 開発者ツール、 [!DNL Workfront Fusion] Devtool 拡張機能を [!DNL Chrome] ブラウザ、 [Chrome Devtool 拡張機能のインストール](#install-the-chrome-Devtool-extension).

1. を開きます。 [!DNL Workfront Fusion] シナリオ。
1. 開く [!DNL Chrome Developer Tools]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl + Shift + I</p> <p> または </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >をドッキングすることをお勧めします。 [!DNL Chrome Developer Console] を下に移動して、モジュールの表示を改善します。

1. 次をクリック： **[!DNL Workfront Fusion]** タブ [!DNL Chrome Dev Tools].

## 以下を使用します。 [!DNL Workfront Fusion] 開発者ツール

Workfront Fusion Devtool は、3 つの主なセクションに分かれています。 これらは、Devtool ウィンドウの左側のパネルにあります。

* [Live Stream](#live-stream)
* [シナリオデバッガー](#scenario-debugger)
* [ツール](#tools)

### Live Stream

Live Stream は、シナリオで「1 回実行」をクリックすると、バックグラウンドで発生していることを表示します。

1. 次をクリック： **[!UICONTROL Live Stream]** アイコン ![](assets/live-stream-icon.png) をクリックして、「Live Stream」セクションを開きます。
1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>アクション</th> 
      <th>手順</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">リクエスト情報の表示</td> 
      <td> <p>シナリオの各モジュールに関する次の情報を表示できます</p> 
       <ul> 
        <li> <p>リクエストヘッダー（API エンドポイント URL、http メソッド、リクエストが呼び出された日時、リクエストヘッダー、クエリ文字列）</p> </li> 
        <li> <p>リクエスト本文</p> </li> 
        <li> <p>応答ヘッダー</p> </li> 
        <li> <p>応答本文</p> </li> 
       </ul> <p>この情報を表示するには、 [!DNL Workfront Fusion] 開発者ツール。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>リクエストと応答を検索</p> </td> 
      <td> <p>検索語句を、 [!DNL Workfront Fusion] 検索語を含むリクエストのみを表示する開発ツール。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>リクエストのリストを削除 </p> </td> 
      <td> <p>開発者ツールの左パネルの右上隅にあるごみ箱アイコンをクリックして、 [!DNL Workfront Fusion] 開発者ツール。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>コンソールログを有効にする</p> </td> 
      <td> <p>コンピューターのアイコンをクリックします。 <img src="assets/console-computer-icon.png"> は、開発者ツールの左パネルの右上隅にあります。</p> <p>コンピュータのアイコンが緑の場合、コンソールでのログインは有効になります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>生の JSON 形式または cURL でのリクエストの取得</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>生の JSON</strong> </p> <p>クリック <strong>[!UICONTROL RAW をコピー ]</strong> をクリックします。</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>クリック <strong>[!UICONTROL cURL をコピー ]</strong> をクリックします。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### シナリオデバッガー

シナリオデバッガーは、より複雑なシナリオで役立ちます。 シナリオ実行の履歴が表示され、名前または ID でモジュールを検索できます。

1. 次をクリック： **[!UICONTROL シナリオデバッガー]** アイコン ![](assets/scenario-debugger-icon.png) をクリックして、シナリオデバッガーを開きます。
1. （オプション）検索語句（名前またはモジュール ID）を、 [!DNL Workfront Fusion] の開発ツール [!UICONTROL シナリオデバッガー] 」セクションに入力します。
1. モジュールの名前をダブルクリックして、シナリオエディターで設定を開きます。
1. 目的の操作をクリックして、リクエストの詳細を表示します。

### ツール

The [!DNL Workfront Fusion] 開発ツールには、シナリオの設定を容易にするツールが備わっています。

1. 次をクリック： **[!UICONTROL ツール]** アイコン ![](assets/console-tools-icon.png) をクリックして、ツールを開きます。
1. 使用するツールを選択します。
1. 以下に示すように、フィールドを設定します。
1. クリック **[!UICONTROL 実行]**.

ツールとそのフィールド：

* [モジュールのフォーカス](#focus-a-module)
* [マッピングによるモジュールの検索](#find-modules-by-mapping)
* [アプリのメタデータの取得](#get-app-metadata)
* [マッピングをコピー](#copy-mapping)
* [フィルターのコピー](#copy-filter)
* [接続をスワップ](#swap-connection)
* [スワップ変数](#swap-variable)
* [アプリをスワップ](#swap-app)
* [Base 64](#base-64)
* [モジュール名をコピー](#copy-module-name)
* [ソースを再マッピング](#remap-source)
* [アプリをハイライト](#highlight-app)
* [GS を移行](#migrate-gs)

#### [!UICONTROL モジュールのフォーカス]

ID で指定したモジュールの設定を開きます。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL モジュール ID]</td>
        <td>設定を開くモジュールの ID を入力します。</td>
    </tr>
</table>

#### [!UICONTROL マッピングによるモジュールの検索]

指定した用語のモジュールの値を検索できます。 出力には、検索した語句を含むモジュールの ID が含まれます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL キーワード ]</td> 
   <td> <p> 検索する語句を入力します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 値のみを使用 ]</p> </td> 
   <td> <p>モジュールフィールドの値のみを検索する場合は、このオプションを有効にします。</p> <p>モジュールフィールドの名前も検索するには、このオプションを無効にします。</p> <p>検索は、名前およびラベルパラメーターを使用して実行されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アプリのメタデータの取得]

アプリのモジュール名または ID でアプリのメタデータを取得します。 これは、例えば、シナリオで使用されるアプリのバージョンを知る必要がある場合に便利です。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ソースモジュール ]</td>
        <td>メタデータを取得するモジュールを選択します。</td>
    </tr>
</table>

#### [!UICONTROL マッピングをコピー]

値をソースモジュールからターゲットモジュールにコピーします。

>[!CAUTION]
>
>正しいソースモジュールとターゲットモジュールを設定していることを確認します。 別のタイプのモジュールを選択すると、ターゲットモジュール内の値が削除されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ]</td> 
   <td> <p> モジュールを選択するか、フィールド値のコピー元となるモジュールの ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target モジュール ]</p> </td> 
   <td> <p>モジュールを選択するか、ソースモジュール値を挿入するモジュールの ID を入力します。</p> <p>重要：ターゲットモジュール内の値は上書きされます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フィルターのコピー]

フィルター設定をソースモジュールからターゲットモジュールにコピーします。

>[!NOTE]
>
>コピー操作は、選択したモジュールの左側に配置されたフィルターに対して実行されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ]</td> 
   <td> <p> モジュールを選択するか、フィルター値のコピー元となるモジュールの ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target モジュール ]</p> </td> 
   <td> <p>モジュールを選択するか、ソースモジュールからフィルター値を挿入するモジュールの ID を入力します。</p> <p>重要：ターゲットモジュール内の値は上書きされます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フォールバックルート設定を保持 ]</p> </td> 
   <td> <p>ソースフィルターは、フォールバックルートとして設定されます。 このオプションを有効にすると、ターゲットフィルタがフォールバックルートとして設定されるようにも設定されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 接続をスワップ]

同じアプリのシナリオ内のすべてのモジュールに、ソースモジュールから接続を複製します。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ソースモジュール ]</td>
        <td>モジュールを選択するか、接続の複製元となるモジュールの ID を入力します。</td>
    </tr>
</table>

#### [!UICONTROL スワップ変数]

シナリオ内で指定した変数を検索し、新しい変数に置き換えます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索する変数 ]</td> 
   <td> <p> 置き換える変数ピルをシナリオのモジュールから探し、この（[!UICONTROL 変数を検索 ]）フィールドにコピーします。 「 」フィールドにはダブルカーリーで囲まれて表示されます。 例: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 置換文字列 ]</p> </td> 
   <td> <p>シナリオ内のモジュールで変数を置き換える変数ピルを探し、この ([!UICONTROL Variable to Find]) フィールドにコピーします。 「 」フィールドにはダブルカーリーで囲まれて表示されます。 例: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL モジュール ]</p> </td> 
   <td> <p>変数を置き換えるモジュールを選択します。 モジュールが選択されていない場合、変数はシナリオ全体で置き換えられます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アプリをスワップ]

シナリオで選択したアプリのバージョンを別のアプリのバージョンに置き換えます。

これは、例えば、Gmail および Email アプリのモジュールを最新バージョンにアップグレードするために使用できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 置き換えアプリ ]</td> 
   <td> <p> 置き換えるアプリを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 次で置換 ]</p> </td> 
   <td> <p>置き換えるアプリを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

入力したデータを Base64 または Base64 にエンコードできます。 一部の要求は Base64 にエンコードされます。 このツールは、エンコードされたリクエスト内の特定のデータを検索する場合に役立ちます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 操作 ] </td> 
   <td> <p>[!UICONTROL Raw Data] フィールドのデータを Base64 にエンコードするか、Base64 を Raw Data にデコードするかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 生データ ]</p> </td> 
   <td> <p> 上の「[!UICONTROL 操作 ]」フィールドで選択したオプションに応じて、生データにデコードする場合は、Base64 または Base64 にエンコードするデータを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL モジュール名をコピー]

選択したモジュールの名前をクリップボードにコピーします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL モジュール ] </td> 
   <td> <p>名前をコピーするモジュールを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ソースを再マッピング]

マッピングソースをモジュール間で変更できます。

最初に、ソースモジュールとして使用するモジュールをシナリオ内のルートに追加する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ] </td> 
   <td> <p> シナリオ内の他のモジュールのマッピングソースとして置き換えるモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target モジュール ]</p> </td> 
   <td> <p>新しいマッピングソースとして使用するモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 編集するモジュール ]</p> </td> 
   <td> <p>シナリオ全体でマッピングを変更しない場合は、マッピングを変更するモジュールを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アプリをハイライト]

シナリオ内の指定されたアプリのモジュールを強調表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 強調表示するアプリ ] </td> 
   <td> <p> シナリオでハイライト表示するアプリを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL バージョン ] </p> </td> 
   <td> <p>ハイライト表示するアプリのバージョンを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ハイライトカラー ]</p> </td> 
   <td> <p> モジュールのハイライト表示に使用する 16 進数の色を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL GS を移行]

このツールは、特にアップグレード用に作成されています [!DNL Google Sheets] （レガシー）モジュールを最新の [!DNL Google Sheets] バージョン。 シナリオルート内のモジュールのレガシーバージョンの直後に、新しいバージョンのモジュールが追加されます。

このモジュールでは、パラメーターを設定する必要はありません。
