---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：問題の提出パス'
description: 問題レポートのビューに、問題が送信された経路を表示できます。 パスは、問題が最初に送信されたキュー、トピックグループ、およびキュートピックを示します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 表示：問題の送信パス

問題レポートのビューに、問題が送信された経路を表示できます。 パスは、問題が最初に送信されたキュー、トピックグループ、およびキュートピックを示します。

![issue_submission_path.png](assets/issue-submission-path-350x66.png)

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
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 問題の送信パスを表示

1. 問題のリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域、クリック **列を追加**.

1. 新しい列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを&#x200B;**テキストモード**」ボックスに置き換えて、次のコードに置き換えます。

   <pre>displayname=問題のパス<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valuefield=displayQueueBreadcrumb <br>valueformat=HTML<br></pre>

1. クリック **ビューを保存**.
