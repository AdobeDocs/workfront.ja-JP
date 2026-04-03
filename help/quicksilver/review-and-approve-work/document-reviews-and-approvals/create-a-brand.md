---
product-area: documents
navigation-topic: approvals
title: コンテンツレビュアーのブランドを作成および管理する
description: コンテンツレビュアーのブランドを作成および管理する
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 9%

---

# コンテンツレビュアーのブランドを作成および管理する

{{highlighted-preview-article-level}}

コンテンツレビュアーは、レビュープロセス中にコンテンツを評価するためにブランドガイドラインを使用します。 Workfrontでブランドを作成するには、ブランドガイドラインを含むPDF ファイルをアップロードするか、ブランド要素を手動で入力します。

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
   <td> <p>あなたはシステム管理者でなければなりません。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Consoleの権限*</td> 
   <td> <p>GenStudioの。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 要件

* Workfront インスタンスでは、統合承認が有効になっている必要があります。

* 組織にはGenStudio Foundationが必要です。
   * WorkfrontのContent Reviewerには、GenStudio Foundationでアセットのレビューおよび承認ワークフローに使用できる機能が用意されています。 作業を完了するためにGenStudio Foundationに直接アクセスする必要はありません。 Content Reviewerを介したGenStudio Foundation機能へのアクセスは、Workfront契約の条件に該当します。
* Adobeには、署名済みのAdobe Gen AI契約書がファイルに登録されている必要があります。
契約書への署名について詳しくは、[Adobe Gen AI契約書への署名](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)を参照してください。


## 前提条件

1. ブランドを作成する前に、Admin ConsoleおよびWorkfrontのアクセスレベルでブランド権限へのアクセス権を付与する必要があります。 手順については、[&#x200B; ブランド権限へのアクセス権の付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)を参照してください。


## PDFを使用したブランドの構築

{{step-1-to-setup}}

1. 左側のパネルで、**レビューと承認** > **ブランド**&#x200B;に移動します。
1. 画面の右上隅にある「**ブランドを追加**」をクリックします。
1. ブランドに名前を付けます。
1. 「**PDFをアップロード**」をクリックして、ブランドファイルをアップロードします。
   ![&#x200B; ブランド pdfをアップロード &#x200B;](assets/upload-PDF.png)
1. 「**続行**」をクリックします。
1. ブランドガイドラインを含む1つ以上のPDF ファイルをアップロードし、**ブランドを追加**&#x200B;をクリックします。
1. ファイルがアップロードされたら、抽出したブランド要素を確認して、ブランドガイドラインに準拠していることを確認します。

   >[!IMPORTANT]
   >
   >ガイドラインは、ファイルと生成AI テクノロジーを使用して生成されるため、不正確な場合があります。 抜き取ったガイドラインに欠けている情報や誤った情報がないか確認し、このブランドを公開する前に編集します。

1. 完了したら、**公開**&#x200B;をクリックして、ブランドをコンテンツレビュー担当者が利用できるようにします。

## ブランドの手動作成

{{step-1-to-setup}}

1. 左側のパネルで、**レビューと承認** > **ブランド**&#x200B;に移動します。
1. 画面の右上隅にある「**ブランドを追加**」をクリックします。
1. ブランドに名前を付けます。
1. 「**手動で追加**」をクリックして、個々の要素を含むブランドを作成します。
1. 必要に応じてブランドの詳細を入力します。 次の要素を追加できます。

   <table>
    <tr>
        <td>使用するタイミング</td>
        <td>マーケターにブランドの使用状況を知らせる。</td>
    </tr>
    <tr>
        <td>音声ガイドライン</td>
        <td>ブランドの声のトーンやスタイルに関するガイダンスを提供する。</td>
    </tr>
    <tr>
        <td>画像ガイドライン</td>
        <td>ブランドのアイデンティティに沿った画像の種類を指定します。</td>
    </tr>
    <tr>
        <td>チャネルガイドライン</td>
        <td>ブランドコミュニケーションに適切なチャネルの概説：</td>
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

   ![&#x200B; ブランド要素を手動で追加](assets/brand-elements.png)


1. 完了したら、**公開**&#x200B;をクリックして、ブランドをコンテンツレビュー担当者が利用できるようにします。
