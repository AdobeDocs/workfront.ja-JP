---
product-area: documents
navigation-topic: approvals
title: 統一されたレビューと承認の概要
description: WorkfrontとFrame.ioが実現する統合レビューと承認の詳細
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: 61a176b006f5d7088b3bdb7568977de6624f9603
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---


# 統一されたレビューと承認の概要

WorkfrontとFrame.ioが提供する統合レビューおよび承認機能により、プロジェクトコーディネーターはWorkfrontでプロジェクトを管理し、作業を計画できます。また、クリエイター、マーケター、ステークホルダーはFrame.ioでアセットをレビューおよび承認できます。

## 統合要件

* WorkfrontとFrame.ioは、同じIdentity Management システム（IMS）組織にデプロイする必要があります。

* ユーザーは、IMS組織内の1つのWorkfront インスタンスにのみ属することができます。

* Workfront インスタンスは、Adobe Unified ExperienceおよびAdobe エンタープライズストレージで有効にする必要があります。

* 統合は、Adobe Professional Servicesで設定する必要があります。


## Adobe Enterprise Storage上に構築

統一されたレビューと承認は、Adobeエンタープライズストレージ上に構築されています。WorkfrontやFrame.ioなどのAdobeエンタープライズ製品全体のアセットの中央リポジトリとして機能する、クラウドベースのストレージソリューションです。<!--, and Creative Cloud.-->

Adobeエンタープライズストレージの主な利点は次のとおりです。

* クリエイティブおよび作業管理アセット向けの統合ストレージレイヤー
* 安全なアクセス制御のためのAdobe Identity Managementシステム（IMS）による一元的な権限
* WorkfrontとFrame.io全体でエンドツーエンドのアセットを可視化<!--, and Creative Cloud apps -->
* エンタープライズニーズに対応する拡張性の高いストレージとノルマの管理

詳しくは、[Adobe エンタープライズストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

## 統一されたレビューと承認

統合されたレビューと承認を利用することで、次のことが可能になります。

* Workfrontから直接レビューや承認を作成、管理できます
* レビューと承認のステータスをリアルタイムで追跡し
* フィードバックと承認を一元化したい
* あらゆる関係者が最新バージョンのアセットにアクセスできる
* AI レビュー担当者を活用してブランドコンプライアンスのレビューを自動化する
* その他

詳しくは、[統一ドキュメント承認：記事インデックス ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)を参照してください。


### Frame.io ビューアの使用

Frame.io ビューアを使用したアセットのレビューと承認 Frame.io ビューアには

* マークアップツールとコメントツール
* バージョン履歴と比較
* ビデオレビュー用のタイムスタンプ付きコメント
* 外出先でのレビューと承認のためのモバイルアクセス

詳しくは、[統合レビューと承認の概要](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md)を参照してください。

#### ビデオレビューの制限

ビデオプルーフのリクエストには、組織の有料Workfront ユーザーライセンスの10%であるStandardとLightの年間上限が設定されています。 このキャップは、組織レベルで適用されます。

Workfront管理者は、使用率がキャップの80%と100%に達すると、通知を受け取ります。

この制限は、Frame.io Enterpriseのお客様には適用されません。

#### Frame.io ビューアでサポートされているファイルタイプ

Frame.io ビューアは、一般的なビデオ、画像、オーディオ、PDF、MS® Officeのすべてのタイプをサポートしています。 サポートされているファイルの詳細なリストについては、[Frame.ioでサポートされているファイルタイプ ](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)を参照してください。

#### Frame.io ビューアへのアクセスとライセンス

Frame.io ビューアは、すべてのWorkfront レビューおよび承認ワークフローのデフォルトビューアです。 有料ライセンスを持つすべてのWorkfront ユーザーに対して自動的に含まれます。 レビューや承認にFrame.io ビューアを使用するために、追加のFrame.io ライセンスは必要ありません。

Frame.ioでアセットをプロジェクトに直接アップロードするなど、この統合で利用可能な追加のFrame.io機能を利用したい場合は、Frame.io エンタープライズライセンスを購入できます。 Adobeの担当者にお問い合わせいただき、デモを予約したり、Frame.io ソリューション全体のメリットをご確認ください。

Workfront プルーフ機能は、この統合では使用できません。

## Workfrontの強力なプロジェクト管理

プロジェクトコーディネーターは、Workfrontの強力なプロジェクト管理機能を活用して、作業を計画、追跡、管理できます。

Workfrontでのプロジェクトの管理について詳しくは、[ プロジェクト：記事インデックス ](/help/quicksilver/manage-work/projects/create-projects/create-project.md)を参照してください。

### 構造と命名規則の適用

統一されたレビューと承認はAdobe エンタープライズストレージを使用して構築されるので、プロジェクトやドキュメントを管理する際に認識すべき構造と命名規則がいくつかあります。

* オブジェクト名は一意である必要があり、重複することはできません
* Adobe エンタープライズストレージでは、階層ツリー内に同じ親を持つピアオブジェクトに一意の名前が必要です
* ドキュメントが同じプロジェクトに属している場合、同じ名前を付けることはできません
* 文書名に次の特殊文字を含めることはできません：\ / : * ? &quot; | &lt; >
* ドキュメント名は最大255文字に制限されています

これらの制限を念頭に置いて、Workfrontでは、競合を防ぐために、必要に応じてオブジェクトまたはドキュメントの名前が自動的に変更されます。

### 共有と権限

この統合の一環として、Workfrontでユーザー権限が制御され、Frame.ioに流れ込みます。 つまり、Frame.ioのプロジェクトにユーザーを招待したり、Frame.ioのユーザー権限を変更したりすることはできません。 これらの操作は、Workfrontのプロジェクト共有モーダルを使用して実行する必要があります。

次の表は、Workfrontの権限がFrame.ioの権限にどのようにマッピングされるかを示しています。

<table>
<tr>
<th>Workfront ユーザー権限</th>
<th>Frame.io ユーザー権限</th>
</tr>
<tr>
<td>管理</td>
<td>編集して共有</td>
</tr>
<tr>
<td>参加</td>
<td>編集して共有</td>
</tr>
<tr>
<td>表示</td>
<td>コメントのみ</td>
</tr>
</table>



### Workfrontのドキュメント管理

Workfrontにアップロードされたドキュメントは、Adobe エンタープライズストレージに保存され、WorkfrontとFrame.ioの両方からアクセスできます。 Workfrontでタスクまたはイシューにドキュメントをアップロードすると、タスクまたはイシューから権限を継承するシステム生成フォルダーがAdobe エンタープライズストレージに作成されます。 そのタスクまたはイシューにアップロードされたすべてのドキュメントは、そのフォルダーに保存され、そこから権限を継承します。 Workfrontのドキュメントについて詳しくは、[新しいドキュメント エリアの概要](/help/quicksilver/documents/managing-documents/documents-area.md)および[Adobe エンタープライズ ストレージ モデルのオブジェクト権限とアクセス レベルの概要](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)を参照してください。

### ドキュメントエクスペリエンスの制限

次のドキュメント機能は含まれません。

<!--* External document providers-->
* Workfrontのプルーフへのアクセス
* Workfrontのドキュメントビューア
* お気に入りドキュメント
* ドキュメントのリクエスト










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->