---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：プルーフへのリンクを含むドキュメントレポート」
description: 「ビュー：プルーフへのリンクを含んだドキュメントレポート」
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 67%

---

# ビュー：プルーフへのリンクを含むドキュメントレポート

<!--Audited: 11/2024-->

このドキュメントビューでは、ドキュメントの現在のバージョンのプルーフへのリンクを挿入できます。

![](assets/view-document-with-proof-link-350x92.png)

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
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

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## プルーフへのリンクを含んだドキュメントレポートを表示

この表示を適用するには次の操作を行います。

1. ドキュメントのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューから、**新規ビュー**&#x200B;を選択します。
1. 「**列を追加**」をクリックします。
1. **テキストモードに切り替え** をクリックしてから、**テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスで検索したテキストを削除し、次のコードに置き換えます。

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >「Your domain」を実際の Workfront ドメインに置き換えます。例えば、会社の Workfront URL が *Company.my.workfront.com* の場合、ドメインは「Company」です。

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。
1. （オプション）ビュー名を更新し、「**ビューを保存**」をクリックします。
1. （オプション）プルーフを含んだドキュメントのみを表示するには、次の手順に従ってフィルターを追加します。

   1. **フィルター**&#x200B;ドロップダウンメニューをクリックし、次に「**新規フィルター**」をクリックします。
   1. **フィルタールールを追加** をクリックして「プルーフ所有者」の入力を開始し、リストに表示されたら **プルーフ所有者 ID** を選択します。
   1. フィルター修飾子に「**ブランクでない**」を選択します。
   1. 「**フィルターの保存**」をクリックします。
   1. （オプション）フィルター名を更新し、「**フィルターを保存**」をクリックします。

1. 「プルーフ リンク」列のリンクをクリックして、ドキュメントの最後のバージョンのプルーフにアクセスします。
