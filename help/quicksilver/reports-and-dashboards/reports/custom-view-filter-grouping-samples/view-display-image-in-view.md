---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：列に文字列ではなく画像を表示する'
description: テキストモードを使用して、ビュー内のオブジェクトの名前を画像に置き換えることができます。 また、置き換えるオブジェクトを開くためのリンクを画像に追加することもできます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 表示：列に文字列ではなく画像を表示する

テキストモードを使用して、ビュー内のオブジェクトの名前を画像に置き換えることができます。 また、置き換えるオブジェクトを開くためのリンクを画像に追加することもできます。

>[!NOTE]
>
>画像は実際の解像度で表示されるので、小さな画像を使用してみてください。

![](assets/replace-project-name-with-image-and-link-350x125.png)

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

## 例：プロジェクトビューのプロジェクト名を画像で置き換えます。

1. Web サイトまたはAdobe Workfront外部のサーバーに画像をアップロードします。 Web ブラウザーを使用して画像にアクセスできる必要があります。

   >[!TIP]
   >
   >* ブラウザーのタイプはそれぞれ異なりますが、すべて URL を表示できます。
   >* Workfrontにアップロードされた画像は使用しないでください。 Workfrontに保存された画像は一般に使用できず、一定期間後に有効期限が切れるアクセスキーを持つので、時間の経過と共に、これらの画像はビューに表示されなくなります。
   >* お使いのコンピューターに保存された画像に固有の URL がありません。 画像のホスティングを提供し、画像をホストするサイトを見つけます。 お客様の組織が既にそのようなサイトを持っている可能性があります。


1. Web ブラウザーを使用して、保存した画像に移動します。
1. 次の手順を実行して、画像の URL を取得します。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 右クリックして「 」を選択します。 **画像の場所をコピー**&#x200B;または **リンクを取得**（ブラウザーに応じて異なります）。 これで、その特定の画像の URL が取得され、クリップボードから貼り付けることができます。
   1. そのリンクを持つユーザー全員がリンクに移動するだけで画像を表示する権限を持ち、そのリンクにアクセスするためにログインする必要がないことを確認します。

1. プロジェクトに移動し、 **詳細** メニュー ![](assets/more-icon-45x33.png) プロジェクト名の横にあるをクリックし、 **編集**.

1. 内 **URL** 「 」フィールドで、画像にリンクを追加します。
1. リストまたはレポートのプロジェクトビューに移動し、そのビューをカスタマイズします。
1. の列見出しをクリックします。 **プロジェクト名**&#x200B;を選択し、「 **テキストモードに切り替え**.

1. 既存のコードの列に次のコードを追加します。

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   選択したイメージは、プロジェクトビューのプロジェクト名に置き換えられ、そのイメージはプロジェクトへのリンクになります。

1. クリック **ビューを保存**.
