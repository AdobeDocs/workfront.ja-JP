---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：配達確認へのリンクを含むレポートをドキュメント化'
description: '表示：配達確認へのリンクを含むレポートをドキュメント化'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 表示：配達確認へのリンクを含むレポートをドキュメント化

このドキュメント表示では、ドキュメントの現在のバージョンの配達確認へのリンクを挿入できます。

![](assets/view-document-with-proof-link-350x92.png)

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

## 配達確認へのリンクを含むドキュメントレポートの表示

このビューを適用するには：

1. ドキュメントのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. クリック **列を追加**.
1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >「Your domain」を実際のWorkfrontドメインに置き換えます。 例えば、会社のWorkfront URL が *Company.my.workfront.com*&#x200B;の場合、ドメインは「会社」です。

1. クリック **保存**&#x200B;を、 **ビューを保存**.
1. ビューの名前を入力し、 **ビューを保存**.
1. （オプション）配達確認を含むドキュメントのみを表示するには、次の手順を実行してフィルターを追加します。

   1. 次をクリック： **フィルター** ドロップダウンメニューで、 **新しいフィルター**.
   1. クリック **フィルタールールを追加** 「配達確認の所有者」と入力し、「 **配達確認の所有者 ID** リストに表示される場合。
   1. 選択 **空白でない** フィルタ修飾子用。
   1. クリック **フィルターを保存**、フィルターの名前を入力し、「 **フィルターを保存**.

1. 「リンクの配達確認」列のリンクをクリックして、ドキュメントの最後のバージョンの配達確認にアクセスします。
