---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：列の文字列ではなく画像を表示します
description: テキストモードを使用して、ビュー内のオブジェクトの名前を画像に置き換えることができます。また、置き換えるオブジェクトを開くためのリンクを画像に追加できます。
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 83%

---

# 表示：列に文字列ではなく画像を表示

<!--Audited: 11/2024-->

テキストモードを使用して、ビュー内のオブジェクトの名前を画像に置き換えることができます。また、置き換えるオブジェクトを開くためのリンクを画像に追加できます。

>[!NOTE]
>
>画像は実際の解像度で表示されるので、小さな画像を使用してください。

![ プロジェクト名を画像とリンクに置き換える ](assets/replace-project-name-with-image-and-link-350x125.png)

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
   <p>フィルターの変更者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
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

## 例：プロジェクトビュー内のプロジェクトの名前を画像に置き換える。

1. Web サイトまたは Adobe Workfront 外部サーバーに画像をアップロードします。Web ブラウザーを使用して画像にアクセスできる必要があります。

   >[!TIP]
   >
   >* ブラウザーのタイプはそれぞれ異なりますが、すべて URL を表示できます。
   >* Workfront にアップロードされた画像は使用しないでください。Workfront に保存された画像は一般に使用できず、一定期間後に有効期限が切れるアクセスキーを持つので、時間の経過と共に、これらの画像はビューに表示されなくなります。
   >* お使いのコンピューターに保存された画像に固有の URL がありません。画像のホスティングを提供し、画像をホストするサイトを見つけます。組織は既にそのようなサイトを持っている可能性があります。

1. Web ブラウザーを使用して、保存した画像に移動します。
1. 次の手順を実行して、画像の URL を取得します。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. ブラウザーに応じて「**画像の場所をコピー**」または「**リンクを取得**」を右クリックして選択します。これで、その特定の画像の URL が取得され、クリップボードから貼り付けることができます。
   1. そのリンクを持つユーザー全員がリンクに移動するだけで画像を表示する権限を持ち、そのリンクにアクセスするためにログインする必要がないことを確認します。

1. プロジェクトに移動し、プロジェクト名の横にある **その他** メニュー ![ その他アイコン ](assets/more-icon-45x33.png) をクリックしてから、**編集** をクリックします。

1. 「**URL**」フィールドで、画像にリンクを追加します。
1. プロジェクトの一覧のプロジェクト ビューに移動します。
1. **表示**&#x200B;ドロップダウンメニューをクリックして、「**新規ビュー**」をクリックします。
1. **プロジェクト名**&#x200B;の列の見出しをクリックし、次に「**テキストモードに切り替え**」をクリックします。

1. 既存のコードの列に次のコードを追加します。

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. **完了**/**ビューを保存** をクリックします。
選択したイメージは、プロジェクトビューのプロジェクト名に置き換えられ、そのイメージはプロジェクトへのリンクになります。
