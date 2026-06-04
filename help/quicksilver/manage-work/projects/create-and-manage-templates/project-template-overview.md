---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートの概要
description: プロジェクトテンプレートを使用すると、組織のプロジェクトに関連する繰り返し可能なプロセス、情報および設定のほとんどを取り込むことができます。
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
TQID: https://experienceleague.adobe.com/9RlRNqkZYIcLjI5-he3f2BMtoXj3R--8MQbVUFmRHqI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 702
ht-degree: 85%

---

# プロジェクトテンプレートの概要

<!-- Audited: 12/2023 -->

プロジェクトテンプレートを使用すると、組織のプロジェクトに関連する繰り返し可能なプロセス、情報および設定のほとんどを取り込むことができます。

タスク、キュートピック、カスタムフォームを定義し、テンプレートにドキュメントを添付することができます。

テンプレートを作成した後、既存のプロジェクトに添付したり、新しいプロジェクトの作成に使用したりできます。 テンプレートのすべての情報は、それを使用して作成されたプロジェクトに転送されます。

## Adobe Workfront でテンプレートを使用するメリット

次に、プロジェクトを作成する際にテンプレートを使用するメリットを示します。

* これにより、繰り返し作業を行う新しいプロジェクトを作成する際の時間と労力を節約できます。
* プロジェクト全体で一貫した情報を持ち、その範囲は似ています。
* プロジェクトのレポートを作成する場合に役立ちます。 例えば、同じテンプレートを共有するプロジェクトについてレポートを作成し、その進行状況を比較して、完成させる方法の改善点を見つけることができます。
* 今後のプロジェクト設定を定義する以外に、テンプレートに今後のプロジェクトに関する次の情報を追加できます。

   * タスク
   * ドキュメント
   * 承認
   * キューの詳細
   * キューのトピック
   * トピックグループ
   * ルーティングルール
   * カスタムフォーム
   * 会社およびグループ情報

## テンプレート作成のベストプラクティス

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

テンプレートを作成する際は、次の点に注意してください。

* テンプレートタスクにユーザーを割り当てない。 タスクは未割り当てのままにできますが、タスクに担当業務を割り当てることをお勧めします。 これにより、テンプレートを使用してプロジェクトを作成する際に、タスクに割り当てられるユーザーがわかります。
* テンプレートタスクには必ず「期間」と「予定時間数」の値を指定してください。 プロジェクト内のすべてのタスクは、タスクを開いたままにできる期間と、タスクが完了するまでに実際にかかる時間の計画時間の値を関連付ける必要があります。 Workfront でリソース管理ツールを使用する場合、この情報を持たないタスクはリソースに対して適切に予算を設定できません。

  期間について詳しくは、次の記事を参照してください。

   * [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [プロジェクト期間の概要](../../../manage-work/projects/planning-a-project/project-duration.md)

  予定時間数について詳しくは、[予定時間数の概要](../../../manage-work/tasks/task-information/planned-hours.md)を参照してください。

* 将来のプロジェクト計画全体を明確に理解している場合は、最後にタスク間の先行タスク関係を追加します。 テンプレートタスクに先行タスクを追加する操作は、プロジェクト上のタスクに先行タスクを追加する操作と似ています。

  タスクに先行タスクを追加する方法については、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

* 今後の使用のためにテンプレートを共有する相手と、テンプレートから作成されるプロジェクトを共有する相手を指定します。 テンプレートの共有については、[プロジェクトテンプレートの共有](../../../manage-work/projects/create-and-manage-templates/share-project-template.md)を参照してください。
* 可能な場合は、グローバルな承認プロセスを使用し、テンプレートおよびテンプレートタスクに追加します。 これにより、タスクや将来のプロジェクトが同じ承認を実行する必要が生じる時間を節約できます。

  承認の作成については、[作業アイテムの承認プロセスを作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)を参照してください。

  承認プロセスと作業アイテムの関連付けの手順については、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。

* 今後のプロジェクトに使用するドキュメントストレージを決めます。 一部の組織では、次のドキュメントストレージタイプにアクセスできます。

   * 従来のWorkfront ストレージ
   * Adobe クラウドストレージ

  ドキュメントの追加は、選択するストレージの種類によって異なります。 テンプレートに対して選択するストレージのタイプは、今後のプロジェクトが継承するストレージのタイプに影響します。

  既存のプロジェクトにテンプレートを追加しても、プロジェクトのストレージタイプには影響しません。

  詳細については、次も参照してください。

   * [プロジェクトテンプレートの作成](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)
   * [プロジェクトと関連オブジェクトのドキュメント管理の概要](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)

## テンプレートの作成方法

次の方法で新しいテンプレートを作成できます。

* 最初から。\
  新しいテンプレートを最初から作成する方法について詳しくは、[プロジェクトテンプレートの作成](../../../manage-work/projects/create-and-manage-templates/create-template.md)を参照してください。

* 既存のプロジェクトから、プロジェクトをテンプレートとして保存。\
  既存のプロジェクトからテンプレートを作成する方法について詳しくは、[プロジェクトからのテンプレート作成](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md)を参照してください。

* 別のテンプレートからコピー。\
  既存のテンプレートのコピーについて詳しくは、[プロジェクトテンプレートをコピー](../../../manage-work/projects/create-and-manage-templates/copy-template.md)を参照してください。

* この例のテンプレートを使用する。\
  サンプルテンプレートを使用したテンプレートの作成について詳しくは、[例からのプロジェクトテンプレートの作成](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md)を参照してください。
