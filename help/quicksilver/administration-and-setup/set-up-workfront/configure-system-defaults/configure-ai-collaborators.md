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
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '1993'
ht-degree: 3%
---
# AI共同作業者の設定

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。 すべての顧客のプレビュー環境でのみ使用できます。</span>

AI協力者とは、AI エージェントをプロジェクト、タスク、イシューに組み込む方法のひとつです。 AI共同作業者を設定し、ユーザーと同じように割り当てることができます。

例えば、ブランドガイドラインを使用してレビューアータイプのAI コラボレーターを設定し、そのコラボレーターにドキュメントのレビューを割り当てることができます。

利用可能なAI共同作業者タイプは次のとおりです。

* AI レビュアー：ブランドまたはAdobe Brand Intelligenceを使用して共同作業者を作成し、その共同作業者をアセットのレビュアーとして割り当てます。

  詳しくは、[Workfront AI レビュアーの基本を学ぶ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)を参照してください。

* 作業エージェント：Adobe CX Coworkerを活用した共同作業者<span class="preview">を作成するか、サポートされている外部プラットフォームから担当者を接続し、共同作業者をタスクまたは問題に割り当てて作業項目を完了します。</span>

  詳しくは、[作業担当者の使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。

  Adobe CX Enterprise Coworkerについて詳しくは、[WorkfrontでのCX Enterprise Coworkerの概要](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)を参照してください。

AI共同作業者が使用するライセンスには請求されません。 組織に200 Workfront ライセンスがあり、AI Collaboratorを作成している場合、201 ライセンスが使用されますが、請求されるのは200のみです。

* <span class="preview"> プロジェクトコーディネーター：外部エージェントを設定することなく、プロジェクトのステータスを監視し、プロジェクトの更新を送信する、すぐに使用できる共同作業者。</span>

  <span class="preview">詳細については、[ プロジェクト コーディネーターの共同作業者の使用](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md)を参照してください。</span>


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
   <td>[!UICONTROL システム管理者]またはグループ管理者</span></td> 
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

<span class="preview">前提条件は、エージェントの出所によって異なります：</span>

* <span class="preview">Adobe ネイティブ：組織でAdobe CX Coworkerを有効にする必要があります。 外部プラットフォームでエージェントを設定したり、外部プラットフォームの資格情報を指定したりする必要はありません。</span>
* 外部プラットフォームまたはカスタムエージェント：Workfrontで作業エージェントを作成する前に、接続する予定のプラットフォームでエージェントを設定します。

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

<span class="preview">次の設定ガイダンスは、Adobe ネイティブのサポートと、まだプレビュー中のオリジンベースの設定モデルを反映しています。</span>

作業エージェントは、Workfrontでタスクまたはイシューに割り当てることができるエージェントです。 名前、アクセスレベルおよびその他の詳細を使用して作業エージェントを設定し、ユーザーを割り当てるようにタスクに割り当てます。

作業用エージェントはエージェントであるため、そのアクションと機能は、エージェントを設定する場所で設定されます。 Work Agentsは、<span class="preview">Coworker、</span>を使用するネイティブ Work Agentsにするか、サポートされている外部プラットフォーム（Copilot Studio、Claude、OpenAI、IBMなど）から取得できます。

>作業担当者は、タスクまたはイシューに割り当てることができます。

作業担当者が使用するライセンスには料金は請求されません。 組織に200 Workfront ライセンスがあり、Work Agentを作成している場合、201 ライセンスが使用されますが、請求されるのは200のみです。

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
   >グループ管理者の場合、このフィールドには管理者であるグループのみが表示されます。 グループ管理者は、少なくとも1つのグループを選択する必要があります。

1. **エージェントの生成元を選択**&#x200B;領域で、<span class="preview">Adobe Native</span>を使用するか、Copilotなどの共通プラットフォームで作成されたエージェントを接続するか、カスタムエージェントを使用するかを選択します。
1. <span class="preview"> （条件付き）Adobe Nativeを選択した場合は、Adobe CX Coworkerが有効になっており、すぐに使用できるAdobe Native Agentを使用することを確認します。</span>
1. （条件付き）共通プラットフォームのエージェントを使用している場合は、エージェントのプラットフォームの認証の詳細を入力します。

   | Platform | 必須の認証 |
   |---|---|
   | Copilot Studio | Web チャネルシークレット |
   | Claude Managed Agents | Anthropic API キー<br> エージェント ID<br>環境ID |
   | OpenAI エージェント | API キー<br> エージェント ID |
   | IBM watsonx Orchestrate | サービス URL<br>API キー<br> エージェント ID |

1. 「**接続をテスト**」をクリックします。 これにより、接続が正しくセットアップされたかどうかを確認できます。
1. **共同作業者が作業を完了した後、共同作業者が実行するアクションを切り替える**&#x200B;領域を選択できます。

   * 通知の送信：エージェントは、更新ストリームにコメントを作成し、作業をリクエストしたユーザー、エージェントを割り当てたユーザー、またはプロジェクトを所有するユーザーをタグ付けします。
   * テキストベースのドキュメントのアップロード
   * タスクを完了としてマーク
   * タスクフィールドの書き込み：エージェントが書き込むことができるフォームとフィールドを選択します。
   * プロジェクトフィールドの書き込み：エージェントが書き込むことができるフォームとフィールドを選択します。

1. 「**保存**」をクリックします。

タスクへの割り当て方法など、作業エージェントの詳細については、[作業エージェントの使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。

### 作業エージェント用のエージェントを作成するためのベストプラクティス

Workfrontで作業エージェントとして使用するエージェントを作成する際には、次のベストプラクティスが役立つ場合があります。 ベストプラクティスを確認するには、エージェントを作成するアプリケーションのセクションをクリックします。

+++ Claude

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



>[!IMPORTANT]
>
>Writerはエージェントの使用を廃止しました。 Writer エージェントを使用して設定された作業エージェントは、10月9日を過ぎると機能しなくなります。 2026.
>
>非推奨（廃止予定）について詳しくは、執筆者ドキュメントの[ エージェントライブラリの移行と非推奨（廃止予定） ](https://support.writer.com/articles/8335689949-migrating-no-code-agents)を参照してください。


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

+++

<div class="preview">

## プロジェクトコーディネーターの設定

プロジェクトコーディネーターは、プロジェクトの状況を監視し、作業を軌道に乗せるのに役立つ、すぐに利用できる共同作業者です。 作業エージェントとは異なり、プロジェクトコーディネーターは外部エージェントを設定する必要がありません。

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. 画面の右上隅にある「**新しい共同作業者**」をクリックします。
1. **プロジェクトコーディネーター**&#x200B;を選択し、**続行**&#x200B;をクリックします。
1. 「**AI Collaborator Name**」フィールドに、プロジェクトコーディネーターの名前を入力します。 これは、プロジェクトの共同作業者として表示される名前です。
1. （オプション）「**AI Collaborator Description**」フィールドに、プロジェクトコーディネーターの役割や目的の説明を入力します。
1. 「**アクセスレベル**」フィールドで、プロジェクトコーディネーターのアクセスレベルを選択します。 このアクセスレベルは、共同作業者がプロジェクトで実行できる操作を制御します。アクセスレベルは、ユーザーが実行できる操作を制御するのと同じ方法です。
1. （オプション）「**グループ**」フィールドで、プロジェクトコーディネーターが関連付けるグループを選択します。

   >[!NOTE]
   >
   >グループ管理者の場合、このフィールドには管理者であるグループのみが表示されます。 グループ管理者は、少なくとも1つのグループを選択する必要があります。

1. **コーディネーターのアクション**&#x200B;領域で、プロジェクト コーディネーターがプロジェクトの更新を送信する方法を指定します。 プロジェクトコーディネーターは、これらのアクションを実行するための権限を持っている必要があります。 また、プロジェクトコーディネーターは、プロジェクトとそのタスクに関するコメントを追加できます。

   プロジェクトの更新には、進捗状況、プロジェクトの健全性、期限切れまたはリスクのあるタスクや承認、欠けているフィールドや割り当てなどが含まれます。

   * 「**ケイデンス**」フィールドで、プロジェクトコーディネーターが毎日または毎週アップデートを送信するかどうかを選択します。
   * （条件付き）週単位を選択した場合、**日** フィールドで、更新が送信される曜日を選択します。
   * 「**時間**」フィールドで、更新を送信する時間を選択します。
   * 「**タイムゾーン**」フィールドで、更新時間のタイムゾーンを選択します。
   * 「**誰が更新プログラムを取得するか**」フィールドで、更新プログラムをプロジェクト所有者またはプロジェクト関係者に送信するかどうかを選択します。 デフォルトはプロジェクトオーナーです。

1. 「**保存**」をクリックします。

プロジェクトコーディネーターを保存したら、ユーザーが使用するレイアウトテンプレートのプロジェクトヘッダーに「**プロジェクトコーディネーター**」フィールドを追加します。 フィールドがヘッダーで使用可能になるまで、ユーザーはプロジェクトにプロジェクトコーディネーターを割り当てることはできません。

手順については、[ レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

プロジェクトに割り当てる方法など、プロジェクトコーディネーターについて詳しくは、[ プロジェクトコーディネーターの共同作業者の使用](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md)を参照してください。

</div>

## AI共同作業者の管理

既存のAI共同作業者を編集、コピー、削除できます。

>[!NOTE]
>
>グループ管理者は、自分が管理者であるグループに関連付けられたAI共同作業者のみを表示し、操作できます。 特定のAI共同作業者に他のグループも関連付けられている場合、グループ管理者はグループを表示できますが、編集することはできません。

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. （条件付き）共同作業者を編集するには、編集する共同作業者の名前をクリックし、「共同作業者を編集」ウィンドウで編集を行い、**保存**&#x200B;をクリックします。
1. （条件付き）共同作業者を削除するには、削除するAI共同作業者の行にある削除アイコン ![削除アイコン ](assets/delete-collaborator-icon.png)をクリックし、**削除**&#x200B;をクリックします。
