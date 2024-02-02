---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：イシューの送信パス」
description: イシューレポートのビューに、イシューが送信されたパスを表示できます。このパスは、イシューが最初に送信されたキュー、トピックグループ、キューのトピックを指します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bee1e066-c3f4-4d74-92b0-ab7f43d52a50
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '294'
ht-degree: 100%

---

# ビュー：イシューの送信パス

イシューレポートのビューに、イシューが送信されたパスを表示できます。このパスは、イシューが最初に送信されたキュー、トピックグループ、キューのトピックを指します。

![issue_submission_path.png](assets/issue-submission-path-350x66.png)

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

## イシューの送信パスを表示

1. イシューのリストに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューから、「**新規ビュー**」を選択します。

1. **列のプレビュー**&#x200B;エリアで、「**列を追加**」をクリックします。

1. 新しい列のヘッダーをクリックし、「**テキスト モードに切り替える**」をクリックします。
1. テキストモード領域にマウスを移動し、「**クリックしてテキストを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>displayname= イシューのパス<br>linkedname=direct <br>namekey=displayQueueBreadcrumb <br>valuefield=displayQueueBreadcrumb <br>valueformat=HTML<br></pre>

1. 「**ビューの保存**」をクリックします。
