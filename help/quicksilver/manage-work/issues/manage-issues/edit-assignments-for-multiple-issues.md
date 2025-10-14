---
product-area: projects
navigation-topic: manage-issues
title: リスト内の複数のイシューに対するユーザー割り当ての変更
description: リスト内の複数のイシューに対するユーザー割り当ての変更
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 87%

---

# リスト内の複数のイシューに対するユーザー割り当ての変更

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

複数のイシューに対するユーザーの割り当てを同時に変更できます。 イシューの編集または一度に 1 つずつ割り当てる方法について詳しくは、次の記事も参照してください。

* [イシューの編集](../../../manage-work/issues/manage-issues/edit-issues.md)
* [イシューの割り当て](../../../manage-work/issues/manage-issues/assign-issues.md)

イシューの割り当てに関する一般情報については、[イシューの割り当て変更の概要](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)を参照してください。

>[!NOTE]
>
>イシューへの割り当てを行うには、少なくとも、そのイシューへの参加権限が必要です。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新規：標準 </p>
   <p>現在：Request 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトおよびタスクへの表示以上のアクセス権を持ち、1 つの問題を割り当てる</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>複数のイシューを割り当てる場合は、イシューが存在するプロジェクトまたはタスクに対する権限以上を投稿します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

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

1. 割り当てを変更するイシューを選択して、**編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/qs-edit-icon.png) をクリックします。

   **イシューの編集**&#x200B;が表示されます。編集している項目は、ページの左上隅に表示されます。

1. 「**割り当て**」セクションに移動して、「**割り当て先**」を選択します。

   ![&#x200B; 割り当てエリア &#x200B;](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 次のいずれかの操作を行います。

   1. 新しい割り当て先を追加するには：

      1. ユーザー、役割またはチームの名前を入力していき、名前がリストに表示されたら選択します。割り当てが追加されても、選択したイシューに対する現在の割り当ては置き換わりません。

         >[!TIP]
         >
         >複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
         >
         >非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
         >
         >* 作業アイテムをアクティブなリソースに再割り当てする。
         >* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。

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
