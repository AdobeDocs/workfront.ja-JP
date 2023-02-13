---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：標準インタフェースに含まれていないオブジェクトを表示する'
description: 標準モードのインタフェースに含まれていないビューオブジェクトに、を表示できます。 これをおこなうには、テキストモードで参照する必要があります。 ビューに含めるフィールドは、次のいずれかの方法で決定できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# [ 表示 ]：標準インタフェースに含まれていないオブジェクトを表示します

標準モードのインタフェースに含まれていないビューオブジェクトに、を表示できます。 これをおこなうには、テキストモードで参照する必要があります。\
ビューに含めることができるフィールドは、次のいずれかの方法で決定できます。

* 以下を使用： [API エクスプローラ](https://one.workfront.com/s/api-explorer) をクリックして、テキストモードで参照できる他のオブジェクトを検出します。\
   API エクスプローラーで説明されているすべてのフィールドがテキストモード用の有効なフィールドではありません。 一部のフィールドは、API を通じてのみレポート可能です。

* 列でオブジェクトの ID フィールドを見つけます。 フィールド ID を持つオブジェクトのほとんどには、対応する列またはフィールド名もあります。この名前には、標準モードのインターフェイスからはアクセスできません。

   テキストモードを使用すると、ID の代わりに列またはフィールド名をビューに含めることができます。その際、 `fieldnameID` と `fieldname:name`.

   例えば、標準モードのインターフェイスでは、 **Portfolio所有者 ID** フィールドはプロジェクトビューで使用できますが、 **Portfolio所有者名** フィールドがではありません。 テキストモードを使用すると、 **Portfolio所有者名** をクリックします。

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

## 例：プロジェクトビューにPortfolio所有者名列を追加する

1. プロジェクトのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、 **新しいビュー**.

1. クリック **列を追加** 次に、「Portfolio所有者 ID」と入力します。 **この列に表示** フィールドに値を入力し、リストに表示されるときに選択します。

1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. を `valuefield` 行 (`valuefield=portfolio:ownerID`) を次の行に置き換えます。

   ```
   valuefield=portfolio:owner:name
   ```

   または

   検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   この例では、レポートは、Portfolioの所有者 ID( `querysort` 行

   >[!TIP]
   >
   >任意のフィールドを置き換えるには `ID` フィールド `name` テキストモードの使用、常に置換 `ID` と `:name` 内 `valuefield` 行

1. クリック **保存**&#x200B;を、 **ビューを保存**.
