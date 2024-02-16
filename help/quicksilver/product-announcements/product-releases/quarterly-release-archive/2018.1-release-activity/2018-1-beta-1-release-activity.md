---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 ベータ版 1 リリースアクティビティ
description: このページでは、2018.1 ベータ 1 リリースのプレビュー環境で最近使用されたすべての変更について説明します。このページの機能は、2017年12月1日（PT）にプレビュー環境で使用できるようになりました。2018年3月（PT）に、実稼動環境で利用できるようになります。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: efcc2217-ab69-4ac4-8e9a-f811eba77d49
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 100%

---

# 2018.1 ベータ版 1 リリースアクティビティ

このページでは、2018.1 ベータ 1 リリースのプレビュー環境で最近使用されたすべての変更について説明します。このページの機能は、2017年12月1日（PT）にプレビュー環境で使用できるようになりました。2018年3月（PT）に、実稼動環境で利用できるようになります。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018年1月に行われたすべての変更のリストについては、[2018.1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)を参照してください。

2018.1 ベータ 1 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [ホームエリアをサポートするようにレイアウトテンプレートをアップデートしました](#updated-layout-template-to-support-the-home-area)
* [Workfront から送信されたプルーフメール通知を無効にする](#disable-proofing-email-notifications-sent-from-workfront)
* [イベントサブスクリプションに追加された新しいリソース](#new-resources-added-to-event-subscriptions)

**すべてのユーザー向け**

* [ホームエリア（作業エリアをアップデート）](#home-area-updated-my-work-area)
* [ビジネスケースと更新されたビジネスケースの概要の下にリソースプランナーデータを表示する](#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary)
* [リソースプランナーに予定時間配分の割合を表示する](#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner)
* [「自動および変更時」と「変更時のみ」の更新タイプトリガーは、タスクが更新されると同時に親オブジェクトに対して更新される](#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated)
* [ガントチャートで使用可能なタイムラインスナップショット](#timeline-snapshot-available-in-the-gantt-chart)

## ホームエリア（作業エリアのアップデート） {#home-area-updated-my-work-area}

新しいホームエリアは、担当作業エリアで現在使用可能な同じデータに対して、代替の拡張ビューを提供します。ホームエリアは、担当作業エリアにおいて次のようなメリットがあります。

* より合理化された直感的なインターフェイス
* パフォーマンスの向上
* リッチテキストの書式設定を使用したタスクと問題の更新

## ホームエリアをサポートするようにレイアウトテンプレートを更新 {#updated-layout-template-to-support-the-home-area}

Workfront 管理者は、組織内のユーザーに割り当てられたレイアウトテンプレートを設定することで、ユーザーがホームエリアにアクセスできるかどうかを決定できます。レイアウトテンプレートを割り当てられていないユーザーは、常にホームエリアにアクセスできます。

詳しくは、「レイアウトテンプレートの作成と管理」を参照してください。

## Workfront から送信されたプルーフメール通知を無効にする {#disable-proofing-email-notifications-sent-from-workfront}

プルーフにコメントを付けたときに、Workfront インスタンスのユーザーが Workfront からメール通知を受け取るかどうかを設定できるようになりました。

以前は、プルーフにコメントを付けると、常に Workfront からプルーフメールが送信されていました。Workfront Proof でも通知が有効になっている場合、ユーザーは重複して通知を受け取っていました。 

Workfront の既存のお客様の場合、プルーフにコメントが付けられるとメールが送信されるように Workfront ではデフォルトで設定されています。

Workfront でプルーフのメール通知を無効にして、Workfront Proof からのみプルーフメールが送信されるようにする方法については、次を参照してください。  

## ビジネスケースと更新されたビジネスケースの概要の下に、リソースプランナーデータを表示します。 {#display-resource-planner-data-under-the-business-case-and-updated-business-case-summary}

プロジェクトのビジネスケースで、リソース予算計上エリアが使用できるようになりました。このエリアでは、リソースプランナーのリソースの予算計上時間数と、それらに関連する予算労力コストを確認できます。

ビジネスケースの「リソース見積もり」エリアの名前が、「従来のリソース見積もり」に変更されました。

この変更の一環として、ビジネスケースの概要には、リソース見積もりとリソース予算計上の両方に基づく財務情報が含まれるようになりました。

この変更以前は、プロジェクトのビジネスケースに関するリソースプランナー情報を表示できませんでした。従来のリソースプールの処理能力プランナーで指定されたリソース見積もり情報のみが表示されます。

ビジネスケースの作成について詳しくは、[プロジェクトのビジネスケースの作成](../../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

## リソースプランナーに予定時間配分の割合を表示する {#display-the-percentage-of-planned-hour-allocation-in-the-resource-planner}

リソースプランナーのユーザービューに新しい列が追加され、予定時間配分を、ユーザーと担当業務の合計使用可能時間に対する割合として表示できるようになりました。

この変更以前は、ユーザーと担当業務に対する予定時間と使用可能時間の合計は別の列として表示されていました。

「予定時間数の割り当て率」列の詳細については、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)の「リソースプランナーでの利用可能時間と予定時間数または FTE の差の表示」節を参照してください。

## 「自動・変更時」と「変更時のみ」の更新タイプトリガーは、タスクが更新されると同時に親オブジェクトに対して更新される {#the-automatic-and-on-change-and-change-only-update-types-trigger-updates-to-the-parent-objects-at-the-same-time-as-tasks-are-updated}

プロジェクト内の下位レベルのオブジェクトが更新された場合の親タスクおよびプロジェクトの更新方法を変更しました。親オブジェクトが更新される時間は、プロジェクトの「更新タイプ」フィールドで決まります。次の更新タイプから選択できます。

* 自動/変更時
* 変更時のみ
* 自動のみ
* 手動のみ

「自動・変更時」または「変更時のみ」の更新タイプを選択すると、個々のタスクに適用した変更が親タスクとプロジェクトにも直ちに適用されるようになりました。

この変更を行う前は、親オブジェクトとプロジェクトのタイムラインを更新するにはページを更新する必要がありました。

プロジェクトの更新タイプについて詳しくは、[プロジェクトの更新タイプの選択](../../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。

## ガントチャートで使用可能なタイムラインスナップショット {#timeline-snapshot-available-in-the-gantt-chart}

ガントチャートで新しいタイムラインスナップショットを使用すると、プロジェクトの全期間の特定のポイントまですばやくスクロールできるようになりました。

タスクまたはプロジェクト一覧を表示しているときに、ガントチャートでより詳細な期間を選択すると、ガントチャートの下部に横スクロールバーが表示されます。スクロールバーをクリックすると、スナップショットにプロジェクトのタイムライン全体を表示できます。ガントチャートのスナップショット内の任意の場所をクリックして、プロジェクトの有効期間の特定のポイントに移動できます。

この変更を行う前は、ガントチャート全体を横にスクロールして特定の時点を見つける必要がありました。または、詳細ビューをズームアウトする必要がありました。

ガントチャートにおける情報の表示方法について詳しくは、[ガントチャートでの情報の表示方法の設定](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

## イベントサブスクリプションに追加された新しいリソース {#new-resources-added-to-event-subscriptions}

次のリソースのイベント購読を作成できます。

* **費用**：費用が追加または変更された場合に通知します。
* **割り当て**：ユーザー、担当業務、またはチームのタスクまたはイシューで割り当てが追加または変更された場合に通知します。
* **タイムシート**：タイムシートが送信、却下、または承認された場合に通知します。

イベント登録について詳しくは、[Event Subscription API](../../../../wf-api/general/event-subs-api.md)を参照してください。
