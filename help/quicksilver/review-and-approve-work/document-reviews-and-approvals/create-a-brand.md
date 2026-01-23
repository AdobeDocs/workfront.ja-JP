---
product-area: documents
navigation-topic: approvals
title: AI レビュアーのブランドの設定
description: AI レビュアーのブランドの設定
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cd2a5560fdf446e8e971afcb640af38b4d301d40
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 10%

---

# AI レビュアーのブランドの設定

>[!IMPORTANT]
>
>この機能は現在ベータ版です。

AI レビュー担当者は、ブランドガイドラインを使用して、レビュープロセス中にコンテンツを評価します。 ブランドガイドラインを含むPDF ファイルをアップロードするか、ブランド要素を手動で入力することにより、Workfrontでブランドを作成できます。

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
   <td> <p>標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者である必要があります。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Consoleの権限</td> 
   <td> <p>Brand Manager をGenStudioする必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 前提条件

* 組織がAdobe IMS（Identity Management System）に移行している必要があります。
* Workfront インスタンスでは、統合承認が有効になっている必要があります。
* GenStudio Foundationが必要です。
* Adobeには、Adobe生成 AI 契約がファイルに署名済みである必要があります。
契約の署名について詳しくは、[Adobe Gen AI 契約への署名 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) を参照してください。

## PDFを使用したブランドの作成

{{step-1-to-setup}}

1. 左側のパネルで、**レビューと承認**/**ブランド** に移動します。
1. 画面の右上隅にある「**ブランドを追加**」をクリックします。
1. ブランドに名前を付けます。
1. 「PDF をアップロード」をクリックして、ブランドファイルをアップロードします。
   ![ ブランド pdf のアップロード ](assets/upload-PDF.png)
1. 「**続行**」をクリックします。
1. ブランドガイドラインを含んだ 1 つ以上のPDF ファイルをアップロードし、「**ブランドを追加**」をクリックします。
1. ファイルがアップロードされたら、抽出したブランド要素をレビューして、ブランドガイドラインに一致していることを確認します。

   >[!IMPORTANT]
   >
   >ガイドラインは、ファイルと生成 AI テクノロジーを使用して生成されるため、不正確な場合があります。 このブランドを公開する前に、抽出したガイドラインで詳細の不足や誤りがないか確認し、それらを編集します。

1. 終了したら、「**公開**」をクリックして、AI レビュー担当者がブランドを使用できるようにします。

## ブランドの手動作成

{{step-1-to-setup}}

1. 左側のパネルで、**レビューと承認**/**ブランド** に移動します。
1. 画面の右上隅にある「**ブランドを追加**」をクリックします。
1. ブランドに名前を付けます。
1. 「**手動で追加**」をクリックして、個々の要素を持つブランドを作成します。
1. 必要に応じて、ブランドの詳細を入力します。 次の要素を追加できます。

   <table>
    <tr>
        <td>使用するタイミング</td>
        <td>マーケターに、このブランドを使用するタイミングを知らせます。</td>
    </tr>
    <tr>
        <td>音声ガイドライン</td>
        <td>ブランドの声のトーンとスタイルに関するガイダンスを提供します。</td>
    </tr>
    <tr>
        <td>画像のガイドライン</td>
        <td>ブランドの ID に合わせる画像のタイプを指定します。</td>
    </tr>
    <tr>
        <td>チャネルガイドライン</td>
        <td>ブランドコミュニケーションに適したチャネルの概要を説明します。</td>
    </tr>
    <tr>
        <td>ロゴ</td>
        <td>ブランドに関連する公式ロゴを含めます。</td>
    </tr>
    <tr>
        <td>カラー</td>
        <td>ブランドのカラーパレットを指定します。</td>
    </tr>
    </table>

   ![ ブランド要素の手動追加 ](assets/brand-elements.png)


1. 終了したら、「**公開**」をクリックして、AI レビュー担当者がブランドを使用できるようにします。
