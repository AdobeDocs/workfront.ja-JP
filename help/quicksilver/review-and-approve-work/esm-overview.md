---
product-area: documents
navigation-topic: approvals
title: Adobe クラウドストレージの概要
description: Adobe クラウドストレージの概要
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: c2fe0c6afbc9b536186bd473e95b3f82f144b06c
workflow-type: tm+mt
source-wordcount: 1061
ht-degree: 1%

---

# Adobe クラウドストレージの概要

Adobe クラウドストレージは、Adobe エンタープライズ製品全体のアセットの中央リポジトリとして機能するクラウドベースのストレージソリューションです。 WorkfrontとFrame.ioの連携は、Adobeクラウドストレージ上に構築されており、シームレスな連携とアセット管理を実現します。

このストレージオプションは、Adobe Creative Cloudなどの他のAdobe製品との将来のアセット管理との統合にも役立ちます。

## 主な特長

* **統合ストレージレイヤー**: Adobe クラウドストレージは、Workfront、Frame.io、Document Cloud、Creative Cloudの共有ストレージバックエンドとして機能します。 これにより、チャネルをまたいだシームレスな共同作業とアセット管理が可能になります。

* **Content supply chainの有効化**: Adobe クラウドストレージは、Adobe Content Supply chain ビジョンの基盤となるコンポーネントであり、さまざまなAdobe アプリケーションで手動ダウンロードや再アップロードを行うことなく、作業中のアセットを管理することができます。

* **権限とアクセスの一元管理**: Adobe クラウドストレージは、エンタープライズレベルのアクセス制御をサポートしており、Adobe IMS（Identity Management System）と統合して、安全でスケーラブルなユーザー権限を実現します。

* **エンドツーエンドのアセットの可視化**: Adobe クラウドストレージに保存されたAssetsは、Workfront、Frame.io、Creative Cloud アプリで直接サーフェイスおよび管理でき、一貫したメタデータ、バージョン管理、監査証跡を提供します。

* **レビューと承認のワークフローとの統合**: Adobe クラウドストレージは、すべてのアセットの信頼できる唯一の情報源として機能することで、クリエイティブなレビューと承認のワークフローを可能にし、フィードバックと承認が一元的に追跡されるようにします。

* **スケーラブルなストレージと割り当て管理**:Adobe クラウドストレージは、スケーラブルなストレージオプションと、Adobe製品全体での統一された割り当て追跡を提供します。

## レビューおよび承認ワークフローとの統合

WorkfrontとFrame.ioの連携により、Adobeのクラウドストレージを活用して、レビューと承認のプロセスを一元管理できます。 この統合により、プロジェクトコーディネーターはWorkfrontでプロジェクトを管理し、作業を計画できるようになります。また、クリエイター、マーケター、ステークホルダーは、Frame.ioでアセットをレビューおよび承認できます。 これにより、あらゆる関係者が最新バージョンのアセットにアクセスでき、フィードバックが一元化されます。

WorkfrontとFrame.ioの連携について詳しくは、[統一されたレビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)を参照してください。

## Adobe クラウドストレージと従来のWorkfront ストレージの違い

既存のWorkfront環境には、Adobe クラウドストレージと従来のWorkfront ストレージが組み合わされています。 Adobe クラウドストレージのリリース前に作成されたオブジェクトは、従来のWorkfront ストレージを使用します。

環境でAdobe クラウドストレージを有効にすると、Adobe クラウドストレージと従来のWorkfront ストレージプロジェクトの両方を作成できます。

>[!NOTE]
>
>新しい環境では、デフォルトでAdobe クラウドストレージが有効になっており、従来のWorkfront ストレージを使用するオプションはありません。


### ドキュメント

#### 新規ドキュメント領域

新しいドキュメント領域は、Adobe クラウドストレージ用に再設計された統合ドキュメント領域です。

