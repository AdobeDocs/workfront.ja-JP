---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 ベータ版 4 リリースアクティビティ
description: このページでは、2018.1 ベータ版 4 リリースに伴いプレビュー環境で利用可能となった最新の変更点について説明します。この機能は、2018年1月24日（PT）にプレビュー環境で使用できるようになりました。2018年3月に、実稼動環境で利用できるようになります。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 100%

---

# 2018.1 ベータ版 4 リリースアクティビティ

このページでは、2018.1 ベータ版 4 リリースに伴いプレビュー環境で利用可能となった最新の変更点について説明します。この機能は、2018年1月24日（PT）にプレビュー環境で使用できるようになりました。2018年3月に、実稼動環境で利用できるようになります。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018年1月に行われたすべての変更のリストについては、[2018.1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)を参照してください。

2018.1 ベータ版 4 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [グループ管理者によるスケジュール管理](#schedules-managed-by-group-administrators)

**すべてのユーザー向け**

* [Workfront 内のプルーフ機能の改善](#proofing-improvements-within-workfront)
* [Workfront Proof でのプルーフ作成 - ユーザーエクスペリエンスの向上と追加機能](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Workfront および Workfront Proof 内のプルーフ機能の改善](#proofing-improvements-within-workfront-and-workfront-proof)
* [Workfront Proof での Basecamp 統合によるルックアンドフィールの更新](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [クリップボードから Workfront への画像のペースト](#paste-images-to-workfront-from-the-clipboard)
* [稼働率レポートの改善](#utilization-report-improvements)
* [Workfront からの予算計上リソース時間数オブジェクトの削除](#remove-the-resource-budgeted-hour-object-from-workfront)
* [レポートの使用状況の統計](#report-usage-statistics)
* [ガントチャートの更新](#gantt-chart-updates)
* [新しいポートフォリオオプティマイザー](#new-portfolio-optimizer)
* [リソースプランナーの「予算日の調整」オプション](#budget-date-adjustment-option-in-the-resource-planner)
* [リソーススケジュール：グループメンバーシップに基づいてユーザーへの割り当てを制限](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [リソーススケジュール：役割に関係なくユーザーへの割り当てを許可](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [絵文字のサポート](#emoji-support)

## Workfront 内のプルーフ機能の改善 {#proofing-improvements-within-workfront}

Workfront 内のドキュメントリストに関して、次の改善が行われました。

* [ドキュメントリストからプルーフの進捗状態を表示](#view-proof-progress-from-the-document-list)
* [ドキュメントリストから概要の印刷を表示する新しいオプション](#new-option-to-view-the-print-summary-from-the-document-list)
* [ドキュメントリストからプルーフを生成または開くためのルックアンドフィールの更新](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [ドキュメントリストのドキュメントから各種リンクを削除](#various-links-removed-from-documents-on-the-document-list)
* [結合プルーフでのファイル名の表示](#view-file-names-on-combined-proofs)
* [ドキュメントリストからプルーフの現在のアクティブなステージを表示](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### ドキュメントリストからプルーフの進捗状態を表示 {#view-proof-progress-from-the-document-list}

ドキュメントリストを表示する際に、プルーフの進捗状態を示すインジケーターがすべてのプルーフに表示されるようになりました。この進捗状態には、送信済み、開封済み、コメントあり、決定が含まれます。

この変更が行われる前は、右パネルでプルーフの進捗状態を表示するには、ドキュメントリストでプルーフを選択する必要がありました。 

詳しくは、[プルーフの進捗状態とステータスの概要](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md)を参照してください。

### ドキュメントリストから概要の印刷を表示する新しいオプション {#new-option-to-view-the-print-summary-from-the-document-list}

プルーフの概要の印刷をドキュメントリストから直接表示できるようになりました。

この変更が行われる前は、概要の印刷はプルーフビューアからのみ表示できました。 

ドキュメントリストから概要の印刷を表示する方法について詳しくは、[Adobe Workfront 内でのプルーフ概要の印刷](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)を参照してください。

### ドキュメントリストからプルーフを生成または開くためのルックアンドフィールの更新 {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

ドキュメントリストのドキュメントにポインタを合わせたときに表示される、プルーフを生成または開くためのオプションが更新されました。これらのオプションがより目立つようになり、ボタンとして表示されるようになりました。

この変更が行われる前は、これらのオプションはドキュメント名の下にリンクとして表示されていました。

詳しくは、次の節を参照してください。

* 。
* の .

### ドキュメントリスト上のドキュメントから削除された各種リンク {#various-links-removed-from-documents-on-the-document-list}

次のアクションは、ドキュメントリスト内の個々のドキュメントのリンクとして使用できなくなりました。

* プルーフの作成
* プルーフ
* 詳細
* 共有
* チェックアウト／チェックイン

ドキュメントリスト内のドキュメント上のボタンとして、以下のアクションを使用できるようになりました。

* プルーフを開く（プルーフの生成後に使用可能）
* プルーフを生成（プルーフがまだ生成されていない場合に使用可能）

「プルーフを開く」または「プルーフを生成」ボタンの横にあるドロップダウンメニューで、次の操作を使用できるようになりました。

* プルーフ詳細
* ドキュメントの詳細
* 概要を印刷

詳しくは、次の節を参照してください。

* 。
* の .

### 組み合わせプルーフでファイル名を表示する {#view-file-names-on-combined-proofs}

組み合わせプルーフを構成する個々のファイル名を表示できるようになりました。この情報は、ドキュメントリストでプルーフが選択されている場合に「詳細」タブに表示されます。

詳しくは、組み合わせプルーフに含まれるすべてのファイルの表示を参照してください。 

### ドキュメントリストからプルーフの現在のアクティブなステージを表示 {#view-the-current-active-stage-of-a-proof-from-the-document-list}

ドキュメントリストでプルーフを選択すると、現在アクティブなステージが「詳細」タブの右側の列に表示されるようになりました。 

詳しくは、[プルーフのアクティブなステージの表示](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md)を参照してください。

## Workfront Proof でプルーフを作成 - ユーザーエクスペリエンスの向上と追加機能 {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Workfront Proof でプルーフを作成する際のユーザーエクスペリエンスが向上したことに加えて、次の追加機能が利用できるようになりました。

* 複数画像を単一プルーフに結合。
* 複数の解像度で web サイトをプルーフ（複数の解像度を個別のプルーフとして作成することも、単一のプルーフに結合することもできます）。
* アップロードプロセス中にファイル名を編集。
* プルーフ作成フォームにカスタムフィールドを含める。
* プルーフメール通知にカスタムメッセージを追加します。
* 追加のプルーフの設定
* URL のプルーフ時のリアルタイムのエラー検証（以前は、エラーが表示されるまでに数分待つ必要がありました）

>[!NOTE]
>
>Workfront Proof のこの新しいプルーフの作成ページは、Workfront でプルーフを作成する際に最近利用可能になったプルーフ作成ページと一致するようになりました。 

詳しくは、[Workfront Proof でプルーフを生成](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)を参照してください。

## Workfront および Workfront Proof 内でのプルーフ機能の改善 {#proofing-improvements-within-workfront-and-workfront-proof}

Workfront および Workfront Proof にドキュメントを追加する場合は、次の変更が適用されます。

* [プルーフのレビュー時にコメントリストのサイズを変更](#resize-the-comment-list-when-reviewing-proofs)
* [静的プルーフのレビュー時にハイパーリンクがアクティブになる](#hyperlinks-are-active-when-reviewing-static-proofs)
* [プルーフを追加する際の改善点](#improvements-when-adding-proofs)

### プルーフのレビュー時にコメントリストのサイズを変更する {#resize-the-comment-list-when-reviewing-proofs}

プルーフビューアーでプルーフをレビューする際に、コメントリストのサイズを変更できるようになりました。

詳細情報は、次を参照してください。

### 静的プルーフのレビュー時にハイパーリンクがアクティブになる {#hyperlinks-are-active-when-reviewing-static-proofs}

プルーフビューアーで静的プルーフを確認する際に、ハイパーリンクがアクティブになりました。ハイパーリンクをクリックして、リンクされたページに移動します。

この機能は、PDF、DOC などのテキストを含むすべてのファイルタイプでサポートされます。画像ファイルはサポートされていません。

### プルーフを追加する際の改善点 {#improvements-when-adding-proofs}

プルーフするドキュメントを追加する際に、次の機能強化を使用できます。 

* 受信者リストの情報が 3 列表示で利用できるようになり、情報を見たり変更したりしやすくなりました。 

  以前は、情報は 1 列で表示されていたので、変更が必要な場合はより多くのクリックが必要でした。 

  詳細情報は、次を参照してください。

* 自動ワークフローを使用する場合は、1 人以上の受信者を 1 つのワークフローステージから別のワークフローステージにドラッグします。ステージに直接ドラッグすることも、ページの上部にある図上のステージにドラッグすることもできます。

  詳細情報は、次を参照してください。

* スクロールしても、ワークフロー図がページの上部に表示されたままになります。図はデフォルトで折りたたまれます。図を展開して、図全体を表示します。

  詳細情報は、次を参照してください。

* プルーフの自動ワークフローにテンプレートを追加する際に、テンプレートが読み込み中であることを示す読み込みアニメーションが表示されます。

  詳細情報は、次を参照してください。

* 次の設定が、新規プルーフページの「プルーフ設定」セクションから「ワークフロー」セクションに移動されました。

   * 主要な校正判断者
   * 必要な校正判断を 1 つにする

## Workfront Proof の Basecamp 統合によるルックアンドフィールのアップデート {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Workfront Proof での Basecamp 統合のルックアンドフィールが更新されました。機能は変わりません。

## クリップボードから Workfront に画像を貼り付け {#paste-images-to-workfront-from-the-clipboard}

システムのクリップボードから画像を貼り付けて、Workfront に画像ファイルを追加できるようになりました。

クリップボードから貼り付ける機能は、以前のリリースで Workfront から削除されましたが、このリリースで再導入されています。この新しい方法は、より合理化され、直感的です。

詳しくは、[クリップボードから画像を貼り付け](../../../../documents/managing-documents/paste-image-clipboard.md)を参照してください。

## 稼働率レポートの改善点 {#utilization-report-improvements}

稼働率レポートには、次の改善点が含まれています。

* プロジェクトの稼働率レポートで収益を表示

  予算計上収益、予定収益、実収益、予算計上差異および予定差異を表示できます。

* 収益と予定コストおよび実際のコストとの比較

  予定収益と共に、予定コストまたは実際のコストを表示できます。利益（％）も表示されます（利益は収益 - コスト / 収益として計算されます）。

* グラフを表示すると収益が表示されます。
* スクロールしたときも、ヘッダーが表示されます。

  稼働率レポートの情報をスクロールしているときも、稼働率レポートの上部にあるヘッダーが常に表示され、レポート内のデータをより簡単に理解できるようになりました。

  以前は、スクロールすると、稼働率レポートの上部にあるヘッダーが表示から外れていました。

* 個々のプロジェクトに関する稼働率レポートが自動的に読み込まれます。

  プロジェクトの稼働率レポートを表示すると、レポートが自動的に読み込まれます。

  この変更を行う前は、レポートを実行する前に「実行」をクリックする必要がありました。

* パフォーマンスの向上

稼働率レポートについて詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## リソース予算計上時間オブジェクトを Workfront から削除 {#remove-the-resource-budgeted-hour-object-from-workfront}

パフォーマンスの問題に対処するために、リソース予算計上時間フィールドが Workfront から一時的に削除されました。

なお、リソース予算計上時間は、リソースプランナーのリソースまたはプロジェクトに対して予算を作成する時間です。当面の間、Web アプリケーションや API を通じてこのフィールドに関するレポートを作成できません。パフォーマンスの問題が解決されたら、このフィールドは将来のリリースで復元されます。

リソースプランナーの予算計上時間について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## レポートの使用状況の統計 {#report-usage-statistics}

レポートのリストで、Workfront レポートに関する次の使用情報を表示できるようになりました。

* 最終表示者
* 最終表示日
* 最終表示者 10 名
* 現在の月／四半期／年を表示
* 表示回数（先月、前四半期、昨年）
* すべてのビュー

このアップデートを行う前は、レポートに表示される使用情報が制限されていました。

レポートの使用方法について詳しくは、[レポートの使用状況の表示](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)を参照してください。

## グループ管理者によるスケジュール管理 {#schedules-managed-by-group-administrators}

グループ管理者は、管理するグループとそのサブグループに関連付けられたスケジュールを作成および編集できます。この変更を行う前は、Workfront 管理者のみがスケジュールを作成および編集できました。

スケジュールの管理について詳しくは、[スケジュールを作成](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

## ガントチャートのアップデート {#gantt-chart-updates}

ガントチャートを編集できるようになりました。ガントチャートを使用して、タスクを次のように更新できます。

* 先行タスク関係を作成
* タスク期間を編集
* タスクの完了率を更新
* リソースの平準化を適用

この変更を行う前は、ガントチャートで先行タスクの関係を削除することしかできず、タスクリストでのみタスクを編集できました。

ガントチャートについて詳しくは、[タスクリストのガントチャートの情報を更新](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)を参照してください。

## 新しいポートフォリオオプティマイザー {#new-portfolio-optimizer}

Workfront のポートフォリオオプティマイザーの領域が新しいルックアンドフィールで更新されました。機能は変更されていません。

ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

## リソースプランナーの「予算日の調整」オプション {#budget-date-adjustment-option-in-the-resource-planner}

予算計上の競合を避けて、時間枠をすばやく確認できるオプションを追加しました。予算計上の競合が発生しない時間枠を確認した後、予算計上時間をその時間に手動で移動できます。これにより、予算日を時間単位で調整できます。この更新以前は、プロジェクトの予算計上の競合を一目で確認することはできませんでした。

リソースプランナーでの予算日の調整について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)の「予算日の調整」の節を参照してください。

## リソーススケジュール：グループメンバーシップに基づくユーザーへの割り当てを制限 {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

スケジュール領域でユーザー割り当てを行う場合（「スケジュール領域での未割り当てのタスクとイシューを手動で割り当てる」を参照）、タスクやイシューが発生したプロジェクトで定義されている、グループのメンバーであるユーザーのみに制限するよう Workfront を設定できるようになりました。 

これは、次の方法で割り当てを行う場合に適用されます。

* 「スケジュール領域での未割り当てのタスクとイシューを手動で割り当てる」の説明に従って、特定のロールのすべてのタスクとイシューにユーザーを割り当てる場合。

  この変更が行われる前は、そのユーザーのグループメンバーシップに関係なく、タスクまたはイシューを常に任意のユーザーに割り当てることができました。 

* 「スケジュール領域での未割り当てのタスクとイシューを手動で割り当てる」の説明に従って、別のユーザーと割り当てを入れ替える場合。

  この変更が行われる前は、そのユーザーのグループメンバーシップに関係なく、タスクまたはイシューを常に任意のユーザーに割り当てることができました。 

* 「スケジュール領域での未割り当てのタスクとイシューを手動で割り当てる」の説明に従って、スケジュールタイムラインからタスクまたはイシューを手動で割り当てる場合。

  この変更が行われる前は、そのユーザーのグループメンバーシップに関係なく、タスクまたはイシューを常に任意のユーザーに割り当てることができました。 

* 「スケジュールエリアでの未割り当てのタスクとイシューを手動で割り当てる」の説明に従って、Workfront にユーザーの自動割り当てを許可する場合。

  この変更が行われる前は、Workfront はグループのメンバーシップに関係なく、タスクとイシューをユーザーに割り当てていました。

このオプションの設定について詳しくは、「リソーススケジュール設定の概要」を参照してください。

## リソーススケジュール：役割に関係なくユーザーへの割り当てを許可 {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

スケジュールエリアでユーザー割り当てを行う場合（「スケジュールエリアでの未割り当てのタスクとイシューを手動で割り当てる」を参照）、ユーザーが自分に割り当てられているタスクやイシューの役割割り当てと一致するユーザープロフィールで定義された役割を持っているかどうかに関係なく、タスクとイシューを任意のユーザーに割り当てることができるように、Workfront を設定できるようになりました。

これは、次の方法で割り当てを行う場合に適用されます。

* 「スケジュールエリアでの未割り当てのタスクとイシューを手動で割り当てる」の「スケジュールエリアで未割り当てのタスクとイシューを手動で割り当てる」で説明されているように、特定のロールのすべてのタスクと課題にユーザーを割り当てる場合。

  この変更が行われる前は、割り当てるユーザーの主な役割は、「役割を選択」フィールドで既に定義されている役割と一致している必要がありました。

* 「スケジュール領域での未割り当てのタスクとイシューを手動で割り当てる」の説明に従って、別のユーザーと割り当てを入れ替える場合。

  この変更が行われる前は、割り当てるユーザーの主な役割は、「役割を選択」フィールドで既に定義されている役割と一致している必要がありました。

* 「スケジュール領域での未割り当てのタスクとイシューを手動で割り当てる」の説明に従って、スケジュールタイムラインからタスクまたはイシューを手動で割り当てる場合。

  この変更が行われる前は、割り当て先のタスクまたはイシューの役割に一致する役割を持つユーザーのみがスケジュールタイムラインに表示されていました。

>[!NOTE]
>
>「スケジュールエリアでの未割り当てのタスクとイシューを手動で割り当てる」で説明されているように、Workfront にユーザーの自動割り当てを許可する場合には適用されません。ユーザー、タスクおよびイシューを自動的に割り当てる場合、一致する役割を持つユーザーのみを割り当てることができます。

このオプションの設定について詳しくは、「リソーススケジュール設定の概要」を参照してください。

## 絵文字のサポート {#emoji-support}

絵文字を挿入することで、Workfront で行ったコメントや更新のトーンを設定できるようになりました。「更新」タブで作成されたコメントに追加された絵文字も、更新メール通知に表示されます。 

詳しくは、[作業の更新](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。
