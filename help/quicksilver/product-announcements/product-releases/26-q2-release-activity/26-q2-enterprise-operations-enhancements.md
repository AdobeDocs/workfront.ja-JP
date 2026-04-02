---
title: 2026年第2四半期のエンタープライズオペレーションの強化
description: 2026年第2四半期のエンタープライズオペレーションの強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 6d2d26d7e40eef593d73f6ee8bc733a3cce007f5
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 8%

---

# 2026年第2四半期のエンタープライズオペレーションの強化

このページでは、プレビュー環境への2026年第2四半期リリースで行われたエンタープライズオペレーションの機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2026年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)を参照してください。

## Adobe Workfrontでエンタープライズオペレーション機能を利用できるようになりました

>[!NOTE]
>
>プレビュー：2026年4月2日（PT）
>実稼動（迅速リリース）：2026年4月15日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

Adobe Workfrontの高度なエンタープライズオペレーション能力は、財務、プロジェクト、エンタープライズアクセスを管理する、統合されたスケーラブルな方法です。 これらの機能は、企業が収益性と効率性を維持しながら業務を遂行するために必要な可視性と管理性を提供します。

### 高度な財務管理

>[!NOTE]
>
>これらの機能は、Workflow Ultimate パッケージの組織でのみ使用できます。

マルチレベルのコスト階層と請求レート階層を利用して、財務を予測、追跡、最適化できます。

この財務管理の機能強化には、次のものが含まれます。

* **レート属性**&#x200B;を使用すると、担当業務を超えたレートにディメンションを追加できます。これにより、レートは担当業務だけでなく、代理店、場所、ブランド、コストセンターなどの要因によっても異なる場合があります。 これらの属性を組み合わせることで、Workfrontは適切な割り当て率を自動的に選択し、プロジェクト全体の財務的な正確性と一貫性を確保できます。

  詳しくは、[ レート属性の定義](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)を参照してください
* **レートカード**&#x200B;は、クライアント固有の請求を体系化された方法で管理し、ロールベースのレートとカスタマイズ可能な属性を組み合わせて、正確で管理されたプロジェクトのコストを確保します。

  詳しくは、[評価カードの管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)および[プロジェクトへの評価カードの添付](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)を参照してください。
* **User and Role Hourly**&#x200B;という新しいコストと収益タイプ。 このタスクタイプが割り当てられている場合、高度なレート階層ロジックによって、レートカード、プロジェクト、割り当て、ジョブロール、ユーザープロファイルなど、様々なレベルの請求レートとコストレートが決定されます。 レート属性とレートカードの適用に使用できる唯一のコストと収益タイプは、ユーザーと役割の時間単位です。

  詳しくは、[収益とコスト階層の概要](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)を参照してください。
* 再設計された&#x200B;**高度な割り当て**&#x200B;のエクスペリエンスと、拡張された設定可能性により、レート、時間枠、プロパティ全体の可視性と制御が向上しました。

  詳しくは、[詳細な割り当てを作成](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)を参照してください。

  4月16日の実稼動リリースの前に、古い高度な割り当てエクスペリエンスと新しい高度な割り当てエクスペリエンスのどちらかを選択できるスイッチが追加されます。 古いエクスペリエンスがデフォルトのままになります
* 請求用の&#x200B;**担当業務**&#x200B;です。この担当業務では、ユーザーの主な担当業務とは異なる担当業務でユーザーに請求できます。 これは、別の料金で請求する必要がある作業を一時的に実行する場合に便利です。

  詳しくは、[請求用の担当業務の設定](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md)を参照してください。
