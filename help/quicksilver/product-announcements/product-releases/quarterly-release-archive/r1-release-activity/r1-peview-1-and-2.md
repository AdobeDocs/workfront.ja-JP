---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 プレビュー 1 および 2
description: このページでは、R1.1 および R1.2 リリースのプレビュー環境で使用できるすべての変更点について説明します。このページに記載されている機能は、2017年1月19日（PT）にプレビュー環境で使用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 98%

---

# R1 プレビュー 1 および 2

このページでは、R1.1 および R1.2 リリースのプレビュー環境で使用できるすべての変更点について説明します。このページに記載されている機能は、2017年1月19日（PT）にプレビュー環境で使用できるようになりました。

R1 で行われたすべての変更のリストについては、[R1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md)を参照してください。

## ごみ箱からのプロジェクト、タスク、イシューの復元

Workfront 管理者は、過去 30 日以内に削除されたプロジェクト、タスクおよびイシューを復元できるようになりました。ドキュメントやカスタムデータなど、プロジェクト、タスクまたはイシューに関連するすべての情報が復元されます。

また、削除されたプロジェクト、タスクまたはイシューに対して記録されている時間数への影響を設定するための新しいオプションも使用できます。詳しくは、[オブジェクトが削除および復元された場合の時間数に対する影響の設定](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md)を参照してください。

