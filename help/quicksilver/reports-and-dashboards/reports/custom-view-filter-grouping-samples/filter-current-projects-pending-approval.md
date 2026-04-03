---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：承認保留の現在のプロジェクトを表示
description: 次のプロジェクトフィルターは、「現在 - 承認保留」ステータスのプロジェクトを表示します。ログインユーザーは、プロジェクトスポンサーまたはポートフォリオマネージャーです。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 79%

---

# フィルター：承認保留の現在のプロジェクトを表示

<!--Audited: 10/2024-->

次のプロジェクトフィルターは、「現在 - 承認保留」ステータスのプロジェクトを表示します。ログインユーザーは、プロジェクトスポンサーまたはポートフォリオマネージャーのいずれかです。

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
   <p>コントリビューターまたはフィルターを変更するリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 承認保留の現在のプロジェクトをフィルター

このフィルターを適用するには、次の手順に従います。

1. プロジェクトのリストに移動します。
1. **フィルター** ドロップダウンメニューから、**新しいフィルター**&#x200B;を選択します。

1. **テキストモード**&#x200B;をクリックします。
1. 表示された領域に、次のコードをコピーして貼り付けます。
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. **適用** / **新規として保存**&#x200B;をクリックします。
