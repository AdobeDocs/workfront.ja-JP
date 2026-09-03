---
title: 2026年第4四半期レポートの強化
description: 2026年第4四半期レポートの強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: ee1fceee828c97db535ccc03c8b428940d6f7eed
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 8%

---

# 2026年第4四半期レポートの強化

このページでは、2026年第4四半期リリースで行われたレポートの機能強化について、プレビュー環境に対して説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第4四半期リリースサイクルのこの時点で利用可能なすべての変更のリストについては、[2026年第4四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)を参照してください。

<!--

## Duplicate dashboards in Canvas Dashboards

>[!NOTE]
>
>Preview: September 3, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

You can now duplicate a Canvas Dashboard using the new **Duplicate dashboard** action. This action is available to any user whose access level grants edit or create rights to Dashboards, even if they only have view access to the specific dashboard being copied. Users without edit or create rights to Dashboards do not see this action.

When you duplicate a dashboard, you can rename it, update its description and currency, and choose which widgets, dashboard filters, and dashboard prompts to carry over to the copy.

Run as user configurations on widgets are only preserved if you are the designated user or a system administrator. Sharing preferences are not copied to the new dashboard, and a confirmation message with a link to the new dashboard displays once the copy is complete.

Previously, there was no way to duplicate a dashboard; users had to rebuild dashboards from scratch to create audience-specific variations.

For more information, see 

-->

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
| 承認待ち | 承認待ち |

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
