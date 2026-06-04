---
product-area: projects
navigation-topic: use-the-home-area
title: ホームエリアで項目を完了としてマーク
description: タスクまたはイシューの担当者である場合は、タスクまたはイシューを完了としてマークできます。 タスクまたはイシューを完了としてマークすると、タスクまたはイシューのステータスが完了に変わります。
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
TQID: https://experienceleague.adobe.com/KIxSnxmDRCIYGQ9Dn-sTJ-LyYQSJQqYloDbyqG9TCOs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 784
ht-degree: 77%

---

# [!UICONTROL ホーム]エリアで項目を[!UICONTROL 完了]とマーク

タスクまたはイシューの担当者である場合は、タスクまたはイシューを完了としてマークできます。 タスクまたはイシューを[!UICONTROL 完了]とマークすると、タスクまたはイシューのステータスは[!UICONTROL 完了]を変更されます。

>[!NOTE]
>
>タスクまたはイシューに割り当てられたリソースの 1 つでない限り、「[!UICONTROL 完了]」ボタンは表示されません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td> 
   <p>標準</p>
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>タスクとイシューに対する[!UICONTROL Edit]アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>作業が必要なタスクやイシューに対する参加以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## マイワークウィジェットで作業アイテムを「完了」としてマークする

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![ メインメニューアイコン ](assets/main-menu-icon.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）「**カスタマイズ**」をクリックして、**マイワーク** ウィジェットを追加します。
1. 作業項目を見つけ、作業項目の「**[!UICONTROL 完了としてマーク]**」をクリックします。
このボタンがどのように表示されるかについて詳しくは、[完了] ボタン ](#understand-the-options-of-the-done-button)のオプションについて理解する[!UICONTROL を参照してください。
   ![自分の作業マークが完了しました](assets/my-work-done.png)


## 概要パネルで作業項目を「完了」にマークする

概要パネルを使用すると、マイタスクとマイイシューのウィジェットで、作業項目を「完了」とマークすることができます。

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![ メインメニューアイコン ](assets/main-menu-icon.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）「**カスタマイズ**」をクリックして、**マイタスク**&#x200B;または&#x200B;**マイイシュー** ウィジェットを追加します。
1. 作業項目にカーソルを合わせて、**概要** アイコンをクリックします。
   ![概要を開く](assets/open-summary-new-home.png)
1. 概要パネルの上部にある「**完了としてマーク**」をクリックします。


## 「[!UICONTROL 完了]」ボタンのオプションについて

デフォルトで、作業アイテムの「[!UICONTROL 完了]」ボタンをクリックすると、その項目のステータスは[!UICONTROL 完了]（タスクの場合）または[!UICONTROL 解決済み]（イシューの場合）に変更されます。

[!DNL Adobe Workfront] 管理者は、「[!UICONTROL 完了]」ボタン関連付けられているステータスをカスタマイズできます。カスタマイズした内容はホームチームに適用できます。

「[!UICONTROL 完了]」ボタンに関連付けられているステータスの数またはタスクまたはイシューに割り当てられているリソースの数に応じて、「[!UICONTROL 完了]」ボタンの外観は変更されます。

* [1 つのステータスに関連付けられた「[!UICONTROL 完了]」ボタン](#done-button-associated-with-one-status)
* [複数のステータスに関連付けられた「[!UICONTROL 完了]」ボタン](#done-button-associated-with-multiple-statuses)
* [複数のリソースに割り当てられた項目の「[!UICONTROL 完了]」ボタン](#done-button-for-items-assigned-to-multiple-resources)

### 1 つのステータスに関連付けられた「[!UICONTROL 完了]」ボタン

「[!UICONTROL 完了]」ボタンが 1 つのステータスに関連付けられ、作業アイテムが割り当てられている場合、ボタンは&#x200B;**[!UICONTROL 完了]**&#x200B;と表示されます。 クリックすると、タスクまたはイシューのステータスは、[!UICONTROL 完了]」ボタンに関連付けされたステータスに変更されます。

![「完了」ボタン](assets/done-button-status.png)

どのステータスが「[!UICONTROL 完了]」ボタンと関連付けされているかを確認するには、[チーム設定の編集](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)で説明されるように、「[!UICONTROL 完了ボタン]」セクションのホームチームの[!UICONTROL チーム設定]を確認します。

ホームチームに割り当てられていない場合、前述の[「[!UICONTROL 完了]」ボタンのオプションについて](#understand-the-options-of-the-done-button)で説明されるように、[!UICONTROL 完了]クリック時にデフォルトのステータスが選択されます。

### 複数のステータスに関連付けられた「[!UICONTROL 完了]」ボタン

「[!UICONTROL 完了]」ボタンが複数のステータスに関連付けられている場合、ドロップダウンメニューのボタンに&#x200B;**[!UICONTROL 完了]**&#x200B;と表示されます。 このシナリオでは、簡単に「[!UICONTROL 完了]」をクリックできません。 ドロップダウンメニューからステータスを選択する必要があります。 作業アイテムの完了に最も適したステータスを選択します。 これにより、作業アイテムのステータスを変更します。

複数のステータスに「[!UICONTROL 完了]」ボタンを関連付けする方法について詳しくは、[タスクの「[!UICONTROL 完了]」ボタンの設定](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)および[イシューの「[!UICONTROL 完了]」ボタンの設定](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)を参照してください。

### 複数のリソースに割り当てられた項目の「[!UICONTROL 完了]」ボタン

タスクまたはイシューが複数のリソースに割り当てられている場合、ドロップダウンメニューのボタンに&#x200B;**[!UICONTROL 完了]**&#x200B;と表示されます。 ドロップダウンメニューでは、**[!UICONTROL 自分のパート]**&#x200B;で完了した状態（チームメンバーがタスクの自分の部分で完了したことを知らせる状態）、または[!UICONTROL 完了] ボタンに関連付けられた状態（アイテムを完了する状態）のいずれかを選択できます。 「**[!UICONTROL 担当部分は完了]**」を選択した後に、作業アイテムは作業リストから削除されますが、作業アイテムに割り当てられている作業アイテムの作業リストには残ります。\
「完了」ボタンが複数のステータスに関連付けられている場合は、そのステータスが「**担当部分は完了**」の下に表示されます。

>[!NOTE]
>
>複数の担当者がいるタスクまたはイシューの場合、各ユーザーには、タスクまたはイシューに対する自分の割り当てが実際に完了したことを示す責任があります。 この理由から、各担当者は「[!UICONTROL 完了]」をクリックし、項目に割り当てられた作業が完了したことを示す必要があります。

![自分のパートで完了](assets/done-with-my-part.png)

