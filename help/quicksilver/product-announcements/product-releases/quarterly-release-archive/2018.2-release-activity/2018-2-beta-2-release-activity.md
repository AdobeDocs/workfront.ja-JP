---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 ベータ版 2 リリースアクティビティ
description: このページでは、2018.2 ベータ版 2 リリースによりプレビュー環境で最近利用可能になったすべての変更について説明します。機能は、2018年4月5日（PT）にプレビュー環境で利用できるようになりました。2018年6月に、実稼動環境で利用できるようになります。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: c8ef68f5-53db-4c3c-af0f-e1c98521ec27
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 100%

---

# 2018.2 ベータ版 2 リリースアクティビティ

このページでは、2018.2 ベータ版 2 リリースによりプレビュー環境で最近利用可能になったすべての変更について説明します。機能は、2018年4月5日（PT）にプレビュー環境で利用できるようになりました。2018年6月に、実稼動環境で利用できるようになります。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018.2 で行われたすべての変更のリストについては、[2018.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md) を参照してください。

2018.2 ベータ 2 リリースには、次の機能強化が含まれています。

* [ホームエリアからフィールドを直接編集](#edit-fields-directly-from-the-home-area)
* [日数で時間を記録](#log-time-in-days)
* [プロジェクト間の先行タスクの関係をプロジェクトリストのガントチャートで表示](#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects)
* [ポートフォリオオプティマイザーで予算計上コストを使用して、ポートフォリオ財務を計算](#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances)
* [稼働率レポート：新規リソース予算計上フィールドエリアから、予算計上時間数を入力](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area)（プレビューのみ）

* [稼働率レポート：プロジェクト上のユーザー別の予算計上時間数を表示](#utilization-report-view-budgeted-hours-by-user-on-a-project)（プレビューのみ）

* [ドキュメントリストのプルーフの進捗状態をプルーフ以外のユーザーが利用可能に](#proof-progress-from-the-document-list-available-to-non-proofing-users)
* [モバイルの改善点](#mobile-improvements)

## ホームエリアからフィールドを直接編集 {#edit-fields-directly-from-the-home-area}

ホームエリアでオブジェクトを選択すると、ホームエリアの右側のパネルから、そのオブジェクトに関連付けられたフィールドを直接編集できます。 

この変更以前は、情報はホームエリアでのみ表示でき、編集はできませんでした。

詳しくは、[ホームエリアでの作業アイテムの更新または編集](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)の[ホームエリアでの作業アイテムの更新または編集](../../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)を参照してください。

## ログ時間（日数） {#log-time-in-days}

Workfront の管理者は、組織内のユーザーがログに記録する時間を日単位と時間単位のどちらにするかを設定できるようになりました。プランナーライセンスを持つユーザーは、自分でこの設定を指定できます。

この変更以前は、ユーザーは時間単位でのみログに記録できました。

この設定は、ユーザープロファイルを編集することで設定できます。詳しくは、[時間を時間数と日数のどちらで記録するかを設定](../../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)を参照してください。

この設定が更新されてからユーザーが日数で時間を記録する方法について詳しくは、[時間を記録](../../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

## プロジェクト間の先行タスクの関係をプロジェクトリストのガントチャートで表示 {#view-cross-project-predecessor-relationships-on-the-gantt-chart-in-a-list-of-projects}

次のプロジェクト一覧で、ガントチャートにプロジェクト間の先行関係を表示できるようになりました。

* ポートフォリオまたはプログラム内の「プロジェクト」タブ
* プロジェクトレポート内

この変更以前は、プロジェクトレベルの個々のタスクに対してのみ、プロジェクト間の先行タスク関係を表示できました。

詳しくは、[ガントチャートに表示する情報の設定](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

## ポートフォリオオプティマイザーで予算計上コストを使用して、ポートフォリオ財務を計算 {#use-budgeted-cost-in-the-portfolio-optimizer-to-calculate-portfolio-finances}

新しいポートフォリオオプティマイザーは、ビジネスケースの新しいリソース予算領域またはリソースプランナーからの予算コストを使用して、次のフィールドを計算するようになりました。

* 純価
* 投資回収率（ROI）
* コスト

以前は、新しいポートフォリオオプティマイザーと従来のポートフォリオオプティマイザーの両方で、レガシー予算コストが使用されていました。レガシーポートフォリオオプティマイザーは、従来の予算原価を使用して、純価値、投資利益率および原価を計算します。

また、Portfolio の財務分野に、新しいリソース管理ツールから新しい値を取り込むための「レガシー ROI」と「レガシー正味価値」の 2 つの新しいフィールドを追加しました。

詳しくは、[ポートフォリオオプティマイザーの概要](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)の記事の[ポートフォリオオプティマイザーの概要](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

## 稼働率レポート：新規リソース予算計上エリアからの予算計上時間数の入力 {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
>この機能は、2018.2 リリースのプレビュー環境の正式リリースには含まれません。このリリースは、2018.3 リリースのベータ版期間中に再導入され、2018.3 リリースでは実稼動環境にリリースされます。 

稼働率レポートの予算計上時間数が、ビジネスケースの新規リソース予算計上エリアで入手可能な情報から入力されるようになりました。

この変更以前は、従来のリソース見積りエリアの情報が使用されていました。

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の記事の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## 稼働率レポート：プロジェクトのユーザー別予算計上時間数の表示 {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>この機能は、2018.2 リリースのプレビュー環境の正式リリースには含まれません。このリリースは、2018.3 リリースのベータ版期間中に再導入され、2018.3 リリースでは実稼動環境にリリースされます。 

プロジェクトの稼働率レポートに、ユーザ別の予算計上時間数が表示されるようになりました。

この変更以前は、稼動率レポートに担当業務別の予算計上時間数が表示されていました。 

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の記事の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## ドキュメントリストのプルーフの進捗状態をプルーフ以外のユーザーが利用可能に {#proof-progress-from-the-document-list-available-to-non-proofing-users}

ドキュメントリストを表示する際に、すべてのユーザーに対してプルーフの進捗状態インジケーター（送信済み、開封済み、コメント作成済み、決定）が表示されるようになりました。これには、プルーフを生成できないユーザーも含まれます（ユーザーがプルーフを生成できるようにする方法について詳しくは、次の節を参照してください）。

この変更以前は、プルーフの進捗状態インジケーターは、プルーフを生成できるユーザーのみに対して表示されていました。

詳しくは、[プルーフの進捗状態とステータスの概要](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md)を参照してください。

## モバイルの改善点 {#mobile-improvements}

モバイルアプリには、次の機能強化が含まれています。

* 他のモバイルアプリケーションで自分と共有されているリンクが、Workfront モバイルアプリで開くようになりました。

  リンクの共有について詳しくは、次を参照してください。

  この更新は、iOS および Android で利用できるようになりました。

* iPhone X をサポートするために、iOS プラットフォームのサポート要件を更新しました。

  サポートされるモバイルデバイスおよびオペレーティングシステムについて詳しくは、次を参照してください。 
