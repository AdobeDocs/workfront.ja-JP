---
title: 2023年第 4 四半期の管理者の機能強化
description: 2023年第 4 四半期の管理者の機能強化
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 97%

---

# 2023年第 4 四半期の管理者の機能強化

このページでは、プレビュー環境に対すして 2023年第 4 四半期に行われた管理者向けのすべての機能強化について説明します。これらの機能強化は、23.10 リリースの実稼動環境で使用できるようになりました。

2023年第 4 四半期のリリースサイクルの現時点で利用可能なすべての変更点のリストについては、[2023年第 4 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)を参照してください。

## 従来のライセンスモデルのお客様が利用可能なプルーフとドキュメントの決定

新しい Adobe Workfront ライセンスモデルにまだ移行していない従来のお客様は、月ごとのユーザーあたりのプルーフとドキュメントに関する決定数を含むデータを、単一のレポートで表示できるようになりました。このデータは、ユーザーの決定レポートを実行する際に使用できます。

詳しくは、[Adobe Workfront のオブジェクトについて](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)および[すべてのユーザーに対するプルーフとドキュメントの決定数の表示](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md)を参照してください。

## カスタムフォームの計算済みフィールドで、$$USER ワイルドカードを使用可能

新しいフォームデザイナーの計算済みカスタムフィールドと外部参照フィールドで、`$$USER` ワイルドカードを使用できるようになりました。計算で `$$USER` を参照すると、現在のユーザーの ID が追加されます。このワイルドカードは別のフィールドで使用することもできます。例えば、`$$USER.{name}` では現在のユーザーの名前が追加されます。

計算済みフィールドについて詳しくは、[フォームデザイナーで計算済みフィールドを追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)を参照してください。

## 外部 API からカスタムフォームへの値オプションの追加

カスタムフォームデザイナーで新しいフィールドタイプ「**外部参照**」を使用できるようになりました。データを外部システムに保存している場合、このフィールドタイプを使用すると、外部 API からオプションを読み込み、カスタムフォーム内の他のフィールド値に基づいてフィルタリングできます。

フォームをオブジェクトに追加すると、API から返される値がドロップダウンフィールドに表示され、ユーザーが選択できます。

>[!NOTE]
>
>新しい&#x200B;**外部参照**&#x200B;フィールドタイプは、従来のフォームビルダーでは使用できません。

詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。
