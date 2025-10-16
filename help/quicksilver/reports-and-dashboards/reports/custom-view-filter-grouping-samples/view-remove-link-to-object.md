---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：列内のオブジェクトへのリンクを削除
description: ビューに表示する一部のオブジェクトは、デフォルトでは、オブジェクトの「詳細」ページにリンクされます。例えば、プロジェクト名を表示する列はプロジェクトへのリンクで、ユーザー名を表示する列はユーザーのプロファイルページへのリンクです。
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 72%

---

# ビュー：列内のオブジェクトへのリンクを削除

<!--Audited: 11/2024-->

ビューに表示する一部のオブジェクトは、デフォルトでは、オブジェクトの「詳細」ページにリンクされます。例えば、プロジェクト名を表示する列はプロジェクトへのリンクで、ユーザー名を表示する列はユーザーのプロファイルページへのリンクです。

すべてのビューに表示される列のテキストモードを使用して、このリンクを削除できます。

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
   <p>ビューの投稿者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


+++


## 例：タスクビューのタスク名の列からタスクへのリンクを削除します。

1. タスクのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、**新しいビュー**&#x200B;をクリックして、新しいビューを作成します。

   または

   **編集アイコン**![ 編集アイコン ](assets/edit-icon.png) をクリックして既存のビューを編集し、ビューを選択します。

1. 「**列を追加**」をクリックして新しい列を追加します。

   または

   オブジェクトへのリンクを含む既存の列をクリックします。

1. **テキストモードに切り替え**/**テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスで検索したテキストを削除し、次のコードに置き換えます。

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >次のように調整して、他のオブジェクトにも同様のコードを使用できます。
   >
   >* コードの `valuefield` 行を `valueexpression` に置き換え、中括弧で囲まれた同じ名前を等号の後に残します。
   >* 列の元のテキストから `link.` で始まる行をすべて削除します。例えば、次の行をすべて削除します。
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。

