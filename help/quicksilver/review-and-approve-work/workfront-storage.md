---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Adobe クラウドストレージ上のWorkfrontへの移行
description: Adobe クラウドストレージでのWorkfrontへの移行計画。 組織が有効になっている場合に何が起こるか、Adobe クラウドストレージオブジェクトで何が異なるか、独自のタイミングでロールアウトする方法について説明します。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# Adobe クラウドストレージ上のWorkfrontへの移行

Adobe上のWorkfrontクラウドストレージは、Frame.ioのビューアでのレビュー、強力な承認ワークフロー、アセットの部門横断的な可視化など、包括的な統合レビューと承認エクスペリエンスを提供します。

この記事は、Workfront管理者がAdobe クラウドストレージに移行するための出発点です。 Adobe クラウドストレージを有効にすると何が起こるかを説明し、変更点の詳細と、変更計画と展開に役立つ記事へのリンクを示します。

## Adobe クラウドストレージが有効になるタイミングを決めます

Workfront管理者が&#x200B;**Setup** > **System** > **Preferences**&#x200B;のデフォルトのストレージオプションとしてAdobe クラウドストレージを有効にするまで、Workfront環境に関する何も変わりません。 それまでは、既存のプロジェクトや新しいプロジェクトは、従来のWorkfront ストレージに保持され、現在使用している承認サービスが維持されます。

管理者がAdobe クラウドストレージをデフォルトのストレージオプションとして有効にする場合：

* Adobe クラウドストレージを使用した新規プロジェクト
* デフォルトのビューアはFrame.ioです
* 統合承認は、デフォルトの承認サービスです

既存のプロジェクトは変更されません。

タイミングを制御することで、エクスペリエンスをテストし、Workfront Fusionのシナリオを更新し、誰かが作業する前に変更をレポートする計画を立てることができます。 詳細な手順については、[組織のAdobe クラウドストレージを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)を参照してください。

## Adobe クラウドストレージでの承認作業

Adobe クラウドストレージプロジェクトでは、デフォルトで統合承認が使用され、Frame.io ビューアでレビューと承認が行われます。 従来のWorkfront ストレージに保持されるオブジェクトは、既存の承認サービス（従来のドキュメント承認または統合承認）を保持します。

>[!NOTE]
>
>Adobe クラウドストレージをデフォルトとして設定しても、従来のWorkfront ストレージオブジェクトで既に使用されている承認サービスは変更されません。 統合承認は、Adobe クラウドストレージで作成された新しいオブジェクトに対してのみデフォルトで使用されます。

Adobe クラウドストレージを導入する前に、承認を管理する担当者が何を期待できるのかを把握しておく必要があります。 詳しくは、[従来のドキュメント承認から統合承認への移行](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md)を参照してください。

## 引越しの計画

次の記事を、準備しながら順を追って説明します。

* [Adobe クラウドストレージの違い](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md)：新しいドキュメント領域とFrame.io ビューアから命名ルール、ストレージクォータ、およびFusionに至るまで、Adobe クラウドストレージオブジェクトの主な違いは次のとおりです。
* [Adobe クラウドストレージのロールアウトを計画](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md)：ロールアウト設定を選択し、1つのグループで試験運用し、ユーザーが驚かないように作業を順序付けする方法。
* [組織のAdobe クラウドストレージを有効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)：組織全体または特定のグループのデフォルトのストレージオプションを設定する手順。
* [&#x200B; レガシーオブジェクトをAdobe クラウドストレージに変換](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md)：レガシーオブジェクトをAdobe クラウドストレージに変換できる3つのケースと、各コンバージョン中に移動する内容。


## 関連する記事

* [Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [統一されたレビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [レビューと承認の統合を始める](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [ドキュメントエリア](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Adobe クラウドストレージモデルのオブジェクト権限とアクセスレベルの概要](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
