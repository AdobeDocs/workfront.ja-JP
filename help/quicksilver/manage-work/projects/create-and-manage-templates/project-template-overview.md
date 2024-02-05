---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートの概要
description: プロジェクトテンプレートを使用すると、組織のプロジェクトに関連する繰り返し可能なプロセス、情報および設定のほとんどを取り込むことができます。
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 100%

---

# プロジェクトテンプレートの概要

<!-- Audited: 12/2023 -->

プロジェクトテンプレートを使用すると、組織のプロジェクトに関連する繰り返し可能なプロセス、情報および設定のほとんどを取り込むことができます。

タスク、キュートピック、カスタムフォームを定義し、テンプレートにドキュメントを添付することができます。

テンプレートを作成した後、既存のプロジェクトに添付したり、新しいプロジェクトの作成に使用したりできます。テンプレートのすべての情報は、それを使用して作成されたプロジェクトに転送されます。

## Adobe Workfront でテンプレートを使用するメリット

次に、プロジェクトを作成する際にテンプレートを使用するメリットを示します。

* これにより、繰り返し作業を行う新しいプロジェクトを作成する際の時間と労力を節約できます。
* プロジェクト全体で一貫した情報を持ち、その範囲は似ています。
* プロジェクトのレポートを作成する場合に役立ちます。例えば、同じテンプレートを共有するプロジェクトについてレポートを作成し、その進行状況を比較して、完成させる方法の改善点を見つけることができます。
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

* テンプレートタスクにユーザーを割り当てないでください。 タスクの割り当てを解除したままにすることもできますが、タスクに担当業務を割り当てることをお勧めします。これにより、テンプレートを使用してプロジェクトを作成する際に、タスクに割り当てられるユーザーがわかります。
* テンプレートタスクには必ず「期間」と「予定時間数」の値を指定してください。プロジェクト内のすべてのタスクは、タスクを開いたままにできる期間と、タスクが完了するまでに実際にかかる時間の計画時間の値を関連付ける必要があります。Workfront でリソース管理ツールを使用する場合、この情報を持たないタスクはリソースに対して適切に予算を設定できません。

  期間について詳しくは、次の記事を参照してください。

   * [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [プロジェクト期間の概要](../../../manage-work/projects/planning-a-project/project-duration.md)

  予定時間数について詳しくは、[予定時間数の概要](../../../manage-work/tasks/task-information/planned-hours.md)を参照してください。

* 将来のプロジェクト計画全体を明確に理解している場合は、最後にタスク間の先行タスク関係を追加します。テンプレートタスクに先行タスクを追加する操作は、プロジェクト上のタスクに先行タスクを追加する操作と似ています。

  タスクに先行タスクを追加する方法については、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

* 今後の使用のためにテンプレートを共有する相手と、テンプレートから作成されるプロジェクトを共有する相手を指定します。テンプレートの共有については、[プロジェクトテンプレートの共有](../../../manage-work/projects/create-and-manage-templates/share-project-template.md)を参照してください。
* 可能な場合は、グローバルな承認プロセスを使用し、テンプレートおよびテンプレートタスクに追加します。これにより、タスクや将来のプロジェクトが同じ承認を実行する必要が生じる時間を節約できます。

  承認の作成については、[作業アイテムの承認プロセスを作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)を参照してください。

  承認プロセスと作業アイテムの関連付けの手順については、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。

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
