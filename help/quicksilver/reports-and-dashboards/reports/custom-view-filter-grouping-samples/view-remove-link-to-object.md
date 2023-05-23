---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '表示：列内のオブジェクトへのリンクを削除します'
description: ビューに表示する一部のオブジェクトは、デフォルトでは、オブジェクトの [ 詳細 ] ページにリンクされます。 例えば、プロジェクトの名前を表示する列は、プロジェクトへのリンクです。ユーザーの名前を表示する列は、ユーザーのプロファイルページへのリンクです。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 表示：列内のオブジェクトへのリンクを削除

ビューに表示する一部のオブジェクトは、デフォルトでは、オブジェクトの [ 詳細 ] ページにリンクされます。 例えば、プロジェクトの名前を表示する列は、プロジェクトへのリンクです。ユーザーの名前を表示する列は、ユーザーのプロファイルページへのリンクです。

すべてのビューに表示される列のテキストモードを使用して、このリンクを削除できます。

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
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 例：タスクビューの [ タスク名 ] 列からタスクへのリンクを削除します。

1. タスクのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、 **新しいビュー** をクリックして、新しいビューを作成します。

   または

   次をクリック： **編集アイコン** ![](assets/edit-icon.png)

   既存のビューを編集するには、ビューを選択します。

1. クリック **列を追加** をクリックして新しい列を追加します。

   または

   オブジェクトへのリンクを含む既存の列をクリックします。

1. クリック **テキストモードに切り替え**.
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。

   <pre>displayname=タスク名<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >次のように調整して、他のオブジェクトにも同様のコードを使用できます。
   >
   >   
   >   
   >   * を **valuefield** コードの行 **valueexpression** です。等号の後の中括弧内に同じ名前を付けます。
   >   
   >   
   >
   >   
   >   
   >   * > で始まるすべての行を削除します。

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. クリック **保存**&#x200B;を、 **ビューを保存**.
