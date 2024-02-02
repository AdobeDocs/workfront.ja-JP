---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：タスクビューでのプログラムとポートフォリオに関する情報の表示
description: このタスクビューには、タスクのプロジェクトに関連付けられたプログラムとポートフォリオが表示されます。この情報は、タスクビューの作成時に Report Builder で使用できません。使用できるのはテキストモードのみです。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '555'
ht-degree: 100%

---

# 表示：タスクビューでのプログラムとポートフォリオに関する情報の表示

このタスクビューには、タスクのプロジェクトに関連付けられたプログラムとポートフォリオが表示されます。この情報は、タスクビューの作成時に Report Builder で使用できません。使用できるのはテキストモードのみです。

タスクリストからプロジェクト、プログラム、ポートフォリオへのリンクも表示されます。

![](assets/view--program-and-portfolio-350x116.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>表示の変更をリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タスクビューでのプログラムとポートフォリオに関する情報の表示

このビューをタスクリストに適用するには：

1. タスクのリストに移動します。
1. 「**ビュー**」ドロップダウンメニューから「**新しいビュー**」を選択します。

1. 「**カラムのプレビュー**」エリアで、1 以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、「**テキストモードに切り替え**」を選択します。
1. 「テキストモード」エリアにマウスを移動し、「**クリックするとテキストを編集できます**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=project:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayname=Program<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=project:program:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=project:program:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program).string(name)<br>column.2.namekey=project<br>column.2.querysort=project:program:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=project:program:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=portfolio<br>column.3.displayname=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=project:portfolio:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=project:portfolio:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:portfolio).string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=project:portfolio:name<br>column.3.valueformat=HTML<br>column.3.width=150 </pre>

1. 「**ビューを保存**」をクリックします。
