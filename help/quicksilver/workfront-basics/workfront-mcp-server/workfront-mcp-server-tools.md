---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP Server Tools
description: Adobe Workfront MCP サーバーを通じて使用可能なツールのリファレンスリストを、Workfront領域ごとにグループ化します。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 2de2dd8d79af0929f010cda304f8d1e008deb553
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 6%

---


# Adobe Workfront MCP Server Tools

{{preview-fast-release-general}}

この記事では、[!DNL Adobe Workfront] MCP サーバーが接続されたAI エージェント プラットフォームに公開するツールについて説明します。 Workfrontのアイテムの検索、作成、更新、削除を求めると、これらのツールが代わりに呼び出されます。

AI エージェント プラットフォームを介してこれらのツールを使用する方法について詳しくは、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)を参照してください。 接続の設定方法について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。

>[!IMPORTANT]
>
>AI エージェント型プラットフォームは、Workfrontアカウント、アクセスレベル、オブジェクト権限を使用してWorkfrontで動作します。 ツールは、Workfrontで対応するアクセス権を持っている場合にのみ機能します。 Adobeは、AI エージェントによるWorkfront データの変更について責任を負いません。


## 読み取りと書き込みのアクション

次の表の各ツールは、「アクション」列で「読み取り」または「書き込み」アクションに分類されます。

* **読み取り**: データを変更せずにWorkfrontから情報を取得します。 たとえば、プロジェクトの検索、ドキュメントのリスト、レコードの詳細の取得などです。
* **書き込み**: Workfront データを作成、更新または削除します。 例えば、プロジェクトの作成、レコードの更新、ビューの削除などです。

Workfront管理者は、AI エージェンティックプラットフォームが使用できるツールのカテゴリを、システム環境設定の2つのトグルで制御します。

* **読み取り専用のMCP ツール** （デフォルトで有効）
* **MCP ツールの書き込み** （既定では無効）

AI エージェンティックプラットフォームがWorkfront アイテムを見つけることができても、作成、更新、削除できない場合は、Workfront管理者に書き込みアクションを有効にするように依頼します。 詳しくは、*Adobe Workfront MCP サーバー*&#x200B;の設定の[管理者の前提条件](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites)を参照してください。

## 承認ツール

### ドキュメント

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| 名前でドキュメントのバージョンを検索 | `approvals_find_document_version_by_name` | ドキュメントの現在のバージョン IDをファイル名で検索します。 部分一致をサポートします。 | 読み取り |
| バージョン IDでドキュメントを取得 | `approvals_get_document_by_version_id` | 既知のドキュメントバージョン IDのドキュメントの詳細（名前、サイズ、アップロード日、アップローダー）を取得します。 | 読み取り |
| ドキュメント範囲を解決 | `approvals_resolve_document_scope` | プロジェクトまたはフォルダーを、そのプロジェクトに含まれるドキュメントバージョン IDのリストに展開します。 プロジェクト、フォルダーおよびフォルダーの名前単位のスコープをサポートします。 | 読み取り |
| スコープ別ドキュメントの取得 | `approvals_get_documents_by_scope` | 非推奨（廃止予定）: 代わりに`insights_find_workfront_data`を使用してください。 このツールは、プロジェクトまたはフォルダー内のドキュメントを一覧表示します。 | 読み取り |
| AEMにリンクされたフォルダーのリスト* | `approvals_list_aem_linked_folders` | Adobe Experience ManagerにリンクされているWorkfront ドキュメントフォルダーを一覧表示します。 | 読み取り |
| ドキュメントを検索 | `approvals_find_document` | 非推奨（廃止予定）: 代わりに`insights_find_workfront_data`を使用してください。 このツールは、ファイル名またはドキュメントのバージョン IDでドキュメントを検索しました。 | 読み取り |
| AEM フォルダーへのドキュメントの送信* | `approvals_send_documents_to_aem_folder` | 1つ以上のWorkfront ドキュメントをAEMにリンクされたフォルダーに移動します。 | 編集 |

