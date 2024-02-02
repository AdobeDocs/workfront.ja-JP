---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「フィルター：承認保留の現在のプロジェクトを表示」
description: 次のプロジェクトフィルターは、「現在 - 承認保留」ステータスのプロジェクトを表示します。ログインユーザーは、プロジェクトスポンサーまたはポートフォリオマネージャーです。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '250'
ht-degree: 100%

---

# フィルター：承認保留の現在のプロジェクトを表示

次のプロジェクトフィルターは、「現在 - 承認保留」ステータスのプロジェクトを表示します。ログインユーザーは、プロジェクトスポンサーまたはポートフォリオマネージャーのいずれかです。

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
   <td> <p>フィルターを変更する場合は「要求」 </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 承認保留の現在のプロジェクトをフィルター

このフィルターを適用するには、次の手順に従います。

1. プロジェクトのリストに移動します。
1. **フィルター**&#x200B;ドロップダウンメニューで、「**新しいフィルター**」を選択します。

1. 「**テキストモードに切り替え**」をクリックします。
1. **レポートのフィルタールールを設定**&#x200B;エリアに次のコードを追加します。
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. 「**フィルターを保存**」をクリックします。
