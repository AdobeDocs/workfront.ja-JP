---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードでのストーリー情報の表示と編集
description: かんばんボード上のストーリータイルを表示する場合、特定の情報は、ストーリータイルから直接、インラインで編集することができます。
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 91dc9946566e15bf32d0d89975e3e6b66b39e873
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 92%

---

# [!UICONTROL スクラム]のボードのストーリー情報の表示と編集

## 表示および編集できる情報について

ストーリーボード上のストーリータイルを表示する場合、次の表の情報を使用できます。ほとんどの情報は、ストーリータイルから直接、インラインで編集できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>情報</strong> </th> 
   <th><strong>表示されている</strong> </th> 
   <th><strong>インラインで編集可能</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>タスクまたはイシューへの直接リンクを含むストーリー名</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトへの直接リンクを含むプロジェクト名<br>このリンクは、イテレーションでアジャイルビューを使用する場合、ストーリー（サブタスクではなく親タスク）にのみ表示されます。プロジェクトでアジャイルビューを使用している場合は表示されません。</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>ストーリー上で完了したポイントまたは時間の数、およびストーリーに割り当てられたポイントまたは時間の数<br>これらの数値は、それぞれのストーリーの [!UICONTROL Percent CompletePercent Complete] を計算して表示するために使用されます。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>それぞれのストーリーおよびイシューの [!UICONTROL Percent Complete]。<br>イテレーションの [!UICONTROL The Percent CompletePercent Complete] は、それぞれのストーリーの [!UICONTROL Percent CompletePercent Complete] に基づいて計算されます。</p> <p>ストーリーまたはイシューの [!UICONTROL Percent Complete] を更新する際に、0 と 100 の間の任意の数を選択できます。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>ストーリーの担当者</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>タイルのカラーまたはカテゴリ</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">[!UICONTROL Adobe Workfront] でのビューの概要</a>の「[!UICONTROL Agile] ビューの作成およびカスタマイズ」で説明されているような、アジャイルビューを修正することによってアジャイルビューに追加された可能性がある追加フィールド（カスタムフィールドを含む）。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p> 
   または
   <p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>タスクまたは問題への [!UICONTROL Contribute] または [!UICONTROL Manage] アクセス</td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ストーリータイルの情報の表示と編集

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 左パネルで、「**[!UICONTROL イテレーション]**」を選択して特定のイテレーションを選ぶか、「**[!UICONTROL 進行中のイテレーション]**」を選択します。

1. [!UICONTROL スクラム]アジャイルストーリーボードに移動します。
1. [!UICONTROL ストーリー]タイルを展開して、ストーリーに関連するすべてのフィールドを表示します。

   ![ ストーリーカード ](assets/agile-storycard-scrum-2021-350x333.png)

1. （オプション）フィールドを編集するには、フィールドをクリックして、変更を加えます。

   ストーリータイルを編集するには、タスクまたはイシューに対する[!UICONTROL 編集]権限が必要です。

>[!NOTE]
>
>[!UICONTROL 完了率]を変更する場合は、0 から 100 の間の数値を入力する必要があります。フィールドは移動できるスライダーではありません。
