---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: かんばんボード上の既存のストーリーへのサブタスクの追加
description: かんばんボード上の既存のストーリーのサブタスクを作成する方法については、この記事を参照してください。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 93%

---

# かんばんボードの既存のストーリーへのサブタスクの追加

既存のストーリーのサブタスクを作成する場合は、次の点に注意してください。

**プロジェクトの[!UICONTROL 概要完了モード]の設定が[!UICONTROL 手動]に設定されている場合：**

* サブタスクを含む親ストーリーを[!UICONTROL 完了]に移動することができ、そうすると、親ストーリーが 100％、[!UICONTROL ステータス]が[!UICONTROL 完了]に更新されます。サブタスクは更新されません。
* ストーリーの[!UICONTROL 完了率]を更新するには、オブジェクトの「[!UICONTROL ストーリー]」タブまたは[!UICONTROL 詳細]ページから更新する必要があります。

**プロジェクトの[!UICONTROL 概要完了モード]の設定が[!UICONTROL 自動]に設定されている場合：**

* 親ストーリーは、ボードを越えて移動することはできません。ストーリーの[!UICONTROL 完了率]を更新するには、サブタスクの[!UICONTROL 完了率]を更新する必要があります。ストーリーの[!UICONTROL 完了率]は、すべてのサブタスクの[!UICONTROL 完了率]に基づいて計算されます。
* サブタスクを含む親ストーリーを[!UICONTROL 完了]に移動すると、親ストーリーが 100％、[!UICONTROL ステータス]が[!UICONTROL 完了]に更新されます。サブタスクも 100％に更新され、[!UICONTROL ステータス]が[!UICONTROL 完了]に更新されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>サブタスクが存在するタスクへの[!UICONTROL Contribute]または[!UICONTROL Manage]アクセス</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL かんばん]ボードの既存のストーリーにサブタスクを追加

1. サブタスクを追加するストーリーを含む[!UICONTROL かんばん]ボードに移動します。
1. [!UICONTROL かんばん]ボードのストーリータイル上のタスクの名前をクリックします。
1. [!DNL Workfront] 内の他のタスクリストと同様に、[サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md)の説明のとおりに、タスクにサブタスクを追加します。
