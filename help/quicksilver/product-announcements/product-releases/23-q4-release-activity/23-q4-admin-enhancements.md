---
title: 2023 年第 4 四半期管理者の機能強化
description: 2023 年第 4 四半期管理者の機能強化
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 2023 年第 4 四半期管理者の機能強化

このページでは、2023 年第 4 四半期のリリースでプレビュー環境に対しておこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、23.10 リリースの実稼動環境で使用できるようになりました。

2023 年第 4 四半期のリリースサイクルで現時点で使用可能なすべての変更点のリストについては、 [2023 年第 4 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## 従来のライセンスモデルのお客様が使用できる配達確認とドキュメントの決定

まだ新しいAdobe Workfrontライセンスモデルに移行していない従来のお客様は、1 ヶ月あたりのユーザーあたりの配達確認/ドキュメントに関する決定数を含むデータを、単一のレポートで表示できるようになりました。 このデータは、ユーザーの決定レポートを実行する際に使用できます。

詳しくは、 [Adobe Workfrontのオブジェクトについて](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) および [すべてのユーザーに対する配達確認およびドキュメントの決定数を表示します](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md).

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
