---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: プルーフとGenStudio for Performance Marketingの統合の基本を学ぶ
description: プルーフとGenStudio for Performance Marketingの統合の基本を学ぶ
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: e67446c6fb3e90d5dc45dd446988e5d02291f775
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 10%

---

# プルーフとGenStudio for Performance Marketingの統合の基本を学ぶ

プルーフとGenStudio for Performance Marketingの統合により、次のことができます

* Workfront プルーフテンプレートを使用したレビューワークフローと承認ワークフローの定義

* プルーフビューアでのGenStudio ドラフトコンテンツのレビューと承認

* 最終承認および公開用にGenStudioでレビューの決定を表示する


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

1. 左上隅の **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、**[!UICONTROL 設定]** ![ 設定アイコン ](/help/_includes/assets/gear-icon-setup.png) をクリックします。
1. 左側のパネルで、**レビューと承認**/**Adobe GenStudio** をクリックします。
1. **プルーフの承認を使用** を有効にします。
   ![GenStudioのプルーフを有効にする ](assets/enable-proofing-gs.png)

## Workfront プルーフテンプレートを使用した承認ワークフローの定義

組織のコンテンツレビュープロセスを頻繁に繰り返したり、同じ人物によってレビューされる場合は、プルーフテンプレートを使用してレビューと承認のワークフローを自動化できます。

1 人または 2 人のレビュー担当者に対して単純な単一ステージテンプレートを作成したり、多数のステージと依存関係を持つ複雑なレビュー用に自動化された複数ステージのテンプレートを作成したりできます。

GenStudioでレビューを開始する際には、必要なテンプレートを選択するだけです。 ユーザーは、任意のプルーフワークフローテンプレートを簡単に変更し、いつでもレビュー担当者とステージを追加または削除できます。

プルーフワークフローテンプレートを使用すると、次のことができます

* 特定のユーザーを追加し、それぞれに指定したプルーフの役割を割り当てる
* 期限の設定
* ステージがアクティブ化されるタイミングを選択
* 完了後にステージをロック
* 必要な校正判断を 1 つにする
* プライマリ意思決定者の指定
* その他

自動ワークフローとテンプレートについて詳しくは、を参照してください。

* [自動ワークフローの概要](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [自動ワークフローテンプレートの作成と管理](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

## プルーフビューアでのGenStudio ドラフトコンテンツのレビューと承認

GenStudioのドラフトコンテンツは、GenStudioのプルーフビューアで直接確認および承認できます。

プルーフビューアを使用すると、次のことができます

* コメントを残す
* ドラフトをマークアップして、変更が必要なものを表示します
* 決定を下す

GenStudioでのレビューと承認について詳しくは、<!--[Workfront Proof integration with GenStudio for Performance Marketing]().--> を参照してください。

## 最終承認および公開用にGenStudioでレビューの決定を表示する

アセットのレビューと承認が完了したら、レビューの決定を確認し、GenStudioから直接コンテンツを公開できます。

詳細は、<!--[link to GS docs]().--> を参照してください
