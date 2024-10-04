---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion でのシナリオの履歴の表示
description: あるシナリオのすべての実行に関する情報を表示したり、特定のデータに関するシナリオのすべての実行を検索したりできます。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 2e26c4e4b5f331ed2e609381ef442f45e90c4faa
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 82%

---

# [!DNL Adobe Workfront Fusion] でのシナリオの履歴の表示

シナリオのイベントや実行に関する情報を表示したり、シナリオのすべての実行で特定のデータを検索したりできます。

シナリオ実行は、シナリオの 1 回の実行を表します。

シナリオイベントは、シナリオを編集、アクティブ化または非アクティブ化するなどの、シナリオに対する変更です。

>[!NOTE]
>
>シナリオの履歴には、過去 30 日間のシナリオのイベントと実行がすべて表示されます。

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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## シナリオ履歴の表示

### [!UICONTROL  シナリオの詳細 ] ページにシナリオ履歴を表示

1. 左パネルの「**[!UICONTROL シナリオ]**」タブ、シナリオの順にクリックします。

   または

   シナリオエディターでシナリオを操作している場合は、ウィンドウの左上隅付近にある左向き矢印 ![](assets/exit-editing-arrow.png) をクリックします。

1. 実行履歴は、右側のパネルの **履歴** タブで確認できます。

   シナリオの実行ごとに、次の詳細が表示されます。

   * 実行が&#x200B;**[!UICONTROL 開始]**&#x200B;した日付
   * **[!UICONTROL ステータス]**（成功または失敗）
   * 実行&#x200B;**[!UICONTROL 期間]**
   * **[!UICONTROL 操作]**&#x200B;の回数
   * **[!UICONTROL データ転送]**&#x200B;のサイズ

   >[!NOTE]
   >
   >実行の詳細がストレージに書き込まれる一方で、シナリオ履歴では、最近実行されたシナリオの横に&#x200B;**処理**&#x200B;バッジが表示されます。処理は、シナリオの実行直後に行われます。数分以上続くことはありません。シナリオ実行の処理中は、シナリオ実行の詳細が表示されない場合があります。

1. 特定のシナリオ実行の詳細を表示するには、右側のパネルでその実行をクリックします。
1. イベントを表示するには、右側のパネルの「**イベント**」タブをクリックします。


### 「[!UICONTROL  履歴 ]」タブでのシナリオ履歴の表示

「[!UICONTROL 履歴]」タブには、[!UICONTROL シナリオの詳細]ページよりも詳細な情報が表示されます。また、[!UICONTROL 履歴]タブで実行のフィルタリングや並べ替えができます。

1. 左パネルの「**[!UICONTROL シナリオ]**」タブをクリックし、シナリオをクリックします。

   または

   シナリオエディターでシナリオを操作している場合は、ウィンドウの左上隅近くにある左向き矢印 ![](assets/exit-editing-arrow.png) をクリックします。

1. ページの左上隅付近にある「**[!UICONTROL 履歴]**」タブをクリックします。
1. （オプション）選択したシナリオの実行に関する詳細（処理されたバンドルを含む）を表示するには、その実行の行にある **[!UICONTROL 詳細]** ボタンをクリックします。

   バンドルの処理について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)でのシナリオ実行フロー を参照してください。

   >[!NOTE]
   >
   >* [!UICONTROL 詳細]リンクは、実行に詳細が含まれる場合にのみ表示されます。
   >
   >* シナリオ履歴では、最近実行したシナリオの横に&#x200B;**処理履歴**&#x200B;バッジが表示され、実行の詳細がストレージに書き込まれます。処理は、シナリオの実行直後に行われます。数分以上続くことはありません。シナリオ実行の処理中は、シナリオ実行の詳細が表示されない場合があります。

1. イベントを表示するには、「**イベントを表示**」切替スイッチを有効にします。

## シナリオ実行履歴のフィルタリング

実行履歴をフィルターして、指定した値を持つ実行のみを表示できます。

1. この記事の[「[!UICONTROL 履歴]」タブでシナリオの実行履歴を表示](#view-scenario-execution-history-on-the-history-tab)で説明されているように、シナリオの全ページ履歴を開きます。
1. フィルタリングしたい列のヘッダーで[!UICONTROL フィルター]アイコン ![](assets/fusion-scenario-filter-icon.png) をクリックします。
1. 「[!UICONTROL フィルター]」ダイアログで、フィルタリングしたい値を入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。

現在アクティブなフィルターが含まれる列には、フィルターアイコンがオレンジ色で表示されます。

## シナリオ実行履歴の並べ替え

シナリオの実行履歴を並べ替えることができます。

1. この記事の[「[!UICONTROL 履歴]」タブでシナリオの実行履歴を表示](#view-scenario-execution-history-on-the-history-tab)で説明されているように、シナリオの全ページ履歴を開きます。
1. フィルタリングしたい列のヘッダーで[!UICONTROL 並べ替え]アイコンをクリックします。
1. オプション：並べ替えの順序を逆にするには、[!UICONTROL 並べ替え]アイコンを再度クリックします。

## シナリオのすべての実行を検索

1. この記事の[「[!UICONTROL 履歴]」タブでシナリオの実行履歴を表示](#view-scenario-execution-history-on-the-history-tab)で説明されているように、シナリオの全ページ履歴を開きます。
1. 実行リスト上部にある「**[!UICONTROL フルテキスト検索]**」をクリックします。

   または

   **Ctrl+Shift+F**（Windows）または **Cmd+Shift+F**（MAC）
[!UICONTROL 履歴で検索]ウィンドウが開きます。

1. (オプション）特定のテキストを含む実行を検索するには、**[!UICONTROL 履歴で検索]**&#x200B;ウィンドウの検索バーにテキストを入力します。

   正確にテキストを検索するには、テキストを二重引用符（&quot;例&quot;）で囲みます。

   >[!INFO]
   >
   >**例：**&#x200B;特定のプロジェクトを作成した実行を検索したい場合、[!UICONTROL フルテキスト検索]バーにプロジェクトIDを入力します。
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (オプション）日付範囲で検索を制限するには、[!UICONTROL 日付範囲別]エリアで検索の開始日と終了日を選択します。

   >[!NOTE]
   >
   >* 過去 30 日間のみ実行できます。
   >
   >* [!DNL Workfront Fusion] は、30 日間、ebhook ペイロードを保存します。作成後 30 日を超える web フックペイロードにアクセスすると、「[!UICONTROL ストレージからファイルを読み取れませんでした。]」というエラーが発生します。


1. （オプション）検索をステータスで制限するには、**[!UICONTROL ステータス別]**&#x200B;ドロップダウンで目的のステータスを選択します。


   利用可能なステータスは、次のとおりです。

   * [!UICONTROL すべて]

   * [!UICONTROL エラー]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （オプション）**[!UICONTROL 日付順に並べ替え]**&#x200B;ドロップダウンで表示される結果の順序を変更します。

1. （オプション）シナリオ実行 ID をコピーするには、**[!UICONTROL 実行 ID をコピー]**&#x200B;アイコンをクリックします。 <img src="assets/copy-fusion-execution-id-icon.png"> を目的の実行の行に入れる

1. （オプション）[!UICONTROL  フルテキスト検索]の結果をクリックして、その情報を含むシナリオモジュール出力バンドルを調べます。
