---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP Server Tools
description: Adobe Workfront MCP サーバーを通じて使用可能なツールのリファレンスリストを、Workfront領域ごとにグループ化します。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 6%

---


# Adobe Workfront MCP Server Tools

この記事では、[!DNL Adobe Workfront] MCP サーバーが接続されたAI エージェント プラットフォームに公開するツールについて説明します。 Workfrontのアイテムの検索、作成、更新、削除を求めると、これらのツールが代わりに呼び出されます。

ツールは、「承認」、「計画」、「ワークフロー」というWorkfront領域ごとにグループ化されます。

AI エージェント プラットフォームを介してこれらのツールを使用する方法について詳しくは、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)を参照してください。 接続の設定方法について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。

>[!IMPORTANT]
>
>AI エージェント型プラットフォームは、Workfrontアカウント、アクセスレベル、オブジェクト権限を使用してWorkfrontで動作します。 ツールは、Workfrontで対応するアクセス権を持っている場合にのみ機能します。 Adobeは、AI エージェントによるWorkfront データの変更について責任を負いません。

## 承認ツール （合計23）

### ドキュメント

<!-- 
VERIFY BEFORE PUBLISHING: The following three tools may not be customer-facing. If engineering confirms they're internal-only, delete these rows from the table below:
- approvals_get_document_by_version_id
- approvals_list_aem_linked_folders
- approvals_send_documents_to_aem_folder
-->

| タイトル | ツール名 | 機能 |
|---|---|---|
| 名前でドキュメントのバージョンを検索 | `approvals_find_document_version_by_name` | ドキュメントの現在のバージョン IDをファイル名で検索します。 部分一致をサポートします。 |
| バージョン IDでドキュメントを取得 | `approvals_get_document_by_version_id` | 既知のドキュメントバージョン IDのドキュメントの詳細（名前、サイズ、アップロード日、アップローダー）を取得します。 |
| プロジェクト別ドキュメントの取得 | `approvals_get_documents_by_project` | Workfront プロジェクト内のドキュメントと、各ドキュメントの現在のバージョン IDを一覧表示します。 |
| ドキュメント範囲を解決 | `approvals_resolve_document_scope` | プロジェクトまたはフォルダーを、そのプロジェクトに含まれるドキュメントバージョン IDのリストに展開します。 プロジェクト、フォルダーおよびフォルダーの名前単位のスコープをサポートします。 |
| AEMにリンクされたフォルダーのリスト | `approvals_list_aem_linked_folders` | Adobe Experience ManagerにリンクされているWorkfront ドキュメントフォルダーを一覧表示します。 |
| AEM フォルダーへのドキュメントの送信 | `approvals_send_documents_to_aem_folder` | 1つ以上のWorkfront ドキュメントをAEMにリンクされたフォルダーに移動します。 |

### 承認ワークフロー

| タイトル | ツール名 | 機能 |
|---|---|---|
| 承認ワークフロー情報を取得 | `approvals_get_approval_info` | 文書バージョンの現在の承認ワークフロー（ステージ、参加者、ステータス）を返します。 |
| 承認ワークフローの作成または更新 | `approvals_create_or_update_approval_workflow` | ドキュメントのバージョンの承認ワークフローステージを作成または更新します。 線形および平行（グラフ）ステージの依存関係をサポートします。 |
| テンプレートから承認を作成 | `approvals_create_approval_from_template` | 既存のテンプレートを使用して、ドキュメントに承認ワークフローを作成します。 |
| 文書の承認を依頼 | `approvals_request_document_approval` | ドキュメントのバージョン（タイトル、承認者/レビュー担当者、オプションの期日およびメッセージ）に対して承認を要求するためのガイド付きフォームを開きます。 |
| 承認ステージの削除 | `approvals_delete_approval_stage` | 承認ワークフローから名前または位置で1つのステージを削除します。 未開始ステージのみを削除できます。 |

### リマインダー

| タイトル | ツール名 | 機能 |
|---|---|---|
| 参加者にリマインダーを送信 | `approvals_send_reminder_to_participants` | 承認段階の特定の参加者にリマインダーメールを送信します。 開始、未完了、未ロックのステージに対してのみ機能します。 |
| 未決定の参加者にリマインダーを送信する | `approvals_send_reminder_to_undecided` | 承認段階で、未決定の参加者全員（通知、開封、コメント付き）にリマインダーメールを送信します。 |

### 承認テンプレート

| タイトル | ツール名 | 機能 |
|---|---|---|
| 承認テンプレートの一覧表示 | `approvals_list_templates` | このWorkfront インスタンスで使用できる承認テンプレートを一覧表示します。 作成者、参加者、使用状況別の並べ替えによるフィルタリングをサポートします。 |
| 名前でテンプレートを検索 | `approvals_search_template_by_name` | 名前で承認テンプレートを検索します（大文字と小文字を区別しない部分一致）。 |
| 承認テンプレートを作成 | `approvals_create_template` | 線形またはグラフベースのステージの依存関係を使用して、新しい承認テンプレートを作成します。 |
| 承認テンプレートを更新 | `approvals_update_template` | 構造化された変更（参加者の追加または削除、ステージ名の変更、期限の設定など）を使用して、既存のテンプレートを更新します。 |

