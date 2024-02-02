---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：タスクリストでのタスクのインデントの表示」
description: このタスクビューでは、タスク名列にコードを追加して、プロジェクトの作業分割構造に従ってインデントされたタスクを表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '286'
ht-degree: 100%

---

# ビュー：タスクリストでのタスクのインデントの表示

このタスクビューでは、タスク名列にコードを追加して、プロジェクトの作業分割構造に従ってインデントされたタスクを表示できます。

![](assets/view-text-mode-indentation-task-list-350x171.png)

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

## タスクリストの列にタスクのインデントを表示する

1. タスクのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックして、「**この列に表示**」フィールドの「タスク名」の入力を開始し、リストに表示されたら選択します。

1. 新しい列で、「**テキストモードに切り替える**」をクリックします。
1. テキストモードエリアにポインタを合わせて、「**クリックするとテキストを編集できます**」をクリックします。
1. 行内にあるテキストを削除し、

   ```
   valuefield=
   ```

   次のコードに置き換えます。

   ```
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. 「**保存**」をクリックし、次に「**表示を保存**」をクリックします。
