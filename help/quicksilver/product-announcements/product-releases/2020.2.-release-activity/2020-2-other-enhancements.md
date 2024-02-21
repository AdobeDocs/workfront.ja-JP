---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 のその他の機能強化
description: このページでは、2020.2 リリースで実稼動環境に追加されたその他すべての機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 100%

---

# 2020.2 のその他の機能強化

このページでは、2020.2 リリースで実稼動環境に追加されたその他すべての機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。

2020.2 リリースで利用可能なすべての変更点の一覧については、[2020.2 リリースの概要](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)を参照してください。

## Workfront 管理者向け：Workfront Classic で作成された新しいレイアウトテンプレートを、新しい Workfront エクスペリエンスで使用できるようになりました。

2019年秋以降に Workfront Classic で作成されたレイアウトテンプレートを、新しい Workfront エクスペリエンスで使用できるようになりました。新しい Workfront エクスペリエンスでこれらのレイアウトテンプレートを更新して、新しい機能を活用し、その環境のユーザーが最大限に使えるようにするのは良いことです。

詳しくは、[レイアウトテンプレート](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)を参照してください。

**利用可能な環境：**

* 新しい Adobe Workfront エクスペリエンス

## グループ固有の承認プロセスは、すべてのオブジェクトで使用できます。

グループに固有の承認プロセスを十分に活用するために、これらのオブジェクトを編集する際に、タスク、イシューおよびプロジェクトに承認プロセスを追加できるようになりました。

リクエストキューやキュートピックを設定するときに、イシューだけでなく、「プロジェクトを編集」ボックスのタスクエリアにあるタスクでも、グループ固有の承認プロセスを自動的に添付することができます。

プロジェクト、タスクおよびイシューに承認プロセスを追加する方法については、次の記事を参照してください。

* [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)
* [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [イシューを編集](../../../manage-work/issues/manage-issues/edit-issues.md)
* [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [キュートピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## カスタムステータスを使用したグループの承認プロセスの作成

グループで独自のワークフローを容易に管理できるように、承認プロセスでグループ固有のカスタムステータスを使用できるようになりました。

以前は、グループ固有の承認プロセスで、グループ独自のカスタムステータスを使用することはできませんでした。システム全体のステータスのみが使用可能で、これらが常にグループ承認プロセスに適合しているとは限りませんでした。

カスタムステータスは、1 回限りの承認プロセスおよびシステム全体の承認プロセスの両方で使用できるようになりました。

* オブジェクト（プロジェクト、タスクまたはイシュー）に対して1 回限りの承認プロセスを作成し、そのオブジェクトの作業グループに関連するステータスのベースにします。グループに関連付けられているカスタムステータスも含まれます。
* グローバル承認プロセスを作成し、そのグループのみ、またはシステム内の全員が利用できるようにします。

承認プロセスへの管理者アクセス権を持つユーザーの場合、承認プロセスの設定に関する情報は、[作業アイテムの承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)にあります（Adobe Workfront Classic を使用している場合は、[承認プロセスの作成](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)を参照してください）。

ユーザーの場合、承認プロセスと作業アイテムの関連付けに関する情報は、[新規または既存の承認プロセスを作業に関連付ける](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)にあります（Adobe Workfront Classic を使用している場合は、[新規または既存の承認プロセスと作業の関連付け](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)を参照してください）。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## 検索用の新しいオーバーレイページ

新しい Workfront エクスペリエンスで、ユーザーが検索ページと以前のページをより快適に行き来できるよう、画面を部分的に覆う検索オーバーレイページを追加しました。

これで、検索メニューの「詳細検索」をクリックしたり、基本検索を実行したりすると、画面の右側からページスライドが開きます。

詳しくは、[Adobe Workfront を検索](../../../workfront-basics/navigate-workfront/search/search-workfront.md)を参照してください。

**利用可能な環境：**

* 新しい Adobe Workfront エクスペリエンス

## イベント登録のアップデート

ユーザーがイシューの判断、トラブルシューティングおよび解決をしやすくするために、動作を修正し、Event Subscriptions API にさらに多くのデータを追加しました。また、次の変更も行いました。

* 基礎となるメッセージング技術の移行
* サービスを再構築して、複雑な依存関係を低減し、より効率的に拡張できるようにしました。
* 監視と警告に関する改善

詳しくは、[FAQ - イベント登録](../../../wf-api/general/event-subs-faq.md)と[イベント登録のベストプラクティス](../../../wf-api/general/event-sub-best-practice.md)を参照してください。
