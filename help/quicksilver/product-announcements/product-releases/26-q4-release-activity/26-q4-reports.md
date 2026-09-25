---
title: 2026年第4四半期レポートの強化
description: 2026年第4四半期レポートの強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: c94c1f3d662cee00a12c786063a4e4db2015361d
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 8%
---
# 2026年第4四半期レポートの強化

このページでは、2026年第4四半期リリースで行われたレポートの機能強化について、プレビュー環境に対して説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第4四半期リリースサイクルのこの時点で利用可能なすべての変更のリストについては、[2026年第4四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)を参照してください。

<!--

## Filter on collection relationships in Canvas Dashboards

>[!NOTE]
>
>Preview: September 24, 2026
>Production fast release: October 14, 2026
>Production for everyone: October 15, 2026

When you build a filter in a Canvas Dashboard, you can now filter on collection relationships, which are fields that link to a group of related records rather than to a single record. For example, you can filter on the status of tasks belonging to a project to show a list of projects that have tasks in the "New" status.

Previously, filtering on collection relationships required text mode.

For more information, see [Report filter reference for Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

-->

## Canvas ダッシュボードでのダッシュボードのコピー

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

新しい&#x200B;**ダッシュボードをコピー** アクションを使用して、キャンバスダッシュボードをコピーできるようになりました。 このアクションは、アクセス レベルがダッシュボードに編集権限または作成権限を付与しているユーザーは、コピーする特定のダッシュボードへの表示アクセス権しか持っていない場合でも、使用できます。 ダッシュボードの編集権限または作成権限を持たないユーザーには、このアクションは表示されません。

ダッシュボードをコピーする場合は、名前を変更し、説明と通貨を更新して、コピーに引き継ぐウィジェット、ダッシュボードフィルター、ダッシュボードプロンプトを選択できます。

ウィジェットのユーザー設定として実行は、指定ユーザーまたはシステム管理者の場合にのみ保持されます。 共有の環境設定は新しいダッシュボードにコピーされず、コピーが完了すると、新しいダッシュボードへのリンクを含む確認メッセージが表示されます。

以前は、ダッシュボードをコピーする方法がありませんでした。ユーザーは、オーディエンス固有のバリエーションを作成するために、ダッシュボードをゼロから再構築する必要がありました。

## カンバスダッシュボードの「承認タイプ」フィールド

>[!NOTE]
>
>すべての人のための制作：2026年8月28日
>[!BADGE スケジュール外]{type=Neutral}

承認エンティティに&#x200B;**承認タイプ** フィールドが含まれるようになりました。このフィールドを使用すると、プルーフの承認、ドキュメントバージョンの承認、取り込み承認およびその他の承認の種類を区別できます。

## Canvas ダッシュボードでの承認用語の更新

>[!NOTE]
>
>すべての人のための制作：2026年8月28日
>[!BADGE スケジュール外]{type=Neutral}

ドキュメントと作業の承認に使用されるCanvas ダッシュボードで使用される次のフィールド名は、わかりやすいように変更されました。

| 前の名前 | 新しい名前 |
| --- | --- |
| ドキュメントの承認 | 承認 |
| ドキュメントの承認ステージ | 承認ステージ |
| ドキュメントの承認ステージ参加者 | 承認ステージ参加者 |
| 承認プロセス | 作業承認プロセス |
| 承認ステージ | 作業承認ステージ |
| 上書きされている | 作業承認者のステータス |
| 承認待ち | 作業の承認待ち |

この変更は、現在のレポートの機能には影響しません。

## Canvas ダッシュボードのピボットテーブルレポート

>[!NOTE]
>
>プレビュー：2026年8月27日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

Canvas ダッシュボードの新しいピボットテーブルレポートタイプでは、正確で完全なロールアップを使用してデータを集約します。 カウント、合計、平均などの指標をダッシュボードで直接作成し、その合計の背後にあるレコードをドリルダウンできます。

詳しくは、「[&#x200B; キャンバスダッシュボードでピボットテーブルレポートを作成する](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md)」を参照してください。

## スケジュールレポートの終了日の適用

>[!NOTE]
>
>プレビュー：2026年8月13日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

スケジュールされたレポートは、無期限の配信を防ぐために終了日が必要になりました。 終了日を通過するスケジュールは、自動的に非アクティブ化されます。

既存のスケジュールは、信頼性を向上させ、不要なシステム使用を減らすために、終了日を更新しました。 また、Workfrontでは、レポートのスケジュールのライフサイクルが終了日に近づいたときに、レポートのスケジュールを管理するのに役立つ可視性と警告も提供されます。

詳しくは、[自動レポート配信のスケジュール &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)を参照してください。

## ネイティブ参照フィールドは、リストとレポートで使用できます

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年8月13日（PT）
>すべての人のための制作：2026年10月15日

Workfrontのリストとレポートにネイティブ参照フィールドを追加できるようになりました。

ネイティブ参照フィールドはカスタムフィールドです。 フィールドがオブジェクトに添付されたカスタムフォーム上にある場合、フィールドはオブジェクトデータから入力されます。 例えば、フィールドが「説明」フィールドを参照し、それがプロジェクトに添付されたカスタムフォーム上にある場合、フィールドはプロジェクトの説明を取り込みます。 （データが利用できない場合、フィールドには「該当なし」と表示される場合があります）。

サポートされているネイティブフィールドのリストを含むネイティブ参照フィールドの作成について詳しくは、[&#x200B; カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。
レポートへのフィールドの追加について詳しくは、[&#x200B; カスタムレポートの作成](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

## 従来のリストやレポートにおける複数選択フィールド値の一貫性のある順序付け

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年8月13日（PT）
>すべての人のための制作：2026年10月15日

複数を選択したカスタムフィールドのオプションが、従来のリストとレポートで一貫した予測可能な順序で表示されるようになりました。 フィールドの順序は、カスタムフォームでのフィールドの配置方法によって決まります。

![&#x200B; カスタムフォームフィールドの順序が、リストまたはレポートで選択した値の順序と一致する](assets/new-field-order-multi-select.png)

以前は、選択したオプションが選択した順序で表示されていたり、一貫性のない順序で表示されていたため、行のスキャンと比較が困難になっていました。

注意：フィールドがテキストモードを使用している場合、新しい並べ替えは適用されません。
