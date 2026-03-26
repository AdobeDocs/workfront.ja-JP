---
product-area: documents
navigation-topic: approvals
title: アドビのエンタープライズストレージの概要
description: アドビのエンタープライズストレージの概要
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 86d5ed6f91bca0b68748a43476710028d34d6ad2
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 2%

---

# アドビのエンタープライズストレージの概要

Adobe エンタープライズストレージは、Adobe エンタープライズ製品全体のアセットの中央リポジトリとして機能するクラウドベースのストレージソリューションです。 WorkfrontとFrame.ioの連携は、Adobeエンタープライズストレージ上に構築されているため、シームレスな連携とアセット管理が可能です。

このストレージオプションは、Adobe Creative Cloudなどの他のAdobe製品との将来のアセット管理との統合にも役立ちます。

## 主な特長

* **統合ストレージレイヤー**: Adobe エンタープライズストレージは、Workfront、Frame.io、Document Cloud、Creative Cloudの共有ストレージバックエンドとして機能します。 これにより、チャネルをまたいだシームレスな共同作業とアセット管理が可能になります。

* **Content supply chainの有効化**: Adobe エンタープライズストレージは、Adobe Content Supply chain ビジョンの基盤となるコンポーネントであり、さまざまなAdobe アプリケーションに手動でダウンロードしたり再アップロードしたりすることなく、作業中のアセットを管理することができます。

* **権限とアクセスの一元管理**: Adobe エンタープライズストレージは、エンタープライズレベルのアクセス制御をサポートしており、Adobe IMS（Identity Management System）と統合して、安全でスケーラブルなユーザー権限を実現します。

* **エンドツーエンドのアセットの可視化**: Adobe エンタープライズストレージに保存されたAssetsは、Workfront、Frame.io、Creative Cloud アプリで直接サーフェイスおよび管理でき、一貫したメタデータ、バージョン管理、監査証跡を提供します。

* **レビューと承認のワークフローとの統合**: Adobe エンタープライズストレージは、すべてのアセットの信頼できる唯一の情報源として機能し、フィードバックと承認が一元的に追跡されるようにすることで、クリエイティブなレビューと承認のワークフローを可能にします。

* **スケーラブルなストレージと割り当て管理**:Adobe エンタープライズストレージは、Adobe製品全体でスケーラブルなストレージオプションと統合された割り当て追跡を提供します。

## レビューおよび承認ワークフローとの統合

WorkfrontとFrame.ioの連携により、Adobeのエンタープライズストレージを活用して、レビューと承認のプロセスを一元管理できます。 この統合により、プロジェクトコーディネーターはWorkfrontでプロジェクトを管理し、作業を計画できるようになります。また、クリエイター、マーケター、ステークホルダーは、Frame.ioでアセットをレビューおよび承認できます。 これにより、あらゆる関係者が最新バージョンのアセットにアクセスでき、フィードバックが一元化されます。

WorkfrontとFrame.ioの連携について詳しくは、[統一されたレビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)を参照してください。

## Adobe エンタープライズストレージと従来のWorkfront ストレージの違い

既存のWorkfront環境には、Adobe エンタープライズストレージと従来のWorkfront ストレージが組み合わされています。 Adobe エンタープライズストレージのリリース前に作成されたオブジェクトは、従来のWorkfront ストレージを使用します。

環境でAdobe エンタープライズストレージを有効にすると、Adobe エンタープライズストレージと従来のWorkfront ストレージプロジェクトの両方を作成できます。

>[!NOTE]
>
>新しい環境では、Adobe エンタープライズストレージがデフォルトで有効になっており、従来のWorkfront ストレージを使用するオプションはありません。


### ドキュメント

#### 新規ドキュメント領域

新しいドキュメント エリアは、Adobe エンタープライズ ストレージ用に再設計された統合ドキュメント エリアです。

更新されたインターフェイスにより、ナビゲーションが簡素化され、わかりやすくなり、チームは単一の統合環境でレビューと承認を容易に管理できるようになります。 詳しくは、[&#x200B; ドキュメント エリアの概要](/help/quicksilver/documents/managing-documents/documents-area.md)を参照してください。

#### 新しいドキュメント権限モデル

>[!IMPORTANT]
>
>Adobe エンタープライズストレージでは、ドキュメントの権限は、従来のWorkfront ストレージとは異なります。 ドキュメントは、リンクされているプロジェクト、タスク、イシューから権限を継承します。

ドキュメントを個別に共有することはできません。 代わりに、タスクまたはイシューごとにフォルダーが自動的に生成され、タスクまたはイシューから権限が継承されます。 タスクまたはイシューにアップロードされたドキュメントは、生成されたフォルダーに保存されます。

新しいドキュメント権限モデルについて詳しくは、[Adobe エンタープライズストレージモデルのオブジェクト権限とアクセスレベルの概要](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)を参照してください。

##### フォルダー上のリンクされたオブジェクト

プロジェクトレベルでは、システム生成フォルダーにリンクされたオブジェクトが表示されます。 フォルダーには、属するタスクまたはイシューと自動的に同じ名前が付けられます。 リンクされたフォルダーは、フォルダーを表示するタスクまたはイシューをシステムが把握する仕組みです。

詳しくは、[&#x200B; ドキュメント権限の仕組み](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)を参照してください。

## Workfront オブジェクト

次の表は、Workfront オブジェクトのAdobe エンタープライズストレージと従来のWorkfront ストレージの機能を比較したものです。

Workfront オブジェクトには、ポートフォリオ、プログラム、プロジェクト、テンプレート、タスク、イシューが含まれます。

| Adobe エンタープライズストレージ | 従来のWorkfront ストレージ |
|---|---|
| <ul><li>Adobe エンタープライズストレージの使用</li><li>Frame.ioとの統合</li><li>新しい文書エクスペリエンスを使用</li><li>厳密な命名規則の適用</li><li>ドキュメントを直接共有することはできません</li><li>ドキュメントは、Frame.ioやCreative Cloudなどの他のAdobe製品で利用できます</li></ul> | <ul><li>Workfront ストレージの使用</li><li>プルーフビューアの使用</li><li>個々のドキュメントの共有をサポート</li></ul> |

### オブジェクトの移動、コピー、変換

Workfront オブジェクトは、ストレージモデルなどの間で移動、コピー、変換できます。 例えば、タスクをAdobe エンタープライズストレージプロジェクトから別のAdobe エンタープライズストレージプロジェクトに移動できます。 タスクをAdobe エンタープライズストレージプロジェクトから従来のWorkfront ストレージプロジェクトに移動することはできません。

これらのアクションは、タスクまたはイシューの「その他」メニューから使用できます。 各アクションは、ドキュメントの完全性、権限の継承、Adobe エンタープライズストレージルールを尊重します。

## Adobe エンタープライズストレージを有効にする

既存のお客様は、契約更新時にAdobe エンタープライズ版ストレージを有効にすることができます。 Adobe エンタープライズ ストレージの有効化について詳しくは、[組織のAdobe エンタープライズ ストレージの有効化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)を参照してください。

>[!NOTE]
>
>新規のお客様は、Adobe エンタープライズストレージをデフォルトで有効にしており、従来のWorkfront ストレージを使用するオプションはありません。



## 考慮事項

* WorkfrontがFrame.ioまたはCreative Cloudと同期しなくなる可能性があります。例えば、アセットがWorkfrontで削除されてもFrame.ioに表示される場合は、Workfront サポートにお問い合わせください。


