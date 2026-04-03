---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: ビュー：標準インターフェイスに含まれていないオブジェクトを表示
description: 標準モードのインターフェイスに含まれていないオブジェクトをビューで表示できます。テキストモードで参照する場合にのみ、これを実行できます。
author: Courtney
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 86%

---

# ビュー：標準インターフェイスに含まれていないオブジェクトの表示

標準モードのインターフェイスに含まれていないオブジェクトをビューで表示できます。テキストモードで参照する場合にのみ、これを実行できます。\
ビューに含めるフィールドは、次のいずれかの方法で決定できます。

* [API エクスプローラー](../../../wf-api/general/api-explorer.md)を使用して、テキストモードで参照できる他のオブジェクトを検出します。\
  API エクスプローラーに記載されているすべてのフィールドが、テキストモードで有効なフィールドであるとは限りません。一部のフィールドは、API 経由でのみレポート可能です。

* 列でオブジェクトの ID フィールドを見つけます。フィールド ID を持つオブジェクトのほとんどには、対応する列またはフィールド名もありますが、標準モードのインターフェイスからはアクセスできない場合があります。

  テキストモードを使用すると、`fieldnameID` を `fieldname:name` に置き換えることで、ID の代わりに列またはフィールド名をビューに含めることができます。

  例えば、標準モードのインターフェイスでは、**ポートフォリオ所有者 ID** フィールドをプロジェクトビューで使用できますが、**ポートフォリオ所有者名**&#x200B;フィールドは使用できません。テキストモードを使用すると、ビューの列に「**ポートフォーリオ所有者名**」を表示できます。

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

## 例：ポートフォリオ所有者名列をプロジェクトビューに追加

1. プロジェクトのリストに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューから、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックして、**この列に表示**&#x200B;フィールドに「ポートフォリオ所有者 ID」を入力し、リストに表示されたら選択します。

1. 「**テキストモードに切り替え**」、「**テキストモードを編集**」の順にクリックします。
1. `valuefield` 行（`valuefield=portfolio:ownerID`）を次の行に置き換えます。

   `valuefield=portfolio:owner:name`

   または

   「**テキストモードを編集**」ボックスにあるテキストを削除し、次のコードに置き換えます。

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   この特定の例では、`querysort` 行で示されているように、ポートフォリオ所有者 ID によってレポートが並べ替えられます。

   >[!TIP]
   >
   >テキストモードを使用して `ID` フィールドを `name` フィールドに置き換えるには、常に `valuefield` 行の `ID` を `:name` に置き換えます。

1. 「**完了**」をクリックし、「**ビューを保存**」をクリックします。
