---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: プルーフと Creative Cloud Express の基本を学ぶ
description: プルーフと Creative Cloud Express の基本を学ぶ
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 2eef36a6-8c61-4e7e-9760-23114f942250
TQID: https://experienceleague.adobe.com/BCihPeFt421LF8Fa0-XRsAmxSMv-T7kqGEZQ3XeZ-EQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: e4bd5f48-22a4-465d-a046-5ffb52e27856id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 520
ht-degree: 11%

---

# Adobe ExpressとWorkfront Proofの連携の詳細

Workfront ProofとAdobe Expressを使用して、以下を行います

* クリエイティブ部門、法務部門、コンプライアンス部門の間でコラボレーションを合理化し、監視を維持しながら公開までの時間を短縮できます

* Workfrontのプルーフビューアで、描画マークアップ、注釈、コメントを使用して詳細なレビューを実施します

* 電子サインと包括的な監査ログにより、企業のコンプライアンス基準を満たすことができます


* Express ブランドのテンプレートからリミックスされたファイルに対する承認を必要とする

* 高度なプルーフテンプレートを使用して、Express テンプレートを多段階のレビューと承認のワークフローにマッピングできます

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Adobe Workfrontパッケージ</td> 
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
   <td role="rowheader">その他の製品</td> 
   <td> 
   <p> Adobe Expressが必要であり、Admin Consoleのユーザーとして商品に追加する必要があります。 </p> </td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 統合要件

* Adobe Expressにアクセスするための使用権限と、Workfront Standard ライセンスを持つ少なくとも1つのWorkfront環境が必要です。

* ユーザーは、Adobe Expressでドラフトのレビューを開始する前に、[Adobe Workfront レビューツールを使用してインタラクティブコンテンツをレビュー](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md)する必要があります。


## Workfrontでの承認ワークフローの設定

Express テンプレートで承認ワークフローを追加するには、事前に標準ライセンスを持つプルーフ管理者がWorkfrontで承認ワークフローを作成する必要があります。

詳しくは、[自動ワークフローテンプレートの作成と管理](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)を参照してください。

## Express テンプレートへの承認ワークフローの追加

Workfrontで承認ワークフローテンプレートを作成した後、Express Enterprise プレミアムライセンスを持つデザイナーは、Adobe Express内で直接Express テンプレートに割り当てることができます。

Express テンプレートがリミックスされると、公開前に承認が必要になり、事前設定された承認ワークフローが自動的にトリガーされます。

Adobe Expressから承認をリクエストするには、標準Workfront ライセンスが必要です。

デザインに関する承認を[取得](https://helpx.adobe.com/express/web/share-and-publish/share-and-collaborate/request-approval.html)する方法について説明します。


## Express テンプレートをリミックスして、レビューと承認のために送信

Adobe Expressから、Express テンプレートをニーズに合わせて再構成できます。 公開する前に、指定された承認者に承認を依頼する必要があります。

コンテンツの制作およびレビュー/承認プロセス全体を通じて、次のことが可能になります

* ファイルを開いたユーザーを確認する
* すべての参加者の決定ステータスの表示
* コメントを読む
* その他

### 承認をリクエストする際にWorkfront プロジェクトを選択する

リミックス Express テンプレートの承認をリクエストする際に、プルーフを送信するWorkfront プロジェクトを選択できます。 これにより、関連するすべてのアセットとプルーフを同じプロジェクト内で整理できます。

プロジェクトが選択されていない場合、プルーフはデフォルトでExpress固有のプロジェクトになります。

詳しくは、[ レビューと承認用にテンプレートを送信](https://helpx.adobe.com/express/web/invite-collaborate/request-approval.html)を参照してください。

## リミックスされたExpress ファイルのレビューと承認

関係者は、Workfrontプルーフビューアでマークアップツールとコメントを使用することで、コピー、法務、ブランドなど、専門分野に関連するフィードバックを提供できます。

また、コンテンツを公開できるように、コンテンツを承認する最終決定を下す責任もあります。

レビューして決定を下すには、少なくともCollaborator Workfront ライセンスが必要です。
