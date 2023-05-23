---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：すべてのプロジェクトチームユーザーと役割を持つプロジェクト'
description: このプロジェクトビューには、プロジェクトチームに割り当てられたユーザーとジョブの役割のリストが表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# 表示：すべてのプロジェクトチームユーザーと役割を持つプロジェクト

このプロジェクトビューには、プロジェクトチームに割り当てられたユーザーとジョブの役割のリストが表示されます。

>[!NOTE]
>
>ジョブの役割がユーザーと同じ行に表示される場合、これは、ユーザーがプロジェクトでその役割を満たしていることや、ユーザーのプロファイルにその役割が割り当てられていることを意味するものではありません。

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## すべてのプロジェクトチームユーザーと役割を持つプロジェクトの表示

1. プロジェクトのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。
   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=チームユーザー<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.namekey=user.plural<br>column.1.stretch=30<br>column.1.type=iterate<br>column.1.valuefield=user:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=チームロール<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles).lists<br>column.2.namekey=jobrole.plural<br>column.2.stretch=10<br>column.2.type=iterate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150.stretch=0</pre>

1. クリック **ビューを保存**.
