---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 ベータ 3 リリースアクティビティ
description: このページでは、2017.2 ベータ 2 リリースに関してプレビュー環境で使用できるすべての変更について説明します。このページの機能は、2017年5月24日（PT）にプレビュー環境で使用できるようになりました。2018年7月下旬から8月上旬（PT）までの間に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9647f3c6-f287-426c-a5e7-eb33b8b22a34
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 100%

---

# 2017.2 ベータ 3 リリースアクティビティ

このページでは、2017.2 ベータ 2 リリースに関してプレビュー環境で使用できるすべての変更について説明します。このページの機能は、2017年5月24日（PT）にプレビュー環境で使用できるようになりました。2018年7月下旬から8月上旬（PT）までの間に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017.2 に実装されたすべての変更のリストについては、[2017.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)を参照してください。

2017.2 ベータ 2 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け：**

* [ごみ箱から項目を一括復元](#restoring-items-in-bulk-from-the-recycle-bin)
* [ユーザー情報を Workfront から ProofHQに同期（ProofHQ および Workfront）](#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront)

**すべてのユーザー向け：**

* [登録ユーザーを表示](#view-subscribed-users)
* [ガントチャートのマイルストーンの表示方法を設定](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [ガントチャートを PDF に書き出す際に凡例を含める](#include-the-gantt-chart-legend-when-exporting-to-pdf)
* [担当作業エリア内でプルーフ承認を表示（Workfront）](#view-proof-approvals-in-the-my-work-area-workfront)
* [担当作業エリア内からプルーフ承認リクエストに対処する際にユーザー名を表示（Workfront）](#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront)
* [ビデオプルーフ用のプルーフビューアを改善（ProofHQ および Workfront）](#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront)
* [別の解像度でリッチメディアプルーフを表示（ProofHQ および Workfront）](#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront)
* [ドキュメントバージョンレポートへのプルーフ作成者オブジェクトの新規追加（Workfront）](#new-proof-creator-object-in-document-version-report-workfront)
* [新しいリソースプール機能をプレビューから一時的に削除](#new-resource-pool-functionality-temporarily-removed-from-preview)

## ごみ箱から項目を一括復元 {#restoring-items-in-bulk-from-the-recycle-bin}

削除済みのプロジェクト、タスク、イシューまたはドキュメントを一度に最大 10 個まで復元できるようになりました。

この変更が行われる前は、削除済みの項目を一度に 1 個しか復元できませんでした。

項目の復元について詳しくは、[削除された項目の復元](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

## 登録ユーザーを表示 {#view-subscribed-users}

登録リンクの横に表示される登録者数を拡大することで、項目に登録しているユーザーを確認できるようになりました。

この機能強化が行われる前は、項目に登録しているユーザーを確認することはできませんでした。

項目の登録について詳しくは、[Adobe Workfront での項目の登録](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)を参照してください。

## ガントチャートでのマイルストーンの表示方法を設定 {#configure-how-milestones-are-displayed-on-the-gantt-chart}

ガントチャートでマイルストーン情報を表示するオプションは 2 つあります。次のマイルストーンインジケーターのいずれかまたは両方を設定できます。

* マイルストーンダイヤモンド（アイコン）

  このアイコンは、ガントチャートでマイルストーンに関連付けられたタスクの後に表示されます。

* マイルストーン線

  マイルストーンに関連付けられたタスクの後には、ガントチャートのすべてのタスクにまたがる線が表示されます。

この変更が行われる前は、ガントチャートにマイルストーンを表示するためのオプション（名称「マイルストーン」）は 1 つのみでした。このオプションでは、マイルストーンのひし形アイコンとの線の両方が有効になりました。これらのインジケーターは分離できませんでした。

ガントチャートでの情報の表示方法の設定について詳しくは、[ガントチャートでの情報の表示方法の設定](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

## ガントチャートを PDF に書き出す際に凡例を含める {#include-the-gantt-chart-legend-when-exporting-to-pdf}

ガントチャートを PDF に書き出す際に、チャートと一緒にチャートの凡例をエクスポートするかどうかを選択できるようになりました。凡例に含まれる項目は、UI でガントチャートに表示できるオプションのみです。これらのオプションは、プロジェクトのタスクに存在する場合、凡例に含まれます。例えば、ガントチャートでマイルストーンの表示を有効にすると、マイルストーンに関連付けられたタスクが 1 つ以上ある場合に限り、凡例にもマイルストーンが表示されます。

この変更が行われる前は、PDF に書き出す際に凡例を除外することはできず、有効になっているか、UI に存在しているかに関係なく、凡例にはガントチャートで使用可能なすべてのオプションとマーカーが含まれていました。

ガントチャートの書き出しについて詳しくは、[ガントチャートの PDF への書き出し](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)を参照してください。

## ユーザー情報を Workfront から ProofHQに同期（ProofHQ および Workfront） {#user-information-is-synchronized-from-workfront-to-proofhq-proofhq-and-workfront}

Workfront でユーザーが作成または更新されると、ユーザー情報（名前およびメール）が Workfront から ProofHQ に同期されるようになりました。 

Workfront から ProofHQ へのユーザー同期について詳しくは、以下を参照してください。

## ドキュメントバージョンレポート（Workfront）の新しい「プルーフ作成者」オブジェクト

{#new-proof-creator-object-in-document-version-report-workfront}

ドキュメントバージョンレポートを作成する際に、新しいプルーフ作成者オブジェクトを使用できるようになりました。このオブジェクトを使用すると、プルーフを作成したユーザーに関する情報をレポートできます。 

ドキュメントバージョンレポートの新しいプルーフ作成者オブジェクトには、他のタイプのオブジェクトレポートで既存のユーザーオブジェクトに対して使用できるすべてのフィールドが含まれています。

>[!NOTE]
>
>この情報は、この機能がそれぞれのプレビュー環境または実稼動環境に初めて導入された時点からのレポートでのみ入手できます。この機能が導入される前のリクエスターオブジェクトに関するレポートでは、情報は利用できません。

[カスタムレポートの作成](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の説明に従ってドキュメントバージョンレポートを作成する際に、プルーフ作成者オブジェクトにアクセスします。

ドキュメントバージョンオブジェクトレポートについて詳しくは、[Adobe Workfront のオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)で[Adobe Workfront のオブジェクトについて](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の節を参照してください。

## 担当作業エリア内でプルーフ承認を表示（Workfront） {#view-proof-approvals-in-the-my-work-area-workfront}

承認を得るために送信したすべてのプルーフ承認が、担当作業エリアの「**承認用に送信した作業**」タブに表示されるようになりました。

この変更以前は、「**承認用に送信した作業**」タブにプルーフ承認は含まれていませんでした。

プルーフの承認は、以下の条件を満たした場合にのみ表示されます。

* 承認が現在承認保留中である
* 承認プロセスが Workfront のライセンス済みユーザーに割り当てられている（ライセンス済みでない Workfront ユーザーに割り当てられている承認プロセスは表示されません）
* 承認プロセスがこの機能のリリース後に開始された（この機能のリリース前に開始された承認プロセスは表示されません）

詳しくは、[承認の表示](../../../../review-and-approve-work/manage-approvals/view-approvals.md)で[承認を表示](../../../../review-and-approve-work/manage-approvals/view-approvals.md)を参照してください。

## 担当作業エリア内からプルーフ承認リクエストに対応する際にユーザー名を表示（Workfront） {#view-user-names-when-addressing-proofing-approval-requests-from-the-my-work-area-workfront}

担当作業エリアからプルーフ承認を承認する際に、承認を要求したユーザーの名前が表示されるようになりました。

詳しくは、[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)にある[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

## ビデオプルーフのプルーフビューアを改善（ProofHQ および Workfront） {#improved-proofing-viewer-for-video-proofs-proofhq-and-workfront}

Workfront と ProofHQ の両方のプルーフビューアが更新され、新しいルックアンドフィール、パフォーマンス向上のための HTML5 アーキテクチャおよび新機能のサポートが導入されています。

新しいプルーフビューアの改善点は次のとおりです。

* フレームごとのプルーフ
* ビデオバッファリング
* コメントリストでの検索機能
* コメントに設定されたアクションがコメントリストの各コメントに表示される
* フルスクリーンモード
* コンテンツのレビュー速度の増減
* コメントおよび返信を追加する際のスペルチェッカー

### プレビュー

新しいプルーフビューアは、次のプレビュー環境でテストに使用できます。

* ProofHQ プレビュー環境

  ProofHQ プレビュー環境について詳しくは、[プレビューサンドボックステスト環境 - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md) を参照してください。

* Workfront プレビュー環境（アカウントがプルーフと共に有効になっている場合）

  Workfront プレビュー環境について詳しくは、[Adobe Workfront プレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。

このリリースの新しいプルーフビューアでは、ビデオプルーフのみをサポートしています。つまり、すべてのビデオプルーフでは新しいプルーフビューアが利用されますが、すべての静的プルーフおよびリッチメディアプルーフでは既存のプルーフビューアーが引き続き利用されます。

### 実稼動

17.2 リリースで実稼動環境にリリースされると、管理者は、新しいプルーフビューアと従来のプルーフビューアのどちらが組織のユーザーに適しているかを選択できます。デフォルトでは、従来のプルーフビューアが使用されます。

新しいビデオプルーフビューアの使用方法については、以下を参照してください。

## リッチメディアプルーフを別の解像度で表示（ProofHQ およびWorkfront） {#view-rich-media-proofs-in-alternate-resolutions-proofhq-and-workfront}

カスタム解像度を指定するか、画像を目的の解像度にドラッグすることで、リッチメディアプルーフの解像度を調整できるようになりました。

この変更以前は、コンテンツをレビューする画面やデバイスに固有の解像度のみを使用して、プルーフをレビューすることができました。

比較モードを使用すると、プルーフの様々な解像度を比較できます。

詳しくは、[デスクトッププルーフビューアーでプルーフを開く](../../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/open-proofs-in-dpv.md)を参照してください。

## 新しいリソースプール機能をプレビューから一時的に削除 {#new-resource-pool-functionality-temporarily-removed-from-preview}

開発上の課題により、新しい「リソース計画」タブを削除し、「レガシーリソース計画」タブの名前を元の「リソース計画」に戻すことにしました。

この変更に伴い、新しいリソースプール機能も削除されました。「リソース計画」の新しいタブとリソースプールの機能は、2017年6月末にプレビューサンドボックス環境に戻ります。
