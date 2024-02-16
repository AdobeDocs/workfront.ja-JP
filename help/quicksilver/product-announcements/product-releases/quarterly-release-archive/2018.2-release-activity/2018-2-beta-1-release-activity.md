---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 1 リリースアクティビティ
description: このページでは、2018.2 Beta 1 リリースのプレビュー環境で利用可能な最新の変更についてすべて説明します。この機能は、2018年3月22日（PT）にプレビュー環境で使用できるようになりました。2018年6月に、実稼動環境で利用できるようになります。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 100%

---

# 2018.2 Beta 1 リリースアクティビティ

このページでは、2018.2 Beta 1 リリースのプレビュー環境で利用可能な最新の変更についてすべて説明します。この機能は、2018年3月22日（PT）にプレビュー環境で使用できるようになりました。2018年6月に、実稼動環境で利用できるようになります。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018.2 で行われたすべての変更のリストについては、[2018.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)を参照してください。

2018.2 Beta 1 リリースには、次の機能強化が含まれています。

* [ガントチャートのタスクの日付の変更](#modify-task-dates-in-the-gantt-chart)
* [「更新」タブからプロジェクトのガントチャートへのアクセス](#access-the-project-gantt-chart-from-the-updates-tab)（一時的に削除）

* [ドキュメントリスト上のドキュメントに様々なリンクを再導入](#various-links-re-introduced-to-documents-on-the-document-list)
* [リソースプランナーのユーザー表示の向上](#user-view-improvements-in-the-resource-planner)
* [新しいプロジェクトリストエクスペリエンス](#new-project-list-experience)
* [「更新」タブの新しい外観](#new-look-for-updates-tab)
* [モバイルの改善点](#mobile-improvements)

## ガントチャートのタスクの日付の変更 {#modify-task-dates-in-the-gantt-chart}

タスクバブルをドラッグして、ガントチャートの予定開始日と予定完了日を変更できるようになりました。この変更により、タイムラインに影響を与えることなく、プロジェクトに what-if シナリオを適用できます。

この変更を行う前は、タスクリストまたはタスクレベルでのみタスクの日付を変更できました。

詳しくは、[タスクリストのガントチャートの情報の更新](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)を参照してください。

## 「更新」タブからプロジェクトのガントチャートへのアクセス {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>この機能は、プレビュー環境から一時的に削除されました。

「更新」タブから新しいプロジェクトのガントチャートにアクセスできるようになりました。ユーザーが、プロジェクトタイムラインに影響を与えるようにタスクのコミット日を変更した場合、プロジェクトのガントチャートでその影響を確認できます。

この変更を行う前は、「プロジェクトのタイムライン」のリンクをクリックすると、従来のガントチャートが開きました。

詳しくは、[コミット日の概要](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)を参照してください。

詳しくは、[ポートフォリオオプティマイザーの概要](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

## ドキュメントリスト上のドキュメントに様々なリンクを再導入 {#various-links-re-introduced-to-documents-on-the-document-list}

18.1 リリースでは、様々なリンクがドキュメントリスト上のドキュメントから削除され、インターフェイスの他のエリアに移動されました（ドキュメント名の横のボタンや、ボタンのドロップダウンメニューで表示されました）。次のリンクは、本リリースでドキュメント名の下に再導入され、ドキュメントリスト内の個々のドキュメントで使用できるようになりました。

* プルーフを生成（プルーフが生成されていない場合に使用可能）
* プルーフを開く（プルーフが生成されたときに使用可能）
* ドキュメントの詳細（プルーフが生成されていない場合に使用可能）
* プルーフの詳細（プルーフが生成されたときに使用可能）
* 概要を印刷

次のアクションは、ドキュメントリスト内のドキュメント上のリンクとして再導入されません。

* 共有（メニューのボタンとして引き続き使用可能）
* チェックアウト、チェックイン（メニューのその他ドロップダウンメニューから引き続き利用可能）

詳しくは、次の節を参照してください。

* &nbsp;
* &nbsp;in&nbsp;

## リソースプランナーのユーザービューの向上 {#user-view-improvements-in-the-resource-planner}

リソースプランナーのユーザービューには、次の改善点が含まれます。

* プロジェクトビューに代わり、ユーザビューがデフォルトのビューになりました。
* 画面上の情報だけでなく、データベース全体から情報を取り込むようにフィルターを改善しました。
* フルスクリーンモード。
* パフォーマンスを高速化および効率化しました。

   * 表示できるユーザー、プロジェクト、役割、タスクの数に関する新しい制限。
   * 遅延読み込み。ユーザーの読み込みを高速化します。

次の機能は、リソースプランナーで一時的に無効になっています。

* ユーザービュー使用時の、リソースプランナーからのデータの書き出し。

この改善が行われる前は、リソースプランナーの読み込みが遅く、表示されるデータに不一致が見られるとの報告がありました。上記の改善により、これらの問題は解消されたはずです。

リソースプランナーのエリアの詳細は、[リソースプランナーのナビゲーションの概要](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)を参照してください。

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## 新しいプロジェクトリストエクスペリエンス {#new-project-list-experience}

プロジェクトのリストを表示する際に、新しいエクスペリエンスを使用できるようになりました。このエクスペリエンスには、パフォーマンスの向上と、よりスムーズで迅速なリストナビゲーションが含まれます。Workfront のプロジェクトエリアにある「プロジェクト」タブのリストのみが、この新しいエクスペリエンスに更新されています。

大部分は、リストの速度と効率が変更されます。次の表示に関する変更も追加されました。

* リストには、デフォルトで最大 2,000 個の項目が表示されます。

  この機能強化以前は、リストに 100 個の項目が表示されていました。

* グループ化は、デフォルトで折りたたまれます。

  この変更が行われる前は、デフォルトでグループ化が展開されていました。

* 行を選択するエリアが行全体に展開されました。

次の機能は、指定したプロジェクトのリストで一時的に無効になっています。

* 列のサイズ変更（この機能は 2018.2 Beta 5 リリースで再導入されました）
* 列の並べ替え
* ステータスアイコンのフィールドは空白で表示されます。（この機能は 2018.2 Beta 5 リリースで再導入されました）
* ガントチャートにアクセスできません。（この機能は 2018.2 Beta 3 リリースで再導入されました）

リストでの作業について詳しくは、[Adobe Workfront 内のリストの概要](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)を参照してください。

## 「アップデート」タブの新しいルック {#new-look-for-updates-tab}

>[!NOTE]
>
>一部のユーザーでは、プレビュー環境で新しい「更新」タブが表示されない場合があります。現在、アドビの開発チームは、可能な限り早く問題のトラブルシューティングを行い、問題解決に至るまでの作業を進めています。

「更新」タブのルックアンドフィールが変更され、インターフェイスの他のエリアとの統一感が増しました。この変更は、プロジェクト、タスク、イシューおよびドキュメントに適用されます。

次の表に、「更新」タブに加えられたアップデートを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>タスク</strong> </p> </th> 
   <th> <p><strong>以前のユーザーアクション</strong> </p> </th> 
   <th> <p><strong>新規ユーザーアクション</strong> </p> </th> 
   <th> <p><strong>詳細情報</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タイムシートで時間をログに記録</p> </td> 
   <td> <p>「時間をログに記録」リンクをクリック</p> </td> 
   <td> <p>「時間をログに記録」ボタンをクリック</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">時間をログに記録</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>「更新」タブでのシステム更新をフィルタリングで除外</p> </td> 
   <td> <p>「システム更新をフィルタリング」リンクをクリック</p> </td> 
   <td> <p>「アクティビティログを表示」切り替えスイッチを無効にする</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>「更新」タブでのシステム更新の表示</p> </td> 
   <td> <p>「すべての更新を表示」をクリック</p> </td> 
   <td> <p>「アクティビティログを表示」切り替えスイッチを有効にする</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>更新またはコメントに対する他のユーザーのタグ付け</p> </td> 
   <td> <p>この更新に他者を含めるアイコンをクリック</p> </td> 
   <td> <p>通知フィールドでユーザーとチームを追加</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>社内のユーザーのみにオブジェクトの表示を許可</p> </td> 
   <td> <p>ロックアイコンをクリック</p> </td> 
   <td> <p>マイ会社の切替スイッチでプライベートを有効にする</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>社外のユーザーに対してオブジェクトの表示を許可</p> </td> 
   <td> <p>ロックアイコンをクリック</p> </td> 
   <td> <p>マイ会社の切り替えスイッチでプライベートを無効にする</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>コメントまたは更新に対して返信または更新を追加</p> </td> 
   <td> <p>「コメント」ボタンをクリック</p> </td> 
   <td> <p>「返信」または「更新」ボタンをクリック</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業の更新</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">タスクのステータスの更新</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">タスクおよびイシューの状況の更新</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">ドキュメントへの更新の追加</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## モバイルの改善点 {#mobile-improvements}

モバイルアプリには、次の機能強化が含まれています。

* 他のモバイルアプリケーションで自分と共有されているリンクが、Workfront モバイルアプリで開くようになりました。

  リンクの共有について詳しくは、以下を参照してください。

  この更新は iOS に今週中にリリースされ、Android の更新はその直後になります。

* iPhone X をサポートするために、iOS プラットフォームのサポート要件を更新しました。

  サポートされるモバイルデバイスおよびオペレーティングシステムについて詳しくは、以下を参照してください。
