---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：プルーフへのリンクを含んだドキュメントレポート」
description: 「ビュー：プルーフへのリンクを含んだドキュメントレポート」
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '356'
ht-degree: 100%

---

# ビュー：プルーフへのリンクを含むドキュメントレポート

このドキュメントビューでは、ドキュメントの現在のバージョンのプルーフへのリンクを挿入できます。

![](assets/view-document-with-proof-link-350x92.png)

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

## プルーフへのリンクを含んだドキュメントレポートを表示

この表示を適用するには次の操作を行います。

1. ドキュメントのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューから、**新規ビュー**&#x200B;を選択します。

1. 「**列を追加**」をクリックします。
1. 「**テキストモードに切り替える**」をクリックします。
1. テキストモードエリアにポインタを合わせ、「**クリックするとテキストを編集できます**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。

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

1. 「**保存**」をクリックし、次に「**ビューの保存**」をクリックします。
1. ビューの名前を入力したあと、「**ビューの保存**」をクリックします。
1. （オプション）プルーフを含んだドキュメントのみを表示するには、次の手順に従ってフィルターを追加します。

   1. **フィルター**&#x200B;ドロップダウンメニューをクリックし、次に「**新規フィルター**」をクリックします。
   1. 「**フィルター規則の追加**」をクリックして、「プルーフ所有者」と入力していき、「**プルーフ所有者 ID**」がリストに表示されたら選択します。
   1. フィルター修飾子に「**ブランクでない**」を選択します。
   1. 「**フィルターの保存**」をクリックし、フィルターの名前を入力したあと、「**フィルターの保存**」をクリックします。

1. 「プルーフ リンク」列のリンクをクリックして、ドキュメントの最後のバージョンのプルーフにアクセスします。
