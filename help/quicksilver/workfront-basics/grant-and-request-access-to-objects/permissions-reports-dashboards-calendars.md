---
title: レポート、ダッシュボード、カレンダーの共有
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront管理者がアクセスレベルを割り当てる際に、ユーザーにレポート、ダッシュボードおよびカレンダーの表示や編集のアクセス権を付与します。 レポート、ダッシュボード、およびカレンダーへのアクセス権の付与の詳細については、「レポート、ダッシュボード、およびカレンダーへのアクセス権の付与」を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# レポート、ダッシュボード、カレンダーの共有

Adobe Workfront管理者がアクセスレベルを割り当てる際に、ユーザーにレポート、ダッシュボードおよびカレンダーの表示や編集のアクセス権を付与します。 レポート、ダッシュボード、およびカレンダーへのアクセス権の付与について詳しくは、 [レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

ユーザーに付与されるアクセスレベルに加えて、共有にアクセスできる特定のレポート、ダッシュボード、またはカレンダーの表示または管理の権限をユーザーに付与することもできます。 オブジェクトに対するユーザー共有権限の付与については、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

各アクセスレベルのユーザーが問題に対してどのような処理を行うかについては、「 [レポート](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) 記事内 [各オブジェクトタイプで使用できる機能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## レポート、ダッシュボード、カレンダーの共有に関する考慮事項

以下の考慮事項に加えて、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理者は、システム内のすべてのユーザーに対して、それらの項目の所有者にならずに、システム内の項目に対する権限を追加または削除できます。

* レポート、ダッシュボードまたはカレンダーの作成者には、デフォルトで、自分に対する管理権限が付与されています。
* レポート、ダッシュボード、カレンダーの共有は、Workfrontで他のオブジェクトを共有する場合と似ています。

   Workfrontでオブジェクトを共有する方法について詳しくは、 [オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

   レポート、ダッシュボード、カレンダーの共有方法については、次の記事も参照してください。

   * [Adobe Workfrontでのレポートの共有](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [ダッシュボードの共有](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [カレンダーレポートの共有](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* レポートやダッシュボードは個別に共有することも、一括で共有することもできます。

   カレンダーは個別にのみ共有できます。 一括で共有することはできません。

* 組み込みのシステムレポートを共有することはできません。 共有できるのは、カスタムレポートのみです。

   システムレポートを新しいカスタムレポートとして保存する方法については、 [レポートのコピーの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

* レポート、ダッシュボードおよびカレンダーに次の権限を付与できます。

   * ビュー

      ![](assets/screen-shot-2014-01-22-at-10.19.55-am.png)

   * 管理

      ![](assets/screen-shot-2014-01-22-at-10.20.13-am.png)

* ダッシュボードを共有すると、ユーザーはデフォルトで、ダッシュボード上のすべてのレポート、カレンダーおよび外部ページに対する表示権限を持ちます。
* リクエストライセンスを持つユーザーは、システム全体のレポートを表示できません。 レポートを表示する必要がある場合は、そのレポートをリクエスターと個別に共有する必要があります。
* プロンプトが表示され、公開されているレポートを共有する場合は、そのプロンプトを使用してレポートを実行できるように、Workfrontにレポートにアクセスするユーザーがログインする必要があります。 Workfrontにログインできない場合は、プロンプトが表示されずにレポートが表示されます。\
   プロンプトを使用したレポートの共有に関する制限の詳細については、「 [プロンプトレポートの共有に関する制限](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) 記事内 [レポートにプロンプトを追加する](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* レポートまたはカレンダーから継承された権限を削除できます。

   継承された権限をオブジェクトから削除する方法について詳しくは、 [オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

* また、レポートやカレンダーを公開またはシステム全体で共有することもできます。

   ダッシュボードを公開して共有することはできませんが、システム全体で共有することはできます。

   >[!CAUTION]
   >
   >機密情報を含むオブジェクトを外部のユーザーと共有する場合は、慎重におこなうことをお勧めします。 これにより、Workfrontのユーザーや組織の一員でなくても、ユーザーは情報を表示できます。
