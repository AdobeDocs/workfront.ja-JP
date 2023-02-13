---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"フィルタ：同じフィールド（''AND''ステートメント）を参照する複数のフィルタールールを作成」'
description: 標準モードのインターフェイスでは、同じフィールド（AND 修飾子を使用）を参照する複数のフィルタを作成しようとすると、レポートを保存して Report Builder を終了すると、いずれかのフィルタが削除されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# フィルター：同じフィールド（「AND」ステートメント）を参照する複数のフィルタールールを作成する

標準モードのインターフェイスでは、同じフィールド（AND 修飾子を使用）を参照する複数のフィルタを作成しようとすると、レポートを保存して Report Builder を終了すると、いずれかのフィルタが削除されます。

**例：** 「green」という単語を含み、名前に「red」という単語を含まないタスクのみを表示する場合があります。 Adobe Workfrontでは、標準モードインターフェイスを使用して次のフィルタールールを保存できません。同じフィールド（タスク名）を参照し、異なる修飾子を使用し、異なる値を参照するからです。

* タスク名/次を含む/緑
* タスク名/次を含まない/赤

ただし、テキストモードを使用してこのフィルターを作成できます。

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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 同じフィールドを参照する複数のフィルタールールを作成する

1. タスクのリストに移動します。
1. 次の **フィルター** ドロップダウンメニューで、「 **新しいフィルター**.
1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 「レポートのフィルタールールを設定」領域に次のコードを追加します。

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >類似したフィルターを作成するには、最初の文を最初に作成します。 例：
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >文を必要な回数だけコピーして貼り付けます。 その後、同じフィールド（この例では「name」）を参照する必要があるステートメントをいくつでも追加でき、追加のステートメントに次の変更を加えます。
   >
   >1. コピーした 2 つの行の前に「AND」を付けます。:1:&quot;, &quot;および:2:&quot;, &quot;および:3:」など ) を含め、新しいフィールドの可能な値ごとに異なります。
   >1. フィールド行を新しいフィールド値（「=」記号の後）に置き換えます。
   >1. モディファイヤ行 (_Mod) を新しいモディファイヤに置き換えます。

   >   
   >これらの文では大文字と小文字が区別されます。

1. クリック **完了**&#x200B;を、 **フィルターを保存**.
