---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: ライセンスタイプ別のオブジェクトや領域へのアクセス
description: 次の表に、各Adobe WorkfrontライセンスでWorkfrontのオブジェクトと領域に対して許可されている最高レベルのアクセス（編集または表示）を示します。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 20%

---

# ライセンスタイプ別のオブジェクトや領域へのアクセス

次の表に、各Adobe WorkfrontライセンスでWorkfrontのオブジェクトと領域に対して許可されている最高レベルのアクセス（編集または表示）を示します。

* **表示**：ユーザーは項目を確認および共有できます。
* **編集**：ユーザーは、項目の作成、編集、削除および共有ができます。

  >[!NOTE]
  >
  >別のユーザーがオブジェクトを共有する場合、共有者はそのオブジェクトを編集できる権限を制限する権限を指定できます。 詳しくは、 [オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | 計画 | 作業 | 確認 | リクエスト | 外部 |
|---|---|---|---|---|---|
| プロジェクト | 編集 | 編集（作成権限なし） | ビュー | 表示（詳細ページのみ） | アクセスなし |
| タスク | 編集 | 編集 | ビュー | ビュー | ビュー |
| イシュー | 編集 | 編集 | 編集 | 編集 | アクセスなし |
| ポートフォリオ | 編集 | ビュー | ビュー | アクセスなし | アクセスなし |
| プログラム | 編集 | ビュー | ビュー | アクセスなし | アクセスなし |
| レポート、ダッシュボード、カレンダー | 編集 | ビュー | ビュー | ビュー&#42; | 表示（カレンダーの場合のみ、共有権限なし） |
| フィルター、ビュー、グループ化 | 編集 | 編集 | 編集 | 編集 | アクセスなし |
| ドキュメント | 編集 | 編集 | 編集 | 編集 | 表示（共有権限なし） |
| ユーザー | 編集 | ビュー | ビュー | ビュー | ビュー |
| チーム | 編集 | 編集 | ビュー | ビュー | アクセスなし |
| テンプレート | 編集 | アクセスなし | アクセスなし | アクセスなし | アクセスなし |
| 財務データ | 編集 | 表示（「プロジェクトの詳細」の「財務」領域のみ） | ビュー | アクセスなし | アクセスなし |
| リソース管理 | 編集 | ビュー | ビュー | アクセスなし | アクセスなし |
| シナリオプランナー | 編集 | 編集 | 編集 | アクセスなし | アクセスなし |
| Workfront Goals | 編集 | 編集 | 編集 | 編集 | アクセスなし |

&#42; リクエストライセンスを持つユーザーは、自分と共有されているレポート、ダッシュボード、カレンダーのみを表示できます。

>[!NOTE]
>
>レビューライセンスまたはリクエストライセンスを持つユーザーは、共有機能に制限があります。 詳しくは、 [Adobe Workfrontライセンスの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>外部ユーザーはWorkfrontで項目を検索できません。 ユーザーは、特別に共有されているドキュメントやカレンダーを表示できます。 また、アイテムを共有しているユーザーを表示することもできます。

次の記事では、各オブジェクトおよび領域に対してアクセス・レベルで許可されるアクセス・レベルに関する詳細情報を示します。

* [プロジェクトへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [問題へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [ドキュメントへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [ポートフォリオへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [プログラムへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [フィルター、ビューおよびグループに対するアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [チームへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [テンプレートへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [リソース管理へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [シナリオプランナーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Adobe Workfront目標へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
