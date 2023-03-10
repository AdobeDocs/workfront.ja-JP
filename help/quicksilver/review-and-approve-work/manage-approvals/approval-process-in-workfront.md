---
content-type: overview
product-area: projects
navigation-topic: approvals
title: 承認プロセスの概要
description: 承認プロセスを作成してオブジェクトに添付すると、指定したユーザーがオブジェクトの進行前に特定の変更を確実に確認できます。
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# 承認プロセスの概要

承認プロセスを作成してオブジェクトに添付すると、指定したユーザーがオブジェクトの進行前に特定の変更を確実に確認できます。

これは、Adobe Workfrontの次のタイプのオブジェクトで使用できます。

* 作業項目（プロジェクト、タスクまたはタスク、テンプレート、テンプレートタスク）
* ドキュメント
*  Proof

承認プロセスの作成手順については、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

この記事では、作業項目に関連する承認プロセスに関する一般的な情報を説明します。

## 承認プロセスのタイプ

Adobe Workfront管理者、または承認プロセスへの管理者アクセス権を持つユーザーは、プロジェクト、タスクおよび問題に対して次の承認プロセスを作成できます。

* **システムレベルのグローバル承認プロセス**:ユーザーは、これらを次のいずれかに添付できます。

   * 「承認」セクションのプロジェクト、タスクまたはイシュー
   * 「プロジェクトを編集」ボックスの「タスクのデフォルトの承認プロセス」領域
   * プロジェクトの「Queue Details」または「Queue Topic」セクションの「Default Approval Process」領域で、 プロジェクトは、リクエストキューとして有効にする必要があります。

