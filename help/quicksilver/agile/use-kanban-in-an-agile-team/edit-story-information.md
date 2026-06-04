---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: ストーリー情報を編集
description: かんばんボード上のストーリータイルを表示する場合、特定の情報は、ストーリータイルから直接、インラインで編集することができます。
author: Courtney
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YNFdopcCAju4MaN2oqssN0Q6H7k0Stg3udO0AipWIMs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 340
ht-degree: 77%

---

# ストーリー情報の編集

## 表示および編集できる情報について {#understand-what-information-can-be-viewed-and-edited}

ストーリータイルを[!UICONTROL かんばん]ボードで表示する場合、次の表の情報が使用できます。 ほとんどの情報は、ストーリータイルから直接、インラインで編集できます。

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
   <td> <p>プロジェクトへの直接リンクを含むプロジェクト名</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>ストーリー上で完了したポイントまたは時間の数、およびストーリーに割り当てられたポイントまたは時間の数<br>これらの数値は、それぞれのストーリーの完了率を計算して表示するために使用されます。</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>ストーリーとイシューごとに[!UICONTROL Percent Complete]が計算されます。<br>[!UICONTROL イテレーションのPercent Complete]は、各ストーリーの[!UICONTROL Percent Complete]に基づいて計算されます。<br></p> <p>ストーリーまたはイシューの [!UICONTROL Percent Complete] を更新する際に、0 と 100 の間の任意の数を選択できます。</p> </td> 
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
   <td> <p>[!DNL Adobe Workfront]</a>の<a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref"> ビューの概要の「アジャイルビューの作成とカスタマイズ」の説明に従って、アジャイルビューを変更してアジャイルビューに追加された可能性がある追加フィールド（カスタムフィールドを含む）</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ストーリータイルの情報の表示と編集

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、続いてドロップダウンメニューから新しいかんばんチームを選択するか、検索バーでチームを検索します。

1. [!UICONTROL かんばん]ボードに移動します。
1. ストーリータイルを展開して、ストーリーに関連するすべてのフィールドを表示します。

   ![&#x200B; ストーリーカード &#x200B;](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. （オプション）フィールドを編集するには、フィールドをクリックしてから変更を加えます。
ストーリータイルを編集するには、タスクまたはイシューに対する[!UICONTROL 編集]権限が必要です。
各フィールドの詳細と編集可能かどうかについては、[表示および編集可能な情報について](#understand-what-information-can-be-viewed-and-edited)を参照してください。

>[!NOTE]
>
>[!UICONTROL 完了率]を変更する場合は、0 から 100 の間の数値を入力する必要があります。 フィールドは移動できるスライダーではありません。
