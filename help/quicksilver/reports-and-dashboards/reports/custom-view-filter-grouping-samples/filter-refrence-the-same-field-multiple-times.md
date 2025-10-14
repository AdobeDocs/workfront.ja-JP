---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「フィルター：同じフィールド（「AND」ステートメント）を参照する複数のフィルタールールを作成する」
description: 標準モードのインターフェイスでは、同じフィールドを参照する複数のフィルターを（AND 修飾子を使用して）作成しようとした場合、レポートを保存して Report Builder を終了すると、フィルターの 1 つが削除されます。
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 86%

---

# フィルター：同じフィールドを参照する複数のフィルタールール（「AND」ステートメント）を作成する

<!--Audited: 10/2024-->

標準モードのインターフェイスでは、同じフィールドを参照する複数のフィルターを（AND 修飾子を使用して）作成しようとした場合、レポートを保存して Report Builder を終了すると、フィルターの 1 つが削除されます。

**例：**&#x200B;名前に「緑」という単語を含み、「赤」という単語を含まないタスクのみを表示したい場合。Adobe Workfront では、同じフィールド（タスク名）を参照しますが、異なる修飾子を使用し、異なる値を参照するので、標準モードインターフェイスを使用して次のフィルタールールを保存することはできません。

* タスク名／含む／緑
* タスク名／含まない／赤

ただし、このフィルターはテキストモードを使用して作成できます。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 同じフィールドを参照する複数のフィルタールールの作成

1. タスクのリストに移動します。
1. **フィルター**&#x200B;ドロップダウンメニューから、「**新規フィルター**」を選択します。
1. **テキストモード** をクリックします。
1. 表示されたボックスに、次のコードを追加します。

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >類似のフィルターを作成するには、まず最初のステートメントを作成します。例：
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >ステートメントを必要な回数だけコピー＆ペーストします。次に、同じフィールド（この場合は「name」）を参照するステートメントを必要な数だけ追加し、追加のステートメントに次の変更を加えます。
   >
   >1. コピーした 2 行の先頭に、新しいフィールドの可能な値ごとに「AND:1:」、「AND:2:」、「AND:3:」などを追加します。
   >1. フィールド行を新しいフィールド値（「=」記号の後）に置き換えます。
   >1. 修飾子行（_Mod）を新しい修飾子に置き換えます。
   >   
   >これらのステートメントでは大文字と小文字が区別されます。

1. **適用** をクリックしてから、**新規保存** をクリックします。