* **グループレベルのグローバル承認プロセス**:ユーザーは、これらを次の項目に添付できます。

   * 「承認」セクションの承認プロセスに関連付けられた、グループに属するプロジェクト、タスクまたは問題
   * 「プロジェクトを編集」ボックスの「タスクのデフォルトの承認プロセス」領域で、承認プロセスに関連付けられたグループに属するプロジェクトを編集します
   * プロジェクトの「Queue Details」または「Queue Topic」セクションの「Default Approval Process」領域で、 プロジェクトは、リクエストキューとして有効にし、承認プロセスに関連付けられたグループに属している必要があります。

   システムレベルまたはグループレベルの承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **単一使用の承認プロセス**:単一のプロジェクト、タスク、タスク、イシュー、テンプレート、またはテンプレートタスクで使用します。 このタイプの承認プロセスは、関連付けられているオブジェクトにのみ影響し、他のオブジェクトに関連付けることはできません。

   単一使用の承認プロセスの作成について詳しくは、 [新規または既存の承認プロセスと作業の関連付け](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>この記事では、「グローバルな承認プロセス」という用語を使用して、「単一使用の承認プロセス」と区別します。 グローバルな承認プロセスは繰り返し使用できます。
>
>「グループレベルのグローバル承認プロセス」とは、特定のグループにのみ関連付けられたステータスを持つ品目に対して繰り返し使用できる承認プロセスを指します。

システムレベルの承認プロセスまたはグループレベルの承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 承認プロセスに関する考慮事項

* 承認プロセスを関連付ける前に、プロジェクト、タスク、タスク、イシュー、テンプレートまたはテンプレートタスクを作成する必要があります。
* 承認プロセスは、常に次の 2 つの重要な要素に関連付けられます。

   * 各承認プロセスは、Workfrontシステムの特定の作業項目ステータスに対応します。 作業項目のステータスを変更する場合、そのステータスに添付された承認を行うには、新しいステータスをその項目に割り当てる前に、そのステータスの変更を確認する必要があります。

      >[!TIP]
      >
      >
      >   
      >   
      >   * グループレベルの承認をグローバルステータスまたはグループレベルのステータスに関連付けることができます。
      >   * 承認プロセスを使用してアイテムのステータスを、承認プロセスに関連付けられたステータス以外のステータスに変更することはできません。

         >   
         >   
         >     例えば、「処理中」のステータスにタスクの承認が関連付けられている場合、承認が許可されると、タスクのステータスは自動的に「処理中」に変わります。 ステータスを「完了」に自動的に変更したり、承認に関連付けられていない他のステータスに自動的に変更することはできません。


   * 承認プロセスに関連付けられるエンティティは、ユーザー、ジョブの役割、チームのいずれかです。 ユーザーは、最終的に承認を許可または却下する責任を負います。 プロジェクトで特定の役割を果たすユーザーに承認を割り当てることができます。 例えば、プロジェクト所有者やスポンサーに承認を割り当てることができます。 詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      次のシナリオが存在します。

      * ジョブの役割に承認を割り当てると、ジョブの役割に関連付けられているプロジェクトチームのユーザーは、承認を決定できます。 承認に関連付けられる役割は、「プライマリの役割」または「その他の役割」のどちらかです。

         プロジェクトチームの詳細については、 [プロジェクトチームの概要](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * チームに承認を割り当てると、そのチームの任意のメンバーが承認を決定できます。 承認に関連付けられたチームは、ホームチームまたはその他のチームのどちらでもかまいません。

         ユーザーの役割とチームについて詳しくは、 [ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 作業項目を作成すると、自動的に承認プロセスが添付されません。 使用する場合は、手動で添付する必要があります。 アイテムへの承認プロセスの添付について詳しくは、 [新規または既存の承認プロセスと作業の関連付け](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Workfront管理者または承認プロセスへの管理者アクセス権を持つユーザーは、システム全体で使用する、システムレベルのグローバル承認プロセスを作成できます。 承認プロセスへの管理者アクセス権を持つグループ管理者は、管理対象の特定のグループに対してのみ使用する、グループレベルのグローバル承認プロセスを作成できます。
* 定義済みのシステムレベルまたはグループレベルのグローバル承認プロセスを作業項目に使用したくない場合、承認プロセスを添付するオブジェクトに対する管理権限を持つ場合は、単一使用の承認プロセスを作成して添付できます。

   >[!NOTE]
   単一使用の承認プロセスは、そのプロセスが作成された特定の品目に対して 1 回だけ使用できます。 グローバルステータスと、プロジェクト、タスク、タスク、テンプレートおよびテンプレートタスクに対する単一使用の承認プロセスに対するグループレベルのステータスを関連付けることができます。

* グループレベルのカスタムステータスを使用してグループレベルの承認プロセスを項目に添付する場合、プロジェクトのグループを変更すると、前のグループの承認ステータスとシステムレベルの承認ステータスの間に競合が生じる可能性があります。 グループを更新する前に、プロジェクト上のグループレベルの承認プロセス、またはそのタスクや問題を削除することを検討してください。 グループレベルの承認プロセスの作成について詳しくは、 [グループレベルの承認プロセス](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). カスタムグループステータスの作成について詳しくは、 [グループのステータスの作成または編集](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). プロジェクトのグループを更新する方法については、 [プロジェクトを編集](../../manage-work/projects/manage-projects/edit-projects.md).

## 承認プロセスのワークフロー

この節では、作業項目の承認に関する以下の事項について説明します。

* [承認プロセスがステータスに依存する方法](#how-approval-processes-rely-on-statuses)
* [一般的なワークフローでの承認プロセスの使用方法](#how-a-typical-workflow-uses-an-approval-process)

### 承認プロセスがステータスに依存する方法 {#how-approval-processes-rely-on-statuses}

承認プロセスにステータスを添付すると、アイテムが適切な順序で部門を移動します。

**例：** 財務部門の承認を必要とするマーケティング部門のステータスに承認プロセスを添付できます。 その後、誰かが作業項目のステータスを「マーケティング部門」に変更すると、財務部門がサインオフするまで、その項目はその部門に移動できません。

作業項目のステータスの詳細については、次の記事を参照してください。

* [システムプロジェクトステータスのリストへのアクセス](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [システムタスクステータスのリストへのアクセス](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [システムの問題ステータスのリストへのアクセス](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### 一般的なワークフローでの承認プロセスの使用方法 {#how-a-typical-workflow-uses-an-approval-process}

次のシナリオでは、承認プロセスを使用して、Workfrontオブジェクトがこの順序の複数の手順で進むにつれて、作業を承認する方法を示します。

1. Workfront管理者または承認プロセスへの管理者アクセス権を持つユーザーが、プロジェクト、タスクまたはイシューの承認プロセスを作成します。

   >[!NOTE]
   テンプレートにプロジェクト承認プロセスを添付し、テンプレートタスクにタスク承認プロセスを添付できます。 この操作を行うと、誰かがテンプレートを使用してプロジェクトを作成すると、承認プロセスがそれぞれプロジェクトまたはタスクの承認プロセスになります。 テンプレートタスクまたはテンプレートタスクに添付された単一使用の承認プロセスは、プロジェクトやタスクに対する単一使用の承認プロセスのままです。

1. プロジェクト、タスクまたはイシューの管理権限を持つユーザーは、承認プロセスをアイテムに添付するか、アイテムに対して単一使用の承認を作成します。
1. 作業項目に割り当てられたユーザーのステータスが、承認プロセスを開始するステータスに変わり、承認プロセスが開始します。 （承認プロセスを作成した人物が、ステータスと承認プロセスの間の関係を定義しました）。
1. 指定された承認者は、承認待ちプロセスに関する通知を受け取り、作業項目を確認します。
1. 指定された承認者がプロセスのすべてのステップを承認すると、承認プロセスは終了します。 また、ステップを拒否した場合は、ステータスが事前定義済みのステータスにリセットされるか、問題が作成されます。 （却下の後に自動ステップのどれが発生するかを定義した承認プロセスを作成した人）

**例：** 広告チームが「印刷準備完了」というステータスと、このステータスに関連付けられた Designer/Copywriter Signoff という承認プロセスを作成しました。 この承認プロセスは次の目的で設定されます。

* チームのデザイナーとコピーライターの承認が必要
* 作業項目の状態を [ 印刷準備完了 ] に変更したときに開始します

パンフレットプロジェクトの所有者は、Designer/Copywriter のサインオフ承認プロセスをパンフレットプロジェクトに添付します。

プロジェクト上の誰かがステータスを [ 印刷準備完了 ] に変更すると、コピーライターとデザイナーは、承認または拒否を求める通知を受け取ります。 承認プロセス中に、承認するかどうかを検討する際に、プロジェクトのステータスが「印刷準備完了 — 承認待ち」と表示されます。

両方のユーザーがWorkfrontでパンフレットを承認すると、プロジェクトのステータスは「印刷準備完了」に変わります。

## ドキュメント承認プロセス

ドキュメントの承認は、より一般的な承認に使用されます。 フィードバックは、「更新」タブのチャット形式で取り込まれます。 承認ボタンを使用して、変更を加えた承認、却下または承認をおこなうことができます。

Workfrontにアップロードした後でドキュメントに承認者を追加するには、 [ドキュメント承認のリクエスト](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## 配達確認の承認プロセス

配達確認の承認は、より深いレビューに使用され、通常はより複雑なワークフローが含まれます。 フィードバックは、校正ビューアのマークアップツールでキャプチャされます。 承認ボタンを使用して、変更を加えた承認、却下または承認をおこなうことができます。

自動ワークフローをドキュメント配達確認に追加し、ワークフロー内の特定のユーザーを配達確認の承認者として指定するには、 [自動ワークフローを使用した高度な配達確認の作成](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 作業項目承認プロセスの設定を行う

Workfrontの管理者は、システムの作業項目承認プロセスのグローバル設定を行うことができます。 これらの設定は、承認プロセスの様々なルールを決定します。例えば、承認決定を開いたままにしておく必要がある期間や、システムで承認委任を管理する方法などです。 承認プロセスの設定について詳しくは、 [グローバル承認設定の指定](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
