---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：タスクをインデントしてタスクの親子関係を表示します
description: タスクリストにカスタムビューを追加し、リストを書き出す前にこのビューが選択されていることを確認することで、書き出したタスクリストで親子関係の区別を維持できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 72%

---

# ビュー：タスクをンデントしてタスク内の親子関係を表示

<!--Audited: 11/2024-->

タスクリストにカスタムビューを追加し、リストを書き出す前にこのビューが選択されていることを確認することで、書き出したタスクリストで親子関係の区別を維持できます。

![&#x200B; 親の子インデント &#x200B;](assets/parent-child-indented-custom-view-350x94.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>ビューの投稿者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


+++

## タスクをインデントしてタスク内の親子関係を表示

1. 書き出すタスクリストが含まれるプロジェクトに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューをクリックし、**新規ビュー**&#x200B;を選択します。
1. 「**タスク名**」列ヘッダーをクリックします。
1. 右上隅の「**テキストモードに切り替え**」を選択します。
1. **テキストモードを編集** をクリックし、既存のテキストをすべて削除します。
1. 次のテキストを貼り付けます。


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. **完了**/**ビューを保存** をクリックします。
