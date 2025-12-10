---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: ライセンス タイプ別のオブジェクトと領域へのアクセス
description: 次の表に、各 Adobe Workfront ライセンスで Workfront のオブジェクトとエリアに対して許可されている最高レベルのアクセス（編集または表示）を示します。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 78%

---

# オブジェクトやエリアへのアクセス権（ライセンスタイプ別）

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>この記事では、従来のアクセスレベルについて説明します。 現在のアクセスレベルについて詳しくは、[ 新しいアクセスレベルの概要 ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) を参照してください。

次の表に、各 Adobe Workfront ライセンスで Workfront のオブジェクトとエリアに対して許可されている最高レベルのアクセス（編集または表示）を示します。

* 表示：ユーザーは、項目を確認し、共有できます。
* 編集：ユーザーは、項目を作成、編集、削除、共有できます。

  >[!NOTE]
  >
  >別のユーザーがオブジェクトを共有する場合、共有者はそのオブジェクトの編集を制限する権限を指定できます。新しいライセンスタイプについて詳しくは、[ オブジェクトに対する共有権限の概要 ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md) を参照してください。

  >[!NOTE]
  >
  >この記事には、従来のライセンスタイプのオブジェクトアクセスに関する情報が含まれています。 新しいライセンスタイプについては、[ 新しいアクセスレベルの概要 ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) および [ 新しいライセンスの概要 ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) を参照してください。

|   | プラン | ワーク | レビュー | リクエスト | 外部 |
|---|---|---|---|---|---|
| プロジェクト | 編集 | 編集（作成権限なし） | 表示 | 表示（詳細ページのみ） | アクセスなし |
| タスク | 編集 | 編集 | 表示 | 表示 | アクセスなし |
| イシュー | 編集 | 編集 | 編集 | 編集 | アクセスなし |
| ポートフォリオ | 編集 | 表示 | 表示 | アクセスなし | アクセスなし |
| プログラム | 編集 | 表示 | 表示 | アクセスなし | アクセスなし |
| レポート、ダッシュボード、カレンダー | 編集 | 表示 | 表示 | 表示&#42; | 表示（カレンダーの場合のみ、共有権限なし） |
| フィルター、ビュー、グループ化 | 編集 | 編集 | 編集 | 編集 | アクセスなし |
| ドキュメント | 編集 | 編集 | 編集 | 編集 | 表示（共有権限なし） |
| ユーザー | 編集 | 表示 | 表示 | 表示 | 表示 |
| チーム | 編集 | 編集 | 表示 | 表示 | アクセスなし |
| テンプレート | 編集 | アクセスなし | アクセスなし | アクセスなし | アクセスなし |
| 財務データ | 編集 | 表示（プロジェクト詳細の財務エリアのみ） | 表示 | アクセスなし | アクセスなし |
| リソース管理 | 編集 | 表示 | 表示 | アクセスなし | アクセスなし |
| シナリオプランナー | 編集 | 編集 | 編集 | アクセスなし | アクセスなし |
| Workfront Goals | 編集 | 編集 | 編集 | 編集 | アクセスなし |

&#42;リクエストライセンスを持つユーザーは、自分と共有されているレポート、ダッシュボードおよびカレンダーのみを表示できます。

>[!NOTE]
>
>レビューライセンスまたはリクエストライセンスを持つユーザーの共有機能は制限されています。 詳しくは、[ライセンスの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)を参照してください。
>
>外部ユーザーは Workfront で項目を検索できません。外部ユーザーは、個別に共有されているドキュメントやカレンダーを表示できます。また、項目を共有しているユーザーを表示できます。

アクセスレベルで各オブジェクトおよびエリアに対して許可される操作について詳しくは、以下の記事を参照してください。

* [プロジェクトへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [タスクへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [イシューへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [ドキュメントへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [ポートフォリオへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [プログラムへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [レポート、ダッシュボード、カレンダーへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [フィルター、ビュー、およびグループ化に対するアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [ユーザーへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [チームに対するアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [テンプレートへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [財務データへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [リソース管理へのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [シナリオプランナーへのアクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Adobe Workfront Goals へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