Workfront でのオブジェクトの復元について詳しくは、[削除した項目の復元](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

最近復元されたプロジェクト、タスクおよびイシューを表示する方法については、[復元された項目の表示](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md)を参照してください。

## 過去、現在および将来の承認ステップを視覚的に表現する承認ダイアグラム

プロジェクト、タスクまたはイシューの承認が保留中の場合に、ダイアグラムが表示されるようになりました。承認ダイアグラムには、承認プロセスの現在のステップ（保留中）が表示されます。また、「承認」タブに移動することなく、過去および将来の承認ステップをすばやく表示できます。

この変更以前は、承認ステップに関する情報は、プロジェクト、タスクまたはイシュー内の「承認」タブでのみ入手可能で、ダイアグラムビューではなくリストビューにのみ表示されていました。（この情報は「承認」タブで引き続き入手でき、変更されません）。

プロジェクトに関しては、承認情報は、プロジェクトタイトルの横のヘッダーに表示されます。タスクおよびイシューに関しては、承認情報は右パネルに表示されます。

詳しくは、[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)の[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

## 承認保留中のオブジェクトを更新するように設定

プロジェクト、タスクまたはイシューが承認保留中の場合、ユーザーによる以下の操作が可能かどうかを設定できるようになりました。

* 承認保留中のプロジェクト、タスクまたはイシューのカスタムフォームを編集する。\
  承認保留中の場合に編集できるようにプロジェクト、タスクおよびイシューを設定する方法については、[グローバル承認設定の指定](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)を参照してください。

* 承認保留中のプロジェクトにイシューを追加する。\
  プロジェクトが承認保留中の場合にユーザーがイシューを追加できるようにプロジェクトを設定する方法については、[システム全体のプロジェクト環境設定の指定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

* 承認保留中のプロジェクト内でタスクやイシューを編集する。\
  プロジェクトが承認保留中の場合にユーザーがタスクやイシューを編集できるようにプロジェクトを設定する方法については、[システム全体のプロジェクト環境設定の指定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

この変更以前は、承認保留中のプロジェクト、タスクおよびイシューを編集できませんでした。また、承認保留中のプロジェクトにイシューを追加したり、承認保留中のプロジェクト内でタスクやイシューを編集したりすることはできませんでした。

## グループへのレイアウトテンプレートの割り当て

レイアウトテンプレートをグループに割り当てることができるようになりました。

この変更以前は、レイアウトテンプレートをユーザー、チームおよび担当業務に割り当てることができました。レイアウトテンプレートをグループに割り当てると、レイアウトテンプレートの割り当て優先度が最も低くなります。 

詳しくは、「レイアウトテンプレートの作成と管理」を参照してください。

## ユーザー通知の一括編集に関する変更

ユーザーのメール通知設定の一括編集に関する機能が変更されました。複数のユーザーを選択してそのメール通知設定を編集する場合、選択したすべてのユーザーに対して、更新する特定の通知のみが変更されます。変更されていないメール通知設定はすべて、ユーザーごとに異なる場合でも、選択したすべてのユーザーについては同じままです。 

この変更以前は、選択したメール通知設定が保存され、変更を保存すると、変更されていないその他の通知設定はすべて選択解除されていました。 

詳しくは、 [独自の電子メール通知を変更する](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 一部のメール通知のルックアンドフィールの更新

次のメール通知のルックアンドフィールが更新されて、新しい UI が反映されました。

* イシュー割り当て
* コミット日の変更
* 自分が参加するプロジェクトの状況がアクティブになった
* 関係者に対する承認決定
* 依存タスクに対する先行タスクの完了
* 承認保留中（プロジェクト、タスク、イシュー）
* プロジェクト、タスク、イシューに関するステータスの変更

プレビューサンドボックスがすべてのユーザーのメールアドレスをクリアするので、この機能をテストできるように、アカウントに関連付けられたメールアドレスを必ず更新してください。メール通知について詳しくは、[Adobe Workfront 通知](../../../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## 複数の通知領域に対応する新しいメールダイジェストオプション

次の通知領域に「日刊ダイジェスト」オプションが追加されました。

* 参加プロジェクトに関する情報
* スポンサーしているプロジェクトに関する情報
* 承認情報
* 担当割り当てされている作業に関する情報
* コミュニケーション

詳しくは、[Adobe Workfront 通知](../../../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。プレビューサンドボックスがすべてのユーザーのメールアドレスをクリアするので、この機能をテストできるように、アカウントに関連付けられたメールアドレスを必ず更新してください。

## グループの公開

グループを公開する際に、グループの所有者にならずにそのグループをユーザーに追加できるようになりました。ユーザーを編集するには、ユーザー管理者アクセス権が必要です。

グループの公開について詳しくは、[グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)の[グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public)の節を参照してください。

## モバイルアプリでのオブジェクトの URL の共有

Workfront モバイルアプリで次のオブジェクトの URL を共有できるようになりました。

* プロジェクト
* タスク
* イシュー
* タイムシート
* ドキュメント

次のアプリケーションでオブジェクトの URL を共有できます。

* テキストメッセージ
* メール
* ストレージドライブ（例：iCloud ドライブ）
* 別のインストール済みアプリケーション（例：Notes、Facebook）
* オブジェクトへのリンクをクリップボードにコピーし、後で他のアプリケーションに貼り付けることができます。 

## 設定のコンテキスト依存ヘルプ

設定メニューのすべての領域が更新されて、領域の右上隅にヘルプアイコンが表示されるようになりました。このアイコンは、その領域に関するヘルプサイト記事へのリンクを提供します。「設定」領域内の一部のセクションにも、ヘルプアイコンが付加されています。 

## より正確な費用率の追加

費用タイプを作成する際に、より正確な費用率を追加できるようになりました。費用率には、小数点以下 4 桁までを含めることができます（例：1.0375）。つまり、この率を使用するすべてのフィールドの精度を高めることができます。

この変更以前は、費用率に小数点以下 2 桁までしか含めることができませんでした（例：1.03）。

費用率の作成について詳しくは、[カスタム費用タイプの作成](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)を参照してください。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1 プレビュー 1 および 2 リリースのウェビナーの録画

このウェビナーは、2017年1月19日（PT）に Workfront リリース準備チームによって実施されました。このウェビナーでは、2017年のリリースの変更点に重点を置き、プレビューでテストできる新機能について説明しています。
