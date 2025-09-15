---
product-area: documents
navigation-topic: approvals
title: Frame.io 統合の概要
description: Frame.io 統合の概要
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---


# Frame.io 統合の概要

Workfrontと Frame.io の統合により、プロジェクトコーディネーターはWorkfrontでプロジェクトを管理し作業を計画できますが、クリエイティブ、マーケター、関係者は Frame.io でアセットをレビューし承認できます。

## Adobe Enterprise Storage Management に基づいて構築

この統合の中核となるのは、Adobe Enterprise Storage Management （ESM）です。ESM は、Workfrontや Frame.io などのAdobe エンタープライズ製品にまたがるアセットの中央リポジトリとして機能するクラウドベースのストレージソリューションです。

Adobe Enterprise Storage Management の主なメリットは次のとおりです。

* クリエイティブおよび作業管理アセット向けの統合ストレージレイヤー
* 安全なアクセス制御を実現する、Adobe IMSを介した一元化された権限
* Workfront、Frame.io、Creative Cloud アプリ <!--coming soon?--> ース全体でアセットをエンドツーエンドで可視化
* 企業のニーズに応える拡張性の高いストレージとクォータ管理

詳しくは、[Adobe エンタープライズストレージ管理の概要 ](help/quicksilver/review-and-approve-work/esm-overview.md) を参照してください。

## 統一されたレビューと承認

Workfrontと Frame.io の統合では、Workfrontの統合承認機能を使用して、レビューと承認を管理します。 統合承認を使用すると、次のことができます。

* Workfrontから直接レビューと承認を作成および管理する
* レビューと承認のステータスをリアルタイムでトラッキングする
* フィードバックと承認を 1 か所で一元化
* すべての関係者がアセットの最新バージョンにアクセスできることを確認します
* AI レビュー担当者を利用して、ブランドコンプライアンスレビューを自動化します
* その他

詳しくは、[ 統合ドキュメント承認：記事インデックス ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md) を参照してください。


### Frame.io ビューアの使用

また、この統合は Frame.io ビューアとも接続します。 Frame.io ビューアは、

* マークアップ ツールとコメント ツール
* バージョン履歴と比較
* ビデオレビューのタイムスタンプ付きコメント
* 外出先でのレビューや承認のためのモバイルアクセス

詳しくは、[Frame.io 統合の概要 ](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md) を参照してください。

#### ビデオレビューの制限

<!--need to confirm these-->

#### Frame.io ビューアでサポートされるファイルタイプ

Frame.io ビューアは、すべての一般的なビデオ、画像、オーディオ、PDFおよび MS® Office タイプをサポートしています。 サポートされているファイルの詳細なリストについては、[Frame.io のタイプ ](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io) を参照してください。

#### Frame.io ビューアのアクセスとライセンス

Frame.io ビューアは、有料ライセンスを持つすべてのWorkfront ユーザーが利用できます。 この統合によるレビューと承認に Frame.io ビューアを使用する場合、追加の Frame.io ライセンスは必要ありません。

組織が Frame.io のプロジェクトへの直接アセットのアップロードなど、Frame.io の追加機能を活用する場合は、Frame.io エンタープライズライセンスを購入できます。<!--link to Frame.io enterprise license info or who to contacT?-->

Workfrontのプルーフ機能は、この統合では使用できません。

## Workfrontの強力なプロジェクト管理

Workfrontと Frame.io の統合により、プロジェクトコーディネーターはWorkfrontの強力なプロジェクト管理機能を活用して、作業の計画、トラッキング、管理を行うことができます。

Workfrontのプロジェクト管理について詳しくは、[ プロジェクト：記事のインデックス ](/help/quicksilver/manage-work/projects/projects-toc.md) を参照してください。

### 構造と命名規則の適用

この統合は ESM を使用して構築されるので、プロジェクトとドキュメントを管理する際に注意すべき構造と命名規則がいくつかあります。

* オブジェクト名は一意である必要があり、複製できません
* ESM には、階層ツリー内の同じ親を持つピア・オブジェクトに対して一意の名前が必要
* ドキュメントが同じプロジェクトに属している場合、ドキュメントに同じ名前を付けることはできません

これらの制限を念頭に置いて、Workfrontは、競合を防ぐために必要に応じてオブジェクトまたはドキュメントの名前を自動的に変更します。

### Workfrontの Document Management

ドキュメントは、この統合でプロジェクトレベルで管理され、現時点ではタスクまたはイシューにアップロードできません。

ドキュメントアクセスは、プロジェクトレベルでも管理されます。 ユーザーがプロジェクトへのアクセス権を持っている場合、そのプロジェクトに関連付けられたすべてのドキュメントにアクセスできます。

<!--Documents can't be dragged as full folders.-->

### ドキュメントエクスペリエンスの制限

この統合は ESM を使用して構築されるので、Workfrontでの元のドキュメントエクスペリエンスにいくつかの制限があります。

#### 制限事項

次の機能は、この統合には含まれません。

* 外部ドキュメント プロバイダー
* プルーフへのアクセス
* Workfrontのドキュメントビューア


#### 一時的な制限

現時点では、次の機能は使用できません。

* お気に入りのドキュメント
* ドキュメントを要求
* Adobe Experience Manager Assetsへのドキュメントの送信
* 複数ステージの承認
* Workfrontでのコメントまたは更新へのドキュメントのアップロード
* Workfrontでのタスクまたは問題へのドキュメントのアップロード