### 参照とユーザー

| タイトル | ツール名 | 機能 |
|---|---|---|
| 現在のユーザーを取得 | `approvals_get_current_user` | 名前、ユーザーID、ホームチーム名、ホームチーム IDなど、呼び出し元ユーザーのWorkfront IDを返します。 |
| 名前でユーザーを検索 | `approvals_find_user_by_name` | Workfront ユーザーのIDを名前（ファジーまたは部分一致）で検索します。 名前、ID、電子メール、タイトル、アバターのURLを返します。 |
| 名前でチームを検索 | `approvals_find_team_by_name` | Workfront チームのIDを名前（ファジーまたは部分一致）で検索します。 |
| 名前でプロジェクトを検索 | `approvals_find_project_by_name` | システム全体で名前の一部が一致する場合に、Workfront プロジェクトを検索します。 |
| 所有者によるプロジェクトの取得 | `approvals_get_projects_by_owner` | 呼び出し元ユーザーがオーナーであるWorkfront プロジェクトを一覧表示します。 |
| Adobe リージョンを取得 | `approvals_get_adobe_region` | クラウドプロバイダーリージョンのAdobe名を返します。 |

## プランニングツール（合計43個）

### ワークスペース

| タイトル | ツール名 | 機能 |
|---|---|---|
| ワークスペースを取得 | `planning_get_workspace` | IDまたはエイリアスでワークスペースの完全な詳細を取得します。 |
| ワークスペースリストを取得 | `planning_get_workspace_list` | カーソルベースのページネーションを使用して、使用可能なすべてのワークスペースを一覧表示します。 |
| ワークスペースを作成 | `planning_create_workspace` | レコードタイプ、フィールド、データを整理するための新しい空のワークスペースを作成します。 |
| テンプレートからワークスペースを作成 | `planning_create_workspace_from_template` | 既存のテンプレートを使用して事前入力された新しいワークスペースを作成します。 |
| ワークスペースを更新 | `planning_update_workspace` | ワークスペース（名前、説明、アイコン、セクション、所有者）の部分的な更新。 |
| ワークスペースを削除 | `planning_delete_workspace` | ワークスペースとそのすべてのデータを完全に削除します。 |
| ワークスペースをテンプレートに変換 | `planning_convert_workspace_to_template` | 既存のワークスペースを再利用可能なテンプレートとして保存します（管理者が必要）。 |
| ワークスペース共有を取得 | `planning_get_workspace_sharing` | ワークスペースの現在の共有と権限の設定を返します。 |
| ワークスペース共有の変更 | `planning_modify_workspace_sharing` | ワークスペースにアクセスできるユーザーと権限レベルを更新します。 |

### レコードタイプ

| タイトル | ツール名 | 機能 |
|---|---|---|
| レコードタイプを取得 | `planning_get_record_type` | フィールドとビューを含む、レコードタイプの完全な詳細を取得します。 |
| レコードタイプの作成 | `planning_create_record_types` | ワークスペースセクション内に1つ以上のレコードタイプを作成します。 |
| レコードタイプを更新 | `planning_update_record_type` | レコードタイプの名前、説明、アイコン、カラーの一部を更新します。 |
| レコードタイプを削除 | `planning_delete_record_type` | レコードタイプとそのすべてのレコード、フィールド、ビューを完全に削除します。 |
| グローバルなレコードタイプのリスト | `planning_list_global_record_types` | 現在のユーザーに表示されるすべての一元的に定義された（グローバル）レコードタイプを一覧表示します。 |
| 追加可能なグローバルレコードタイプのリスト | `planning_list_addable_global_record_types` | 特定のワークスペースに追加できるグローバルレコードタイプを一覧表示します。 |
| ワークスペースへのグローバルレコードタイプの追加 | `planning_add_global_record_type_to_workspace` | 指定されたワークスペースにグローバルレコードタイプをリンクします。 |
| ワークスペースからグローバルレコードタイプを削除 | `planning_remove_global_record_type_from_workspace` | ワークスペースからグローバルレコードタイプのリンクを解除し、そのワークスペース内のすべてのレコードを削除します。 |
| 外部記録ワークスペースの取得 | `planning_get_external_record_workspaces` | 特定の外部レコードに接続されているワークスペースとレコードタイプを検索します。 |
| レコードタイプの共有を取得 | `planning_get_record_type_sharing` | 特定のレコードタイプの共有と権限を返します。 |
| レコードタイプの共有を変更 | `planning_modify_record_type_sharing` | レコードタイプにアクセスできるユーザーと権限レベルを更新します。 |

