---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: カンバンボードの既存のストーリーへのサブタスクの追加
description: かんばんボード上の既存のストーリーのサブタスクを作成する方法については、この記事を参照してください。
author: Courtney
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Wbiao1UjwOzItIGJkh1E9A81RcUfLDJqgYjRDL46qvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 305
ht-degree: 92%

---

# かんばんボードの既存のストーリーへのサブタスクの追加

既存のストーリーのサブタスクを作成する場合は、次の点に注意してください。

**プロジェクトの[!UICONTROL 概要完了モード]の設定が[!UICONTROL 手動]に設定されている場合：**

* サブタスクを含む親ストーリーを[!UICONTROL 完了]に移動することができ、そうすると、親ストーリーが 100％、[!UICONTROL ステータス]が[!UICONTROL 完了]に更新されます。 サブタスクは更新されません。
* ストーリーの[!UICONTROL 完了率]を更新するには、オブジェクトの[!UICONTROL ストーリー]タブまたは[!UICONTROL 詳細]ページから更新する必要があります。

**プロジェクトの[!UICONTROL 概要完了モード]の設定が[!UICONTROL 自動]に設定されている場合：**

* 親ストーリーは、ボードを越えて移動することはできません。 ストーリーの[!UICONTROL 完了率]を更新するには、サブタスクの[!UICONTROL 完了率]を更新する必要があります。 ストーリーの[!UICONTROL 完了率]は、すべてのサブタスクの[!UICONTROL 完了率]に基づいています。
* サブタスクを含む親ストーリーを[!UICONTROL 完了]に移動すると、親ストーリーが 100％、[!UICONTROL ステータス]が「[!UICONTROL 完了]」に更新されます。 サブタスクも 100％となり、[!UICONTROL ステータス]が「[!UICONTROL 完了]」に更新されます。

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
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>サブタスクが属するタスクへのアクセス権を設定または管理する</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL かんばん]ボードの既存のストーリーにサブタスクを追加

1. サブタスクを追加するストーリーを含む[!UICONTROL かんばん]ボードに移動します。
1. [!UICONTROL かんばん]ボードのストーリータイル上のタスクの名前をクリックします。
1. [!DNL Workfront] 内の他のタスクリストと同様に、[サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md)の説明のとおりに、タスクにサブタスクを追加します。
