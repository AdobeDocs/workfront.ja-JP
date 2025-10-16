---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：承認保留の現在のプロジェクトを表示
description: 次のプロジェクトフィルターは、「現在 - 承認保留」ステータスのプロジェクトを表示します。ログインユーザーは、プロジェクトスポンサーまたはポートフォリオマネージャーです。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 72%

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
   <p>フィルターの変更者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
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
1. **フィルター** ドロップダウンメニューから「**新しいフィルター**」を選択します。

1. **テキストモード** をクリックします。
1. 表示された領域で、次のコードをコピーして貼り付けます。
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. **適用**/**新規保存** をクリックします。