* 日付が有効な&#x200B;**為替レート**。

  詳しくは、[為替レートの設定](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。
* タスク **に**&#x200B;残業乗数を追加する機能。この機能は、そのタスクのすべての予定時間を乗算し、予定収益の計算に影響します。

  詳しくは、[残業率の定義](/help/quicksilver/manage-work/projects/project-finances/define-overtime-ratio.md)を参照してください。
* **すべての請求情報を保持**&#x200B;し、今後の変更を防ぐためのプロジェクトレベルのコントロール。

  詳しくは、[プロジェクトを編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。
* **レートカードで定義されている担当業務エイリアス**。 レートカードがプロジェクトに添付されている場合、内部担当者名ではなく、プレースホルダーの割り当て、費用、レポートなどの情報にエイリアスが表示されます。

  詳しくは、[レートカードの管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)を参照してください。

### 履歴データトレーシング

**プロジェクトスナップショット**&#x200B;を使用して、プロジェクトをより効果的に管理し、情報に基づいた意思決定を行います。

詳しくは、[ プロジェクトのスナップショットの作成と表示](/help/quicksilver/manage-work/projects/create-projects/create-snapshots.md)を参照してください。

>[!NOTE]
>
>* プロジェクトスナップショットは、Workflow Ultimate パッケージの組織でのみ使用できます。
>* 製品スナップショットにはプレビューリリースはなく、4月16日に実稼動環境に直接リリースされます。

### エンタープライズ権限

**ビジネスプロファイル**&#x200B;は、安全でスケーラブルなシステムアクセスを提供し、エンタープライズガバナンスの強化に役立ちます。

詳しくは、[ ビジネスプロファイルの概要](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md)を参照してください。

>[!NOTE]
>
>ビジネスプロファイルは、Workflow Ultimate パッケージの組織でのみ使用できます。

また、コストと請求データの両方を表示する権限は、ユーザーアクセスレベルとオブジェクト権限の両方で、一般的な財務権限から分離されています。 詳しくは、[財務データへのアクセスの許可](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)および[オブジェクトに対する財務権限の共有](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)を参照してください。

>[!NOTE]
>
>すべてのWorkfront パッケージとWorkflow パッケージでは、個別のコストと請求の権限を組織で使用できます。

### カスタムフォームとフィールドの機能強化

カスタムフォームの高度なロジックにより、より明確なインサイトを獲得し、より正確なプロジェクト管理と財務管理を実現できます。

カスタムフォームの機能強化は次のとおりです。

* 新しい&#x200B;**高度なロジックタイプ**：高度な表示、デフォルト値、条件付き書式設定、編集可能性

  詳細については、[ カスタムフォームとフィールドへのロジックルールの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)を参照してください。

  >[!NOTE]
  >
  >新しいロジックタイプは、Workflow PrimeまたはUltimate パッケージの組織でのみ使用できます。

* フォームデザイナーのインターフェイスが強化されました。
   * フォーム名がデザイナーの左上に表示され、スクロールすると長いフォームに名前が表示されるようになりました。
   * フォームが添付できるオブジェクトタイプは、ドロップダウンリストにあります。
   * すべてのロジックタイプについて、フィールドにロジックインジケーターを表示または非表示にすることができます。 表示およびスキップロジックのタイプは、影響を受ける両方のフィールドの指標を示します。 他のすべてのロジックタイプは、1つのフィールドに影響します。

  詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

  >[!NOTE]
  >
  >これらの機能は、すべてのWorkfrontおよびワークフローパッケージの組織で使用できます。

* チーム、レートカード、担当業務にカスタムフォームを追加できる
詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

  >[!NOTE]
  >
  >* レートカードや担当業務にカスタムフォームを追加するには、ワークフローUltimateパッケージが必要です。
  >* チームにカスタムフォームを追加することは、すべてのWorkfrontおよびワークフローパッケージで組織が使用できます。

* 通貨形式のフィールドに対する&#x200B;**財務権限タイプ**の設定。特定の権限が設定されているユーザーのみにアクセスを許可します
詳しくは、[ カスタムフィールド内の財務データへのアクセスを制限](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/restrict-access-to-financial-data.md)を参照してください。

  >[!NOTE]
  >
  >この機能は、すべてのWorkfrontおよびワークフローパッケージの組織で使用できます。

### レイアウトテンプレートの機能強化

>[!NOTE]
>
>これらの機能は、すべてのWorkfrontおよびワークフローパッケージの組織で使用できます。


レイアウトテンプレートでは、追加のオブジェクトのヘッダーと左側のナビゲーションメニューをカスタマイズし、メインメニューでの項目の表示と非表示をより簡単にできます。 また、レイアウトテンプレートを使用して、ユーザーがプロジェクト、タスク、イシュー、ポートフォリオ、プログラムの&#x200B;**詳細** メニュー（3 ドットメニュー）をクリックしたときに表示されるオプションを決定することもできます。

詳しくは、[レイアウトテンプレートの作成および管理](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

### カスタムローカライゼーション

>[!NOTE]
>
>この機能は、Workflow PrimeまたはUltimate パッケージの組織でのみ使用できます。

カスタムローカライゼーションを使用すると、様々な言語でカスタム用語やフレーズを定義できます。 次に、Workfrontでは、これらの用語がブラウザー設定で設定された言語で表示されます。
例えば、「Target Audience」というラベルを設定して、ドイツ語の「Zielgruppe」に変換できます。 Adobe IMSアカウントの言語としてドイツ語を設定したユーザーは、英語で「Target Audience」というラベルが付いたフィールドのラベルとして「Zielgruppe」という単語を見ることができます。

詳しくは、[ カスタムローカライゼーションの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md)を参照してください。

### ビジネスルールでアクションを自動化

>[!NOTE]
>
>これらの機能は、Workflow Ultimate パッケージの組織でのみ使用できます。

Workfront管理者は、特定の条件が満たされたときに、作成、編集、または変更されたオブジェクトのアクションを自動化するようにビジネスルールを設定できるようになりました。 使用可能なアクションには、オブジェクトの共有や、カスタムフォームのオブジェクトへの添付などがあります。

詳しくは、[ ビジネスルールの作成と編集](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)を参照してください。


