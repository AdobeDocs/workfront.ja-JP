---
title: フィールドを削除
description: Adobe Workfront Planning では、関係なくなったカスタムフィールドを削除できます。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 56%

---



# フィールドの削除

{{planning-important-intro}}

Adobe Workfront Planning では、カスタムフィールドを作成して、レコードに関する情報を格納できます。

Workfront Planning でのカスタムフィールドの作成について詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

関係がなくなった Workfront Planning フィールドは削除できます。

## Workfront Planning フィールドの削除に関する考慮事項：

* レコードタイプのテーブルビューでのみフィールドを削除できます。
* レコードの主フィールドは削除できません。
* フィールドに格納されている情報はすべて削除され、復元できません。
* 接続したレコードフィールドを削除すると、接続したすべてのルックアップフィールドも接続元のレコードタイプから削除されます。 接続先のレコードタイプの接続済みレコードフィールドも、接続先のレコードから削除されます。

  例えば、キャンペーンを製品と呼ばれる別のレコードタイプに接続し、キャンペーンから「製品の接続」フィールドと「製品のステータス」ルックアップフィールドを削除すると、次の項目が削除されます。

   * キャンペーンの「接続済み製品」フィールド
   * キャンペーンの「製品ステータス」ルックアップフィールド
   * 製品の「キャンペーンに接続」フィールド。

  詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront計画*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準 </p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--

OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## フィールドを削除

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. レコード フィールドを削除するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプが表示されます。

1. レコードタイプのカードをクリックします。

1. （条件付き）選択していない場合は、レコードタイプページで **テーブル表示** のタブをクリックします。

   そのレコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。

1. 削除するフィールドを列ヘッダーで見つけてその上にポインタを合わせ、フィールド名の後の下向き矢印をクリックします。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 「**削除**」をクリックします。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 「**削除**」をクリックして確定します。

   フィールドが削除され、復元できなくなり、レコードと関連付けられなくなります。
