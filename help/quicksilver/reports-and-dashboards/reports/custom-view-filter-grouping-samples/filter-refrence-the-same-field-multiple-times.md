---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「フィルター：同じフィールドを参照する複数のフィルタールール（「AND」ステートメント）を作成する」
description: 標準モードのインターフェイスでは、同じフィールドを参照する複数のフィルターを（AND 修飾子を使用して）作成しようとした場合、レポートを保存して Report Builder を終了すると、フィルターの 1 つが削除されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '447'
ht-degree: 100%

---

# フィルター：同じフィールドを参照する複数のフィルタールール（「AND」ステートメント）を作成する

標準モードのインターフェイスでは、同じフィールドを参照する複数のフィルターを（AND 修飾子を使用して）作成しようとした場合、レポートを保存して Report Builder を終了すると、フィルターの 1 つが削除されます。

**例：**&#x200B;名前に「緑」という単語を含み、「赤」という単語を含まないタスクのみを表示したい場合。Adobe Workfront では、同じフィールド（タスク名）を参照しますが、異なる修飾子を使用し、異なる値を参照するので、標準モードインターフェイスを使用して次のフィルタールールを保存することはできません。

* タスク名／含む／緑
* タスク名／含まない／赤

ただし、このフィルターはテキストモードを使用して作成できます。

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
   <td> <p>フィルターを変更する場合は「要求」 </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 同じフィールドを参照する複数のフィルタールールの作成

1. タスクのリストに移動します。
1. **フィルター**&#x200B;ドロップダウンメニューから、「**新規フィルター**」を選択します。
1. 「**テキスト モードに切り替える**」をクリックします。
1. テキストモード領域にポインタを合わせ、「**クリックするとテキストを編集できます**」をクリックします。
1. 「報告書のフィルター ルールを設定してください」領域に、次のコードを追加します。

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

1. 「**完了**」をクリックして、「**フィルターの保存**」を選択します。
