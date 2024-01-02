---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'グループ化：グループ内の表示名を編集'
description: リストやレポートのグループ名を、より身近な名前に変更できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# グループ化：グループ内の表示名を編集します

<!--Audited: 01/2024-->

グループ名を、ユーザーにとってより身近な名前に変更できます。

例えば、標準のPortfolio名のグループ化をプロジェクトのリストに適用すると、グループの名前は次のように表示されます。 *Portfolio：名前：`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

テキストモードを使用してこのグループ化を変更し、読みやすい名前を表示できます。

![](assets/grouping-edited-name-350x160.png)

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
   <td>

<p>新規： </p>
   <ul>
   <li> <p>グループを変更するコントリビューター </p></li>
   <li><p>レポートを変更するための標準</p></li></ul>

<p> 現在：</p>
   <ul>  
   <li><p>グループ化を変更するリクエスト </p></li>
   <li><p>レポートを変更する計画</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してグループ化を変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## グループ内の表示名を編集

プロジェクトグループ内の表示名を変更するには、次の手順に従います。

1. プロジェクトのリストに移動します。
1. 次から： **グループ化** ドロップダウンメニューで、「 **新しいグループ化**.

1. クリック **グループを追加**&#x200B;をクリックし、「Portfolio名」と入力します。 **最初の基準：** フィールドに値を入力し、リストに表示されるときに選択します。

1. クリック **テキストモードに切り替え**.
1. 次のいずれかの操作を行います。

   * 次のコードを、 **レポートをグループ化** ボックス：


     `group.0.displayname=Your Value`


     または、この場合は次のようになります。

     `group.0.displayname=Portfolio`

   * グループのテキストモードインターフェイスで「name」という単語が含まれる行をすべて削除し、次の行を追加します。

     `group.0.name=Your Value`

     または、この場合は次のようになります。

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >また、 `group.0.name=` そして `group.0.displayname=` 行が空白の場合、グループ化にはグループ化の基準となる値が表示されます。


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. クリック **完了**&#x200B;を、 **グループ化を保存**.

   グループ化のデフォルト名は、テキストモードの情報に従って変更されます。
