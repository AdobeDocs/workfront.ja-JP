---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: かんばんボード上の既存のストーリーにサブタスクを追加します
description: かんばんボード上の既存のストーリーのサブタスクを作成する方法については、この記事を参照してください。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# かんばんボード上の既存のストーリーにサブタスクを追加します

既存のストーリーのサブタスクを作成する場合は、次の点に注意してください。

**次の場合に [!UICONTROL 概要完了モード] プロジェクトの設定が次のように設定されている [!UICONTROL 手動]:**

* サブタスクを含む親ストーリーを [!UICONTROL 完了]：親ストーリーを 100%に更新し、 [!UICONTROL ステータス] から [!UICONTROL 完了]. サブタスクは更新されません。
* 次の手順で [!UICONTROL 完了率] ストーリーを更新するには、 [!UICONTROL ストーリー] タブまたは [!UICONTROL 詳細] ページに表示されます。

**次の場合に [!UICONTROL 概要完了モード] プロジェクトの設定が次のように設定されている [!UICONTROL 自動]:**

* 親ストーリーをボードの向こうに移動することはできません。 次の手順で [!UICONTROL 完了率] このストーリーの場合、 [!UICONTROL 完了率] サブタスクの この [!UICONTROL 完了率] というのは、 [!UICONTROL 完了率] すべてのサブタスクの
* サブタスクを含む親ストーリーの移動先 [!UICONTROL 完了] 親ストーリーを 100%に更新し、 [!UICONTROL ステータス] から [!UICONTROL 完了]. サブタスクも 100%に更新され、 [!UICONTROL ステータス] が [!UICONTROL 完了].

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>サブタスクが存在するタスクへの [!UICONTROL Contribute] または [!UICONTROL Manage] アクセス</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## サブタスクを [!UICONTROL かんばん] ボード

1. 次に移動： [!UICONTROL かんばん] サブタスクを追加するストーリーを含むボード。
1. ストーリータイル上のタスクの名前をクリックします。 [!UICONTROL かんばん] ボード。
1. 内の他のタスクリストと同様に、タスクにサブタスクを追加します [!DNL Workfront]( [サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md).
