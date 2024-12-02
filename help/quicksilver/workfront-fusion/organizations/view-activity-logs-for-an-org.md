---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion での組織のアクティビティログの表示
description: シナリオの作成やアクティブ化など、組織のアクティビティのログを表示できます。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: 686113b6dd658db6390b425946e5b80593a4dbd1
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 22%

---

# Adobe Workfront Fusion での組織のアクティビティログの表示

<!--Move to new repo-->

シナリオの作成やユーザーの招待など、組織のアクティビティのログを表示できます。

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

## アクティビティログの表示

1. 左側のナビゲーションパネルで、**組織概要**![ 組織概要アイコン ](assets/org-overview-icon.png) をクリックします。
1. アクティビティログを表示する組織に現在所属していない場合は、画面の右上隅にある組織名をクリックし、ドロップダウンから組織を選択します。
1. 画面上部付近の **[!UICONTROL アクティビティログ]** タブをクリックします。

   アクティビティログページが開きます。
1. （オプション）指定した条件で結果を制限するには、アクティビティログをフィルタリングします。

   手順については、この記事の [ アクティビティログのフィルタリング ](#filter-the-activity-logs) を参照してください。
1. （オプション）適用したフィルターをクリアするには、画面の右上付近にあるフィルターを見つけて、フィルターのボックスの **X** をクリックします。
1. （任意）ログをエクスポートします。

   手順については、この記事の [ アクティビティログのエクスポート ](#export-the-activity-logs) を参照してください。


## アクティビティログのフィルタリング

1. 左側のナビゲーションパネルで、**組織概要**![ 組織概要アイコン ](assets/org-overview-icon.png) をクリックします。
1. アクティビティログを表示する組織に現在所属していない場合は、画面の右上隅にある組織名をクリックし、ドロップダウンから組織を選択します。
1. 画面上部付近の **[!UICONTROL アクティビティログ]** タブをクリックします。

   アクティビティログページが開きます。
1. **フィルター**![ フィルターアイコン ](assets/filter-activity-log.png) をクリックします。
1. フィールドをクリックして、次のフィルターを 1 つ以上設定します。

   * **開始日と終了日**：カレンダーから日付を選択し、（オプション）時間を入力します。
   * **ユーザー**：ドロップダウンからユーザーを選択します。
   * **チーム**：ドロップダウンからチームを選択します。 自分がメンバーになっているチームのみがドロップダウンに表示されます。
   * **エンティティ**：アクティビティログを表示する Fusion オブジェクトのタイプを選択します。
   * **アクション**：アクティビティログを表示するアクションを選択します。

1. **適用** をクリックします。

## アクティビティログのエクスポート

1. 左側のナビゲーションパネルで、**組織概要**![ 組織概要アイコン ](assets/org-overview-icon.png) をクリックします。
1. アクティビティログを表示する組織に現在所属していない場合は、画面の右上隅にある組織名をクリックし、ドロップダウンから組織を選択します。
1. 画面上部付近の **[!UICONTROL アクティビティログ]** タブをクリックします。

   アクティビティログページが開きます。
1. カレンダーから日付範囲を選択し、（オプション）時間を入力します。
1. Excel ファイルと CSV ファイルのどちらをエクスポートするかを選択します。
1. 「**適用**」をクリックします。





