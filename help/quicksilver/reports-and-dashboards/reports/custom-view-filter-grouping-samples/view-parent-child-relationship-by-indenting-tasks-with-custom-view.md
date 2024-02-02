---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：タスクをインデントしてタスク内の親子関係を表示」
description: タスクリストにカスタムビューを追加し、リストを書き出す前にこのビューが選択されていることを確認することで、書き出したタスクリストで親子関係の区別を維持できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '299'
ht-degree: 100%

---

# ビュー：タスクをンデントしてタスク内の親子関係を表示

タスクリストにカスタムビューを追加し、リストを書き出す前にこのビューが選択されていることを確認することで、書き出したタスクリストで親子関係の区別を維持できます。

![](assets/parent-child-indented-custom-view-350x94.png)

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

## タスクをインデントしてタスク内の親子関係を表示

1. 書き出すタスクリストが含まれるプロジェクトに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューをクリックし、**新規ビュー**&#x200B;を選択します。

1. 画面の左上隅でフィルターに名前を付けます。
1. 「**タスク名**」列ヘッダーをクリックします。

1. 右上隅の「**テキストモードに切り替える**」を選択します。
1. テキストボックス内の任意の場所をクリックしてテキストを編集し、既存のテキストをすべて削除します。
1. 次のテキストを貼り付けます。

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. 「**保存**」をクリックします。
1. 「**ビューを保存**」をクリックします。
