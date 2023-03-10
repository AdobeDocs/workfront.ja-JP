---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 プレビュー 3
description: このページでは、R1.3 リリースでプレビュー環境で使用できるすべての変更について説明します。 このページの機能は、2017 年 2 月 2 日にプレビュー環境で使用できるようになりました。
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 2%

---

# R1 プレビュー 3

このページでは、R1.3 リリースでプレビュー環境で使用できるすべての変更について説明します。 このページの機能は、2017 年 2 月 2 日にプレビュー環境で使用できるようになりました。

R1 で行われたすべての変更のリストについては、 [R1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 外部ファイルをリンクする方法を改善しました

外部ソース (Googleドライブ、ボックス、Dropboxなど ) からドキュメントをリンクするオプションが、ドキュメント領域でより目立つ場所になりました。 

さらに、ドキュメントプロバイダーからのファイルを初めてリンクする前にドキュメントプロバイダーを認証する操作が、より直感的になりました（外部プロバイダーからファイルをリンクする際の追加手順になります）。

これらの変更を行う前は、「ドキュメント」領域の「ドキュメントを追加」ダイアログボックス内に、外部ソースからファイルをリンクするオプションが用意されていました。 ドキュメントを外部ソースから初めてリンクする場合は、ドキュメントをリンクするユーザーが「セットアップ」領域でそのドキュメントプロバイダーを認証する必要がありました。

詳しくは、  [外部アプリケーションからドキュメントをリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## カレンダーの作業チームの更新

>[!NOTE]
>
>リソーススケジュールツールは廃止され、23.1 リリースでWorkfrontから削除されました。 ワークロード・バランサを使用したリソースのスケジュール設定の詳細は、 [ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

チームで使用できるカレンダーの操作に、追加の機能とルックアンドフィールが追加されました。 チームの [ 作業カレンダー ] は、プロジェクトのリソーススケジュールツールと同様に機能するようになりました。

更新されたチームのカレンダーの作業には、次の改善点が含まれています。

* ユーザーをアルファベット順またはロール別にグループ化して表示します。
* プロジェクトの優先度、ステータス、個々のプロジェクトでスケジュールタイムラインをフィルタリングします。 スケジューリングタイムラインを、役割およびユーザー別にフィルタリングすることもできます。 （「フィルター」領域のオプションは、プロジェクトのリソースをスケジュールする場合と比べて少なくなります）。
* スケジュールタイムラインに問題が含まれます。
* ユーザーの割り当てを表示し、特定のタスクおよび 1 日の問題にユーザーが割り当てられる時間数を変更します。
* 特定の日にユーザーが過度に割り当てられた時点を示す指標を表示します。
* 完了した作業をスケジュールタイムラインに表示するかどうかを設定します。

プロジェクトのリソースをスケジュールする際のリソーススケジュールツールとの違い：

* チームメンバー全員が、チームの [ 作業カレンダー ] に表示されます。\
   プロジェクトのリソースをスケジュールする場合、「未割り当て」領域の 1 つ以上のタスクのロールと一致するロールを持つユーザーのみが表示されます。
* [ スワップ ] ツールは、チームの [ カレンダーで作業 ] には含まれていません。
* チームメンバーは誰でも、チームのカレンダーで作業を変更できます。\
   プロジェクトのリソースをスケジュールする場合、リソースマネージャのみがプロジェクトのリソース決定を行うことができます。
* タスクは、チームの [ カレンダーで作業 ] にデフォルトで表示されます。\
   プロジェクトのリソースをスケジュールする場合、デフォルトでは問題は表示されません。

更新されたチームのカレンダー作業の詳細については、「リソースのスケジュール設定」を参照してください。

## リソーススケジュールの強化

スケジュールタイムラインには、次の機能強化が含まれています。

* 「フィルターを使用して、スケジューリング・タイムラインに表示するユーザーを制御する」
* タスクの割り当て後も、ユーザーがタイムラインに留まる

### フィルターを使用して、スケジュールタイムラインに表示するユーザーを制御します {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>リソーススケジュールツールは廃止され、23.1 リリースでWorkfrontから削除されました。 ワークロード・バランサを使用したリソースのスケジュール設定の詳細は、 [ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

これで、フィルターを使用して、スケジューリングタイムラインに表示するユーザーと、「未割り当て」領域に表示するタスクおよび問題を制御できるようになりました。 フィルタでユーザを選択すると、[ 未割り当て ] 領域のタスクの役割割り当てに一致する役割割り当てがあるかどうかに関係なく、選択したユーザのみが表示されます。 現在そのユーザーに割り当てられているすべてのタスクも表示されます。

この変更以前は、フィルターは未割り当て領域に表示されたタスクと問題のみを制御していました。 ユーザーが「未割り当て」領域でタスクのロール割り当てに一致した場合にのみ、スケジュールタイムラインに表示されていました。

フィルタを使用して、スケジューリングタイムラインに表示する内容を制御する方法の詳細は、「スケジュール領域の情報をフィルタ」および「スケジュール領域の未割り当てタスクと問題を手動で割り当てる」を参照してください。

### タスクの割り当て後も、ユーザーがタイムラインに留まる {#users-remain-on-the-timeline-after-being-assigned-a-task}

タスクまたはタスクが割り当てられた後も、一致する役割が割り当てられたタスクまたはタスクが残っていない場合でも、ユーザーはスケジューリングタイムラインに留まります。 これにより、ユーザーが割り当てられた後に、必要な変更を加えることができます。

この変更がおこなわれる前は、タスクまたはイシューが割り当てられた直後に、「未割り当て」領域に、一致するロール割り当てを持つタスクまたはイシューが残っていない場合、ユーザーはスケジュールタイムラインから消えます。

詳細については、「スケジュール領域で未割り当てタスクと問題を手動で割り当てる」を参照してください。

## オブジェクト名の変更によるWorkfrontの用語のカスタマイズ

特定のオブジェクトの名前を変更して、Workfrontの用語をカスタマイズできるようになりました。\
レイアウトテンプレートを使用すると、次の作業オブジェクトの名前を、組織のニーズに合わせて変更できます。

* ポートフォリオ
* プログラム
* プロジェクト
* タスク
* 問題

例えば、組織内でプロジェクトの代わりにキャンペーンを使用する場合は、「プロジェクト」オブジェクトの名前を「Campaign」に置き換えることができます。

この置換を行うと、アプリケーションの次の領域に、更新されたオブジェクト名が表示されます。

* グローバルナビゲーションバー
* すべてのタブ
* すべてのメニュー 
* Report Builder とレポート要素（ビュー、フィルターおよびグループ）
* 保存ボタン
* 書き出されたファイル
* メール

以下の領域では、更新されたオブジェクトの名前は表示されません。

* リソース見積り
* リソース バジェット マネージャ
* キャパシティ プランナ
* リソース グリッド
* チーム ビルダー
* Portfolio最適化 
* モバイルアプリ
* Outlook アドイン

レイアウトテンプレートを使用してWorkfrontの用語をカスタマイズする方法の詳細は、「レイアウトテンプレートの作成と管理」の「用語のカスタマイズ」の節と、 [Adobe Workfrontのオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## レポートに承認の開始日と終了日を含める

レポートを作成または変更する際に、次のフィールドを含めることができるようになりました。

* 承認パス開始日
* 承認パス完了日

これらのフィールドでは、現在または最新の承認パスがいつ開始されたか、および完了とマークされた日時を把握できます。

これらのフィールドについて詳しくは、 [Adobe Workfrontの用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

承認パス、承認パスの作成方法とトリガー方法、承認プロセスで使用する機能について詳しくは、 [作業項目の承認プロセスの作成](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

次のフィールドはWorkfrontから削除され、レポートに含めることができなくなりました（これらのフィールドは、承認自体に関する情報ではなく、プロジェクトに関する情報を提供し、多くの場合誤って使用されていました）。

* 承認計画開始日
* 見込み承認開始日
* 承認推定開始日

## 「おこなったリクエスト」の新しい電子メールダイジェストオプション

通知設定の「おこなった要求」領域に、「日別ダイジェスト配信」オプションが追加されました。

詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

この機能をテストするには、アカウントに関連付けられた電子メールアドレスを必ず更新してください。 プレビューサンドボックスは、すべてのユーザーの E メールアドレスをクリアするので、これが必要です。

## ドキュメント承認電子メール通知のルックアンドフィールを更新しました

「ドキュメントの承認」の通知のルックアンドフィールが、新しい UI で更新されました。

電子メール通知について詳しくは、 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).

この機能をテストするには、アカウントに関連付けられた電子メールアドレスを必ず更新してください。 プレビューサンドボックスは、すべてのユーザーの E メールアドレスをクリアするので、これが必要です。

## マイルストーン表示の機能強化

プロジェクトリストまたはプロジェクトレポートの表示時に使用できる「マイルストーン」ビューに、次の機能強化が含まれるようになりました。

* 計画日は編集可能です
* プロジェクトおよびタスクの完了率が表示されます

この変更を行う前に、日付を編集したり、達成率を表示したりするには、個々のタスクに移動する必要がありました。

詳しくは、 [マイルストーンビューの使用](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
