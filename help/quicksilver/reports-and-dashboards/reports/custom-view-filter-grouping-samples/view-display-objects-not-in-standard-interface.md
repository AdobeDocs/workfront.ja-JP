---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：標準インターフェイスに含まれていないオブジェクトの表示」
description: 標準モードのインターフェイスに含まれていないオブジェクトをビューで表示できます。テキストモードで参照する場合にのみ、これを実行できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 100%

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

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 例：ポートフォリオ所有者名列をプロジェクトビューに追加

1. プロジェクトのリストに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューから、「**新規ビュー**」をクリックします。

1. 「**列を追加**」をクリックして、**この列に表示**&#x200B;フィールドに「ポートフォリオ所有者 ID」を入力し、リストに表示されたら選択します。

1. 「**テキストモードに切り替え**」をクリックします。
1. テキストモード領域にポインタを合わせ、「**クリックしてテキストを編集**」をクリックします。
1. `valuefield` 行（`valuefield=portfolio:ownerID`）を次の行に置き換えます。

   ```
   valuefield=portfolio:owner:name
   ```

   または

   「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。

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

1. 「**保存**」、「**ビューを保存**」の順にクリックします。
