---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion でシナリオの実行履歴を表示します
description: あるシナリオのすべての実行に関する情報を表示したり、特定のデータに関するシナリオのすべての実行を検索したりできます。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# でのシナリオの実行履歴の表示 [!DNL Adobe Workfront Fusion]

あるシナリオのすべての実行に関する情報を表示したり、特定のデータに関するシナリオのすべての実行を検索したりできます。

シナリオの実行履歴には、過去 30 日間のシナリオのすべての実行が表示されます。

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA) </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## シナリオのすべての実行を表示

### でシナリオ実行履歴を表示 [!UICONTROL シナリオの詳細] ページ

1. 次をクリック： **[!UICONTROL シナリオ]** タブをクリックし、シナリオをクリックします。

   または

   シナリオエディタでシナリオを操作している場合は、左向き矢印をクリックします。 ![](assets/exit-editing-arrow.png) ウィンドウの左上隅付近にある

1. 右側のリストで情報を表示します。

   ![](assets/open-history-tab-350x202.png)

   色

   また、をクリックすると、この情報の完全なページ表示を確認できます。 フルページ表示では、履歴をフィルタリングして、特定の実行を表示できます。

   シナリオの実行ごとに、次の詳細が表示されます。

   * 実行日 **[!UICONTROL 開始済み]**
   * **[!UICONTROL ステータス]** （成功または失敗）
   * 実行 **[!UICONTROL 期間]**
   * 数 **[!UICONTROL 運用]**
   * サイズ **[!UICONTROL データ転送]**
   * リンク先 **[!UICONTROL 詳細]**

### でシナリオ実行履歴を表示 [!UICONTROL 履歴] タブ

この [!UICONTROL 履歴] 「 」タブには、以下の項目よりも詳細な情報が表示されます [!UICONTROL シナリオの詳細] ページ。 また、 [!UICONTROL 履歴] タブをクリックします。

1. 次をクリック： **[!UICONTROL シナリオ]** タブをクリックし、シナリオをクリックします。

   または

   シナリオエディタでシナリオを操作している場合は、左向き矢印をクリックします。 ![](assets/exit-editing-arrow.png) ウィンドウの左上隅付近にある

1. 次をクリック： **[!UICONTROL 履歴]** ページの左上隅付近のタブ
1. （オプション）処理されたバンドルを含む、選択したシナリオの実行に関する詳細情報を表示するには、 **[!UICONTROL 詳細]** リンク。

   バンドルの処理について詳しくは、 [のシナリオ実行フロー [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >この [!UICONTROL 詳細] リンクは、実行に詳細が含まれる場合にのみ表示されます。

## シナリオ実行履歴のフィルター

実行履歴をフィルターして、指定した値を持つ実行のみを表示できます。

1. シナリオの全ページ履歴を開きます ( [でシナリオ実行履歴を表示 [!UICONTROL 履歴] タブ](#view-scenario-execution-history-on-the-history-tab) 」を参照してください。
1. 次をクリック： [!UICONTROL フィルター] アイコン ![](assets/fusion-scenario-filter-icon.png) 」をクリックします。
1. 内 [!UICONTROL フィルター] ダイアログで、フィルターに使用する値を入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

現在アクティブなフィルターが含まれる列には、フィルターアイコンがオレンジ色で表示されます。

## シナリオ実行履歴の並べ替え

シナリオの実行履歴を並べ替えることができます。

1. シナリオの全ページ履歴を開きます ( [でシナリオ実行履歴を表示 [!UICONTROL 履歴] タブ](#view-scenario-execution-history-on-the-history-tab) 」を参照してください。
1. 次をクリック： [!UICONTROL 並べ替え] アイコンをクリックします。
1. オプション：並べ替えの順序を逆にするには、 [!UICONTROL 並べ替え] アイコンを再度クリックします。

## シナリオのすべての実行を検索

1. 次をクリック： **[!UICONTROL シナリオ]** アイコン ![](assets/scenarios-icon.png) 左のパネルで、シナリオをクリックします。

   または

   シナリオエディタでシナリオを操作している場合は、左向き矢印をクリックします。 ![](assets/exit-editing-arrow.png) ウィンドウの左上隅付近にある

1. 次をクリック： **[!UICONTROL 履歴]** タブをクリックします。
1. クリック **[!UICONTROL フルテキスト検索]** をクリックします。

   または

   タイプ **Ctrl+Shift+F** (Windows) または **Cmd+Shift+F** (Mac) [!UICONTROL 履歴で検索] ウィンドウが開きます。

1. （オプション）特定のテキストを含む実行を検索するには、 **[!UICONTROL 履歴で検索]** ウィンドウ

   正確なテキストを検索するには、テキストを二重引用符 (&quot;example&quot;) で囲みます。

   >[!INFO]
   >
   >**例：** 特定のプロジェクトを作成した実行を検索する場合は、 [!UICONTROL フルテキスト検索] バー。
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. （オプション）日付範囲で検索を制限するには、目的の検索の開始日と終了日を [!UICONTROL 日付範囲別] 領域

   >[!NOTE]
   >
   >* 過去 30 日間のみ実行できます。
   >
   >* [!DNL Workfront Fusion] は、30 日間、webhook ペイロードを保存します。 作成後 30 日を超える Webhook ペイロードにアクセスすると、「[!UICONTROL ストレージからファイルを読み取れませんでした。]&quot;



1. （オプション）検索をステータスで制限するには、「 **[!UICONTROL ステータス別]** ドロップダウン。


   利用可能なステータスは次のとおりです。

   * [!UICONTROL すべて]

   * [!UICONTROL エラー]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （オプション）結果の表示順を **[!UICONTROL 日付で並べ替え]** ドロップダウン。

1. （オプション）シナリオ実行 ID をコピーするには、 **[!UICONTROL 実行 ID をコピー]** アイコン <img src="assets/copy-fusion-execution-id-icon.png"> （目的の実行の行）

1. （オプション） [!UICONTROL フルテキスト検索] 情報を含むシナリオモジュール出力バンドルを調べます。
