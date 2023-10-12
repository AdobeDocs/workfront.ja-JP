---
title: 2023 年第 4 四半期管理者の機能強化
description: 2023 年第 4 四半期管理者の機能強化
author: Lisa
feature: Product Announcements
source-git-commit: 8488cb46b3dd9b377c59121597db5b6fe784fdab
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# 2023 年第 4 四半期管理者の機能強化

このページでは、2023 年第 4 四半期のリリースでプレビュー環境に対しておこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、23.10 リリースの実稼動環境で利用できるようになります。

2023 年第 4 四半期のリリースサイクルで現時点で使用可能なすべての変更点のリストについては、 [2023 年第 4 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## カスタムフォームの計算フィールドで、$$USER ワイルドカードを使用できるようになりました

The `$$USER` 新しいフォームデザイナーで、計算カスタムフィールドと外部参照フィールドでワイルドカードを使用できるようになりました。 参照 `$$USER` 計算では、現在のユーザーの ID が追加されます。 別のフィールドでワイルドカードを使用することもできます。 例： `$$USER.{name}` 現在のユーザーの名前を追加します。

計算フィールドについて詳しくは、 [フォームデザイナーで計算フィールドを追加する](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## 外部 API からカスタムフォームに値オプションを追加する

新しいフィールドタイプ **外部参照**&#x200B;をカスタムフォームデザイナーで使用できるようになりました。 データを外部システムに保存している場合、このフィールドタイプを使用すると、外部 API からオプションを読み込み、カスタムフォーム内の他のフィールド値に基づいてフィルタリングできます。

フォームをオブジェクトに追加すると、API から返される値がドロップダウンフィールドに表示され、ユーザーが選択できます。

>[!NOTE]
>
>新しい **外部参照** フィールドタイプは、従来のフォームビルダーでは使用できません。

詳しくは、 [フォームデザイナーを使用したフォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
