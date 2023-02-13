---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：タスクの'
description: タスクリストにカスタムビューを追加し、リストをエクスポートする前にこのビューが選択されていることを確認することで、エクスポートしたタスクリストで親と子の関係の区別を維持できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 表示：タスクをインデントして、タスク内に親子関係を表示する

タスクリストにカスタムビューを追加し、リストをエクスポートする前にこのビューが選択されていることを確認することで、エクスポートしたタスクリストで親と子の関係の区別を維持できます。  

![](assets/parent-child-indented-custom-view-350x94.png)

1. 書き出すタスクリストが含まれるプロジェクトに移動します。
1. 次をクリック： **表示** ドロップダウンメニューで、 **新しいビュー**.

1. 画面の左上隅でフィルターに名前を付けます。
1. をクリックします。 **タスク名** 列ヘッダー。

1. 選択 **テキストモードに切り替え** をクリックします。
1. テキストボックス内の任意の場所をクリックして、テキストを編集し、既存のテキストをすべて削除します。
1. 次のテキストを貼り付けます。

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. 「**保存**」をクリックします。
1. クリック **ビューを保存**.
