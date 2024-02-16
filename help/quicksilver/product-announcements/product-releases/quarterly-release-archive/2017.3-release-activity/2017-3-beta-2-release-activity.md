---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta 2 リリースアクティビティ
description: このページでは、2017.3 Beta 2 リリース（PT）でプレビュー環境で最近使用されたすべての変更について説明します。このページの機能は、2017年8月23日にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f3293166-ef91-4623-828b-9530d746296d
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 100%

---

# 2017.3 Beta 2 リリースアクティビティ

このページでは、2017.3 Beta 2 リリース（PT）でプレビュー環境で最近使用されたすべての変更について説明します。このページの機能は、2017年8月23日にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017年3月に行われたすべての変更のリストについては、[2017.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)を参照してください。

2017.3 Beta 2 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [ステージのアクティベーションによるワークフローへのアクセス制限（Workfront Proof）](#restrict-access-to-workflows-by-stage-activation-workfront-proof)

**すべてのユーザー向け**

* [表示を変更する「リソースプランナー」オプション](#resource-planner-option-to-change-the-view)
* [プロジェクトの稼働率レポート内のコンテンツのフィルタリング](#filter-content-within-a-utilization-report-on-a-project)
* [プロジェクトの稼働率レポートでのコスト情報の表示](#view-cost-information-in-the-utilization-report-on-a-project)
* [ユーザーの項目の登録と登録解除](#subscribing-and-unsubscribing-users-to-items)
* [レポートまたはビューでのサブスクライバーリストの表示](#viewing-the-subscriber-list-in-a-report-or-view)
* [通信メールの新しい外観](#new-look-for-communication-emails)

## 表示を変更する「リソースプランナー」オプション {#resource-planner-option-to-change-the-view}

リソースプランナーで、担当業務別にリソースの割り当てと空き時間を表示できるようになりました。このオプションを選択すると、最初にリソースプランナーを担当業務別に表示し、次に各担当業務を展開して関連プロジェクトを表示し、次にプロジェクトを展開して、担当業務とプロジェクトに関連するユーザーを表示できます。この表示を使用すると、関連付けられているプロジェクトに関係なく、最初にすべての担当業務を予算で割り当てやすくなります。

この変更が行われる前は、プロジェクト、担当業務、ユーザーの順でしか、リソースプランナーの情報を表示できませんでした。

リソースプランナーでのリソース計画について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## レポートリストに関するダッシュボード情報

>[!NOTE]
>
>この機能は、プレビューで一時的に無効になっています。

レポートオブジェクトのレポートおよびリストで「ダッシュボード」フィールドが使用できるようになりました。このフィールドは、レポートオブジェクトのレポートとリストの表示とフィルターで使用できます。表示に追加されると、レポートが追加されたダッシュボードのリストが表示されます。

この変更以前は、レポートがダッシュボードにリストされているかどうかを確認できませんでした。レポートの管理について詳しくは、[レポートへのアクセスと整理](../../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md)の[レポートへのアクセスと整理](../../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md)を参照してください。

## プロジェクトの稼働率レポート内のコンテンツのフィルタリング {#filter-content-within-a-utilization-report-on-a-project}

プロジェクトの稼働率レポートに表示される内容をフィルタリングできます。

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## プロジェクトの稼働率レポートでのコスト情報の表示 {#view-cost-information-in-the-utilization-report-on-a-project}

時間情報に加えて、稼働率レポート内にコスト情報を表示できるようになりました。

この変更以前は、稼働率レポートには時間情報のみが表示されていました。

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## ユーザーの項目の登録と登録解除 {#subscribing-and-unsubscribing-users-to-items}

管理および共有権限を持つ項目の更新ストリームに登録することで、管理者や同業者を作業上で更新し続けることができます。

ユーザーが項目を登録または登録解除すると、項目の更新ストリームに対してレコードが自動的に作成されます。

登録すると、ユーザーは登録済みオブジェクトの更新ストリームにコメントが追加されるたびに、アプリ内通知を受け取ります。さらに、サブスクライバーは、メールおよびモバイル通知を受信するよう選択できます。

ユーザーのオブジェクトへの登録と登録解除について詳しくは、[Adobe Workfront の項目を登録](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)内の[Adobe Workfront の項目を登録](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)を参照してください。

## レポートまたはビューでのサブスクライバーリストの表示 {#viewing-the-subscriber-list-in-a-report-or-view}

サブスクライバー「フィールドをレポートまたは表示に追加すると、プロジェクト、タスク、またはイシューのサブスクライバーをすばやく表示できます。レポートまたはビューへのフィールドの追加について詳しくは、[Adobe Workfront の用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

## 通信メールの新しい外観 {#new-look-for-communication-emails}

コミュニケーションメールのルックアンドフィールが更新され、オブジェクトで行われたコミュニケーションに関するより多くのコンテキストが提供されます。コメントスレッドをすばやくフォローし、通信に含まれるユーザーを表示できるようになりました。

詳しくは、[Adobe Workfront 通知](../../../../workfront-basics/using-notifications/wf-notifications.md)の [Adobe Workfront 通知](../../../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## ステージのアクティベーションによるワークフローへのアクセス制限（Workfront Proof） {#restrict-access-to-workflows-by-stage-activation-workfront-proof}

>[!NOTE]
>
>このオプションは、スタンドアロンの Workfront Proof アプリケーションを使用する場合にのみ利用可能です。Workfront と統合された Workfront Proof インスタンスを使用する場合は利用できません。

Workfront Proof で、特定のステージに関連付けられたユーザーに対して、自動ワークフローを含むプルーフを表示するタイミングを設定できるようになりました。

ユーザーに表示されるプルーフを設定できます。

* プルーフが作成され次第。
* ユーザーが関連付けられているステージがアクティブになった後のみ。 
