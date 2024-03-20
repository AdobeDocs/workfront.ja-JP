---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Devtool でのシナリオのデバッグ
description: Adobe Workfront Fusion Devtool を使用すると、シナリオを理解し、トラブルシューティングできます。 開発ツールは、Chrome Developer Tools にパネルを追加します。 このデバッガーパネルを使用すると、シナリオのすべての手動実行を確認し、実行されたすべての操作を確認し、実行されたすべての API 呼び出しの詳細を表示できます。エラーが発生したモジュール、操作または単一の応答を確認し、その知識を使用してシナリオを改良できます。
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 7fe35f70cfc7ef346584e3cf525c2553f867ed1f
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 76%

---

# でのシナリオのデバッグ [!DNL Adobe Workfront Fusion] 開発者ツール

The [!DNL Adobe Workfront Fusion] 開発者ツールを使用すると、シナリオを理解し、トラブルシューティングできます。 開発ツールは、 [!DNL Chrome Developer Tools]. このデバッガーパネルを使用すると、シナリオのすべての手動実行を確認し、実行されたすべての操作を確認し、実行されたすべての API 呼び出しの詳細を表示できます。エラーが発生したモジュール、操作または単一の応答を確認し、その知識を使用してシナリオを改良できます。

>[!NOTE]
>
>デバッガーパネルでのログ記録は、機密のシナリオ、自動実行、正常な操作に対して制限されるか、使用できなくなります。

Fusion Devtool のビデオの紹介と説明については、

