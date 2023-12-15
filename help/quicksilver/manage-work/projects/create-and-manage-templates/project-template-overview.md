---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートの概要
description: プロジェクトテンプレートを使用すると、組織内のプロジェクトに関連する繰り返し可能なプロセス、情報、設定のほとんどをキャプチャできます。
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# プロジェクトテンプレートの概要

<!-- Audited: 12/2023 -->

プロジェクトテンプレートを使用すると、組織内のプロジェクトに関連する繰り返し可能なプロセス、情報、設定のほとんどをキャプチャできます。

タスク、キュートピック、カスタムフォームを定義し、テンプレートにドキュメントを添付することができます。

テンプレートを作成した後、既存のプロジェクトに添付したり、新しいプロジェクトの作成に使用したりできます。 テンプレートに関するすべての情報は、テンプレートを使用して作成されたプロジェクトに転送されます。

## Adobe Workfrontでテンプレートを使用するメリット

次に、プロジェクトを作成する際にテンプレートを使用するメリットを示します。

* これにより、繰り返し作業を行う新しいプロジェクトを作成する際の時間と労力を節約できます。
* プロジェクト全体で一貫した情報を持ち、その範囲は似ています。
* プロジェクトのレポートを作成する場合に役立ちます。 例えば、同じテンプレートを共有するプロジェクトについてレポートを作成し、その進行状況を比較して、改善点を見つけることができます。
* 今後のプロジェクト設定を定義する以外に、テンプレートに今後のプロジェクトに関する次の情報を追加できます。

   * タスク
   * ドキュメント
   * 承認
   * キューの詳細
   * キュー トピック
   * トピックグループ
   * ルーティング規則
   * カスタムForms
   * 会社およびグループ情報

## テンプレート作成のベストプラクティス

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

テンプレートを作成する際は、次の点に注意してください。

* テンプレートタスクにユーザーを割り当てないでください。 タスクの割り当てを解除したままにすることもできますが、タスクにジョブの役割を割り当てることをお勧めします。 これにより、テンプレートを使用してプロジェクトを作成する際に、タスクに割り当てられるユーザーがわかります。
* テンプレートタスクには必ず「期間」と「予定時間」の値を指定してください。 プロジェクト内のすべてのタスクは、タスクを開いたままにできる期間と、タスクが完了するまでに実際にかかる時間の計画時間の値を関連付ける必要があります。 Workfrontでリソース管理ツールを使用する場合、この情報を持たないタスクはリソースに対して適切に予算を設定できません。

  期間について詳しくは、次の記事を参照してください。

   * [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [プロジェクト期間の概要](../../../manage-work/projects/planning-a-project/project-duration.md)

  予定時間については、 [計画時間の概要](../../../manage-work/tasks/task-information/planned-hours.md).

* 将来のプロジェクト計画全体を明確に理解している場合は、最後にタスク間の先行タスク関係を追加します。 テンプレートタスクに先行タスクを追加する操作は、プロジェクト上のタスクに先行タスクを追加する操作と似ています。

  タスクに先行タスクを追加する方法については、「 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* 今後の使用のためにテンプレートを共有する相手と、テンプレートから作成されるプロジェクトを共有する相手を指定します。 テンプレートの共有について詳しくは、 [プロジェクトテンプレートの共有](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* 可能な場合は、グローバルな承認プロセスを使用し、テンプレートおよびテンプレートタスクに追加します。 これにより、タスクや将来のプロジェクトが同じ承認を実行する必要が生じる時間を節約できます。

  承認の作成について詳しくは、 [作業項目の承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  作業項目への承認プロセスの関連付けについて詳しくは、 [新規または既存の承認プロセスを作業に関連付ける](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## テンプレートの作成方法

新しいテンプレートは、次の方法で作成できます。

* ゼロから。\
  新しいテンプレートを最初から作成する方法について詳しくは、「 [プロジェクトテンプレートの作成](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* 既存のプロジェクトから、プロジェクトをテンプレートとして保存する。\
  既存のプロジェクトからテンプレートを作成する方法について詳しくは、 [プロジェクトからテンプレートを作成](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* 別のテンプレートからコピーする。\
  既存のテンプレートのコピーについて詳しくは、 [プロジェクトテンプレートのコピー](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* この例のテンプレートを使用する。\
  サンプルテンプレートを使用したテンプレートの作成について詳しくは、 [例からプロジェクトテンプレートを作成する](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
