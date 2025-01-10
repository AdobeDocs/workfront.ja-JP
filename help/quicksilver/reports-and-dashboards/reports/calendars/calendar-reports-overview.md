---
content-type: overview
product-area: calendars
navigation-topic: calendars-navigation-topic
title: カレンダーレポートの概要
description: カレンダーレポートは、作業内容を視覚的に表現する動的なレポートです。日付情報は、タスク、イシュー、プロジェクトのカレンダーレポートで表示できます。
author: Lisa
feature: Reports and Dashboards
exl-id: c65cf8ab-e37f-42a4-9a81-70962629e9ba
source-git-commit: d90459cb4f6fb1960552f0ab174e963582312b5c
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 99%

---

# カレンダーレポートの概要

<!-- Audited: 01/2024 -->

カレンダーレポートは、作業内容を視覚的に表現する動的なレポートです。次のオブジェクトの日付情報をカレンダーレポートに表示できます。

* タスク
* イシュー
* プロジェクト

[!DNL Adobe Workfront] のカレンダーレポートにアクセスできる権限は、アクセスレベルを通じて決定されます。カレンダーレポートの表示に必要なアクセス権について詳しくは、[レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)を参照してください。

## 独自のカレンダーを作成

次の場合に、[!DNL Workfront] は既定の個人用カレンダーを自動的に作成します。

* その他のカレンダーに対してアクセス権がない新規作成ユーザーが、初めてカレンダーレポートページにアクセスした場合

  または

* すべてのカレンダーを手動で削除してしまい、他のカレンダーにアクセスできない場合

>[!NOTE]
>
>システム全体の共有カレンダーや、自分で特別に共有したカレンダーなどの他のカレンダーにアクセスできる場合、個人用カレンダーは作成されません。

また、自分でカレンダーを作成したり、他のユーザーが共有しているカレンダーにアクセスしたりすることもできます。[!DNL Workfront] でアクセスできるカレンダーの数に制限はありません。

>[!NOTE]
>
>カレンダーレポートを作成するには、アクセスレベルに、[!UICONTROL レポート]、[!UICONTROL ダッシュボード]、[!UICONTROL カレンダー]に対する[!UICONTROL 編集]アクセス権が必要です。詳しくは、[!DNL Workfront] 管理者にお問い合わせください。

## 日付ごとに項目をグループ化する

各カレンダーレポート内で、カレンダーの焦点を絞るための項目のグループを作成できます。例えば、特定のプロジェクトのすべてのタスクの日付、現在プロジェクトで作業中のマーケティングチームメンバー、およびプロジェクトチームに割り当てられた期限切れのイシューを表示するカレンダーグループを作成できます。詳しくは、次の記事を参照してください。

* [カレンダーレポートで[!UICONTROL 予定日]を使用](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
* [カレンダーレポートで[!UICONTROL 見込み日]を使用](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
* [カレンダーレポートでのカスタム日付フィールドの使用](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)

>[!NOTE]
>
>カレンダーレポートの実行時に 504 エラーが発生した場合は、レポートで使用しているフィルターが多すぎる可能性があります。フィルターの数を減らすと、レポートを実行できます。
