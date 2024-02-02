---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：列の内容を非表示にする」
description: ビューの列で情報を非表示にしたい場合があります。これを行うには、列のテキストモードを変更します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '419'
ht-degree: 100%

---

# 表示：列の内容を非表示にする

ビューの列で情報を非表示にしたい場合があります。これを行うには、列のテキストモードを変更します。

>[!TIP]
>
>* 非表示の列を使用して、ビューに表示しない特定のオブジェクトで並べ替えることができます。\
>  例えば、タスクビューでタスク番号順に並べ替え、タスク番号情報をビューで非表示にすることができます。この場合、列で参照されるオブジェクトはビューの並べ替えに役立ちますが、そのオブジェクトの情報はビューには表示されません。
>* 列を非表示にする場合、列の情報は非表示になりますが、列はビューに依然として存在します。
>

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

## 例：タスクビューでのタスク番号列の並べ替えと非表示

1. タスクのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックして、「**このカラムに表示**」フィールドに「タスク番号」と入力していき、リストに表示されたら選択します。

1. 「**テキストモードに切り替える**」をクリックします。
1. テキストモードエリアにポインタを合わせて、「**クリックするとテキストを編集できます**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>このコードの重要な変更点は次のとおりで、その結果、列が非表示になります。

   ```
   displayname
   ```

   この行は空白にする必要があります。

   ```
   valuefield
   ```

   これは *value* に置き換えられており、空白にする必要があります。

   ```
   width
   ```

   フィールドに応じて、この値は *0* または *1* にする必要があります。

1. 「**保存**」をクリックして、「**ビューの保存**」します。
