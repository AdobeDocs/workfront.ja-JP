---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 新しいライセンスによるオブジェクトやエリアへのアクセス
description: 次の表に、各 Adobe Workfront ライセンスで Workfront のオブジェクトとエリアに対して許可されている最高レベルのアクセス（編集または表示）を示します。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: aefa43697ae0d4edd5300acb94a9880b3cd0c94f
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 100%

---

# 新しいライセンスによるオブジェクトやエリアへのアクセス

<!-- Audited: 2/2024 -->

次の表に、各 Adobe Workfront ライセンスで Workfront のオブジェクトとエリアに対して許可されている最高レベルのアクセス（編集または表示）を示します。

* **表示**：ユーザーは項目を確認し共有できます。
* **編集**：ユーザーは項目の作成、編集、削除および共有ができます。

  >[!NOTE]
  >
  >別のユーザーがオブジェクトを共有する場合、共有者はそのオブジェクトの編集を制限する権限を指定できます。詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>標準</td>
        <td>ライト</td>
        <td>コントリビューター</td>
        <td>外部</td>
    </tr>
    <tr>
        <td>プロジェクト</td>
        <td>編集</td>
        <td>表示</td>
        <td>表示</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>タスク</td>
        <td>編集</td>
        <td>表示</td>
        <td>表示</td>
        <td>表示</td>
    </tr>
    <tr>
        <td>イシュー</td>
        <td>編集</td>
        <td>編集</td>
        <td>編集</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>ポートフォリオ</td>
        <td>編集</td>
        <td>表示</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>プログラム</td>
        <td>編集</td>
        <td>表示</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>レポート、ダッシュボード、カレンダー</td>
        <td>編集</td>
        <td>表示</td>
        <td>ビュー*</td>
        <td>表示（カレンダーの場合のみ、共有権限なし）</td>
    </tr>
    <tr>
        <td>フィルター、ビュー、グループ化</td>
        <td>編集</td>
        <td>編集</td>
        <td>編集</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>ドキュメント</td>
        <td>編集</td>
        <td>編集</td>
        <td>編集</td>
        <td>表示（共有権限なし）</td>
    </tr>
    <tr>
        <td>ユーザー</td>
        <td>編集</td>
        <td>表示</td>
        <td>表示</td>
        <td>表示</td>
    </tr>
    <tr>
        <td>チーム</td>
        <td>編集</td>
        <td>表示</td>
        <td>表示</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>テンプレート</td>
        <td>編集</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>財務データ</td>
        <td>編集</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>リソース管理</td>
        <td>編集</td>
        <td>表示</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>シナリオプランナー</td>
        <td>編集</td>
        <td>表示</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>編集</td>
        <td>編集</td>
        <td>編集</td>
        <td>アクセスなし</td>
    </tr>
</table>

&#42; 投稿者ライセンスを持つユーザーは、自分と共有されているレポート、ダッシュボード、およびカレンダーのみを表示できます。

>[!NOTE]
>
>ライトライセンスまたは投稿者ライセンスを持つユーザーは、共有機能に制限があります。詳しくは、[ライセンスの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)を参照してください。
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