* [Fusion Development Tool](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [開発ツールのチュートリアル](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html?lang=en)

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

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

1. クリック [このリンク](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) に行く [!DNL Workfront Fusion] の開発ツール [!UICONTROL [!DNL Chrome] Web ストア].
1. 「**[!UICONTROL [!DNL Chrome]]** に追加」をクリックします。
1. 開いたウィンドウで、権限を確認します。権限に同意する場合は、「**[!UICONTROL 拡張機能を追加]**」をクリックします。

The [!DNL Workfront Fusion] Devtool 拡張機能が [!DNL Chrome] 拡張機能。


#### 次を見つけます。 [!DNL Workfront Fusion] 開発者ツール

次の手順で [!DNL Workfront Fusion] 開発者ツール、 [!DNL Workfront Fusion] Devtool 拡張機能を [!DNL Chrome] ブラウザ、 [Chrome Devtool 拡張機能のインストール](#install-the-chrome-Devtool-extension).

1. [!DNL Workfront Fusion] シナリオを開きます。
1. [!DNL Chrome Developer Tools] を開く：

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
   >[!DNL Chrome Developer Console] を下にドッキングして、モジュールの表示を改善することをお勧めします。

1. [!DNL Chrome Dev Tools] で「**[!DNL Workfront Fusion]**」タブをクリックします。

## 以下を使用します。 [!DNL Workfront Fusion] 開発者ツール

Workfront Fusion Devtool は、3 つの主なセクションに分かれています。 これらは、Devtool ウィンドウの左側のパネルにあります。

* [ライブストリーム](#live-stream)
* [シナリオデバッガー](#scenario-debugger)
* [ツール](#tools)

### ライブストリーム

ライブストリームは、シナリオで「1 回実行」をクリックすると、バックグラウンドで発生していることを表示します。

1. **[!UICONTROL ライブストリーム]**&#x200B;アイコン ![](assets/live-stream-icon.png) をクリックして、「ライブストリーム」セクションを開きます。
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
      <td> <p>シナリオの各モジュールに関して、次の情報を表示できます。</p> 
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
      <td role="rowheader"> <p>コンソールログを有効化</p> </td> 
      <td> <p>コンピューターのアイコンをクリックします。 <img src="assets/console-computer-icon.png"> は、開発者ツールの左パネルの右上隅にあります。</p> <p>コンピューターアイコンが緑の場合、コンソールでのログは有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Raw JSON 形式または cURL でリクエストを取得</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Raw JSON</strong> </p> <p>クリック <strong>[!UICONTROL RAW をコピー ]</strong> をクリックします。</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>クリック <strong>[!UICONTROL cURL をコピー ]</strong> をクリックします。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### シナリオデバッガー

シナリオデバッガーは、より複雑なシナリオで役に立ちます。シナリオ実行の履歴が表示され、名前または ID でモジュールを検索できます。

1. **[!UICONTROL シナリオデバッガー]**&#x200B;アイコン ![](assets/scenario-debugger-icon.png) をクリックして、シナリオデバッガーを開きます。
1. （オプション）検索語句（名前またはモジュール ID）を、 [!DNL Workfront Fusion] の開発ツール [!UICONTROL シナリオデバッガー] 」セクションに入力します。
1. モジュールの名前をダブルクリックして、そのモジュールの設定をシナリオエディターで開きます。
1. 目的の操作をクリックして、リクエストの詳細を表示します。

### ツール

The [!DNL Workfront Fusion] 開発ツールには、シナリオの設定を容易にするツールが備わっています。

1. **[!UICONTROL ツール]**&#x200B;アイコン ![](assets/console-tools-icon.png) をクリックして、ツールを開きます。
1. 使用するツールを選択します。
1. 下記のフィールドを設定します。
1. 「**[!UICONTROL 実行]**」をクリックします。

ツールとそのフィールド：

* [モジュールのフォーカス](#focus-a-module)
* [マッピングによるモジュールの検索](#find-modules-by-mapping)
* [アプリのメタデータの取得](#get-app-metadata)
* [マッピングのコピー](#copy-mapping)
* [フィルターのコピー](#copy-filter)
* [接続の交換](#swap-connection)
* [変数の交換](#swap-variable)
* [アプリの交換](#swap-app)
* [Base 64](#base-64)
* [モジュール名のコピー](#copy-module-name)
* [ソースの再マッピング](#remap-source)
* [アプリのハイライト表示](#highlight-app)
* [GS の移行](#migrate-gs)

#### [!UICONTROL モジュールのフォーカス]

ID で指定したモジュールの設定が開きます。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Module ID]</td>
        <td>設定を開くモジュールの ID を入力します。</td>
    </tr>
</table>

#### [!UICONTROL マッピングによるモジュールの検索]

指定した語句に対応するモジュールの値を検索できます。出力には、検索した語句を含んだモジュールの ID が含まれています。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> 検索する語句を入力します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Use Only Values]</p> </td> 
   <td> <p>モジュールフィールドの値のみを検索する場合は、このオプションを有効にします。</p> <p>モジュールフィールドの名前も検索する場合は、このオプションを無効にします。</p> <p>検索は、name および label パラメーターを使用して実行されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アプリのメタデータの取得]

アプリのモジュール名または ID でアプリのメタデータを取得します。これは、例えば、シナリオで使用されるアプリのバージョンを知る必要がある場合に便利です。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>メタデータを取得するモジュールを選択します。</td>
    </tr>
</table>

#### [!UICONTROL マッピングのコピー]

ソースモジュールからターゲットモジュールに値をコピーします。

>[!CAUTION]
>
>正しいソースモジュールとターゲットモジュールを設定していることを確認します。別のタイプのモジュールを選択すると、ターゲットモジュール内の値は削除されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> フィールド値のコピー元となるモジュールを選択するか、そのモジュールの ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>ソースモジュール値の挿入先となるモジュールを選択するか、そのモジュールの ID を入力します。</p> <p>重要：ターゲットモジュール内の値は上書きされます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フィルターのコピー]

ソースモジュールからターゲットモジュールにフィルター設定をコピーします。

>[!NOTE]
>
>コピー操作は、選択したモジュールの左側に配置されたフィルターに対して実行されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> フィルター値のコピー元となるモジュールを選択するか、そのモジュールの ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>ソースモジュールのフィルター値の挿入先となるモジュールを選択するか、そのモジュールの ID を入力します。</p> <p>重要：ターゲットモジュール内の値は上書きされます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>ソースフィルターは、フォールバックルートとして設定されます。ターゲットフィルターがフォールバックルートとして設定されるように指定するには、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 接続の交換]

同じアプリのシナリオ内のすべてのモジュールに、ソースモジュールの接続を複製します。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>接続の複製元となるモジュールを選択するか、そのモジュールの ID を入力します。</td>
    </tr>
</table>

#### [!UICONTROL 変数の交換]

指定された変数をシナリオ内で検索し、新しい変数に置き換えます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> 置き換える変数ピルをシナリオのモジュールから探して、この（「[!UICONTROL Variable to Find]」）フィールドにコピーします。フィールドには二重波括弧で囲まれて表示されます。例：<code>&#123;&#123;5.value&#125;&#125;</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace With]</p> </td> 
   <td> <p>シナリオ内のモジュールで変数を置き換える変数ピルを探し、この（[!UICONTROL Variable to Find]）フィールドにコピーします。フィールドには二重波括弧で囲まれて表示されます。例：<code>&#123;&#123;5.value&#125;&#125;</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>変数を置き換えるモジュールを選択します。モジュールが選択されていない場合、変数はシナリオ全体で置き換えられます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アプリをスワップ]

シナリオで選択したアプリのバージョンを別のアプリのバージョンに置き換えます。

これは、例えば、Gmail およびメールアプリのモジュールを最新バージョンへのアップグレードに使用できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Replaced]</td> 
   <td> <p> 置き換える元のアプリを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace with]</p> </td> 
   <td> <p>置き換える先のアプリを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

入力したデータを Base64 にエンコードまたは Base64 からデコードできます。一部のリクエストは Base64 にエンコードされています。このツールは、エンコードされたリクエスト内の特定のデータを検索する場合に役立ちます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operation] </td> 
   <td> <p>[!UICONTROL Raw Data] フィールドのデータを Base64 にエンコードするか、Base64 を生データにデコードするかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Raw Data]</p> </td> 
   <td> <p> 上記の [!UICONTROL Operation] フィールドで選択したオプションに応じて、Base64 にエンコードするデータ、または生データにデコードする Base64 を入力します。</p> </td> 
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
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>名前をコピーするモジュールを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ソースを再マッピング]

マッピングソースをあるモジュールから別のモジュールへ変更できるようになります。

最初に、シナリオでルートへのソースモジュールとして使用するモジュールを追加する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> シナリオ内の他のモジュールのマッピングソースとして置き換えるモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>新しいマッピングソースとして使用するモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
   <td> <p>シナリオ全体でマッピングを変更しない場合は、マッピングを変更するモジュールを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アプリをハイライト]

シナリオ内の指定されたアプリのモジュールをハイライト表示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Highlighted] </td> 
   <td> <p> シナリオでハイライト表示するアプリを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>ハイライト表示するアプリのバージョンを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Highlight Color]</p> </td> 
   <td> <p> モジュールのハイライト表示に使用する 16 進数の色を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL GS を移行]

このツールは、[!DNL Google Sheets]（レガシー）モジュールを最新の [!DNL Google Sheets] バージョンにアップグレードするために特別に作成されました。シナリオルート内のモジュールのレガシーバージョンの直後に、新しいバージョンのモジュールが追加されます。

このモジュールでは、パラメーターを設定する必要はありません。
