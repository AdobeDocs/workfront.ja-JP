---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect の使用状況指標の表示
description: 「Workfront Data Connect Metrics」タブを使用すると、毎月のコンピューティング利用時間と実行されたクエリ数の両方に従って、組織の使用状況指標を表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: 7764e512a3fb30a89e6645a4d8544a5fcffee231
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 9%

---

# [!DNL Workfront Data Connect] 使用状況指標の表示

「[!DNL Workfront Data Connect][!UICONTROL &#x200B; 指標 &#x200B;]」タブを使用すると、使用された計算時間と実行されたクエリ数の両方に従って、組織の使用状況指標を表示できます。 組織では、ライセンスタイプと Data Connect アドオンの購入に基づいて、利用可能な月間計算時間が制限されています。 「[!UICONTROL &#x200B; 指標 &#x200B;]」タブには、使用状況に関連した利用可能な月別の計算時間数に関する情報が表示されます。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>Ultimate</p>
    <p>ワークフロー Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である必要があります</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 使用指標と利用可能な計算時間を表示する

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、[!UICONTROL **設定**] をクリックします。

1. 左側のパネルで、[!UICONTROL **システム**]/[!UICONTROL **データアクセス**] をクリックします。

1. 「[!UICONTROL **指標**]」タブをクリックします。 使用状況の指標は **使用状況を計算** グラフに表示され、実行されたクエリの数は **クエリ数** グラフに表示されます。

   ![&#x200B; データ接続の使用状況指標 &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. （オプション） [!UICONTROL **表示を選択**] ドロップダウンメニューを使用して、両方のグラフに含まれる情報の時間範囲を変更できます。

1. （オプション）「**使用状況を計算**」グラフの上にあるチェックボックスを使用して、表示と非表示を切り替えることができます。
   * [!UICONTROL **日別計算時間**] – 組織が毎日使用する計算時間の数。
   * [!UICONTROL **月別累積計算時間**] – 組織が 1 か月に使用した計算時間の合計。 毎月 0 にリセットします。
   * [!UICONTROL **月別の計算時間割**] - ライセンスやアドオンの購入に基づいて組織で利用できる計算時間数です。
