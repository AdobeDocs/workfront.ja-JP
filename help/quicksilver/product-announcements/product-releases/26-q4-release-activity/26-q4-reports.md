---
title: 2026年第4四半期レポートの強化
description: 2026年第4四半期レポートの強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: c34c4f351010980098b3efece8643a5f5620917f
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 5%

---

# 2026年第4四半期レポートの強化

このページでは、2026年第4四半期リリースで行われたレポートの機能強化について、プレビュー環境に対して説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第4四半期リリースサイクルのこの時点で利用可能なすべての変更のリストについては、[2026年第4四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)を参照してください。

## スケジュールレポートの終了日の適用

>[!NOTE]
>
>プレビュー：2026年8月13日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

スケジュールされたレポートは、無期限の配信を防ぐために終了日が必要になりました。 終了日を通過するスケジュールは、自動的に非アクティブ化されます。

既存のスケジュールは、信頼性を向上させ、不要なシステム使用を減らすために、終了日を更新しました。 また、Workfrontでは、レポートのスケジュールのライフサイクルが終了日に近づいたときに、レポートのスケジュールを管理するのに役立つ可視性と警告も提供されます。

詳しくは、[自動レポート配信のスケジュール ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)を参照してください。

<!--

## Updated column headers for dependent connected record fields

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

We've made visual improvements to the column headers for a dependent connected record field in the table view.

For information, see [Manage dependent connections](/help/quicksilver/planning/architecture/manage-dependent-connections.md).

-->

## ネイティブ参照フィールドは、リストとレポートで使用できます

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年8月13日（PT）
>すべての人のための制作：2026年10月15日

Workfrontのリストとレポートにネイティブ参照フィールドを追加できるようになりました。

ネイティブ参照フィールドはカスタムフィールドです。 フィールドがオブジェクトに添付されたカスタムフォーム上にある場合、フィールドはオブジェクトデータから入力されます。 例えば、フィールドが「説明」フィールドを参照し、それがプロジェクトに添付されたカスタムフォーム上にある場合、フィールドはプロジェクトの説明を取り込みます。 （データが利用できない場合、フィールドには「該当なし」と表示される場合があります）。

サポートされているネイティブフィールドのリストを含むネイティブ参照フィールドの作成について詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。
レポートへのフィールドの追加について詳しくは、[ カスタムレポートの作成](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

## 従来のリストやレポートにおける複数選択フィールド値の一貫性のある順序付け

>[!NOTE]
>
>プレビュー：2026年7月30日（PT）
>プロダクション高速リリース：2026年8月13日（PT）
>すべての人のための制作：2026年10月15日

複数を選択したカスタムフィールドのオプションが、従来のリストとレポートで一貫した予測可能な順序で表示されるようになりました。 フィールドの順序は、カスタムフォームでのフィールドの配置方法によって決まります。

![ カスタムフォームフィールドの順序が、リストまたはレポートで選択した値の順序と一致する](assets/new-field-order-multi-select.png)

以前は、選択したオプションが選択した順序で表示されていたり、一貫性のない順序で表示されていたため、行のスキャンと比較が困難になっていました。

注意：フィールドがテキストモードを使用している場合、新しい並べ替えは適用されません。