* これらのツールを使用するには、Workfront インスタンスでネイティブの[!DNL Adobe Experience Manager]統合が設定されている必要があります。 詳しくは、[Adobe Experience Manager Assets統合の概要](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md)を参照してください。


*AEM フォルダーへのドキュメントの送信は、Adobe クラウドストレージ上のプロジェクトではまだサポートされていません。 今後のリリースでサポートが予定されています。


<!--
| List AEM-linked folders* | `approvals_list_aem_linked_folders` | Lists Workfront document folders that are linked to Adobe Experience Manager. | Read |
-->

### 承認ワークフロー

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| 承認ワークフロー情報を取得 | `approvals_get_approval_info` | 文書バージョンの現在の承認ワークフロー（ステージ、参加者、ステータス）を返します。 <span class="preview">複数のパスを持つ承認の場合、各パスとそのステージが表示されます。</span> | 読み取り |
| 承認ワークフローの作成または更新 | `approvals_create_or_update_approval_workflow` | ドキュメントのバージョンの承認ワークフローステージを作成または更新します。 <span class="preview">1つのステージのトラックまたは複数の並行レビューパスをサポートしています。</span> | 編集 |
| テンプレートから承認を作成 | `approvals_create_approval_from_template` | 既存のテンプレート <span class="preview">を使用して、複数の並行パスを定義するテンプレートを含むドキュメントに対して承認ワークフローを作成します。</span> | 編集 |
| 承認ステージの削除 | `approvals_delete_approval_stage` | 承認ワークフローから名前または位置で1つのステージを削除します。 未開始ステージのみを削除できます。 | 編集 |
| <span class="preview">承認へのパスの追加</span> | <span class="preview">`approvals_add_path_to_approval`</span> | <span class="preview">既存の承認ワークフローに新しい並行レビューパスを追加するので、1つの文書バージョンで複数のレビュートラックが同時に実行されます。</span> | <span class="preview">Write</span> |
| <span class="preview">承認からパスを削除</span> | <span class="preview">`approvals_remove_path_from_approval`</span> | <span class="preview">承認ワークフローから並行パスを削除します。 最初のパスは削除できません。完了またはロックされたステージを含むパスは保護されます。</span> | <span class="preview">Write</span> |
| <span class="preview"> パスにステージを追加</span> | <span class="preview">`approvals_add_stage_to_path`</span> | <span class="preview">同時承認ワークフロー内の特定のパスの最後にレビューステージを追加します。</span> | <span class="preview">Write</span> |
| <span class="preview"> パスからステージを削除</span> | <span class="preview">`approvals_remove_stage_from_path`</span> | <span class="preview">同時承認ワークフローの特定のパスから、開始されていないステージを削除します。 各パスには、少なくとも1つのステージを保持する必要があります。</span> | <span class="preview">Write</span> |
| <span class="preview"> パスのステージの並べ替え</span> | <span class="preview">`approvals_reorder_stages_in_path`</span> | <span class="preview">同時承認ワークフローの1つのパス内のステージの順序を変更します。</span> | <span class="preview">Write</span> |

<!--
| Add and remove participants for an approval in bulk | `approvals_bulk_update_approval_participants`<br>`approvals__submit_bulk_update_approval_participants` | Adds or removes participants to or from multiple approvals at the same time. Currently, bulk updates can be applied only across a single project. Bulk updates across multiple projects will be available in the near future. | Write |
-->

<!--
| Request document approval | `approvals_request_document_approval` | Opens a guided form for requesting approval on a document version (title, approvers/reviewers, optional due date and message). | Write |
-->

