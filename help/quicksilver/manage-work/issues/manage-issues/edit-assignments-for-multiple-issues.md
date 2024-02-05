---
product-area: projects
navigation-topic: manage-issues
title: リスト内の複数のイシューに対するユーザー割り当ての変更
description: リスト内の複数のイシューに対するユーザー割り当ての変更
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 98%

---

# リスト内の複数のイシューに対するユーザー割り当ての変更

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

複数のイシュー問題に対するユーザー割り当てを同時に変更できます。イシューを 1 件ずつ編集または割り当てる方法については、次の記事も参照してください。

* [イシューの編集](../../../manage-work/issues/manage-issues/edit-issues.md)
* [イシューの割り当て](../../../manage-work/issues/manage-issues/assign-issues.md)

問題の割り当てに関する一般的な情報については、 [問題の割り当ての変更の概要](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>イシューへの割り当てを行うには、少なくとも、そのイシューへの参加権限が必要です。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

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

## 複数のイシューの割り当てを変更

1. 割り当てを変更するイシューが含まれているイシューリストに移動します。
1. （オプション）変更する担当者に割り当てられているイシューのみを表示するフィルターを作成します。

   例えば、特定の役割を割り当て先とするイシューのみを表示するフィルターを作成できます。次に、その役割を特定のユーザーに置き換えることができます。次の操作を実行します。

   1. **フィルター**&#x200B;ドロップダウンリストをクリックして、「**新規フィルター**」をクリックします。

      新規フィルターダイアログボックスが表示されます。

   1. 「**フィルター規則の追加**」をクリックします。
   1. 特定の役割をフィルタリングするには、「**割り当てられた役割**」を展開して、「**ID**」をクリックします。

      または

      特定のユーザーをフィルタリングするには、「**割り当てられたユーザー**」を展開して、「**ID**」をクリックします。

      >[!TIP]
      >
      >「**割り当て先**」は使用しないでください。このフィールドは、すべての担当者ではなく、イシュー所有者のみを指します。

   1. ドロップダウンリストで、「**が次に等しい**」をフィルター修飾子として選択します。
   1. フィルタリングするユーザーまたは役割の名前を入力していき、名前がドロップダウンリストに表示されたら、それをクリックします。
   1. 「**フィルターの保存**」をクリックします。

1. 割り当てを変更するイシューを選択し、**編集**&#x200B;アイコン ![](assets/qs-edit-icon.png) をクリックします。

   **問題の編集**&#x200B;が表示されます。編集している項目は、ページの左上隅に表示されます。

1. 「**割り当て**」セクションに移動して、「**割り当て先**」を選択します。

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 次のいずれかの操作を行います。

   1. 新しい割り当て先を追加するには：

      1. ユーザー、役割またはチームの名前を入力していき、名前がリストに表示されたら選択します。割り当てが追加されても、選択したイシューに対する現在の割り当ては置き換わりません。

         >[!TIP]
         >
         複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
         >
         非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
         >
         * 作業アイテムをアクティブなリソースに再割り当てする。
         * 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。

         選択したすべてのイシューに共通する情報が表示されます。例えば、すべてのイシューに同じユーザーが割り当てられている場合、そのユーザーが&#x200B;**割り当て先**&#x200B;列に表示されます。選択したイシューに共通する情報でない場合は、情報は表示されません。

   1. 個々の割り当て先を削除するには：

      1. 割り当てリストに割り当て先が表示されている場合は、削除する割り当て先の名前の横にある **X アイコン**&#x200B;をクリックします。

         または

         （条件付き）削除対象の割り当て先が、選択したイシューの一部にのみ割り当てられているので「割り当て」セクションに表示されない場合は、「**担当者の削除**」をクリックして、削除する割り当て先の名前を入力していき、名前がドロップダウンリストに表示されたらクリックします。

      1. 「**担当者の削除**」をもう一度クリックして、削除する別の割り当て先を追加します。

   1. 既存の割り当て先をすべて削除するには：

      1. 「**既存の担当者をすべて削除**」をクリックし、「**はい、担当者をすべて削除します**」をクリックします。

         これにより、共通の割り当て先（編集ダイアログボックスに表示されている割り当て先）だけでなく、選択したすべてのイシューの割り当て先もすべて削除されます。

1. （オプション）イシューに関連付けるために選択した割り当て先について、次のいずれかのオプションを変更します。

   * **イシュー所有者**：ラジオボタンを選択して、どの割り当て先をイシューの所有者に指名するかを指定します。選択しない場合、Adobe Workfront は最初の割り当て先をイシューの所有者として指名します。チーム割り当てには使用できません。
   * **割り当て先の役割**：ドロップダウンリストから役割を選択します。選択しない場合、Workfront はユーザーの主要役割を自動的に選択します。

1. 「**変更を保存**」をクリックします。
