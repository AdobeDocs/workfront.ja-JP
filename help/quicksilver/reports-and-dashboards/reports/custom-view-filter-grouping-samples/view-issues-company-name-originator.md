---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：発信元の会社名に関するイシュー」
description: このイシュービューには、イシューを送信したユーザーに関連付けられた会社名が表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '481'
ht-degree: 100%

---

# ビュー：発信元の会社名に関するイシュー

このイシュービューには、イシューを送信したユーザーに関連付けられた会社名が表示されます。

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## 発信元の会社名に関するイシューを表示

この表示を適用するには次の操作を行います。

1. イシューのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューから、**新規表示**&#x200B;を選択します。

1. **列のプレビュー**&#x200B;エリアで、1 つを除くすべての列を削除します。
1. 残りの列のヘッダーをクリックし、「**テキストモードに切り替え**」を選択します。
1. テキストモードエリアにカーソルを置き、「**クリックしてテキストを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=val<br>column.0.link.lookup=link.view<br>column.0.link.value=val(objCode)<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=140<br>column.1.descriptionkey=originator<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ownerID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=owner:objCode<br>column.1.link.valueformat=val<br>column.1.listsort=nested(owner).string(name)<br>column.1.namekey=originator.abbr<br>column.1.querysort=owner:name<br>column.1.valuefield=owner:name<br>column.1.valueformat=HTML<br>column.1.width=151<br>column.2.descriptionkey=entrydate<br>column.2.listsort=atDateAsAtDate(entryDate)<br>column.2.namekey=entrydate.abbr<br>column.2.querysort=entryDate<br>column.2.valuefield=entryDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=age<br>column.3.listsort=doubleAsDouble(age)<br>column.3.namekey=age<br>column.3.querysort=age<br>column.3.valuefield=howOld<br>column.3.valueformat=val<br>column.3.width=80<br>column.4.viewalias=statusicons<br>column.4.displayname=フラグ<br>column.4.linkedname=direct<br>column.4.namekey=statusicons<br>column.4.valuefield=<br>column.4.valueformat=HTML<br>column.4.querysort=<br>column.4.tile.name=component.issuestatusicons<br>column.4.tile.pdfcomponent=issueStatusIcons<br>column.4.delimiter=<br>column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp<br>column.5.description=発信元の会社名<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=owner:companyID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valuefield=owner:company:objCode<br>column.5.link.valueformat=val<br>column.5.listsort=nested(owner:company).string(name)<br>column.5.name=発信元の会社<br>column.5.querysort=owner:company:name<br>column.5.valuefield=owner:company:name<br>column.5.valueformat=HTML<br>column.5.width=151</pre>

1. 「**ビューを保存**」をクリックします。
