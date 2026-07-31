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
source-git-commit: dc6bfcd7d3431532c1227f6cd31f22445882143f
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 4%

---

# AI共同作業者の設定


<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。 プレビューサンドボックス環境でのみ使用できます。</span>


AI協力者とは、AI エージェントをプロジェクトやタスクに組み込む手法のひとつです。 AI共同作業者を設定し、ユーザーと同じように割り当てることができます。

例えば、ブランドガイドラインを使用してレビューアータイプのAI コラボレーターを設定し、そのコラボレーターにドキュメントのレビューを割り当てることができます。

利用可能なAI共同作業者タイプは次のとおりです。

* レビュアー：ブランドまたはAdobe Brand Intelligenceを使用して共同作業者を作成し、その共同作業者をアセットのレビュアーとして割り当てます。

  詳しくは、[Workfront Content Reviewerの基本を学ぶ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)を参照してください。

* タスクコラボレーター：コパイロットまたはライターを使用して共同作業者を作成し、共同作業者をタスクに割り当ててタスクレベルの作業を完了します。

  詳しくは、[&#x200B; タスクコラボレーターの使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>Standard、Prime、またはUltimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

### AI レビュー担当者の場合：

* 署名済みのAdobe Gen AI契約書がファイルに登録されている必要があります。

  詳しくは、「[Adobe生成AI契約書に署名する](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)」を参照してください。WorkfrontのAI アシスタントの記事を参照してください。
* レビューアータイプのAI コラボレーターに使用するには、Workfrontでブランドを設定しておく必要があります。

  手順については、[&#x200B; コンテンツレビュアーのブランドの作成と管理](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)を参照してください。
* レビュアーAI コラボレーターにAdobe Brand Intelligenceを使用するには、Workfrontの統合されたレビューと承認のエクスペリエンスを使用する必要があります。</span>

  詳しくは、[統合レビューと承認の基本を学ぶ](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)を参照してください。</span>

<div class="preview">

### タスクコラボレーターの場合

タスクコラボレーターとして使用する前に、Claude、Copilot Studio、またはWriterでエージェントを設定する必要があります。

</div>

## レビュー担当者タイプのAI コラボレーターを新規作成する

レビュアーAI共同作業者は、Workfront ブランドまたはAdobe ブランドインテリジェンスを使用するように設定できます。

* **ブランド**：ブランドはWorkfrontで作成されます。 Workfrontでブランドを作成するには、ブランドガイドラインを含むPDF ファイルをアップロードするか、ブランド要素を手動で入力します。
* **Adobe Brand Intelligence**: AIの共同作業者がAdobe Brand Intelligenceを使用してアセットをレビューすると、レビュー担当者によるコメントをFrame.ioで表示できます。 </span>


{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. 画面の右上隅にある「**新しい共同作業者**」をクリックします。
1. **Reviewer**&#x200B;をクリックしてから、**Continue**&#x200B;をクリックします。
1. 「共同作業者の名前」フィールドに、共同作業者の名前を入力します。 これは、タスクで使用可能な担当者のリストに表示される名前です。
1. 共同作業者がレビューにブランドを使用するか、Adobe Brand Intelligenceを使用するかを選択します。
1. （条件付き） AI共同作業者がブランドを使用する場合は、使用するブランドとブランドガイドラインを選択します。
1. 「**保存**」をクリックします。

<div class="preview">

## タスクコラボレーターの設定

タスクコラボレーターは、Workfrontでタスクに割り当てることができるMCP エージェントです。 タスクコラボレーターを名前、アクセスレベル、その他の詳細で設定し、ユーザーを割り当てるように割り当てます。

タスクコラボレーターはMCP エージェントであるため、そのアクションと機能は、エージェントを設定する場所で設定されます。 現在、タスクコラボレーターとして使用されるエージェントは、Copilot Studio、Claude、またはWriterで作成できます。

タスクコラボレーターとして機能するエージェントを作成する際のベストプラクティスの一覧については、[&#x200B; タスクコラボレーターのエージェントを作成するためのベストプラクティス &#x200B;](#best-practices-for-creating-an-agent-for-a-task-collaborator)を参照してください。

### Workfrontでのタスクコラボレーターの設定

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. 画面の右上隅にある「**新しい共同作業者**」をクリックします。
1. **タスクエージェント**&#x200B;を選択し、**続行**&#x200B;をクリックします。
1. 「AI共同作業者の名前」フィールドに、共同作業者の名前を入力します。 これは、タスクで使用可能な担当者のリストに表示される名前です。
1. 「AI共同作業者の説明」フィールドに、共同作業者の目的または実行するアクションの説明を入力します。
1. 「アクセスレベル」フィールドで、この共同作業者のアクセスレベルを選択します。 このアクセスレベルは、共同作業者の機能を制御し、アクセスレベルはユーザーの機能を制御するのと同じように制御します。
1. **エージェントのオリジンを選択**&#x200B;領域で、CopilotやWriterなどの共通プラットフォームで作成されたエージェントを接続するか、カスタムエージェントを使用するかを選択します。
1. （条件付き）共通プラットフォームのエージェントを使用している場合は、エージェントのプラットフォームの認証の詳細を入力します。

   | Platform | 必須の認証 |
   |---|---|
   | Copilot Studio | Web チャネルシークレット |
   | Claude Managed Agents | Anthropic API キー<br> エージェント ID<br>環境ID |
   | ライター | API キー<br> アプリケーション ID |

1. 「**接続をテスト**」をクリックします。 これにより、接続が正しくセットアップされたかどうかを確認できます。
1. **共同作業者が作業を完了した後、共同作業者が実行するアクションを切り替える**&#x200B;領域を選択できます。
1. 「**保存**」をクリックします。

タスクへの割り当て方法など、タスクコラボレーターについて詳しくは、[&#x200B; タスクコラボレーターの使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。


### タスクコラボレーターのエージェントを作成するためのベストプラクティス

Workfrontでタスクコラボレーターとして使用するエージェントを作成する際には、次のベストプラクティスが役立つ場合があります。 ベストプラクティスを確認するには、エージェントを作成するアプリケーションのセクションをクリックします。

+++ クロード

1. [platform.claude.com](https://platform.claude.com/)にあるClaude Consoleに移動します。
1. API キーを作成します。
   1. API キーの下で、右上隅の「**キーを作成**」をクリックします。
   1. 名前と有効期限を入力します。
   1. キーをコピーして、安全で安全な場所に保存します。 Workfrontでタスクコラボレーターを設定するには、このキーが必要です。

1. 環境を作成します。
   1. **Managed Agents** > **Environments**&#x200B;の下で、右上隅の&#x200B;**Create Environment**&#x200B;をクリックします。
   1. 必要に応じて、名前とホスティングタイプを指定します。
   1. 必要に応じて、共有パッケージとメタデータを設定します。環境は複数のエージェントで再利用でき、パッケージとメタデータを共有できます。
      環境IDは、環境名の左上隅に表示されます。

1. エージェントを作成します。
   1. Managed Agents/Agentsで、右上隅の&#x200B;**Create Agent**&#x200B;をクリックします。
   1. 必要に応じて、名前、モデル、システムプロンプト、スキル、ツールを提供します。タスク共同作業者は、タスクのコンテキストをこのエージェントに渡し、そのエージェントが作業を実行するので、説明が必要です。
      エージェント IDは、左上隅のエージェント名の下に表示されます。

1. WorkfrontでTask Collaboratorを設定します。
   1. API キー、環境ID、エージェント IDを入力します
   1. 「**接続をテスト**」をクリックして確認します。

1. タスクコラボレーターをWorkfront タスクに割り当てます。
   1. タスク共同作業者は、すべての先行タスクが完了した後に起動します。

+++
<!--
+++ Copilot Studio



+++
-->
+++ ライター

Writerでタスクコラボレーターとして使用するエージェントを作成する場合は、次のワークフローをお勧めします。

エージェントの作成について詳しくは、[&#x200B; ライターのドキュメント &#x200B;](https://dev.writer.com/no-code/introduction)を参照してください。

1. Writer AI Studioでノーコードアプリを作成します。
1. 1つのテキスト入力フィールドを追加します。 デフォルト名「テキスト入力」を使用できます。
1. プロンプトに`@TextInput`を追加します。 アプリ設定の「プロンプト」セクションで、プロンプトテンプレートが入力変数を参照していることを確認します。 これが欠ければ、モデルはタスクデータを見ることはできません。
1. プロンプトを調整して、すぐに出力を生成します。 回答する前に、ユーザーに説明や追加のコンテキストを求める指示を削除します。 例：「入力を受け取ったら、コンテンツ生成リクエストとして扱い、出力を即座に生成します。 明確化を求めるな」
1. API キーとアプリケーション IDをコピーします。 Workfrontでタスクコラボレーターを設定するには、タスクコラボレーターが必要です。

   * WriterでAPI キーを設定する方法については、Writer ドキュメントの[Quickstart](https://dev.writer.com/home/quickstart)を参照してください。
   * Writerでアプリケーション IDを設定する方法については、Writer ドキュメントの「[API](https://dev.writer.com/home/applications)を介してノーコードエージェントを呼び出す」を参照してください。

1. WorkfrontでTask Collaboratorを設定します。 設定の一部として、API キーとアプリケーション IDを入力し、**接続をテスト**&#x200B;をクリックして確認します。
1. タスクコラボレーターをWorkfront タスクに割り当てます。 共同作業者は、タスクの先行タスクがすべて完了すると作業を開始します。

+++

</div>

## AI共同作業者の管理

既存のAI共同作業者を編集、コピー、削除できます。

{{step-1-to-setup}}

1. 左側のナビゲーションで、**AI Collaborators**&#x200B;をクリックします。
1. （条件付き）共同作業者を編集するには、編集する共同作業者の名前をクリックし、「共同作業者を編集」ウィンドウで編集を行い、**保存**&#x200B;をクリックします。
1. （条件付き）共同作業者をコピーするには、コピーするAI共同作業者の行にあるコピーアイコン ![&#x200B; コピーアイコン &#x200B;](assets/copy-ai-collaborator.png)をクリックし、コピーの名前をクリックして、共同作業者を編集ウィンドウで編集し、**保存**&#x200B;をクリックします。
1. （条件付き）共同作業者を削除するには、削除するAI共同作業者の行にある削除アイコン ![削除アイコン &#x200B;](assets/delete-collaborator-icon.png)をクリックし、**削除**&#x200B;をクリックします。
