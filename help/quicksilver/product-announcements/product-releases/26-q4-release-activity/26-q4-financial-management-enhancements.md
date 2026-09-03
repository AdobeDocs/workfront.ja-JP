---
title: 2026年第4四半期の財務管理の強化
description: 2026年第4四半期の財務管理の強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 3%

---

# 2026年第4四半期の財務管理の強化

このページでは、プレビュー環境への2026年第4四半期リリースで行われたFinancial Managementの機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第4四半期リリースサイクルのこの時点で利用可能なすべての変更のリストについては、[2026年第4四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)を参照してください。

## 企業の請求率の向上

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日

会社の請求レート機能に複数の更新が行われました。

### WorkfrontとWorkflowのパッケージをご利用のお客様は

* Workfrontの他の領域と一致する、より現代的なデザインで、会社の請求率を追加および編集するためのダイアログボックスを更新しました。
* 「会社レベルの請求レートを許可してプロジェクトレベルの請求レートを上書きする」設定では、会社がプロジェクトに追加されたときにレートの上書きが適切に追加され、予定収益計算では会社レベルの請求レートが使用されます。
* プロジェクト レベルで一般財務を編集および請求率を編集するアクセス権を持たないユーザーは、そのプロジェクトに会社を追加できなくなりました。

### Workflow Ultimate パッケージをご利用のお客様のみ

会社レベルの請求レートに適用できるレート属性が利用可能になりました。 また、適用日は会社の料金にも適用できます。

注意：会社レベルのレートは、レート階層に追加されていません。

詳しくは、[会社レベルで担当業務の請求率を上書きする](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)および[会社レベルの請求率でプロジェクトレベルの請求率を上書きする](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)を参照してください。

## 属性階層が自動的に接続されたままになります

>[!NOTE]
>
>プレビュー：2026年9月3日（PT）
>プロダクション高速リリース：2026年9月17日（PT）
>すべての人のための制作：2026年10月15日
>この機能は、Workflow Ultimate パッケージの組織でのみ使用できます。

高度な割り当てなど、Workfrontの様々な領域でレート属性をフィルターとして使用する場合、親子フィルタリングに追加の検証が適用されるようになりました。

以前は、1つの属性を親に、その親を祖父母にリンクした場合、元の属性も祖父母に属するものとして自動的に認識されませんでした。 これで、最下位レベルの属性を選択すると、その上のすべてのレベルが自動的に割り当てられます。

属性について詳しくは、[ レート属性の定義](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)を参照してください。
