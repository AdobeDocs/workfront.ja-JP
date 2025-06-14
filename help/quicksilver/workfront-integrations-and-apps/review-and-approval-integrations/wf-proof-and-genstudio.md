---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: GenStudio for Performance MarketingとWorkfront Proofの統合の概要
description: GenStudio for Performance MarketingとWorkfront Proofの統合の概要
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: 4b0ba0112138b91b12e10f4770ecab3db4e3fddb
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 7%

---

# GenStudio for Performance MarketingとWorkfront Proofの統合の概要

GenStudio for Performance MarketingとWorkfront Proofの統合により、次のことが可能になります

* Workfront プルーフテンプレートを使用したレビューワークフローと承認ワークフローの定義

* Workfront プルーフビューアでのGenStudio for Performance Marketing ドラフトコンテンツのレビューと承認

* 最終承認および公開用にGenStudio for Performance Marketingでレビューの決定を表示する

GenStudio for Performance Marketingでのレビューと承認について詳しくは、[Workfront ProofとGenStudio for Performance Marketingの統合 ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/approve/proof-integration) を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>任意</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>現在：標準 </p> 
   <p>レガシー：プラン </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> 
   <p> GenStudio for Performance Marketingが必要であり、Admin Consoleのユーザーとして製品に追加される必要があります。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 統合要件

* WorkfrontとGenStudio for Performance Marketingは、同じ IMS 組織にデプロイする必要があります。

* ユーザーは、IMS 組織内の 1 つのWorkfront インスタンスにのみ属することができます。

* Workfront インスタンスは、Adobe統合エクスペリエンスで有効にする必要があります。

* Workfrontの設定領域で統合を有効にする必要があります。


## Workfrontでの統合の有効化

この統合を有効にするには、システム管理者である必要があります。

1. 左上隅の **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、**[!UICONTROL 設定]** ![ 設定アイコン ](/help/_includes/assets/gear-icon-setup.png) をクリックします。
1. 左側のパネルで、**レビューと承認**/**Adobe GenStudio** をクリックします。
1. **プルーフの承認を使用** を有効にします。
   ![GenStudio設定のプルーフを有効にする ](assets/enable-proofing-gs.png)

## Workfront プルーフテンプレートを使用した承認ワークフローの定義

組織のコンテンツレビュープロセスを頻繁に繰り返したり、同じ人物によってレビューされる場合は、プルーフテンプレートを使用してレビューと承認のワークフローを自動化できます。

### Workfrontでのプルーフテンプレートの作成

1 人または 2 人のレビュー担当者に対して単純な単一ステージテンプレートを作成したり、多数のステージと依存関係を持つ複雑なレビュー用に自動化された複数ステージのテンプレートを作成したりできます。

Workfrontでの自動ワークフローとテンプレートの作成について詳しくは、以下を参照してください。

* [自動ワークフローの概要](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [自動ワークフローテンプレートの作成と管理](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

### GenStudio for Performance Marketingのテンプレートを選択または変更

GenStudio for Performance Marketingでレビューを開始する際には、必要なテンプレートを選択するだけです。 ユーザーは、任意のプルーフワークフローテンプレートを簡単に変更し、いつでもレビュー担当者とステージを追加または削除できます。

詳しくは、[ レビューと承認をリクエスト ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/approve/request-review) を参照してください。

## Workfront プルーフビューアでのGenStudio for Performance Marketing ドラフトコンテンツのレビューと承認

Workfront プルーフビューアを使用して、GenStudio for Performance Marketingで直接ドラフトコンテンツを確認および承認できます。

プルーフビューアを使用すると、次のことができます

* コメントを残す
* ドラフトをマークアップして、変更が必要なものを表示します
* 決定を下す

詳しくは、[ コンテンツのレビューと編集 ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/approve/review-and-edit) を参照してください。


>[!IMPORTANT]
>
>GenStudio for Performance Marketingでドラフトのレビューを開始する前に、[Adobe Workfront レビューツールを使用してインタラクティブコンテンツをレビュー ](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) をインストールする必要があります。


## 最終承認および公開用にGenStudio for Performance Marketingでレビューの決定を表示する

アセットのレビューと承認が完了したら、レビューの決定を確認し、GenStudio for Performance Marketingから直接コンテンツを公開できます。

詳しくは、「[ 承認されたコンテンツの公開 ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/approve/publish-content)」を参照してください。
