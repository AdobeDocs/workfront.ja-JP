---
title: 2026年第3四半期レポートの強化
description: 2026年第3四半期レポートの強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b9c63e1ca4b2b301ee104ee84151a2d0148a8cea
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 3%

---

# 2026年第3四半期レポートの強化

このページでは、2026年第3四半期リリースで行われたレポートの機能強化について、プレビュー環境に対して説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2026年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2026年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)を参照してください。

## カスタム式の実際の時間の変更

>[!NOTE]
>
>プレビュー：2026年6月1日> プロダクション高速リリース：2026年6月1日>全員のプロダクション：2026年6月1日

2025年、新しい実時間数フィールドがWorkfront データベースに`actualWorkRequiredDouble`として追加され、既存の実時間数フィールド （`actualWorkRequired` データベース内）の名前が従来の実時間数に変更されました。 詳しくは、[&#x200B; リリースノート &#x200B;](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-project-enhancements.md)を参照してください。

2026年6月、`actualWorkRequired` （従来の実際の時間）を使用する既存のカスタム式は、代わりに`actualWorkRequiredDouble` （実際の時間）を使用するように移行されました。 `actualWorkRequired`は、計算および数式で使用できなくなりました。

また、すべてのレポートで`actualWorkRequiredDouble`を使用することを強くお勧めします。

フィールドを置き換える場合、`actualWorkRequired`は値を分単位で保存し、`actualWorkRequiredDouble`は小数点以下桁で時間単位で値を保存することに注意してください。

実際の時間について詳しくは、[実際の時間を表示](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md)を参照してください。

## キャンバスダッシュボードレポートのカスタム通貨データフィールド

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

Canvas ダッシュボードレポートでは、システム設定で複数の為替レートが設定されている場合など、列、フィルター、グループ化、集計などのカスタム通貨データフィールドがサポートされるようになりました。 カスタム通貨データフィールドが列または集計として表示される場合、フィールドがレポートレベルでロックされていない限り、値はダッシュボードの為替レートトグルで選択された通貨に変換されます。

2回目の為替レート通貨が追加された後に、「制限フィールド」メッセージで以前に失敗したレポートがレンダリングされるようになりました。 複数の為替レートが定義されている場合、計画通貨フィールドは引き続き制限されます。

詳しくは、[&#x200B; キャンバスダッシュボードでの通貨フィールドの使用](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)を参照してください。

## Canvas ダッシュボードレポートでのデータ精度の向上

>[!NOTE]
>
>プレビュー：2026年5月14日>実稼動高速リリース：2026年6月11日>全員の実稼動：2026年7月16日
>
>Canvas ダッシュボードは現在ベータ版です。

Canvas ダッシュボードで、フィルターまたはフィールドが関連するレコードを横断する際に重複する行を防ぐために、レポートクエリが構造化されるようになりました。これにより、カウント、合計、およびその他の集計が正確な値を返します。

以前は、関連レコード間の結合は、関連レコードごとに親レコードを1回繰り返すことができました。 たとえば、特定のユーザーに割り当てられたタスクにフィルタリングされたプロジェクトレポートでは、一致するタスクごとに各プロジェクトが1回繰り返されます。 プロジェクトの予算を合計したKPIは、1,250 ドルではなく6,000 ドルになります。

Canvas ダッシュボードのインターフェイスに変更はありません。 既存のレポートは、このリリース後に正確なデータを自動的に返します。