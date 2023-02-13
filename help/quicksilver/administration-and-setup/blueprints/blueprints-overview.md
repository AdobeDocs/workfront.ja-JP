---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントの概要
description: ブループリントは、成長する作業管理システムの作成に役立つ基本的な構成要素を提供します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# ブループリントの概要

ブループリントは、成長する作業管理システムの作成に役立つ基本的な構成要素を提供します。 システム管理者は、ブループリントカタログを参照して、すぐに使用できるプロジェクトテンプレートをインストールできます。 他のユーザーは、カタログを参照して、ブループリントのインストールを要求できます。 詳しくは、 [ブループリントカタログを参照し、ブループリントのインストールをリクエストします](../../administration-and-setup/blueprints/browse-catalog.md).

各ブループリントは、部門と特定の成熟度レベルをターゲットとし、実績のあるベストプラクティスをシステムに迅速に実装するのに役立ちます。 以下に詳しく説明する成熟度レベルは、ブループリントカタログカードと詳細に示されます。

**[!UICONTROL 管理]:** 管理されたプロジェクトテンプレートは、アクティビティと成果物が標準手順として完全に受け入れられる前に、新しいビジネスプロセスの採用をサポートします。 新しいプロセスの各ステップに必ず従うタスクが含まれます。

**[!UICONTROL 統合]:** 統合プロジェクトテンプレートは、ビジネス機能が標準の操作手順を通じてサポートされることを前提としています。 プロセスのコントリビューターは、プロセスに従うために完了する必要がある手順とタスクを把握しています。 このプロセスをサポートするプロジェクトテンプレートに含まれるタスクの数は、レポート作成の目的で必要なマイルストーンやその他の主な成果物のみを追跡するためのタスク数を少なくします。

## 適切なブループリントを検索

ブループリントは、使用例、成熟度レベル、インストールステータス、およびカタログの右側にあるフィルターを使用してタイプ別に参照できます。 興味を持つブループリントを見つけたら、詳細ページで詳細を表示できます。

### ブループリントのタイプ

ブループリントのタイプは、ブループリントに含まれる内容を示します。 タイプは、カタログ内のブループリントカードの下部に表示されます。 ブループリントは複数のタイプを持つことができます。

次のタイプのブループリントを使用できます。

* プロジェクトテンプレート：プロジェクトテンプレートに関連付けられた標準オブジェクト（タスク、問題、役割、チーム）と、これらのオブジェクトに関連する一部の環境設定が含まれます。 詳しくは、 [ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md).
* 組織構造：組織の構造（会社、グループ、ロール、チーム）に関連付けられたオブジェクトが含まれます。 詳しくは、 [ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md).
* ダッシュボード：実装サービスなど、特定のユースケース向けの 1 つ以上のダッシュボードが含まれます。

<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

現在のブループリントを確認するには、 [使用可能なブループリントのリスト](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

###  の詳細を表示

各ブループリントには詳細ページが含まれます。 このページから、次の操作を実行できます。

* ワークフローの内容の概要を表示
* ブループリントの概要を読む
* インストール履歴を表示します ( **[!UICONTROL 詳細を見る]** ブループリントと共にインストールされるオブジェクトの完全なリストを表示するには )
* 役割、チーム、会社、グループの説明を表示
* プロジェクトテンプレートなど、特定のブループリントの視覚的な例を確認する（ブラウザーで完全な画像をプレビューしたり、ダウンロードしたりできます）

![[!UICONTROL ブループリントの詳細] ページ](assets/blueprint-details-page-2022.png)

## ブループリントのインストール

システム管理者は、実稼動環境またはサンドボックス環境に直接インストールできます。 詳しくは、 [ブループリントのインストール](../../administration-and-setup/blueprints/blueprints-install.md) または [ブループリントの設定](../../administration-and-setup/blueprints/configure-template-package.md).

インストール後に、次に実行する最適なアクションについて不明な場合があります。 詳しくは、 [ブループリントのインストール後に実行するアクション](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## ブループリントとテンプレートに関する追加のメモ

ブループリントでは、 [!DNL Adobe Workfront]. ブループリントを使用すると、新しいテンプレートをすばやく作成して、より多くの作業を整理できます。 [!DNL Workfront].

ブループリントをコピーまたは編集することはできません。 ただし、ブループリントからソリューションをインストールした後は、通常の方法でブループリント内のレコードを更新するのと同じ方法で、ブループリントから作成されたプロジェクトテンプレート、ジョブの役割、またはチームを変更できます [!DNL Workfront] インターフェイス。 また、ブループリントをインストールすると、テンプレートは [!UICONTROL テンプレート] ～の面積 [!DNL Workfront] 元のブループリントは [!UICONTROL ブループリント] 領域 必要に応じてテンプレートの調整を開始する前に、テンプレートのコピーを作成する必要はありません。

ブループリントは、環境で設定されたものを削除または置き換えません。 新しいテンプレートを作成するブループリントをインストールして既存のテンプレートを置き換える場合は、テンプレートからプロジェクトを作成するプランナー間での混乱を避けるために、以前のバージョンを非アクティブ化することをお勧めします。
