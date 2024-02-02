---
product-area: projects
navigation-topic: use-the-home-area
title: ホームエリアで項目を完了としてマーク
description: タスクまたはイシューの担当者である場合は、タスクまたはイシューを完了としてマークできます。タスクまたはイシューを完了としてマークすると、タスクまたはイシューのステータスが完了に変わります。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: ht
source-wordcount: '808'
ht-degree: 100%

---

# [!UICONTROL ホーム]エリアで項目を[!UICONTROL 完了]とマーク

タスクまたはイシューの担当者である場合は、タスクまたはイシューを完了としてマークできます。タスクまたはイシューを[!UICONTROL 完了]とマークすると、タスクまたはイシューのステータスは[!UICONTROL 完了]を変更されます。

>[!NOTE]
>
>タスクまたはイシューに割り当てられたリソースの 1 つでない限り、「[!UICONTROL 完了]」ボタンは表示されません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>タスクとイシューに対する[!UICONTROL Edit]アクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されているか [!DNL Workfront] 管理者に確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>作業が必要なタスクやイシューに対する参加以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト </a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## タスクまたはイシューを[!UICONTROL 完了]としてマーク

タスクまたはイシューに割り当てられたユーザーのみが、タスクまたはイシューを[!UICONTROL 完了]としてマークできます。

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) をクリックして、「**[!UICONTROL ホーム]**」をクリックします。
1. **[!UICONTROL 作業リスト]**&#x200B;で、作業待ちの項目を探します。
1. 次のいずれかの操作を行います。

* 作業アイテムの「**[!UICONTROL 完了]**」をクリックします。\
   このボタンの表示方法について詳しくは、[「[!UICONTROL 完了]」ボタンのオプションについて](#understand-the-options-of-the-done-button)を参照してください。

* 完了としてマークする項目を選択し、右側のパネルで「**[!UICONTROL 更新状態]**」をクリックして、項目のステータスを[!UICONTROL 完了]または[!UICONTROL クローズ]に等しいステータスに変更します。

## 「[!UICONTROL 完了]」ボタンのオプションについて

デフォルトで、作業アイテムの「[!UICONTROL 完了]」ボタンをクリックすると、その項目のステータスは[!UICONTROL 完了]（タスクの場合）または[!UICONTROL 解決済み]（イシューの場合）に変更されます。

[!DNL Adobe Workfront] 管理者は、「[!UICONTROL 完了]」ボタン関連付けられているステータスをカスタマイズできます。カスタマイズした内容はホームチームに適用できます。

「[!UICONTROL 完了]」ボタンに関連付けられているステータスの数またはタスクまたはイシューに割り当てられているリソースの数に応じて、「[!UICONTROL 完了]」ボタンの外観は変更されます。

* [1 つのステータスに関連付けられた「[!UICONTROL 完了]」ボタン](#done-button-associated-with-one-status)
* [複数のステータスに関連付けられた「[!UICONTROL 完了]」ボタン](#done-button-associated-with-multiple-statuses)
* [複数のリソースに割り当てられた項目の「[!UICONTROL 完了]」ボタン](#done-button-for-items-assigned-to-multiple-resources)

### 1 つのステータスに関連付けられた「[!UICONTROL 完了]」ボタン

「[!UICONTROL 完了]」ボタンが 1 つのステータスに関連付けられ、作業アイテムが割り当てられている場合、ボタンは&#x200B;**[!UICONTROL 完了]**&#x200B;と表示されます。クリックすると、タスクまたはイシューのステータスは、[!UICONTROL 完了]」ボタンに関連付けされたステータスに変更されます。

![「完了」ボタン](assets/Done.png)

どのステータスが「[!UICONTROL 完了]」ボタンと関連付けされているかを確認するには、[チーム設定の編集](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)で説明されるように、「[!UICONTROL 完了ボタン]」セクションのホームチームの[!UICONTROL チーム設定]を確認します。

ホームチームに割り当てられていない場合、前述の[「[!UICONTROL 完了]」ボタンのオプションについて](#understand-the-options-of-the-done-button)で説明されるように、[!UICONTROL 完了]クリック時にデフォルトのステータスが選択されます。

### 複数のステータスに関連付けられた「[!UICONTROL 完了]」ボタン

「[!UICONTROL 完了]」ボタンが複数のステータスに関連付けられている場合、ドロップダウンメニューのボタンに&#x200B;**[!UICONTROL 完了]**&#x200B;と表示されます。このシナリオでは、簡単に「[!UICONTROL 完了]」をクリックできません。ドロップダウンメニューからステータスを選択する必要があります。作業アイテムの完了に最も適したステータスを選択します。これにより、作業アイテムのステータスを変更します。

複数のステータスに「[!UICONTROL 完了]」ボタンを関連付けする方法について詳しくは、[タスクの「[!UICONTROL 完了]」ボタンの設定](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)および[イシューの「[!UICONTROL 完了]」ボタンの設定](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)を参照してください。

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### 複数のリソースに割り当てられた項目の「[!UICONTROL 完了]」ボタン

タスクまたはイシューが複数のリソースに割り当てられている場合、ドロップダウンメニューのボタンに&#x200B;**[!UICONTROL 完了]**&#x200B;と表示されます。ドロップダウンメニューで、「**[!UICONTROL 担当部分は完了]**」（これにより、チームメンバーは、お客様のタスクの一部が完了したことを知ることができます）、または「[!UICONTROL 完了]」ボタン（項目を完了する）に関連するステータスのどちらかを選択できます。「**[!UICONTROL 担当部分は完了]**」を選択した後に、作業アイテムは作業リストから削除されますが、作業アイテムに割り当てられている作業アイテムの作業リストには残ります。\
「完了」ボタンが複数のステータスに関連付けられている場合は、そのステータスが「**担当部分は完了**」の下に表示されます。

>[!NOTE]
>
>複数の担当者がいるタスクまたはイシューの場合、各ユーザーには、タスクまたはイシューに対する自分の割り当てが実際に完了したことを示す責任があります。この理由から、各担当者は「[!UICONTROL 完了]」をクリックし、項目に割り当てられた作業が完了したことを示す必要があります。

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
