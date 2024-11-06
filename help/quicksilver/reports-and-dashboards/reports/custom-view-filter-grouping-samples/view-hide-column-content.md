---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：列の内容を非表示'
description: ビューの列で情報を非表示にしたい場合があります。これを行うには、列のテキストモードを変更します。
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 79%

---

# 表示：列の内容を非表示にする

<!--Audited: 11/2024-->

ビューの列で情報を非表示にしたい場合があります。これを行うには、列のテキストモードを変更します。

>[!NOTE]
>
>* 非表示の列を使用して、ビューに表示しない特定のオブジェクトで並べ替えることができます。\
>  例えば、タスクビューでタスク番号順に並べ替え、タスク番号情報をビューで非表示にすることができます。この場合、列で参照されるオブジェクトはビューの並べ替えに役立ちますが、そのオブジェクトの情報はビューには表示されません。
>* 列を非表示にする場合、列の情報は非表示になりますが、列はビューに依然として存在します。
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：<ul><li>ビューを変更する場合は Contributor</li><li>レポートを変更する場合は Standard</li></ul></p><p>または</p>現在：<ul><li>表示の変更をリクエスト</li><li>レポートを変更するためのプラン</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 例：タスクビューでのタスク番号列の並べ替えと非表示

1. タスクのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックして、「**このカラムに表示**」フィールドに「タスク番号」と入力していき、リストに表示されたら選択します。

1. **テキストモードに切り替え** をクリックし、**テキストを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスで検索したテキストを削除し、次のコードに置き換えます。

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   このコードの重要な変更点は次のとおりで、その結果、列が非表示になります。

   * `displayname=`：この行は空白にする必要があります。
   * `valuefield=`：これは `value` に置き換えられました。空白にする必要があります。
   * `width=`: フィールドによって、値は **0** または **1** である必要があります。

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。
