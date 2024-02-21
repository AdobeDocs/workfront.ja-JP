---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 プロジェクトの機能強化
description: このページでは、実稼動環境に対する 2020.2 リリースで行われたすべてのプロジェクトの機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 150bc838-d6a5-445a-af77-62c4ed74dd1b
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 100%

---

# 2020.2 プロジェクトの機能強化

このページでは、実稼動環境に対する 2020.2 リリースで行われたすべてのプロジェクトの機能強化について説明します。これらの機能強化は、2020年5月11日（PT）の週に実稼動環境で利用できるようになりました。

2020.2 リリースで利用可能なすべての変更点の一覧については、[2020.2 リリースの概要](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)を参照してください。

## Workfront 管理者向け：新規プロジェクトのステータスが非表示またはロック解除された場合の新しいフェールセーフ

セットアップで、プロジェクトの作成時にすべての新規プロジェクトが特定のステータスを持つように環境を設定します。Workfront でプロジェクトが正しく機能するには、プロジェクトが新しい場合でも、常にステータスが必要なので、これは重要です。

新規プロジェクトに常にステータスがあることを確実にするため、管理者が新規プロジェクトに設定されたステータスを非表示にしたりロックを解除したりした場合でも、新規プロジェクトに新たなステータスをもう一度設定するまで、システムはステータスリストの最初のステータスをすべての新規プロジェクトに割り当てるようになりました。

すべての新規プロジェクトのステータスに対する環境設定については、[システム全体のプロジェクト環境の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)（Adobe Workfront Classic を使用している場合は、[プロジェクト環境の設定](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298?lang=ja)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## Workfront 管理者向け：プロジェクト環境設定のデザインの向上

プロジェクト環境の設定をより直感的に使いやすくしました。

* タイトルはオプションラベルよりも大きくなり、探しているものをすばやく見つけることができます。
* 分割線と余白で各セクションが区切られ、作業に集中しやすくなります。
* 「1 日あたりの通常の勤務時間」などのオプションに無効な数値を入力すると、警告メッセージが、「保存」をクリックした後ではなく、すぐに表示されます。
* オプションラベルは、Workfront の他の場所（詳細エリアやレポートなど）にある、対応するインターフェイステキストに一致します。

プロジェクトの環境設定エリアについては、[システム全体のプロジェクト環境の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)（Adobe Workfront Classic を使用している場合は、[プロジェクト環境の設定](https://one.workfront.com/s/article/Setting-Project-Preferences-1883392298?lang=ja)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## レポートリストで保持される、選択したフィルター、ビュー、グループ化

現在は、ユーザーが Workfront をログアウトしてから再度ログインした場合でも、特定のレポートに適用した最後のフィルター、ビュー、グループが選択されます。

以前は、ユーザーがフィルター、ビュー、グループをレポートリストに適用し、そのページから移動すると、次にその同じレポートに移動したときには、デフォルトのフィルター、ビュー、グループが表示されていました。

**利用可能な環境：**

* 新しい Adobe Workfront エクスペリエンス
* Adobe Workfront Classic

## タスクを別のプロジェクトに移動したりコピーしたりすると、タスクがプロジェクトのタイムライン内に収まる場合、タスクの制約が維持されます

タスクをコピーしたり、別のプロジェクトに移動したりする際に、Workfront が日付特有のタスクの制約を処理する方法を向上しました。日付固有のタスクの制約の例としては、必須開始日、必須終了日、固定日、遅くとも開始する日があります。

例えば、必須開始日の制約があるタスクを、予定開始日がそのタスクの開始日より早い別のプロジェクトに移動またはコピーすると、そのタスクはコピーまたは移動後も制約を保持します。必須開始日の制約があるタスクを、予定開始日がそのタスクの開始日より遅い別のプロジェクトに移動またはコピーすると、そのタスクの制約は「できるだけ早く」に変わります。

この変更を行う前は、タスクの制約は常に「できるだけ早く」に変わります。

タスクの移動については、[タスクを移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)（Adobe Workfront Classic を使用している場合は、[タスクを移動](https://one.workfront.com/s/article/Moving-Tasks-2081996259?lang=ja)）を参照してください。

タスクのコピーについては、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)（Adobe Workfront Classic を使用している場合は、[タスクのコピーと複製](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605?lang=ja)）を参照してください。

すべてのタスクの制約の概要については、[タスクの制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)（Adobe Workfront Classic を使用している場合は、[タスクの制約の概要](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848?lang=ja)）を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

## 詳細タブまたはタスクリストで変更を加える際にデータが失われるのを防ぐ

プロジェクトレベルのタスクリストにあるオブジェクトやタスクの詳細ページの情報を更新して、変更を手動で保存する際、未保存の変更があることを知らせる警告メッセージを表示して、データが失われるのを防ぎます。変更を保存する前に実行できるアクションは、お気に入りにオブジェクトをサブスクライブまたは追加するだけです。

リスト内のタスクの編集について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

**利用可能な環境：**

* 新しい Adobe Workfront エクスペリエンス

