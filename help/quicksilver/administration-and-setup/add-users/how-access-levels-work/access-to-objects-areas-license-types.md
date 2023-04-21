---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 新しいライセンスを受けるために、によるオブジェクトや領域へのアクセス
description: 次の表に、各Adobe WorkfrontライセンスでWorkfrontのオブジェクトと領域に対して許可されている最高レベルのアクセス（編集または表示）を示します。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 18%

---

# 新しいライセンスを受けるために、によるオブジェクトや領域へのアクセス

次の表に、各Adobe WorkfrontライセンスでWorkfrontのオブジェクトと領域に対して許可されている最高レベルのアクセス（編集または表示）を示します。

* **表示**:ユーザーは、項目を確認および共有できます。
* **編集**:ユーザーは、項目の作成、編集、削除、共有をおこなうことができます。

   >[!NOTE]
   >
   >別のユーザーがオブジェクトを共有する場合、共有者はそのオブジェクトを編集できる権限を制限する権限を指定できます。 詳しくは、 [オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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
        <td>ビュー</td>
        <td>表示（詳細ページのみ）</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>タスク</td>
        <td>編集</td>
        <td>ビュー</td>
        <td>ビュー</td>
        <td>ビュー</td>
    </tr>
    <tr>
        <td>問題</td>
        <td>編集</td>
        <td>編集</td>
        <td>編集</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>ポートフォリオ</td>
        <td>編集</td>
        <td>ビュー</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>プログラム</td>
        <td>編集</td>
        <td>ビュー</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>レポート、ダッシュボード、カレンダー</td>
        <td>編集</td>
        <td>ビュー</td>
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
        <td>ビュー</td>
        <td>ビュー</td>
        <td>ビュー</td>
    </tr>
    <tr>
        <td>チーム</td>
        <td>編集</td>
        <td>ビュー</td>
        <td>ビュー</td>
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
        <td>ビュー</td>
        <td>アクセスなし</td>
        <td>アクセスなし</td>
    </tr>
    <tr>
        <td>シナリオプランナー</td>
        <td>編集</td>
        <td>ビュー</td>
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

&#42; 寄稿者ライセンスを持つユーザーは、自分と共有されているレポート、ダッシュボード、およびカレンダーのみを表示できます。

>[!NOTE]
>
>Light ライセンスまたは寄稿者ライセンスを持つユーザーは、共有機能に制限があります。 詳しくは、 [ライセンスの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
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