更新されたインターフェイスにより、ナビゲーションが簡素化され、わかりやすくなり、チームは単一の統合環境でレビューと承認を容易に管理できるようになります。 詳しくは、[&#x200B; ドキュメント エリアの概要](/help/quicksilver/documents/managing-documents/documents-area.md)を参照してください。

#### 新しいドキュメント権限モデル

>[!IMPORTANT]
>
>Adobe クラウドストレージでは、ドキュメントの権限は従来のWorkfront ストレージとは異なります。 ドキュメントは、リンクされているプロジェクト、タスク、イシューから権限を継承します。

ドキュメントを個別に共有することはできません。 代わりに、タスクまたはイシューごとにフォルダーが自動的に生成され、タスクまたはイシューから権限が継承されます。 タスクまたはイシューにアップロードされたドキュメントは、生成されたフォルダーに保存されます。

新しいドキュメント権限モデルについて詳しくは、[Adobe クラウドストレージモデルのオブジェクト権限とアクセスレベルの概要](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)を参照してください。

##### フォルダー上のリンクされたオブジェクト

プロジェクトレベルでは、システム生成フォルダーにリンクされたオブジェクトが表示されます。 フォルダーには、属するタスクまたはイシューと自動的に同じ名前が付けられます。 リンクされたフォルダーは、フォルダーを表示するタスクまたはイシューをシステムが把握する仕組みです。

詳しくは、[&#x200B; ドキュメント権限の仕組み](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)を参照してください。

#### Adobe Cloud Drive

Adobe Cloud Driveは、Adobe クラウドストレージプロジェクトをMacまたはWindows コンピューターにドライブとしてマウントするデスクトップアプリケーションです。 Adobe Cloud Driveは、Adobe クラウドストレージと作業の同期を維持しながら、任意のアプリケーションでファイルを開き、編集および保存できます。 詳しくは、[Adobe Cloud Driveの概要](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)を参照してください。

## Workfront オブジェクト

次の表は、Workfront オブジェクトのAdobe クラウドストレージと従来のWorkfront ストレージの機能を比較したものです。

Workfront オブジェクトには、ポートフォリオ、プログラム、プロジェクト、テンプレート、タスク、イシューが含まれます。

| Adobe クラウドストレージ | レガシー Workfront ストレージ |
|---|---|
| <ul><li>Adobe クラウドストレージの使用</li><li>Frame.ioとの統合</li><li>新しい文書エクスペリエンスを使用</li><li>厳密な命名規則の適用</li><li>ドキュメントを直接共有することはできません</li><li>ドキュメントは、Frame.ioやCreative Cloudなどの他のAdobe製品で利用できます</li></ul> | <ul><li>Workfront ストレージの使用</li><li>プルーフビューアの使用</li><li>個々のドキュメントの共有をサポート</li></ul> |

### オブジェクトの移動、コピー、変換

ほとんどの場合、Workfront オブジェクトをストレージモデルと同様に移動、コピー、変換できます。 例えば、タスクを1つのAdobe クラウドストレージプロジェクトから別のAdobe クラウドストレージプロジェクトに移動できます。

具体的には、従来のWorkfront ストレージオブジェクトをAdobe クラウドストレージに変換できます。

* 従来のWorkfront ストレージタスクをAdobe クラウドストレージプロジェクトに変換します。
* 従来のWorkfront ストレージポートフォリオをAdobe クラウドストレージポートフォリオに変換します。
* 従来のAdobe ストレージテンプレートからWorkfront クラウドストレージプロジェクトを作成します。

これらの変換中に、ドキュメントとドキュメントフォルダーが従来のWorkfront ストレージからAdobe クラウドストレージに移動することはありません。

詳しくは、[Adobe クラウドストレージでのWorkfrontへの移行](/help/quicksilver/review-and-approve-work/workfront-storage.md)の[&#x200B; オブジェクトポータビリティ &#x200B;](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)を参照してください。

## Adobe クラウドストレージを有効にする

Adobe クラウドストレージをサポートするWorkfrontのバージョンを使用している必要があります。 お客様の組織がまだサポートされているバージョンを使用していない場合は、Adobe アカウント担当者にお問い合わせください。

お客様の環境でAdobe クラウドストレージを有効にする方法については、[お客様の組織でAdobe クラウドストレージを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)を参照してください。

>[!NOTE]
>
>新規のお客様は、Adobe クラウドストレージをデフォルトで有効にしており、従来のWorkfront ストレージを使用するオプションはありません。



## サンドボックス環境でのAdobe クラウドストレージ

Adobe クラウドストレージは[!DNL Workfront] サンドボックス環境で利用できるため、実稼動環境で有効にする前にテストできます。 ただし、Frame.io ビューアはサンドボックスでは利用できないため、統一されたレビューと承認のエクスペリエンスを本番環境で検証する必要があります。

カスタムリフレッシュサンドボックスがある場合は、サンドボックス内のAdobe クラウドストレージ機能にアクセスするために、Adobe クラウドストレージをサポートするWorkfrontのバージョンにアップグレードした後でリフレッシュする必要があります。 詳しくは、[&#x200B; カスタムリフレッシュサンドボックス環境 [!DNL Adobe Workfront] を参照してください。](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## 考慮事項

* WorkfrontがFrame.ioまたはCreative Cloudと同期しなくなる可能性があります。例えば、アセットがWorkfrontで削除されてもFrame.ioに表示される場合は、Workfront サポートにお問い合わせください。