### リマインダー

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| 参加者にリマインダーを送信 | `approvals_send_reminder_to_participants` | 承認段階の特定の参加者にリマインダーメールを送信します。 開始、未完了、未ロックのステージに対してのみ機能します。 | 編集 |
| 未決定の参加者にリマインダーを送信する | `approvals_send_reminder_to_undecided` | 承認段階で、未決定の参加者全員（通知、開封、コメント付き）にリマインダーメールを送信します。 | 編集 |

### 承認テンプレート

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| 承認テンプレートの一覧表示 | `approvals_list_templates` | このWorkfront インスタンスで使用できる承認テンプレートを一覧表示します。 作成者、参加者、使用状況別の並べ替えによるフィルタリングをサポートします。 | 読み取り |
| 名前でテンプレートを検索 | `approvals_search_template_by_name` | 名前で承認テンプレートを検索します（大文字と小文字を区別しない部分一致）。 | 読み取り |
| 承認テンプレートを作成 | `approvals_create_template` | 線形またはグラフベースのステージの依存関係を使用して、新しい承認テンプレートを作成します。 | 編集 |
| 承認テンプレートを更新 | `approvals_update_template` | 構造化された変更（参加者の追加または削除、ステージ名の変更、期限の設定など）を使用して、既存のテンプレートを更新します。 | 編集 |
| 関係者に承認の一括リマインド | `approvals_send_approval_reminder` | プロジェクト、フォルダー、キャンペーン、または期日ウィンドウ全体で、すべての保留中の承認者に承認リマインダーメールを送信します。 | 編集 |
| 承認テンプレートの一括更新 | `approvals_update_template` | テンプレートのアセットへの適用、新しいテンプレートをゼロから作成する、既存の承認フローから作成する、テンプレートの編集、テンプレートやアセットをまたいだ一括操作など、複数のテンプレートに対してテンプレートの更新を実行します。 | 編集 |
| 承認参加者を一括で追加または削除します。 | `approvals_update_approval_participants`と`approvals__submit_update_approval_participants` | 単一のオペレーションで、ポートフォリオ、プログラム、プロジェクトスコープ全体にわたって参加者を追加、削除、置き換えます。 | 編集 |


