---
product-area: projects
navigation-topic: manage-issues
title: リスト内の複数の問題に対するユーザー割り当てを変更する
description: リスト内の複数の問題に対するユーザー割り当てを変更する
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# リスト内の複数の問題に対するユーザー割り当てを変更する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

複数のイシューに対するユーザー割り当てを同時に変更できます。 問題の編集や割り当てについては、次の記事も参照してください。

* [問題の編集](../../../manage-work/issues/manage-issues/edit-issues.md)
* [問題の割り当て](../../../manage-work/issues/manage-issues/assign-issues.md)

問題の割り当てに関する一般情報については、 [問題の割り当ての変更の概要](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>1 つのイシューに割り当てを行うには、少なくとも Contribute の権限が必要です。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>問題へのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>問題に対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 複数の問題の割り当てを変更

1. 割り当てを変更するタスクの一覧を表示します。
1. （オプション）変更する担当者に割り当てられた問題のみを表示するフィルターを作成します。

   例えば、特定の役割を担当者として持つ問題のみを表示するフィルターを作成できます。 次に、役割を特定のユーザーに置き換えます。 次の操作を実行します。

   1. 次をクリック： **フィルター** ドロップダウンリストから、 **新しいフィルター**.

      [ 新しいフィルタ ] ダイアログボックスが表示されます。

   1. クリック **フィルタールールを追加します。**
   1. 特定の役割に対してフィルターを適用するには、を展開します。 **割り当ての役割、** 次に、 **ID。**

      または

      特定のユーザーに対してフィルターを適用するには、を展開します。 **割り当てユーザー、** 次に、 **ID。**

      >[!TIP]
      >
      >使用しない **割り当て先** このフィールドは、すべての担当者ではなく、問題の所有者のみを参照するので、

   1. ドロップダウンリストで、「 」を選択します。 **次と等しい** をフィルタ修飾子として使用します。
   1. フィルターするユーザーまたは役割の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。
   1. クリック **フィルターを保存します。**

1. 割り当てを変更する懸案事項を選択し、 **編集** アイコン ![](assets/qs-edit-icon.png).

   この **問題の編集** が表示されます。 編集された項目は、ページの左上隅に表示されます。

1. 次に移動： **割り当て** 「 」セクションで、「 **担当者**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 次のいずれかの操作を行います。

   1. 新しい担当者を追加するには：

      1. ユーザー、ロール、またはチームの名前を入力し、リストに表示されたら選択します。 割り当てが追加され、選択した問題に対する現在の割り当ては置き換えられません。

         >[!TIP]
         複数のユーザー、ジョブの役割またはチームを割り当てることができます。 アクティブなユーザー、ジョブの役割およびチームのみを割り当てることができます。
         非アクティブ化前にユーザー、ジョブの役割、またはチームが割り当てられた場合、そのユーザーは作業項目に割り当てられたままになります。 この場合、次の操作をお勧めします。
         * 作業項目をアクティブなリソースに再割り当てする。
         * 非アクティブなチームのユーザをアクティブなチームに関連付け、作業項目をアクティブなチームに再割り当てします。


         選択したすべての問題で共通する情報が表示されます。 例えば、同じユーザーがすべてのイシューに割り当てられている場合、そのユーザーは **担当者** 列。 選択した問題に関する情報が共通でない場合は、情報は表示されません。
   1. 個々の担当者を削除するには：

      1. 次をクリック： **X アイコン** 担当者が「割り当て」リストに表示される場合に削除する担当者の名前の横に表示されます。

         または

         （条件付き）削除する担当者が、選択した問題の一部にのみ担当者が割り当てられているので、[ 割り当て ] セクションに表示されない場合は、[ **担当者を削除** 削除する担当者の名前を入力し、ドロップダウンリストに表示されたら、名前をクリックします。

      1. クリック **担当者を削除** 再度追加して、削除する別の担当者を追加します。
   1. 既存のすべての担当者を削除するには：

      1. クリック **既存の担当者をすべて削除**&#x200B;を選択し、「 **はい、すべての担当者を削除します**.

         これにより、共通の担当者（編集ダイアログボックスに表示される担当者）だけでなく、選択したすべての問題に関するすべての担当者も削除されます。



1. （オプション）問題に関連付けるために選択した担当者に対して、次のオプションを変更します。

   * **問題の所有者：** ラジオボタンを選択して、どの担当者を問題の所有者に指定するかを指定します。 選択しない場合、Adobe Workfrontは最初の担当者を問題の所有者に指定します。 チーム割り当てには使用できません。
   * **担当者の役割**:ドロップダウンリストから役割を選択します。 選択しない場合、Workfrontはユーザーのプライマリロールを自動的に選択します。

1. クリック **変更を保存**.
