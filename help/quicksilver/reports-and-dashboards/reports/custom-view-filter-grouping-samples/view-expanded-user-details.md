---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：展開されたユーザーの詳細
description: このユーザービューには、ユーザーに関する情報が表示されます。名前、アクセスレベル、会社に加えて、グループ、チーム、担当業務のリストが表示されます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 67%

---

# ビュー：ユーザーの詳細の展開

<!--Audited: 11/2024-->

このユーザービューには、ユーザーに関する情報が表示されます。名前、アクセスレベル、会社に加えて、グループ、チーム、担当業務のリストが表示されます。

![expanded_user_view.png](assets/expanded-user-view-350x75.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>ビューの投稿者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーの詳細の展開を表示

この表示を適用するには次の操作を行います。

1. ユーザーのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューから、**新規表示**&#x200B;を選択します。

1. **列のプレビュー**&#x200B;領域で、1 つを除くすべての列を削除します。
1. 残りの列のヘッダーをクリックし、**テキストモードに切り替え** > **テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスで検索したテキストを削除し、次のコードに置き換えます。

   ```
   column.0.descriptionkey=name 
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=accesslevel
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=accessLevel:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=accessLevel:objCode
   column.1.link.valueformat=val
   column.1.linkedname=accessLevel
   column.1.listsort=string(displayName)
   column.1.namekey=accesslevel
   column.1.querysort=name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=accessLevel:displayName
   column.1.valueformat=HTML
   column.1.viewalias=accessLevel:displayName
   column.1.width=100
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.value=val(objCode)
   column.2.listdelimiter=
   column.2.listmethod=nested(userGroups).lists
   column.2.namekey=group.plural
   column.2.stretch=50
   column.2.type=iterate
   column.2.valuefield=group:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.displayname=Teams
   column.3.listdelimiter=
   column.3.listmethod=nested(teams).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={name}
   column.3.valueformat=HTML
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.value=val(objCode)
   column.4.listdelimiter=
   column.4.listmethod=nested(userRoles).lists
   column.4.namekey=jobrole.plural
   column.4.stretch=50
   column.4.type=iterate
   column.4.valuefield=role:name
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=company
   column.5.link.linkproperty.0.name=ID
   column.5.link.linkproperty.0.valuefield=company:ID
   column.5.link.linkproperty.0.valueformat=int
   column.5.link.lookup=link.view
   column.5.link.valuefield=company:objCode
   column.5.link.valueformat=val
   column.5.linkedname=company
   column.5.listsort=nested(company).string(name)
   column.5.namekey=company
   column.5.querysort=company:name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=company:name
   column.5.valueformat=HTML
   column.5.width=150
   ```

1. **完了**/**ビューを保存** をクリックします。
