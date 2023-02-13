---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 プレビュー 1 および 2
description: このページでは、R1.1 リリースと R1.2 リリースでプレビュー環境で使用できるすべての変更について説明します。 このページの機能は、2017 年 1 月 20 日にプレビュー環境で使用できるようになりました。
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# R1 プレビュー 1 および 2

このページでは、R1.1 リリースと R1.2 リリースでプレビュー環境で使用できるすべての変更について説明します。 このページの機能は、2017 年 1 月 20 日にプレビュー環境で使用できるようになりました。

R1 で行われたすべての変更のリストについては、 [R1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## ごみ箱からプロジェクト、タスク、および問題を復元する 

Workfront管理者は、過去 30 日以内に削除されたプロジェクト、タスクおよび問題を復元できるようになりました。 ドキュメントやカスタムデータを含め、プロジェクト、タスク、またはイシューに関連するすべての情報が復元されます。

また、プロジェクト、タスク、または削除された問題に対して記録される時間に対する影響を設定する新しいオプションも使用できます。 詳しくは、 [オブジェクトが削除され、復元される時間に対する影響を設定する](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Workfrontでのオブジェクトの復元について詳しくは、 [削除した項目を復元](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

最近復元されたプロジェクト、タスク、問題を表示する方法については、 [復元された項目を表示](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## 承認ダイアグラムに、前、現在および将来の承認ステップが視覚的に表示されます

プロジェクト、タスクまたはイシューで承認が保留中の場合に、ダイアグラムが表示されるようになりました。 承認ダイアグラムには、承認プロセスの現在のステップ（保留中）が表示されます。また、「承認」タブに移動することなく、前後の承認ステップをすばやく表示できます。

この変更以前は、承認手順に関する情報は、プロジェクト、タスクまたはイシュー内の「承認」タブでのみ表示され、ダイアグラムビューではなく、リストビューでのみ表示されていました。 （この情報は引き続き「承認」タブで使用でき、変更されません）。

プロジェクトでは、承認情報は、プロジェクトタイトルの横のヘッダーに表示されます。 タスクおよび問題に関しては、承認情報が右側のパネルに表示されます。

詳しくは、 [作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## 承認待ちの更新オブジェクトを設定

プロジェクト、タスクまたは問題が承認待ちの場合、ユーザーが以下を実行できるかどうかを設定できるようになりました。

* 承認待ちのプロジェクト、タスクまたはイシューのカスタムフォームを編集します。\
   承認待ちの場合に編集するプロジェクト、タスクおよび問題を設定する方法について詳しくは、 [グローバル承認設定の指定](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* 承認待ちのプロジェクトにイシューを追加します。\
   プロジェクトが承認待ちの場合にユーザーがイシューを追加できるようにプロジェクトを設定する方法について詳しくは、 [システム全体のプロジェクト環境設定の指定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 承認待ちのプロジェクト内のタスクと問題を編集します。\
   プロジェクトが承認待ちの場合にユーザーがタスクや問題を編集できるようにプロジェクトを設定する方法については、 [システム全体のプロジェクト環境設定の指定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

この変更がおこなわれる前は、承認待ちのプロジェクト、タスクおよびタスクを編集できませんでした。また、承認待ちのプロジェクトにイシューを追加できず、承認待ちのプロジェクト内でタスクとイシューを編集できなかった問題も修正されました。

## レイアウトテンプレートをグループに割り当てる

これで、レイアウトテンプレートをグループに割り当てることができます。

この変更を行う前に、ユーザー、チーム、ジョブの役割にレイアウトテンプレートを割り当てることができます。 レイアウトテンプレートをグループに割り当てると、レイアウトテンプレートの割り当ての優先順位が最も低くなります。 

詳細は、「レイアウトテンプレートの作成と管理」を参照してください。

## ユーザー通知の一括編集に関する変更

ユーザーの電子メール通知設定を一括編集する際の機能が変更されました。 複数のユーザーを選択して通知 E メールの設定を編集する場合、選択したすべてのユーザーに対して、更新する特定の通知のみが変更されます。 変更されていない電子メール通知設定は、ユーザーごとに異なる場合でも、選択したすべてのユーザーに対して同じままです。 

この変更以前は、選択した電子メール通知設定が保存され、変更を保存すると、その他の変更されていない通知設定はすべて選択解除されていました。 

詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 複数の電子メール通知のルックアンドフィールを更新しました

次の E メール通知のルックアンドフィールが、新しい UI で更新されました。

* 問題の割り当て
* 日付変更のコミット
* 自分が参加するプロジェクトの状況がアクティブになった
* 関係者に対する承認の決定
* タスク扶養家族に対する先行タスクの完了
* 承認待ち（プロジェクト、タスク、タスク）
* プロジェクト、タスク、問題に対するステータスの変更

プレビューサンドボックスがすべてのユーザーの電子メールアドレスをクリアするので、この機能をテストできるよう、アカウントに関連付けられた電子メールアドレスを必ず更新してください。    電子メール通知について詳しくは、 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## 複数の通知領域に対応する新しい電子メールダイジェストオプションが追加されました。

次の通知領域には、「日別ダイジェスト」オプションが追加されています。

* 自分が参加しているプロジェクトに関する情報
* スポンサーしているプロジェクトに関する情報
* 承認情報
* 担当割り当てされている作業に関する情報
* コミュニケーション

詳しくは、 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).  プレビューサンドボックスがすべてのユーザーの電子メールアドレスをクリアするので、この機能をテストできるよう、アカウントに関連付けられた電子メールアドレスを必ず更新してください。 

## グループを公開する

グループを公開する際に、グループの所有者にならずにそのグループをユーザーに追加できるようになりました。 ユーザーを編集するには、ユーザー管理者アクセス権が必要です。

グループを公開する方法について詳しくは、 [グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) セクション [グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## モバイルアプリでのオブジェクトの URL の共有 

Workfrontモバイルアプリ上の以下のオブジェクトで URL を共有できるようになりました。

* プロジェクト
* タスク
* 問題
* タイムシート
* ドキュメント

次のアプリケーションでオブジェクトの URL を共有できます。

* テキストメッセージ
* E メール
* ストレージドライブ（iCloud ドライブなど）
* 別のインストール済みアプリケーション ( 例：Notes、Facebook)
* オブジェクトへのリンクをクリップボードにコピーし、後で他のアプリケーションに貼り付けることができます。 

## 設定の状況依存ヘルプ

設定メニューのすべての領域が更新され、領域の右上隅にヘルプアイコンが表示されました。 このアイコンは、その領域に関するヘルプサイト記事へのリンクを提供します。 「設定」領域内の一部のセクションも、ヘルプアイコンで更新されました。 

## より正確な費用レートの追加

費用タイプを作成する際に、より正確な費用レートを追加できるようになりました。 費用レートには、小数点以下 4 文字までを含めることができます（例：1.0375）。 つまり、この率を使用するフィールドの精度を高めることができます。

この変更以前は、費用レートに小数点以下 2 文字までしか含めることができません（例：1.03）。

費用レートの作成の詳細については、 [カスタム経費タイプを作成](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1 プレビュー 1 および 2 リリースのウェビナー録画

このウェビナーは、2017 年 1 月 19 日にWorkfront Release Readiness チームによって提示されました。 このウェビナーでは、2017 年のリリースの変更に重点を置いており、プレビューでテストできる新機能について説明しています。
