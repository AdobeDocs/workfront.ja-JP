---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：タスクの後続タスクの一覧を列に追加する'
description: タスクビューに列を追加して、タスクの後続タスクの一覧を表示できます。 「タスクの後続タスク」列には、後続タスクの番号と名前が表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 表示：タスクの後続タスクの一覧を列に追加する

タスクビューに列を追加して、タスクの後続タスクの一覧を表示できます。 この **タスクの後続タスク** 列には、後続の番号と名前が含まれます。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクの後続タスクの一覧を列に追加する

この列をタスクビューに追加するには、次の手順に従います。

1. 既存のタスクビューに移動します。
1. 「表示」ドロップダウンメニューを展開し、「 」を選択します。 **表示をカスタマイズ**.
1. クリック **列を追加**.
1. クリック **テキストモードに切り替え**.
1. マウスを **この列に表示** 領域をクリックし、 **クリックしてテキストを編集**.

1. 「テキストモード」ボックスのすべてのテキストを削除し、次のコードに置き換えます。

   <pre>displayname=タスクの後続タスク<br>listdelimiter=<br><br>listmethod=nested(successors).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({successor}.{taskNumber}、' - ',{successor}。{name})<br>valueformat=HTML</pre>

1. クリック **ビューを保存**.
