---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'フィルター：配信予定レポートを表示'
description: このレポートフィルターには、Adobe Workfrontで自動的に配信されるようにスケジュールされたすべてのレポートが表示されます。 標準ビューで使用するのに最適です。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# フィルター：配信予定レポートの表示

このレポートフィルターには、Adobe Workfrontで自動的に配信されるようにスケジュールされたすべてのレポートが表示されます。 標準ビューで使用するのに最適です。

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
   <td> <p>フィルターの変更リクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してフィルターを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## レポート配信フィルター

このフィルターを適用するには：

1. レポートのリストに移動します。
1. 次の **フィルター** ドロップダウンメニューで、「 **新しいフィルター**.

1. クリック&#x200B;**テキストモードに切り替え**.
1. 内 **レポートのフィルタールールの設定** 領域にコピーして、次のコードを貼り付けます。

   ```
   scheduledReportID=0<br>scheduledReportID_Mod=notnull
   ```

1. クリック **フィルターを保存**.
