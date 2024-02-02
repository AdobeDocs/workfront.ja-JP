---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: かんばんボードの既存のストーリーへのサブタスクの追加
description: かんばんボード上の既存のストーリーのサブタスクを作成する方法については、この記事を参照してください。
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: ht
source-wordcount: '363'
ht-degree: 100%

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

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront]管理者がアクセスレベルを変更する方法については、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>サブタスクが存在するタスクへの[!UICONTROL Contribute]または[!UICONTROL Manage]アクセス</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!UICONTROL かんばん]ボードの既存のストーリーにサブタスクを追加

1. サブタスクを追加するストーリーを含む[!UICONTROL かんばん]ボードに移動します。
1. [!UICONTROL かんばん]ボードのストーリータイル上のタスクの名前をクリックします。
1. [!DNL Workfront] 内の他のタスクリストと同様に、[サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md)の説明のとおりに、タスクにサブタスクを追加します。
