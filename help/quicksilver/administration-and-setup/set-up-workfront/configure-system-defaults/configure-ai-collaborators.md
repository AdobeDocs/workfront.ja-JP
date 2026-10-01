---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: AI共同作業者の設定
description: Adobe Workfront管理者は、AI共同作業者を設定し、プロジェクトやタスクに割り当てることができます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3cf7495f827156fabac1214b38a104ed826d558c
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 2%
---
# AI共同作業者の設定

{{preview-fast-release-general}}

AI協力者とは、AI エージェントをプロジェクト、タスク、イシューに組み込む方法のひとつです。 AI共同作業者を設定し、ユーザーと同じように割り当てることができます。

例えば、ブランドガイドラインを使用してレビューアータイプのAI コラボレーターを設定し、そのコラボレーターにドキュメントのレビューを割り当てることができます。

利用可能なAI共同作業者タイプは次のとおりです。

* AI レビュアー：ブランドまたはAdobe Brand Intelligenceを使用して共同作業者を作成し、その共同作業者をアセットのレビュアーとして割り当てます。

  詳しくは、[Workfront AI レビュアーの基本を学ぶ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)を参照してください。

* 作業エージェント：Claude、OpenAI、Copilot、Writerなどの標準AI プラットフォームを使用して共同作業者を作成し、その共同作業者をタスクや問題に割り当てて作業項目を完了させます。

  詳しくは、[作業担当者の使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>Select、Prime、またはUltimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL システム管理者] <span class="preview">またはグループ管理者</span></td> 
  </tr> 
  </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* [AI レビュー担当者向け](#for-ai-reviewers)
* [作業担当者の場合](#for-work-agents)

### AI レビュー担当者の場合：

* 署名済みのAdobe Gen AI契約書がファイルに登録されている必要があります。

  詳しくは、「[Adobe生成AI契約書に署名する](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)」を参照してください。WorkfrontのAI アシスタントの記事を参照してください。
* AI レビュアーに使用するには、Workfrontでブランドを設定しておく必要があります。

  手順については、[AI レビュアーのブランドの作成と管理](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)を参照してください。
* AI レビュアーにAdobe Brand Intelligenceを使用するには、Workfrontの統一されたレビューと承認のエクスペリエンスを使用する必要があります。

  詳しくは、[統合レビューと承認の概要](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)を参照してください。

### 作業担当者の場合

作業用エージェントとして使用する前に、Claude、Copilot Studio、Writer、OpenAI、またはIBMでエージェントを設定する必要があります。

>[!NOTE]
>
>アドビは、あらゆるエージェントプロバイダーへの接続を目指しています。そのため、お使いのプロバイダーが現在Work Agentsと互換性がない場合は、アカウントチームにお問い合わせください。

## 新しいAI レビュアーの作成

AI レビュー担当者は、Workfrontブランド、つまりAdobe Brand Intelligenceを使用するように設定できます。

* **ブランド**：ブランドはWorkfrontで作成されます。 Workfrontでブランドを作成するには、ブランドガイドラインを含むPDF ファイルをアップロードするか、ブランド要素を手動で入力します。
* **Adobe Brand Intelligence**: AIの共同作業者がAdobe Brand Intelligenceを使用してアセットをレビューすると、Frame.ioでAIのレビュー担当者が行ったコメントを表示できます。


{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. 画面の右上隅にある「**新しい共同作業者**」をクリックします。
1. **Reviewer**&#x200B;をクリックしてから、**Continue**&#x200B;をクリックします。
1. 「共同作業者の名前」フィールドに、共同作業者の名前を入力します。 これは、タスクで使用可能な担当者のリストに表示される名前です。
1. 共同作業者がブランドを使用するか、レビューにAdobe Brand Intelligenceを使用するかを選択します。
1. （条件付き） AI共同作業者がブランドを使用する場合は、使用するブランドとブランドガイドラインを選択します。
1. 「**保存**」をクリックします。

## 作業エージェントの設定

作業エージェントは、Workfrontでタスクまたはイシューに割り当てることができるエージェントです。 名前、アクセスレベルおよびその他の詳細を使用して作業エージェントを設定し、ユーザーを割り当てるようにタスクに割り当てます。

作業用エージェントはエージェントであるため、そのアクションと機能は、エージェントを設定する場所で設定されます。 現在、作業用エージェントとして使用されるエージェントは、Copilot Studio、Claude、またはWriter、OpenAI、およびIBMで作成できます。

作業担当者は、タスクまたはイシューに割り当てることができます。

作業エージェントとして機能するエージェントを作成する際のベストプラクティスの一覧については、[作業エージェントのエージェント作成に関するベストプラクティス ](#best-practices-for-creating-an-agent-for-a-work-agent)を参照してください。

* [Workfrontでの作業エージェントの設定](#configure-a-work-agent-in-workfront)
* [作業エージェント用のエージェントを作成するためのベストプラクティス](#best-practices-for-creating-an-agent-for-a-work-agent)

### Workfrontでの作業エージェントの設定

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. 画面の右上隅にある「**新しい共同作業者**」をクリックします。
1. **作業エージェント**&#x200B;を選択し、**続行**&#x200B;をクリックします。
1. 「AI共同作業者の名前」フィールドに、共同作業者の名前を入力します。 これは、タスクで使用可能な担当者のリストに表示される名前です。
1. 「AI共同作業者の説明」フィールドに、共同作業者の目的または実行するアクションの説明を入力します。
1. 「アクセスレベル」フィールドで、この共同作業者のアクセスレベルを選択します。 このアクセスレベルは、共同作業者の機能を制御し、アクセスレベルはユーザーの機能を制御するのと同じように制御します。
1. （オプション）グループ フィールドで、作業エージェントが関連付けるグループを選択します。

   >[!NOTE]
   >
   ><span class="preview"> グループ管理者の場合、このフィールドには管理者であるグループのみが表示されます。 グループ管理者は、少なくとも1つのグループを選択する必要があります。</span>

1. **エージェントのオリジンを選択**&#x200B;領域で、CopilotやWriterなどの共通プラットフォームで作成されたエージェントを接続するか、カスタムエージェントを使用するかを選択します。
1. （条件付き）共通プラットフォームのエージェントを使用している場合は、エージェントのプラットフォームの認証の詳細を入力します。

   | Platform | 必須の認証 |
   |---|---|
   | Copilot Studio | Web チャネルシークレット |
   | Claude Managed Agents | Anthropic API キー<br> エージェント ID<br>環境ID |
   | Writer エージェント | API キー<br> アプリケーション ID |
   | <span class="preview">OpenAI Agents</span> | <span class="preview">API キー<br> エージェント ID</span> |
   | <span class="preview">IBM watsonx Orchestrate</span> | <span class="preview"> サービス URL<br>API キー<br> エージェント ID</span> |

1. 「**接続をテスト**」をクリックします。 これにより、接続が正しくセットアップされたかどうかを確認できます。
1. **共同作業者が作業を完了した後、共同作業者が実行するアクションを切り替える**&#x200B;領域を選択できます。

   * <span class="preview">通知を送信：エージェントは、更新ストリームにコメントを作成し、作業を要求したユーザー、エージェントを割り当てたユーザー、またはプロジェクトを所有するユーザーをタグ付けします。</span>
   * <span class="preview"> ドキュメントをアップロード </span>
   * <span class="preview"> タスク完了をマーク </span>
   * タスクフィールドの書き込み：エージェントが書き込むことができるフォームとフィールドを選択します。

1. 「**保存**」をクリックします。

タスクへの割り当て方法など、作業エージェントの詳細については、[作業エージェントの使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。

### 作業エージェント用のエージェントを作成するためのベストプラクティス

Workfrontで作業エージェントとして使用するエージェントを作成する際には、次のベストプラクティスが役立つ場合があります。 ベストプラクティスを確認するには、エージェントを作成するアプリケーションのセクションをクリックします。

+++ クロード

1. [platform.claude.com](https://platform.claude.com/)にあるClaude Consoleに移動します。
1. API キーを作成します。
   1. API キーの下で、右上隅の「**キーを作成**」をクリックします。
   1. 名前と有効期限を入力します。
   1. キーをコピーして、安全で安全な場所に保存します。 WorkfrontでWork Agentを設定するには、このキーが必要です。

1. 環境を作成します。
   1. **Managed Agents** > **Environments**&#x200B;の下で、右上隅の&#x200B;**Create Environment**&#x200B;をクリックします。
   1. 必要に応じて、名前とホスティングタイプを指定します。
   1. 必要に応じて、共有パッケージとメタデータを設定します。 環境は複数のエージェントで再利用でき、パッケージとメタデータを共有できます。
      環境IDは、環境名の左上隅に表示されます。

1. エージェントを作成します。
   1. Managed Agents/Agentsで、右上隅の&#x200B;**Create Agent**&#x200B;をクリックします。
   1. 必要に応じて、名前、モデル、システムプロンプト、スキル、ツールを提供します。 作業用エージェントはタスクのコンテキストをこのエージェントに渡し、その後は作業を実行するので、説明が必要です。
      エージェント IDは、左上隅のエージェント名の下に表示されます。

1. WorkfrontでWork Agentを設定します。
   1. API キー、環境ID、エージェント IDを入力します
   1. 「**接続をテスト**」をクリックして確認します。

1. Work AgentをWorkfront タスクに割り当てます。
   1. すべての先行タスクが完了すると、作業エージェントが起動します。

+++
<!--
+++ Copilot Studio



+++
-->
+++ ライター

>[!NOTE]
>
> Writer エージェントをWork エージェントとして使用できますが、Writer プレイブックをWork エージェントとして使用することはできません。

Writerで作業エージェントとして使用するエージェントを作成する場合は、次のワークフローをお勧めします。

エージェントの作成について詳しくは、[ ライターのドキュメント ](https://dev.writer.com/no-code/introduction)を参照してください。

1. Writer AI Studioでノーコードアプリを作成します。
1. 1つのテキスト入力フィールドを追加します。 デフォルト名「テキスト入力」を使用できます。
1. プロンプトに`@TextInput`を追加します。 アプリ設定の「プロンプト」セクションで、プロンプトテンプレートが入力変数を参照していることを確認します。 これが欠ければ、モデルはタスクデータを見ることはできません。
1. プロンプトを調整して、すぐに出力を生成します。 回答する前に、ユーザーに説明や追加のコンテキストを求める指示を削除します。 例：「入力を受け取ったら、コンテンツ生成リクエストとして扱い、出力を即座に生成します。 明確化を求めるな」
1. API キーとアプリケーション IDをコピーします。 WorkfrontでWork Agentを設定する必要があります。

   * WriterでAPI キーを設定する方法については、Writer ドキュメントの[Quickstart](https://dev.writer.com/home/quickstart)を参照してください。
   * Writerでアプリケーション IDを設定する方法については、Writer ドキュメントの「[API](https://dev.writer.com/home/applications)を介してノーコードエージェントを呼び出す」を参照してください。

1. WorkfrontでWork Agentを設定します。 設定の一部として、API キーとアプリケーション IDを入力し、**接続をテスト**&#x200B;をクリックして確認します。
1. Work AgentをWorkfront タスクに割り当てます。 作業エージェントは、タスクの先行タスクがすべて完了すると作業を開始します。

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## AI共同作業者の管理

既存のAI共同作業者を編集、コピー、削除できます。

>[!NOTE]
>
><span class="preview"> グループ管理者は、自分が管理者であるグループに関連付けられているAI共同作業者のみを表示し、操作できます。 特定のAI Collaboratorに他のグループも関連付けられている場合、グループ管理者はそれを表示できますが、編集することはできません。</span>

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. （条件付き）共同作業者を編集するには、編集する共同作業者の名前をクリックし、「共同作業者を編集」ウィンドウで編集を行い、**保存**&#x200B;をクリックします。
1. （条件付き）共同作業者を削除するには、削除するAI共同作業者の行にある削除アイコン ![削除アイコン ](assets/delete-collaborator-icon.png)をクリックし、**削除**&#x200B;をクリックします。
