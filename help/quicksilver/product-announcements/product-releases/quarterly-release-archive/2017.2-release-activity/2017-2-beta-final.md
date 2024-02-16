---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 最終ベータ版
description: このページでは、2017.2 リリースのプレビュー環境で最近行われた変更について説明します。このページの機能は、2017年6月28日（PT）にプレビュー環境で使用できるようになりました。2017年7月26日（PT）に、実稼動環境で使用可能になります。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 99%

---

# 2017.2 最終ベータ版

このページでは、2017.2 リリースのプレビュー環境で最近行われた変更について説明します。このページの機能は、2017年6月28日（PT）にプレビュー環境で使用できるようになりました。2017年7月26日（PT）に、実稼動環境で使用可能になります。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017.2 に実装されたすべての変更のリストについては、[2017.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)を参照してください。

2017.2 ベータ版最終リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け：**

* [HTML5 ビデオプルーフビューアーの可用性の決定（ProofHQ および Workfront）](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [SAML 2.0 の SHA-256 証明書をサポート](#support-sha-256-certificates-for-saml-2-0)
* [マッピング属性の先行入力](#type-ahead-for-mapping-attributes)
* [API 機能強化：ユーザー割り当てへのアクセス](#api-enhancement-access-user-allocations)

**すべてのユーザーの場合：**

* [リソースプランナー](#resource-planner)
* [プロジェクトの新しいスケジュールエリア（チームビルダー）](#new-scheduling-area-in-a-project-team-builder)
* [リソーススケジュール設定：デフォルトで少ない項目数を表示する](#resource-scheduling-show-fewer-items-by-default)
* [リソーススケジュール設定：タスクとイシューをドラッグ時にドロップインジケーターと超過割り当てを表示する](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [リソーススケジュール設定：ユーザー割り当てが 30 分単位に四捨五入されなくなった](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [TSV および PDF 形式での使用状況レポートの書き出し](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 ベータ版最終版](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 ベータ版最終版](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [担当作業エリア（Workfront）にプルーフ決定が表示される](#proof-decision-displays-in-the-my-work-area-workfront)
* [プリセット解像度でのリッチメディアプルーフの表示（ProofHQ および Workfront）](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [リッチメディアプルーフに関するコメントのサブページへの URL を表示（ProofHQ および Workfront）](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [既存の標準ビューに基づくカスタムビューの作成（ProofHQ）](#create-custom-views-based-on-existing-standard-views-proofhq)
* [レポートエリアのフィルター（ProofHQ）](#filter-the-reporting-area-proofhq)
* [レポートでの最小値と最大値の表示（ProofHQ）](#display-minimum-and-maximum-values-in-reports-proofhq)
* [プルーフの承認用のアプリ内通知](#in-app-notification-for-proof-approval)
* [モバイル機能の強化](#mobile-improvements)
* [コンマを含むフィールド値のフィルターステートメントに追加されるスラッシュ](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [複数の請求レート](#multiple-billing-rates)
* [新しい「予算計上リソース時間」フィールド](#new-resource-budgeted-hour-field)
* [タスクおよびイシューの詳細ページで「割り当て先」エリアにユーザーの担当業務を表示](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

## プロジェクトの新しいスケジュール設定エリア（チームビルダー） {#new-scheduling-area-in-a-project-team-builder}

プロジェクト（旧称チームビルダー）のスケジュール設定エリアは、より直感的な最新のユーザーインターフェイスに再設計されました。新しいスケジュール設定機能は、Workfront の他のエリアで現在使用可能なリソーススケジュール設定機能とより密接に一致するようになりました。

改善点は次のとおりです。

* プロジェクトチームのメンバーに対する現在のリソース割り当てを表示し、割り当てを行う際に、より十分な情報に基づいた意思決定を行うことができる
* スケジュールのタイムライン上のタスク期間を視覚的に表す
* スケジュールタイムラインに表示される情報がフィルタリングされる
* スケジュールタイムラインから直接、プロジェクトチームにユーザーを簡単に追加および削除できる

次の機能は、リソースをスケジュールする場合はツールの他のエリアで使用できますが、チームスケジュールエリアでリソースをスケジュールする場合は使用できません。

* 親タスクを設定してスケジュールタイムラインに表示する
* スケジュールタイムラインに表示するプロジェクト名を設定
* スワップツールを使用してユーザー割り当てを変更
* ポートフォリオ、プログラム、プロジェクトでフィルタリング

チームスケジュールエリアで使用できる機能について詳しくは、「リソースのスケジュール設定の概要」を参照してください。

## リソーススケジュール設定：デフォルトで表示する項目数を減らす {#resource-scheduling-show-fewer-items-by-default}

デフォルトでは、1 日に最大 10 個の作業アイテムが、特定のユーザーのスケジュールタイムラインに表示されるようになりました。リストを展開して、そのユーザーに現在割り当てられているすべてのタスクとイシューを表示できます。

これにより、ユーザーに多くのタスクやイシューが割り当てられた場合に、スケジュールタイムラインを参照しやすくなります。

この変更以前は、すべてのユーザーに対して、すべてのタスクとイシューが常に表示されていました。

スケジュールタイムラインでユーザーにタスクとイシューを割り当てる方法について詳しくは、「スケジュールエリアで未割り当てタスクとイシューを手動で割り当て」を参照してください。

## リソーススケジュール設定：タスクとイシューをドラッグ時にドロップインジケーターと超過割り当てを表示 {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

ドラッグ＆ドロップ操作によりスケジュールタイムラインでタスクまたはイシューをユーザーに割り当てると、タスクまたはイシューを解放して割り当てを完了する前に、次の情報が表示されるようになりました。

* ユーザーの行にドロップインジケーターが表示されます。これにより、割り当てを行う前に項目が割り当てられている場所を確認できます。
* スケジュールタイムラインでユーザー割り当てが有効になっている場合、割り当てが完了してユーザーが割り当て超過になると、赤い割り当て超過インジケーターが表示されます。

これらの変更以前は、タスクまたはイシューをリリースする前に、情報は表示されませんでした。

スケジュールタイムラインでユーザーにタスクとイシューを割り当てる方法について詳しくは、「スケジュールエリアで未割り当てタスクとイシューを手動で割り当て」を参照してください。

## リソーススケジュール設定：ユーザー割り当てが 30 分単位に丸められなくなった {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

複数のユーザーがタスクやイシューに割り当てられた場合、またはタスクやイシューが複数日にわたる場合、Workfront は、割り当てられたユーザーや日数に予定時間数を均等に配分しようとします。時間は、デフォルトで最も近い小数点第 2 位を四捨五入します（例：1.33）。

以前は、配分された時間を手動で変更した場合、時間は調整されて最も近い 30 分単位に四捨五入されました（例えば、1.33 は 1.5 に四捨五入されます）。

現在は、時間は調整されず、最も近い 30 分単位に四捨五入されません（例えば、1.33 は 1.33 のままです）。

## API 機能強化：ユーザー割り当てへのアクセス {#api-enhancement-access-user-allocations}

Workfront API を使用して、ユーザー割り当ての背景色にアクセスできるようになりました。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## TSV および PDF 形式で稼働率レポートを書き出す {#export-the-utilization-report-in-tsv-and-pdf-formats}

XLSX 形式に加えて、プロジェクトの稼働率レポートを TSV および PDF 形式で書き出せるようになりました。

この変更以前は、稼働率レポートを XLSX 形式でのみ書き出すことができました。

稼働率レポートの書き出しについて詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)内の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## 自分の作業エリア内（Workfront）にプルーフ決定を表示 {#proof-decision-displays-in-the-my-work-area-workfront}

自分の作業エリアの「マイ承認」タブでプルーフ承認を表示すると、プルーフ決定が自分の作業エリアに表示され、Workfront 内の新しい「更新」ボタンをクリックするか、次にブラウザーページを更新するまで保持されます。

この変更以前は、プルーフに対する決定が既に行われたことは示されておらず、ブラウザーを更新するまで、プルーフは「マイ承認」タブに表示されたままでした。

詳しくは、[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)の[作業の承認](../../../../review-and-approve-work/manage-approvals/approving-work.md)を参照してください。

## プリセット解像度でリッチメディアプルーフを表示（ProofHQ および Workfront） {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

プレビュー環境の以前のリリースでは、カスタム解像度を指定するか、画像を目的の解像度にドラッグすることで、リッチメディアプルーフの解像度を調整する機能が導入されました。

様々な携帯電話、タブレット、ノート、デスクトップのプリセット解像度オプションから選択できるようになりました。

詳しくは、[プルーフビューアでインタラクティブなプルーフの解像度を変更](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)内の「プリセット解像度の表示」を参照してください。

## リッチメディアプルーフに関するコメントのサブページへの URL を表示（ProofHQ および Workfront） {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>この機能は、現在、実稼働環境で使用できます。

リッチメディアプルーフのサブページにコメントする際に、サブページの URL がコメントに表示されるようになりました。

この変更以前は、コメントが参照しているサブページが明確ではありませんでした。

詳しくは、次を参照してください。

## HTML5 ビデオプルーフビューア（ProofHQ および Workfront）が利用できるかどうかを確認 {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

ProofHQ の Workfront 管理者は、組織内のユーザーがビデオプルーフ用の新しい HTML5 プルーフビューアにアクセスできるかどうかを指定できます。

Workfront でこのオプションを設定する方法について詳しくは、以下を参照してください。

## 既存の標準ビューに基づいてカスタムビューを作成（ProofHQ） {#create-custom-views-based-on-existing-standard-views-proofhq}

標準ビューに基づいてカスタムビューを作成できるようになりました。標準ビューの列、並べ替え、フィルターの各オプションは、デフォルトで新規ビューに含まれます。

この変更以前に、カスタムビューを作成するには、最初からビューを作成する必要がありました。 

詳しくは、[Workfront Proof でのカスタムビューの作成と管理](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)の[カスタムビューの作成](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating)を参照してください。

## レポートエリアをフィルタリング（ProofHQ） {#filter-the-reporting-area-proofhq}

デフォルトでは、「レポート」タブに表示されるデータには、ProofHQ システムからのすべての情報が含まれます。フィルターを使用して、必要に応じた情報のみを表示できるようになりました。 

詳しくは、[Workfront Proof でのレポートの実行](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md)の[レポートのフィルタリング](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports)を参照してください。

## レポートに最小値と最大値を表示（ProofHQ） {#display-minimum-and-maximum-values-in-reports-proofhq}

レポートの表示時にグラフに最小値と最大値を表示するかどうかを設定できるようになりました。

詳しくは、[Workfront Proof でのレポートの実行](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md)の[レポートの表示](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports)を参照してください。

## SAML 2.0 の SHA-256 証明書をサポート {#support-sha-256-certificates-for-saml-2-0}

SAML 2.0 で SSO 用に Workfront を設定する際の Secure Hash Algorithm 256（SHA-256）のサポートを開始しました。このリリース以前は、Secure Hash Algorithm 1（SHA-1）のみをサポートしていました。

SAML 2.0 での Workfront の設定について詳しくは、[SAML 2.0 での Adobe Workfront の設定](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)を参照してください。

## マッピング属性の先行入力 {#type-ahead-for-mapping-attributes}

属性マッピングダイアログボックスの既定値のフィールドタイプが、先行入力フィールドに更新されました。この変更以前は、「既定値」フィールドのタイプはドロップダウンになっていました。

この変更は、次の SSO プロトコルに適用されます。

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 は属性マッピングをサポートしていません。

## モバイルの改善点 {#mobile-improvements}

>[!NOTE]
>
>モバイルアプリケーションは、メインの Workfront アプリケーションとは独立してリリースされます。このセクションに記載されている機能のリリースは 8 月初旬となります。

Android および iOS の両方のプラットフォームのモバイルアプリに、次の機能が追加されますた。

* モバイルアプリからのリクエストの送信
* モバイルアプリのタイムシートの新しいエントリ
* モバイルアプリからのカスタムフォーム編集
* モバイルアプリでのプルーフの承認リクエスト

Android プラットフォーム向けのこれらの機能の一部では、パブリックベータ版プログラムが提供されます。

モバイル向けの今後のベータ版プログラムについて詳しくは、[ベータ版](https://support.workfront.com/hc/ja-jp/sections/115000743248)ページを参照してください。

Workfront モバイルアプリの使用について詳しくは、次を参照してください。  

## コンマを含むフィールド値のフィルターステートメントに追加されるスラッシュ {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

テキストモードでフィルターを作成し、コンマを含むフィールド値のフィルタリングを行う場合は、値を 1 つのフィルターオプションとして読み取るために、値を区切るコンマの前にスラッシュ（「/」）を追加する必要があります。これは、次のフィールドタイプにのみ該当します。

* ドロップダウン
* ラジオボタン
* チェックボックス

この変更以前は、コンマを含むオプションをがあるフィールドをフィルタリングすることはできませんでした。

この変更について詳しくは、 [フィルターの概要](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## 複数の請求レート {#multiple-billing-rates}

プロジェクトレベルで、同じ担当業務に対して複数の請求レートの上書きを追加できるようになりました。この新機能を使用すると、請求レートの上書きごとに日付範囲を定義できます。指定した日付範囲では、プロジェクトのタスクに割り当てられた担当業務に異なる請求料率が適用されます。請求料率にプロジェクトの時間数を掛けて、収益を計算します。請求料率の日付範囲内で計算された収益は、その率でロックされたままになり、プロジェクトの更新時に担当業務の率として更新されません。実収益の場合、請求料率を上書きする前にログに記録された時間は再計算されず、現在の請求料率が反映されます。請求料率の上書きがプロジェクトに追加される前に記録された時間は、その時点での担当業務の請求料率に関連付けられます。

この変更以前は、担当業務の請求料率を上書きできたのは 1 回限りで、実収益は請求料率が変更される前に記録されたすべての時間の現在の請求料率を反映するように再計算されていました。

請求料率および収益について詳しくは、[請求と収益の概要](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)を参照してください。

プロジェクトレベルでの担当業務の請求料率の上書きについて詳しくは、[担当業務の請求料率の上書きおよびプロジェクトでの収益の計算の概要](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)を参照してください。

## リソースプランナー {#resource-planner}

このリリースでは、ユーザーエリアの新しい「計画」タブの再設計の一環として、リソースプランナーの第 1 段階を導入します。リソースプランナーを使用すると、リソースプール内のユーザーが、リソースマネージャーの現在のすべてのプロジェクトに割り当てられる時間を予算計上できます。リソースプランナーには、プロジェクト別、担当業務別およびユーザー別の次の割り当て数が表示されます。

* 利用可能時間数
* 予定時間数
* 予算計上時間数
* 時間差異（予算計上時間数と予定時間数の差）
* 正味時間差（利用可能時間数と予算計上時間数の差）

リソースプランナーの使用について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## 新しいリソース予算計上時間数フィールド {#new-resource-budgeted-hour-field}

新しい計画機能とリソースプランナーをサポートするために、Report Builder に新しいフィールドが追加されました。このフィールドを使用して、予算計上リソース時間数に関するレポートを作成できます。このフィールドは、プロジェクトで予算計上されているリソースの時間数を取り込みます。従来のリソース計画機能を使用してリソースを予算計上する場合、このフィールドは使用できません。

リソースプランナーでの予算計上時間数の使用について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## プルーフ承認のアプリ内通知 {#in-app-notification-for-proof-approval}

プルーフの承認者として指定されると、決定を待つプルーフの承認に関するアプリ内通知が届きます。通知には、次のテキストが表示されます：`<User name>` さんがこのプルーフの承認を依頼しています。ユーザー情報が得られない場合、通知は「このプルーフにはあなたの承認が必要です」に変わります。

この機能強化以前は、プルーフの承認者として指定された視覚的な唯一の表示は、担当作業エリアの新規プルーフリクエストでした。

アプリ内通知について詳しくは、[アプリ内通知の表示と管理](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)を参照してください。

## タスクおよびイシューの詳細ページで「割り当て先」エリアにユーザーの担当業務を表示 {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

タスクまたはイシューの詳細ページを表示すると、割り当て先エリアの担当者の名前の下に、担当業務が表示されるようになりました。この担当業務は、タスクまたはイシューの担当業務の割り当てに一致するユーザーの担当業務を表します。タスクまたはイシューが担当業務に割り当てられていない場合、割り当てられたユーザーのプライマリ担当業務が表示されます。

この変更以前は、「割り当て先」エリアのユーザー名の下に、ユーザーのタイトルのみが表示されていました。 
