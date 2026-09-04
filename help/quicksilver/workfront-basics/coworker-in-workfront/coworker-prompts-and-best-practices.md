---
title: CX担当者のプロンプトとベストプラクティス
content-type: reference
description: WorkfrontでCoworkerを使用する際のベストプラクティスについて説明し、プロンプトの例の一覧を表示します。
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 2%

---

# CX担当者のプロンプトとベストプラクティス

&lt;! – これを使用しないでください – 代わりにMCPのサンプル プロンプト記事にリンクし、MCPの最新リリースで更新されていることを確認します – >

>[!IMPORTANT]
>
>CX Coworkerは現在、ヘルスケアや金融など、機密データを扱う業界の企業には利用できません。 AI アシスタントは、これらの組織で利用できます。 詳しくは、[AI アシスタントの概要](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)を参照してください。

CX Coworkerでは、自然言語を使用して、Workfront WorkflowやWorkfront Planningを活用できます。

Adobe Experience Cloud Agent Orchestratorに含まれているチームです。

Agent Orchestratorについて詳しくは、[Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/ja/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator)を参照してください。

## アクセス要件

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>Select、Prime、またはUltimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準または光</p>
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td><p>基本スキル以外の機能を使用する場合は、Adobe Agent Orchestratorを購入している必要があります。</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td><p>Coworkerを通じて任意のオブジェクトを操作するには、適切な権限が必要です。</p> <p>例えば、同僚を通じてプロジェクトに関する情報を受け取るには、少なくともそのプロジェクトに対する表示権限が必要です。</p></td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* Workfrontの管理者が、組織のAI アシスタントを有効にしている必要があります。

  詳しくは、「AI アシスタントの概要」の「[AI アシスタントの前提条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)」を参照してください。
* Workfront管理者が、アクセスレベルに対してAI アシスタントを有効にしている必要があります。

  詳しくは、[AI アシスタントの有効化または無効化](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)を参照してください。

## 考慮事項

CX Workfrontを利用する際には、次の制約を考慮してください。

### 可逆性

一部のアクションは元に戻すことができます。 例えば、オブジェクトが作成された場合、その作成を元に戻すことができます。

ただし、オブジェクトの削除など、一部のアクションは&#x200B;**not**&#x200B;を元に戻すことができます。 Coworkerを通じてデータに対してアクションを実行する際には、この点を考慮することをお勧めします。

### データ/オブジェクトのカバレッジの制約

* カスタムフィールドのクエリとレポートは初期段階にあり、一部のスキル（API ベースのクエリヘルパーなど）では、集計とフィルタリングのための任意のカスタムフィールドをまだ処理していません。

### インタラクション/ユーザーエクスペリエンスの制限

* CX担当者は、現在、個々のユーザーのスタイルや好みから長期的に「学習」することはありません。 あらゆるチャットでは、現在の会話と製品知識のみが使用されます。
* 会話のコンテキストは、1つのチャットセッション内に保持されます。 新しいページを開いたり、アシスタントを閉じたりすると、会話履歴がリセットされます。
* 承認手順がConfluenceやSharePointなどの外部アプリケーションにあり、URL フィールドのみを介してリンクされている場合、Coworkerは現在、それらのページを取得して理由を付けません。

### データ保存/顧客管理キー

* CX CoworkerはAdobe Experience Platform Agent Orchestratorの一部であるため、Coworkerとのやり取りのデータはWorkfrontではなくAdobe Experience Platformに保存されます。 したがって、このデータは、Workfront Customer Managed Keys （BYOK）契約の対象ではありません。

## 汎用的な基本AI スキル

>[!IMPORTANT]
>
>これらの一般的な機能は、署名済みのAdobe AI契約書をファイルに登録しているすべてのユーザーが使用できます。

これらの一般的なスキルのベストプラクティスとプロンプトについては、[AI アシスタント プロンプトとベストプラクティス ](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md)を参照してください。

<!--Follow up with Oznur-->

### 製品知識

CX Coworkerは、Workfrontのドキュメントから取得した手順や参照情報を提供することができます。

Workfront ドキュメントから情報を取得する方法について詳しくは、[AI アシスタントのヘルプを参照してください](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)。

例：タスク期間タイプを変更するにはどうすればよいですか？

### プロジェクト、タスク、イシューの要約

CX Coworkerは、Workfrontにアップロードされたプロジェクト、タスク、またはイシュー<!--, or documents-->を要約できます。

