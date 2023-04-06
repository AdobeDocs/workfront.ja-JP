---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: ライセンスタイプ別のオブジェクトおよび領域への従来のアクセス
description: 次の表に、Adobe Workfrontの各レガシーライセンスでWorkfrontのオブジェクトと領域に対して許可されている最高レベルのアクセス（編集または表示）を示します。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 19%

---

# ライセンスタイプ別のオブジェクトおよび領域への従来のアクセス

次の表に、各Adobe WorkfrontライセンスでWorkfrontのオブジェクトと領域に対して許可されているレガシーアクセス（編集または表示）の最高レベルを示します。

* **表示**:ユーザーは、項目を確認および共有できます。
* **編集**:ユーザーは、項目の作成、編集、削除、共有をおこなうことができます。

   >[!NOTE]
   >
   >別のユーザーがオブジェクトを共有する場合、共有者はそのオブジェクトを編集できる権限を制限する権限を指定できます。 詳しくは、 [オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | 計画 | 作業 | 確認 | リクエスト | 外部 |
|---|---|---|---|---|---|
| プロジェクト | 編集 | 編集（作成権限なし） | ビュー | 表示（詳細ページのみ） | アクセスなし |
| タスク | 編集 | 編集 | ビュー | ビュー | ビュー |
| 問題 | 編集 | 編集 | 編集 | 編集 | アクセスなし |
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
>レビューライセンスまたはリクエストライセンスを持つユーザーは、共有機能に制限があります。 詳しくは、 [Adobe Workfrontライセンスの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md) または [Adobe Workfrontレガシーライセンスの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>外部ユーザーはWorkfrontで項目を検索できません。 ユーザーは、特別に共有されているドキュメントやカレンダーを表示できます。 また、アイテムを共有しているユーザーを表示することもできます。

各オブジェクトおよび領域に対してレガシーアクセスレベルで許可される内容に関する詳細は、次の記事を参照してください。

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