### レコード

| タイトル | ツール名 | 機能 |
|---|---|---|
| レコードを取得 | `planning_get_record` | IDで単一レコードの完全な詳細を取得します。 |
| レコードの検索 | `planning_search_records` | レコードタイプ内のレコードを検索してフィルタリングします。 |
| 一括記録アクション | `planning_bulk_record_actions` | 1回のリクエストで複数のレコードを作成、更新、削除または復元します。 |
| 接続レコードを作成 | `planning_create_connection_record` | 接続されている外部システム（Workfront プロジェクトなど）に新しいレコードを作成します。 |
| レコードの更新の順序 | `planning_update_records_order` | レコードタイプ内のレコードの表示順序を変更します。 |
| レコードの変更ログを取得 | `planning_get_record_change_log` | レコードのフィールドレベルの編集履歴を返します。 |
| レコードの共有を取得 | `planning_get_record_sharing` | 特定のレコードの共有設定を返します。 |
| レコード共有の変更 | `planning_modify_records_sharing` | 1つ以上のレコードにアクセスできるユーザーと権限レベルを更新します。 |

### フィールド

| タイトル | ツール名 | 機能 |
|---|---|---|
| フィールドを取得 | `planning_get_field` | IDでフィールドの詳細と値のスキーマを取得します。 |
| フィールドの作成 | `planning_create_fields` | レコードタイプに1つ以上のフィールド（列）を追加します。 |
| フィールドを更新 | `planning_update_field` | フィールドの名前、説明、オプション、設定の一部を更新します。 |
| フィールドを削除 | `planning_delete_field` | レコードタイプからフィールドとそのすべてのデータを完全に削除します。 |

### ビュー

| タイトル | ツール名 | 機能 |
|---|---|---|
| ビューを取得 | `planning_get_view` | ID別のビューの詳細を返します。 |
| ビューを作成 | `planning_create_view` | レコードタイプの新しいテーブル、タイムライン、またはカレンダービューを作成します。 |
| ビューを更新 | `planning_update_view` | 既存のビューの設定、フィルター、並べ替えを部分的に更新します。 |
| ビューを削除 | `planning_delete_view` | ビューを完全に削除します（レコードは影響を受けません）。 |
| ビュー共有を取得 | `planning_get_view_sharing` | 特定のビューの共有設定を返します。 |
| ビュー共有を変更 | `planning_modify_view_sharing` | ビューにアクセスできるユーザーと権限レベルを更新します。 |

### テンプレート

| タイトル | ツール名 | 機能 |
|---|---|---|
| テンプレートリストを取得 | `planning_get_template_list` | 使用可能なすべてのワークスペーステンプレートとサマリー情報を一覧表示します。 |
| テンプレートを取得 | `planning_get_template` | IDで特定のテンプレートの詳細を取得します。 |

### 検索とユーティリティ

| タイトル | ツール名 | 機能 |
|---|---|---|
| リソースの検索 | `planning_search_resources` | ワークスペース、レコードタイプ、名前でビューを検索します。 |
| 共有データを検索 | `planning_search_sharing_data` | 共有と権限のユーザー、グループ、チーム、役割、会社名を検索します。 |
| ユーザーを検索 | `planning_search_users` | ページネーションをサポートするユーザーを検索します。 |

## ワークフローツール（合計5つ）

ワークフローツールは、AI エージェント基盤が、プロジェクト、タスク、イシュー、時間、割り当て、プログラム、ポートフォリオなど、あらゆるWorkfrontオブジェクトと連携するために使用する汎用的なアクションです。

| タイトル | ツール名 | 機能 |
|---|---|---|
| オブジェクトを検索 | `workflow_search_any_object` | 柔軟なフィルターパラメーター、順序付け、ページネーションを使用して、Workfront オブジェクトを検索します。 |
| オブジェクトを作成 | `workflow_create_any_object` | プロジェクト、タスク、イシュー、時間、割り当て、プログラム、ポートフォリオなどの新しいWorkfront オブジェクトを作成します。 |
| オブジェクトを更新 | `workflow_update_any_object` | 既存のWorkfront オブジェクトのフィールドを更新します。 |
| オブジェクトを削除 | `workflow_delete_any_object` | IDでWorkfront オブジェクトを削除します。 アクションを実行する前に、明示的なユーザー確認が必要です。 |
| フィールド名を解決 | `workflow_resolve_field_names_any_object` | ユーザーが提供したフィールド名またはラベルを、基礎となるWorkfront API フィールド名に変換します。これにより、AI エージェント基盤は正確なリクエストを構築できます。 |

## ツールの更新方法

Adobeが新しいバージョンのWorkfront MCP サーバーをリリースすると、AI エージェンティックプラットフォームは新しいツールセットを自動的に使用します。 システムに再接続したり、変更を加えたりする必要はありません。