プロジェクト、タスク、問題の概要について詳しくは、[AI アシスタントを使用した要約](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)を参照してください。

例：「Fall Campaign 2026」というプロジェクトを要約します。

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## WORKFRONTのCX担当者

* [プロジェクト、タスク、イシューの情報](#project-task-and-issue-information)
* [プロジェクト管理および作業管理](#project-and-work-management)
* [コンテンツと承認](#content-and-approvals)

### プロジェクト、タスク、イシューの情報

CX Coworkerは、プロジェクト、タスク、イシュー（概要やプロジェクトの健全性など）に関する情報を提供します。

次の領域のドキュメントとアセットの承認のサンプルプロンプトを参照してください。

* [プロジェクト、タスク、イシューに関する情報を検索](#find-information-about-projects-tasks-or-issues)
* [プロジェクト、タスク、イシューの要約](#summarize-projects-tasks-or-issues)
* [ プロジェクト、プログラム、またはポートフォリオのプロジェクトの正常性を表示](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### プロジェクト、タスク、イシューに関する情報を検索

* プロジェクト
  * ブランドマーケティングチームのアクティブなプロジェクトをすべて表示する
  * 「デジタル」カテゴリのQ4 キャンペーンポートフォリオにプロジェクトのリストが必要です。
  * Creative サービス会社のユーザーがプロジェクトマネージャーとして管理しているプロジェクトを表示します。
* タスク
  * Joan Harrisに割り当てられたすべてのタスクを取得します。
  * UX チームに割り当てられた「デザイン」カテゴリのタスクを表示します。
  * ホリデープロモーションプログラムでコピーライターに割り当てられたタスクが必要です。
* イシュー
  * 「技術」カテゴリの「Web サイトの再設計」プロジェクトのすべての問題を表示します。
  * QA グループから報告されたすべての未解決の問題を確認します。
  * グローバルテクノロジー企業の開発者に割り当てられた問題が必要です。

#### プロジェクト、タスク、イシューの要約

* 「このプロジェクトの概要」
* 「このプロジェクトの最終週の概要」

#### プロジェクト、プログラム、ポートフォリオのプロジェクトの正常性を表示

>[!NOTE]
>
>この機能を使用するには、組織をProject Health ベータ版に登録する必要があります。

* 「アクティブなプロジェクトの健全性を表示する」
* 「このプログラムの健全性を示してください」

### プロジェクト管理および作業管理

タスクや割り当てなどのプロジェクトを作成および管理できます。

次の領域のプロジェクトと作業管理のプロンプト例を参照してください。

* [プロジェクトの作成、更新、削除](#create-update-or-delete-projects)
* [ユーザープロンプトに基づいて適切なプロジェクトテンプレートを特定する](#identify-the-right-project-template-based-on-user-prompt)
* [ プロジェクト内のタスクを追加、編集、またはカスタマイズする](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### プロジェクトの作成、更新、削除

プロジェクトをゼロから作成したり、テンプレートから作成したり、プロジェクトを更新したり、削除したりできます。

* 3月10日から4月30日まで、「Q2 Innovation Sandbox」という空白のプロジェクトを作成します。 私をオーナーとして設定してください。
* 統合マーケティングキャンペーンテンプレートを使用して、Lucent AI Launch - NAというプロジェクトを作成します。 2月5日に開始し、現在の値に設定します。
* 3月1日から6月15日までの間に、「Web サイトのリデザイン - EMEA」というプロジェクトを作成します。 これは優先度が高く、EMEA Marketingが所有し、マーケティング担当バイスプレジデントがスポンサーとなり、約25万ドルの予算を組み、コンバージョンの向上を目標にヨーロッパに重点を置いて1,200時間を計画しました。
* Lucent AI Launch - NA プロジェクトの場合は、Q2に移行し、無料トライアルを推進する目的を変更し、4月中旬に終了し、予算を$150,000に増やし、緊急としてマークします。
* 第2四半期に完了する現在のマーケティングプロジェクトのうち、高い優先度または緊急の優先度を示す順に並べたものを表示します。

#### タスクの追加または編集

プロジェクト内のタスクを追加または編集したり、プロジェクトの作成に使用するテンプレートのタスクリストをカスタマイズしたりできます。

* 「ランディングページ QA」という新しいタスクをプロジェクトに追加し、4月22日から4月26日までスケジュールします。
* 4月18日に完了するようにデザインレビュータスクを更新し、クリエイティブチームに割り当てます。
* プロジェクトから「アセットの印刷」生産タスクを削除します。
* このプロジェクト内で、未完了で4月1日から4月30日の間に開始される予定のすべてのタスクを表示します。
* 「キャンペーン起動」タスクの先行タスクとして「法的承認」を設定します。
* 4月15日から4月16日にスケジュールされた「最終コピーポリッシュ」という新しいタスクを追加し、「コピーレビュータスク」を4月10日に移動し、「追加レビューラウンド」タスクを削除して、「最終コピーポリッシュ」をメールビルドの先行タスクとして設定します。
* プロジェクト作成フローでは、プロジェクトでタスクとすべき成果物について、できるだけ多くの情報を提供するようにします。

#### 割り当ての作成、更新、削除

ユーザーまたは担当業務の割り当てを作成、更新、削除できます。

* プロジェクト「製品起動用ランディングページの設計」で、現在割り当てられていないすべてのタスクに対して、適切な担当業務と推奨される予定時間を特定します。
* 「キャンペーンサイトのGA4 トラッキングの実装」、「コンバージョンイベントの設定」、「分析データの検証」など、いくつかの未割り当てのタスクがあります。 各業務の適切な担当業務と見積もられた時間を提案できますか？
* クリエイティブ作業「EMEA ディスプレイ広告用に3つのバナーバリエーションを作成」、「修正を適用」、「最終アセットを書き出し」の場合、最適な担当業務を割り当て、各タスクに必要な労力を見積もります。
* 「第2四半期製品発売」、「Web サイトのリデザイン - EMEA」、「有料メディアキャンペーン - NA」のプロジェクト全体で、割り当てられていないすべてのタスクを特定し、各タスクに推奨される予定時間を含む適切な担当業務を割り当てます。

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### コンテンツと承認

CX Coworkerは、Workfrontでドキュメントとアセットの承認を管理するのに役立ちます。

ドキュメントとアセットの承認を操作する際には、次の点を考慮してください。

* Coworkerでこの機能を使用するには、組織でコンテンツ承認を有効にする必要があります。
* AIは人間を代理して承認や却下を行うことはできません。 Workfront AI Reviewerを除く、意思決定は利用者に依存します。

  Workfront AI レビュアーについて詳しくは、[Workfront AI レビュアーの基本を学ぶ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)を参照してください。
* この機能はWorkfront内に存在し、外部のツールやドキュメントプロバイダーとのやり取りに使用することはできません。
* 最適なエクスペリエンスを得るには、この機能を統合承認エクスペリエンスで使用します。

  統合承認について詳しくは、[統合承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)を参照してください。

次の領域のドキュメントとアセットの承認のサンプルプロンプトを参照してください。

* [承認参加者の追加または削除](#add-or-remove-approval-participants)
* [レビュー待ちの単一アセットを関係者に通知](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [単一のアセットに対する承認テンプレートの追加、更新、適用](#add-update-or-apply-approval-templates-for-a-single-asset)

#### 承認参加者の追加または削除

* Sarah ChenとMiguel Alvarezを現在のドキュメントの承認者として追加します。
* この承認からJennifer Ottoを削除します。
* 承認の決定を行っていないユーザーを削除します。
* spring-campaign.pdfに「最終レビュー」という新しいステージを追加します。
* winter-campaign.pdfの第2段階で、MarkとSarahを承認者として、Philをレビュアーとして追加します
* winter-campaign.pdfの場合、最初のステージには今日の午後5時に期限を設定し、最終レビューには明日の午後5時に期限を設定します
* 木曜日の午後5時に期限を設定し、JimとPamを承認者、Oscarをレビュアーとして含めて、fall-campaign.pngに最終チェックステージを追加します
* レビュー担当者としてfall-campaign.pngにMark Jonesを追加します。
* fall-campaign.png用に、3つのステージ、1つのデザイン 2つのコピーライティング、3つの法務ステージで多段階の承認を作成してみましょう。 各段階で必要な決定はひとつだけです。 Mike、Sally、Janeをデザインに、Chris、Richard、Markをコピーライティングに、Phil、Tom、SarahをLegalに追加しましょう。

#### レビュー待ちの単一アセットを関係者に通知

* アセット「Spring Campaign Video」の承認者に、返信していないリマインダーを送信します。
* このアセット「Spring Campaign Video」を承認していない人に通知します。
* 「ブランドガイドラインPDF」に関して、まだ決めていない方はいますか？ リマインダーを送る：

#### 単一のアセットに対する承認テンプレートの追加、更新、適用

* 「Marketing Launch」の承認テンプレートを、「Spring Campaign Video」という名前のアセットに適用します。
* Creativeのレビュー、法務、最終承認の3つのステージを使用して、新しい承認テンプレートを作成します。
* ジュリア・サントスとシェーン・ベイカーをステージ 1に追加。
* 「Product Launch」テンプレートを編集して、Elizabeth Petersonを最終承認ステージに追加します。
* 「Urgent Review」というテンプレートを1つのステージで作成し、Olivia Kimに割り当てます。
* Rick Kuvecを削除し、Karen Sterlingをステージ 2に追加して、「Creative Review」テンプレートを更新します。


## WORKFRONT PlanningのCX担当者

### プランニングレコードの操作

* [レコードの作成、削除、複製、復元](#create-delete-duplicate-or-restore-records)
* [レコードを他のレコードにリンク](#link-records-to-other-records)
* [レコードへのフィールドの編集、更新、または追加](#edit-update-or-append-a-field-to-a-record)
* [アクセス レコードの変更履歴](#access-record-change-history)

#### レコードの作成、削除、複製、復元

* 「Summer Sale 2026」という新しいキャンペーンレコードを作成します
* Widget Proという名前の新しい製品レコードを追加し、価格$299
* John Smith氏のリードレコードを作成できます？
* Old Promoという名前のキャンペーンレコードを削除します
* 作成したテストレコードを削除する
* レコード ID Rc123abc456を削除できますか？
* Q1 キャンペーンレコードの複製
* このキャンペーンをコピーして新しいキャンペーンを作成できますか？
* ホリデープロモーションキャンペーンのコピーを作成
* 誤って削除したキャンペーンを復元する
* 削除したプロジェクトレコードを復元できますか？
* 誤ってレコードを削除した場合、復元できますか？

#### レコードを他のレコードにリンク

* サマーキャンペーンのレコードをQ2 イニシアチブにリンクする
* この製品を関連するマーケティング施策に結び付けられますか？
* この3つのリードをエンタープライズアカウントのレコードに関連付ける必要があります

#### レコードへのフィールドの編集、更新、または追加

* 夏季キャンペーンの予算フィールドを$75,000に更新します
* このプロジェクト レコードのステータスを「完了」に変更できますか？
* John Doeをこのイニシアチブの「チームメンバー」フィールドに追加します

#### アクセス レコードの変更履歴

* サマーキャンペーンのレコードの変更履歴を表示
* 誰がこのプロジェクトを変更し、何を変更したかを表示できますか？
* 先週このレコードでおこなわれたすべての更新を確認する必要があります

### Workfront計画でのSystem Designerの使用

* [ワークスペースの作成と設定](#create-and-configure-workspaces)
* [レコードタイプの定義](#define-record-types)
* [フィールドと数式フィールドのデザイン](#design-fields-and-formula-fields)
* [カスタムビューの構築](#build-custom-views)


#### ワークスペースの作成と設定

* 「Marketing Campaigns 2026」という新しいプランニングワークスペースを作成します
* 製品計画ワークスペースを更新して、カラーを青に変更し、説明を追加します
* 自分がアクセスできるすべてのプランニング ワークスペースを表示する

#### レコードタイプの定義

* プランニングワークスペースで「キャンペーン」という新しいレコードタイプを作成します
* イニシアチブのレコードタイプを更新して、そのアイコンと説明を変更します
* マーケティングプランニングワークスペースのすべてのレコードタイプを表示する

#### フィールドと数式フィールドのデザイン

* 予算フィールドを、通貨タイプを持つプランニングキャンペーンのレコードタイプに追加します
* キャンペーン終了日までの残り日数を計算する数式フィールドをPlanningに作成します
* プランニングワークスペースの「優先度」フィールドを更新して、さらにドロップダウンオプションを追加します

#### カスタムビューの構築

* プランニングでタイムラインビューを作成し、開始日と終了日でキャンペーンスケジュールを確認する
* アクティブなステータスのみをフィルタリングする新しいテーブルビューをプランニングイニシアチブに追加
* プランニングのアクティブなキャンペーン表示を複製し、並べ替えを変更します。