### 参照とユーザー

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| 名前でプロジェクトを検索 | `approvals_find_project_by_name` | システム全体で名前の一部が一致する場合に、Workfront プロジェクトを検索します。 | 読み取り |
| 所有者によるプロジェクトの取得 | `approvals_get_projects_by_owner` | 呼び出し元ユーザーがオーナーであるWorkfront プロジェクトを一覧表示します。 | 読み取り |
| 現在のユーザーを取得 | `approvals_get_current_user` | 2026年8月13日（PT）に削除されました。 このツールは、名前、ユーザーID、ホームチーム名、ホームチーム IDなど、呼び出し元ユーザーのWorkfront IDを返しました。 同様の機能については、「インサイトツールで現在のユーザーを取得[&#128279;](#insights-tools)」を参照してください。 | 読み取り |
| 名前でユーザーを検索 | `approvals_find_user_by_name` | 非推奨（廃止予定）: 代わりに`insights_search_users`を使用してください。 このツールは、WorkfrontユーザーのIDを名前（ファジーまたは部分的に一致）で検索し、名前、ID、メール、タイトル、アバターURLを返します。 | 読み取り |
| 名前でチームを検索 | `approvals_find_team_by_name` | 非推奨（廃止予定）: 代わりに`insights_find_id_by_name`を使用してください。 このツールは、Workfront チームのIDを名前（ファジーまたは部分一致）で検索しました。 | 読み取り |
| プロジェクトの検索 | `approvals_find_projects` | 非推奨（廃止予定）: 代わりに`insights_find_workfront_data`を使用してください。 このツールは、Workfront プロジェクトを検索し、オプションで名前でフィルタリングしたり、呼び出し元ユーザーが所有するプロジェクトに限定したりしました。 | 読み取り |

## プランニングツール

>[!IMPORTANT]
>
>* MCPをWorkfront Planningで使用するには、Adobe Workfront Planningを含むWorkfront パッケージに属している必要があります。

### ワークスペース

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| ワークスペースを取得 | `planning_get_workspace` | IDまたはエイリアスでワークスペースの完全な詳細を取得します。 | 読み取り |
| ワークスペースリストを取得 | `planning_get_workspace_list` | カーソルベースのページネーションを使用して、使用可能なすべてのワークスペースを一覧表示します。 | 読み取り |
| ワークスペースを作成 | `planning_create_workspace` | レコードタイプ、フィールド、データを整理するための新しい空のワークスペースを作成します。 | 編集 |
| テンプレートからワークスペースを作成 | `planning_create_workspace_from_template` | 既存のテンプレートを使用して事前入力された新しいワークスペースを作成します。 | 編集 |
| ワークスペースを更新 | `planning_update_workspace` | ワークスペース（名前、説明、アイコン、セクション、所有者）の部分的な更新。 | 編集 |
| ワークスペースを削除 | `planning_delete_workspace` | ワークスペースとそのすべてのデータを完全に削除します。 | 編集 |
| ワークスペースをテンプレートに変換 | `planning_convert_workspace_to_template` | 既存のワークスペースを再利用可能なテンプレートとして保存します（管理者が必要）。 | 編集 |
| ワークスペース共有を取得 | `planning_get_workspace_sharing` | ワークスペースの現在の共有と権限の設定を返します。 | 読み取り |
| ワークスペース共有の変更 | `planning_modify_workspace_sharing` | ワークスペースにアクセスできるユーザーと権限レベルを更新します。 | 編集 |

### レコードタイプ

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| レコードタイプを取得 | `planning_get_record_type` | フィールドとビューを含む、レコードタイプの完全な詳細を取得します。 | 読み取り |
| レコードタイプの作成 | `planning_create_record_types` | ワークスペースセクション内に1つ以上のレコードタイプを作成します。 | 編集 |
| レコードタイプを更新 | `planning_update_record_type` | レコードタイプの名前、説明、アイコン、カラーの一部を更新します。 | 編集 |
| レコードタイプを削除 | `planning_delete_record_type` | レコードタイプとそのすべてのレコード、フィールド、ビューを完全に削除します。 | 編集 |
| グローバルなレコードタイプのリスト | `planning_list_global_record_types` | 現在のユーザーに表示されるすべての一元的に定義された（グローバル）レコードタイプを一覧表示します。 | 読み取り |
| 追加可能なグローバルレコードタイプのリスト | `planning_list_addable_global_record_types` | 特定のワークスペースに追加できるグローバルレコードタイプを一覧表示します。 | 読み取り |
| ワークスペースへのグローバルレコードタイプの追加 | `planning_add_global_record_type_to_workspace` | 指定されたワークスペースにグローバルレコードタイプをリンクします。 | 編集 |
| ワークスペースからグローバルレコードタイプを削除 | `planning_remove_global_record_type_from_ws` | ワークスペースからグローバルレコードタイプのリンクを解除し、そのワークスペース内のすべてのレコードを削除します。 | 編集 |
| 外部記録ワークスペースの取得 | `planning_get_external_record_workspaces` | 特定の外部レコードに接続されているワークスペースとレコードタイプを検索します。 | 読み取り |
| レコードタイプの共有を取得 | `planning_get_record_type_sharing` | 特定のレコードタイプの共有と権限を返します。 | 読み取り |
| レコードタイプの共有を変更 | `planning_modify_record_type_sharing` | レコードタイプにアクセスできるユーザーと権限レベルを更新します。 | 編集 |

### レコード

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| レコードを取得 | `planning_get_record` | IDで単一レコードの完全な詳細を取得します。 | 読み取り |
| レコードの検索 | `planning_search_records` | レコードタイプ内のレコードを検索してフィルタリングします。 | 読み取り |
| 一括記録アクション | `planning_bulk_record_actions` | 1回のリクエストで複数のレコードを作成、更新、削除または復元します。 | 編集 |
| 接続レコードを作成 | `planning_create_connection_record` | 接続されている外部システム（Workfront プロジェクトなど）に新しいレコードを作成します。 | 編集 |
| レコードの更新の順序 | `planning_update_records_order` | レコードタイプ内のレコードの表示順序を変更します。 | 編集 |
| レコードの変更ログを取得 | `planning_get_record_change_log` | レコードのフィールドレベルの編集履歴を返します。 | 読み取り |
| レコードの共有を取得 | `planning_get_record_sharing` | 特定のレコードの共有設定を返します。 | 読み取り |
| レコード共有の変更 | `planning_modify_records_sharing` | 1つ以上のレコードにアクセスできるユーザーと権限レベルを更新します。 | 編集 |

### フィールド

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| フィールドを取得 | `planning_get_field` | IDでフィールドの詳細と値のスキーマを取得します。 | 読み取り |
| フィールドの作成 | `planning_create_fields` | レコードタイプに1つ以上のフィールド（列）を追加します。 | 編集 |
| フィールドを更新 | `planning_update_field` | フィールドの名前、説明、オプション、設定の一部を更新します。 | 編集 |
| フィールドを削除 | `planning_delete_field` | レコードタイプからフィールドとそのすべてのデータを完全に削除します。 | 編集 |

### ビュー

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| ビューを取得 | `planning_get_view` | ID別のビューの詳細を返します。 | 読み取り |
| ビューを作成 | `planning_create_view` | レコードタイプの新しいテーブル、タイムライン、またはカレンダービューを作成します。 | 編集 |
| ビューを更新 | `planning_update_view` | 既存のビューの設定、フィルター、並べ替えを部分的に更新します。 | 編集 |
| ビューを削除 | `planning_delete_view` | ビューを完全に削除します（レコードは影響を受けません）。 | 編集 |
| ビュー共有を取得 | `planning_get_view_sharing` | 特定のビューの共有設定を返します。 | 読み取り |
| ビュー共有を変更 | `planning_modify_view_sharing` | ビューにアクセスできるユーザーと権限レベルを更新します。 | 編集 |

### テンプレート

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| テンプレートリストを取得 | `planning_get_template_list` | 使用可能なすべてのワークスペーステンプレートとサマリー情報を一覧表示します。 | 読み取り |
| テンプレートを取得 | `planning_get_template` | IDで特定のテンプレートの詳細を取得します。 | 読み取り |

### 検索とユーティリティ

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| リソースの検索 | `planning_search_resources` | ワークスペース、レコードタイプ、名前でビューを検索します。 | 読み取り |
| 共有データを検索 | `planning_search_sharing_data` | 共有と権限のユーザー、グループ、チーム、役割、会社名を検索します。 | 読み取り |
| ユーザーを検索 | `planning_search_users` | ページネーションをサポートするユーザーを検索します。 | 読み取り |

## ワークフローツール

ワークフローツールは、AI エージェント基盤が、プロジェクト、タスク、イシュー、時間、割り当て、プログラム、ポートフォリオなど、あらゆるWorkfrontオブジェクトと連携するために使用する汎用的なアクションです。

### オブジェクトとフィールド

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| オブジェクトを検索 | `workflow_search_any_object` | 柔軟なフィルターパラメーター、順序付け、ページネーションを使用して、Workfront オブジェクトを検索します。 | 読み取り |
| オブジェクトを作成 | `workflow_create_any_object` | プロジェクト、タスク、イシュー、時間、割り当て、プログラム、ポートフォリオなどの新しいWorkfront オブジェクトを作成します。 | 編集 |
| オブジェクトを更新 | `workflow_update_any_object` | 既存のオブジェクトのフィールドを更新します。 また、タスクまたはイシューを別のプロジェクトに移動したり、タスクまたはイシューを新しいプロジェクト（またはイシューをタスクに変換）に変換したり、タスク先行者（依存関係）を設定したりすることもできます。 | 編集 |
| オブジェクトを削除 | `workflow_delete_any_object` | IDでWorkfront オブジェクトを削除します。 アクションを実行する前に、明示的なユーザー確認が必要です。 | 編集 |
| フィールド名を解決 | `workflow_resolve_field_names_any_object` | ユーザーが提供したフィールド名またはラベルを、基礎となるWorkfront API フィールド名に変換します。これにより、AI エージェント基盤は正確なリクエストを構築できます。 | 読み取り |
| ワークフロードキュメントを読む | `workflow_read_workflow_docs` | ツール使用ガイドやオブジェクト固有の操作プレイブックなど、Workfront Workflow ドキュメントを読み込みます。 これは、ワークフローアクションを実行する前に必要な最初の手順です。 | 読み取り |

### オブジェクトツール機能の更新

オブジェクトの更新ツールは、フィールド値を変更するだけのものではありません。 また、プロジェクト間の作業の再配置、作業項目の新しいオブジェクトへの昇格、タスクの依存関係の接続も可能です。

#### タスクまたは問題を別のプロジェクトに移動する

移動すると、作業項目が再設定されます。 オブジェクトはIDとリンクを保持し、別のプロジェクトまたは親タスクにのみ存在します。

>[!NOTE]
>
>プレーンフィールドの更新で「プロジェクト」フィールドを設定しても、タスクやイシューは移動しません。 代わりに移動機能を使用してください。

* **タスクを移動**: タスクをターゲットプロジェクトに移動し、オプションでターゲット親タスクの下に移動します。
* **イシューを移動**：イシュー（リクエスト）をターゲットプロジェクトに移動します。

プロンプトの例：

* 「タスク *ワイヤーフレーム*&#x200B;を&#x200B;*モバイルアプリ再設計* プロジェクトに移動します。」
* 「このリクエストを&#x200B;*Q4 Launch* プロジェクトに移動します。」

#### イシューまたはタスクをプロジェクトに変換する

>[!NOTE]
>
>変換すると、新しいオブジェクトが生成されます。 ソース品目がプロセスで消費されます。

* **タスクをプロジェクトに変換**：タスクから新しいプロジェクトを作成します。 必要に応じて、タスクのカスタムデータをコピーし、プロジェクトテンプレートに基づいて新しいプロジェクトを作成できます。
* **イシュー（リクエスト）をプロジェクトに変換**：イシューから新しいプロジェクトを作成します。 必要に応じて、イシューのカスタムデータをコピーし、ネイティブフィールド値をコピーして、プロジェクトテンプレートを適用できます。
* **イシュー（リクエスト）をタスクに変換**：イシューから既存のプロジェクトにタスクを作成します。

各コンバージョンでは、新しく作成したオブジェクトとリンクが返され、Workfrontで直接開くことができます。

プロンプトの例：

* 「タスク *Web サイト更新*&#x200B;を、標準テンプレートを使用して&#x200B;*Web サイト更新2026*&#x200B;というプロジェクトに変換します。」
* 「このリクエストをプロジェクトに変換し、カスタムフィールドをコピーします。」

#### タスク先行者（依存関係）の設定

タスクの先行タスクを定義できます。 先行タスクでは、次の依存関係タイプに加えて、オプションのラグ時間がサポートされます。

* **Finish-Start （FS）**: タスクは、先行タスクの完了時に開始されます。 （Default）
* **Start-Start （SS）**: タスクは、先行タスクの開始時に開始されます。
* **Finish-Finish （FF）**: タスクは、先行タスクが完了すると終了します。
* **Start-Finish （SF）**: タスクは、先行タスクの開始時に終了します。

作業日数に遅延（遅延）またはリード（負の遅延）を追加し、1つのタスクで複数の先行タスクを連結し、別のプロジェクトでタスクを参照できます。

プロンプトの例：

* 「*デザイン*&#x200B;の完了後に&#x200B;*開発*&#x200B;を開始する。」
* 「*QA*&#x200B;を、*開発*&#x200B;が開始する2日間の遅延で開始するように設定します。」
* 「タスク#3とタスク#5を&#x200B;*Launch*&#x200B;の先行タスクとして追加します。」

### コメント

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| クエリコメント | `comment-stream_query_comments` | ページ付きのオブジェクト IDでコメントをクエリします。 | 読み取り |
| コメントを取得 | `comment-stream_get_comment` | IDによる単一のコメントを取得します。 | 読み取り |
| コメント数を取得 | `comment-stream_get_comments_count` | オブジェクトのトップレベルの合計コメント数を取得します。 | 読み取り |
| コメントを作成 | `comment-stream_create_comment` | オブジェクトに新しいコメントを作成します。 | 編集 |
| 返信を作成 | `comment-stream_create_reply` | 既存のコメントへの返信を作成します。 | 編集 |
| コメントを更新 | `comment-stream_update_comment` | 既存のコメントまたは返信を更新します。 | 編集 |
| コメントを削除 | `comment-stream_delete_comment` | IDでコメントを削除します。 | 編集 |
| 反応を追加 | `comment-stream_add_reaction` | コメントに反応（いいね）を追加します。 | 編集 |
| 反応を削除 | `comment-stream_remove_reaction` | コメントから反応（いいね）を削除します。 | 編集 |

### インサイトツール

インサイトツールは、Workfront オブジェクトに関する情報を取得します。

| タイトル | ツール名 | 機能 | アクション |
| --- | --- | --- | --- |
| ドキュメントを読む | `insights_read_docs` | 条件、ステータス、日付、フィールドパスなど、Workfront プレイブックまたはドメインのドキュメントを読み込みます。 これは、データを照会する前に必要な最初のステップです。 | 読み取り |
| 現在のユーザーを取得 | `insights_get_current_user` | 名前、ID、URLなど、独自のWorkfront IDを取得します。 | 読み取り |
| フィールドを検索 | `insights_search_fields` | プロジェクト、タスク、イシュー、ユーザー、ポートフォリオ、チームなどの使用可能なフィールド（標準およびカスタム）を検索します。 | 読み取り |
| フィールドパスを取得 | `insights_get_field_paths` | データクエリツールで必要な、エンティティのドット表記フィールドパスを解決します。 | 読み取り |
| 名前でIDを検索 | `insights_find_id_by_name` | プロジェクト、タスク、ユーザー、ポートフォリオなど、任意のWorkfront オブジェクトのIDを名前で検索します。 | 読み取り |
| Workfrontデータの検索 | `insights_find_workfront_data` | Workfrontデータを検索、フィルタリング、カウント、並べ替え、集計します。 これがメインのクエリとレポートツールです。 | 読み取り |
| オブジェクトを要約 | `insights_summarize_object` | IDで1つのWorkfront オブジェクトを取得して要約します。 | 読み取り |
| エンティティのリスト | `insights_list_entities` | クエリに使用できるすべてのWorkfront オブジェクトタイプを一覧表示します。 | 読み取り |
| ユーザーを検索 | `insights_search_users` | Workfront インスタンス内のユーザーを名前で検索します。 完全または部分的な名前を入力し、一致するユーザーのトップを取得します。 これには、AIの共同作業者「ボット」を通常のユーザーと一緒に含めることもできます。 | 読み取り |




## ツールの更新方法

Adobeが新しいバージョンのWorkfront MCP サーバーをリリースすると、AI エージェンティックプラットフォームは、更新されたツールセットを自動的に使用します。 システムに再接続したり、変更を加えたりする必要はありません。



## その他のツールは近日リリース予定

今後、Workfront MCP サーバーに次のツールを追加する予定です。

* ボード


