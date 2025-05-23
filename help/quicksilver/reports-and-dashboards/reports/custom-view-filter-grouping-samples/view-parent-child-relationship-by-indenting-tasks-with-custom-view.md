---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：タスクをインデントしてタスクの親子関係を表示します
description: タスクリストにカスタムビューを追加し、リストを書き出す前にこのビューが選択されていることを確認することで、書き出したタスクリストで親子関係の区別を維持できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 81%

---

# ビュー：タスクをンデントしてタスク内の親子関係を表示

<!--Audited: 11/2024-->

タスクリストにカスタムビューを追加し、リストを書き出す前にこのビューが選択されていることを確認することで、書き出したタスクリストで親子関係の区別を維持できます。

![ 親の子インデント ](assets/parent-child-indented-custom-view-350x94.png)

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
   <td> <p> 現在： 
   <ul>
   <li>表示の変更をリクエスト</li> 
   <li>レポートを変更するためのプラン</li>
   </ul>
     </p>
     <p> 新規： 
   <ul>
   <li>ビューを変更する場合は Contributor</li> 
   <li>レポートを変更する場合は Standard</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
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
