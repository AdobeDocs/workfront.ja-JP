---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect の使用状況指標の表示
description: 「Workfront Data Connect Metrics」タブを使用すると、毎月の計算時間数と実行されたクエリ数の両方に基づいて、組織の使用状況メトリクスを表示できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 11%

---

# [!DNL Workfront Data Connect]の使用状況の指標を表示

「[!DNL Workfront Data Connect] [!UICONTROL 指標]」タブを使用すると、使用された計算時間と実行されたクエリ数の両方に基づいて、組織の使用状況の指標を表示できます。 組織は、ライセンスの種類とData Connect アドオンの購入に基づいて、月間計算に利用できる時間が制限されています。 「[!UICONTROL 指標]」タブには、使用済みの計算時間に関する利用可能な月次の計算時間に関する情報が表示されます。

## アクセス要件

+++ 展開してアクセス要件を表示します。 

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
   <td> <p>あなたはWorkfrontの管理者でなければなりません</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 使用状況の指標と使用可能な計算時間の表示

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、[!UICONTROL **Setup**]&#x200B;をクリックします。

1. 左側のパネルで、[!UICONTROL **システム**]/[!UICONTROL **データアクセス**]&#x200B;をクリックします。

1. 「[!UICONTROL **指標**]」タブをクリックします。 使用状況の指標は&#x200B;**Compute Usage** グラフに表示され、実行されたクエリの数は&#x200B;**クエリ数** グラフに表示されます。

   ![ データ接続の使用状況の指標](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. （オプション）両方のグラフに含まれる情報の時間範囲を変更するには、[!UICONTROL **ビューを選択**] ドロップダウンメニューを使用します。

1. （オプション） **使用状況を計算** グラフの上にあるチェックボックスを使用して、表示または非表示にできます。
   * [!UICONTROL **毎日の計算時間数**] – 組織が毎日使用する計算時間数。
   * [!UICONTROL **月間累積計算時間数**] – 組織が1か月間に使用した計算時間数の合計数。 毎月ゼロにリセットされます。
   * [!UICONTROL **月間計算時間許可**] - ライセンスやアドオンの購入に基づいて、組織で利用可能な計算時間数。
