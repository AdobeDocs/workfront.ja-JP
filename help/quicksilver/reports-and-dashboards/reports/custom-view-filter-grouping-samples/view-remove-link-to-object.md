---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：列内のオブジェクトへのリンクを削除」
description: ビューに表示する一部のオブジェクトは、デフォルトでは、オブジェクトの「詳細」ページにリンクされます。例えば、プロジェクト名を表示する列はプロジェクトへのリンクで、ユーザー名を表示する列はユーザーのプロファイルページへのリンクです。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: ht
source-wordcount: '442'
ht-degree: 100%

---

# ビュー：列内のオブジェクトへのリンクを削除

ビューに表示する一部のオブジェクトは、デフォルトでは、オブジェクトの「詳細」ページにリンクされます。例えば、プロジェクト名を表示する列はプロジェクトへのリンクで、ユーザー名を表示する列はユーザーのプロファイルページへのリンクです。

すべてのビューに表示される列のテキストモードを使用して、このリンクを削除できます。

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

## 例：タスクビューのタスク名の列からタスクへのリンクを削除します。

1. タスクのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、**新しいビュー**&#x200B;をクリックして、新しいビューを作成します。

   または

   **編集アイコン** ![](assets/edit-icon.png)をクリック

   既存のビューを編集するには、ビューを選択します。

1. 「**列を追加**」をクリックして新しい列を追加します。

   または

   オブジェクトへのリンクを含む既存の列をクリックします。

1. 「**テキストモードに切り替える**」をクリックします。
1. テキストモードエリアにポインタを合わせ、「**クリックしてテキストを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >次のように調整して、他のオブジェクトにも同様のコードを使用できます。
   >
   >* コードの **valuefield** 行を **valueexpression** に置き換え、等号の後の中括弧内に同じ名前を付けます。
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

1. 「**保存**」をクリックし、次に「**表示を保存**」をクリックします。
