---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: プルーフと Creative Cloud Express の概要
description: プルーフと Creative Cloud Express の概要
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 2eef36a6-8c61-4e7e-9760-23114f942250
source-git-commit: dce2d9413b3a363d6508cabec0147c260817ed98
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 5%

---

# Adobe ExpressとWorkfront Proofの統合の概要

Workfront ProofとAdobe Expressを使用すると、次のことができます

* クリエイティブチーム、法務チーム、コンプライアンスチーム間の共同作業を効率化し、管理を維持しながら公開までの時間を短縮します

* 描画マークアップ、注釈、Workfront プルーフビューアを使用したコメントを使用して、ディープレビューを行います

* 電子署名と完全な監査ログにより、企業のコンプライアンス基準に対応


* Express ブランド・テンプレートからの再混在ファイルに対する承認が必要

* 高度なプルーフテンプレートを使用した、複数ステージのレビューと承認のワークフローへの高速テンプレートのマッピング

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
   <p>標準 </p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> 
   <p> Adobe Expressが必要であり、Admin Consoleのユーザーとして製品に追加される必要があります。 </p> </td> 
  </tr>

</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 統合要件

* WorkfrontとAdobe Expressは、同じ IMS 組織にデプロイする必要があります。

* Adobe製品チームが、お使いのアカウントでこの連携を有効にする必要があります。

  >[!IMPORTANT]
  >
  >Adobe ExpressとWorkfront Proofの統合は、複数のリリースを通じて使用できるようになります。最初に、Adobe Admin Console内の同じ組織 ID に関連付けられたWorkfrontとAdobe Expressを持つアカウントを使用し、次に、IMS 組織をまたいで作業しているユーザーを持つお客様を使用します。 統合を有効にする場合は、カスタマーサクセスまたは戦略担当営業にお問い合わせください。

* Adobe Expressでドラフトのレビューを開始する前に、[Adobe Workfront レビューツールを使用してインタラクティブコンテンツをレビュー ](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) をインストールする必要があります。


## Workfrontでの承認ワークフローの設定

標準ライセンスを持つプルーフ管理者は、ユーザーが Express テンプレートに承認ワークフローを追加する前に、Workfrontで承認ワークフローを作成する必要があります。

詳しくは、[ 自動ワークフローテンプレートの作成と管理 ](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md) を参照してください。

## Express テンプレートに承認ワークフローを追加する

承認ワークフローテンプレートがWorkfrontで作成されると、Express Enterprise Premium ライセンスを持つデザイナーは、Adobe Express内で直接 Express テンプレートに割り当てることができます。

Express テンプレートを混在し直す場合は、公開する前に承認が必要です。これにより、事前設定済みの承認ワークフローが自動的にトリガーされます。

Adobe Expressの承認をリクエストするには、標準Workfront ライセンスが必要です。

[ デザインの承認を得る ](https://helpx.adobe.com/jp/express/web/share-and-publish/share-and-collaborate/request-approval.html) 方法を説明します。


## Express テンプレートをリミックスして、レビューと承認を受けるために送信

Adobe Express ユーザーは、ニーズに合わせて Express テンプレートを混在させることができます。 公開する前に、指定された承認者の承認をリクエストする必要があります。

コンテンツの作成およびレビューと承認のプロセスを通じて、ユーザーは以下を行うことができます

* 誰がファイルを開いたかを確認
* すべての参加者の決定ステータスの表示
* コメントを読む
* その他

<!--Learn how to get approval on designs.   
need link to help article-->

## Remixed Express ファイルの確認と承認

関係者は、Workfront プルーフビューアでマークアップツールとコメントを使用して、専門知識の分野（コピー、法務、ブランドなど）に関連するフィードバックを提供できます。

また、コンテンツを公開できるように、コンテンツを承認する最終的な決定を下す責任もあります。

レビューして決定を行うには、少なくとも共同作業者Workfront ライセンスが必要です。
