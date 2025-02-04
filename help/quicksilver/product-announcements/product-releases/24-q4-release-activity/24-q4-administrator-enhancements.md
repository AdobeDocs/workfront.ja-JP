---
title: 2024年第 4 四半期の管理者の機能強化
description: 2024年第 4 四半期の管理者の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4f4694dd-a6cb-46b7-b2cf-fe24ed9419f5
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 18%

---

# 2024年第 4 四半期の管理者の機能強化

このページでは、プレビュー環境に対すして 2024年第 4 四半期に行われた管理者向けのすべての機能強化について説明します。これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2024年第 4 四半期のリリースサイクルの現時点で利用可能なすべての変更点のリストについては、[2024年第 4 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md)を参照してください。

## 環境の昇格でアクセスレベルを使用できるようになりました

>[!NOTE]
>
>プレビューリリース：2024 年 10 月 17 日（PT）、すべてのお客様向けの実稼動リリース：24.10 リリースで（2024 年 10 月 17 日（PT））

環境プロモーション機能の機能を拡張するために、アクセスレベルを含める機能を追加しました。 これで、サンドボックス環境でアクセスレベルを設定し、そのアクセスレベルを実稼動環境に昇格させることができます。

以前は、環境のプロモーションにアクセスレベルを使用できませんでした。

環境のプロモーションに使用できるオブジェクトの詳細については、「環境のプロモーションの概要」の [ 環境のプロモーションでサポートされているオブジェクト ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) を参照してください。

## カスタムフォームのカウンターにフィールド数が表示されます

>[!NOTE]
>
>プレビューリリース：2024 年 10 月 1 日（PT）、すべてのお客様向けの実稼動リリース：24.10 リリース付き（2024 年 10 月 17 日（PT））

カスタムフォームのフィールドは 500 個に制限されています。 長いフォームの場合、フォーム上のフィールド数と、上限に近づいているかどうかを把握するのは難しい場合があります。

左下のカスタムフォームにカウンターが追加されました。 カウンターは、フォームで使用されているフィールドの数を表示し、フォームデザイナー内でスクロールすると、常に表示されます。

詳しくは、[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

## レイアウトテンプレートで「すべてを選択」オプションが使用できるようになりました

>[!NOTE]
>
>プレビューリリース：2024年8月29日（PT）、すべての顧客向けの実稼動版リリース：2024年8月29日（PT）

レイアウトテンプレートでフィールドをより簡単に表示または非表示にするために、レイアウトテンプレートの詳細ビューの概要エリアと財務エリアに **すべてを選択** チェックボックスが追加されました。 このオプションは、「**ユーザーに表示されるものをカスタマイズ** の下でプロジェクト、タスク、イシュー、Portfolio、またはプログラムを選択した場合に使用できます。 すべてのオブジェクトに「財務」エリアが表示されるわけではなく、各エリアのフィールドはオブジェクトによって異なります。

詳しくは、[ レイアウトテンプレートを使用して詳細ビューをカスタマイズする ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md) を参照してください。

## 環境プロモーションパッケージのロールバック

>[!NOTE]
>
>プレビューリリース：2024年8月29日（PT）。迅速リリース用の実稼動版：24.9 リリース（2024年9月12日（PT））。四半期リリース用の実稼動版：24.10 リリース（2024年10月17日（PT））

環境のプロモーションをより柔軟かつ使いやすくするために、ロールバック機能を有効にしました。 現在は、24 時間以内にパッケージをロールバックでき、環境昇格パッケージの影響を受けた以前の設定をより簡単に復元できます。

以前は、設定は手動で、または別の環境プロモーションパッケージを通じて復元されていました。

環境プロモーションパッケージのロールバックについて詳しくは、[ 環境プロモーションパッケージのロールバック ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-rollback.md) を参照してください。

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3434025/){target=_blank}

## カスタムフォームデザイナーのレイアウトボタンでは、2 列または 3 列を使用できます

>[!NOTE]
>
>~~プレビューリリース：2024 年 8 月 12 日（PT）~~、高速リリースの実稼動：なし、四半期リリースの実稼動：なし
>
>_この機能はプレビューから削除されており、今後のリリースではリリースされません。_

カスタムフォームデザイナーの「レイアウト」ボタンを使用すると、2 列または 3 列の作業領域から選択できます。 元のフォームデザイナーでは 3 つの列を使用し、フィールド設定は右端の列に表示されます。 2 つの列を選択すると、左端の列のフィールド ライブラリの横にフィールド設定が表示されます。

詳しくは、[ カスタムフォームの概要 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md) を参照してください。
