---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''グループ化：グループ化内のすべてのオブジェクトに共通の計算値でリスト結果を整理します'
description: タスクを「完了率」でグループ化し、0 ～ 25、26 ～ 50、51 ～ 75、75 ～ 99、100 の範囲で表示することができます。 テキストモードを使用してグループ化を作成し、作成できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# グループ化：グループ化内のすべてのオブジェクトに共通の計算値でリスト結果を整理

タスクを「完了率」でグループ化し、0 ～ 25、26 ～ 50、51 ～ 75、75 ～ 99、100 の範囲で表示することができます。 テキストモードを使用してグループ化を作成し、作成できます。

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
   <td> <p>グループ化を変更するリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してグループ化を変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## グループ化内のすべてのオブジェクトに共通の計算値でリスト結果を整理

タスクのリストにこのグループを適用するには、次の手順に従います。

1. タスクのリストに移動します。
1. 次の **グループ化**&#x200B;ドロップダウンメニューで、「 **新しいグループ化**.

1. クリック **テキストモードに切り替え**.
1. 空きスペースに、次のコードを追加します。

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. クリック **完了**&#x200B;を、 **グループ化を保存**.
