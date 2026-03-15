---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: グループ化：グループ化の表示名を編集する
description: リストやレポートのグループ化を、ユーザーにとってよりなじみのある名前に変更できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 73%

---

# グループ化：グループ化の表示名の編集

<!--Audited: 01/2024-->

グループ名を、ユーザーにとってより身近な名前に変更できます。

例えば、標準のポートフォリオ名のグループ化をプロジェクトのリストに適用すると、グループ化の名前は&#x200B;*ポートフォリオ：名前：`<name of portfolio>`* として表示されます。

![未編集の名前でグループ化しています](assets/grouping-unedited-name-350x167.png)

テキストモードを使用してこのグループ化を変更し、読みやすい名前を表示できます。

![編集した名前でグループ化](assets/grouping-edited-name-350x160.png)

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
   <p>フィルターの変更をコントリビューターまたはリクエスト </p>
   <p>レポートを変更するための「標準」または「プラン」</p>
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

## グループ化の表示名を編集

プロジェクトのグループ化の表示名を変更するには、次の手順に従います。

1. プロジェクトのリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで「**新規グループ化**」を選択します。

1. [**グループ化の追加**]をクリックし、[**グループ化：**]フィールドに「Portfolio名」と入力し、一覧に表示されたら選択します。

1. 「**テキスト モードに切り替える**」をクリックします。
1. 次のいずれかの操作を行います。

   * 次のコードを、「**報告書のグループ化**」ボックスにある既存のテキストに追加します。


     `group.0.displayname=Your Value`


     例えば、次のコードを入力すると、表示名が「Portfolio」に変わります。

     `group.0.displayname=Portfolio`

   * グループ化のテキストモードインターフェイスで、「name」という単語が含まれる行をすべて削除したあと、次の行を追加します。

     `group.0.name=Your Value`

     例えば、次のコードを入力すると、表示名が「Portfolio」に変わります。

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >また、`group.0.name=` と `group.0.displayname=` の行を空白にすることもできます。この場合、グループ化にはグループ化の基準となる値が表示されます。


     ![名前のない編集済みの名前でグループ化しています](assets/grouping-edited-name-no-name-350x162.png)

1. 「**完了**」をクリックし、「**グループ化の保存**」をクリックします。
1. （オプション）グループ名を更新し、**[グループの保存]**&#x200B;をクリックします。

   グループ化のデフォルト名は、テキストモードの情報に従って変更されます。
