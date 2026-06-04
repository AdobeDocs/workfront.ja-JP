---
title: 2024年第 2 四半期の管理者の機能強化
description: 2024年第 2 四半期の管理者の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
TQID: https://experienceleague.adobe.com/xcYDVGJSTKtR0dRM3EhQf62WokddEzsudevZ6Ur6Wn0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 827
ht-degree: 96%

---

# 2024年第 2 四半期の管理者の機能強化

このページでは、プレビュー環境の 2024年第 2 四半期リリースで行われた管理者の機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2024年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2024年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md)を参照してください。

## 表示ロジックとスキップロジックが、フォーム designer のプレビューモードで使用可能

>[!NOTE]
>
>プレビューリリース：2024年3月28日（PT）。すべてのお客様向けの実稼動版：24.4（2024年4月11日（PT））

ベータ版のカスタムフォーム designer では、プレビューモードで、表示ロジックをテストし、ロジックをスキップできるようになりました。 以前は、ロジックが適用されている場合でも、すべてのフィールドがプレビューに表示されていました。

フォーム designer でのカスタムフォームのプレビューについて詳しくは、[フォーム designer を使用したフォームの整理とプレビュー](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)を参照してください。

## 会社とユーザーによる高度なカスタムフォームフィールドのサポート

>[!NOTE]
>
>プレビューリリース：2024年3月14日（PT）。すべてのお客様向けの実稼動版：24.4（2024年4月11日（PT））

カスタムフォームを会社またはユーザーに添付すると、外部参照フィールドや Workfront ネイティブフィールドなどの高度なカスタムフォーム機能が使用できるようになりました。 高度な機能は、会社を編集ダイアログやユーザーを編集ダイアログではなく、会社の詳細ページとユーザーの詳細ページで使用できます。 これらのフィールドタイプを使用するには、新しいフォーム designer でカスタムフォームを作成する必要があります。

カスタムフォームフィールドについて詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## JumpSeat 統合が、新しいパッケージタイプで使用可能

>[!NOTE]
>
>プレビューリリース：2024年2月26日（PT）。迅速リリース用の実稼動版：24.3 リリース（2024年3月14日（PT））。すべてのお客様向けの実稼動版：24.4（2024年4月11日（PT））

既存の JumpSeat 統合は、新しいパッケージタイプ（Select、Prime、Ultimate など）のいずれかを使用するアカウントで使用できるようになりました。 統合を有効にするには、アクティブな JumpSeat サブスクリプションが引き続き必要です。

JumpSeat 統合について詳しくは、[JumpSeat 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md)を参照してください。

## Workfront ネイティブフィールドが、フォーム designer（Beta）で使用可能

>[!NOTE]
>
>プレビューリリース：2024年2月29日（PT）。迅速リリース用の実稼動版：24.3 リリース（2024年3月14日（PT））。すべてのお客様向けの実稼動版：24.4（2024年4月11日（PT））

Workfront にネイティブなフィールドをカスタムフォームに追加できるようになりました。 この新しいフィールドタイプを使用すると、カスタムフィールドで既存のデータを再作成することなく、論理的な方法でデータを整理してユーザーに表示できます。

カスタムフォームフィールドリストで「ネイティブフィールド」を選択してフィールドをフォーム designer に追加すると、フォームのオブジェクトに対して任意のネイティブフィールドを選択できます。 例えば、フォーム designer の上部にある「オブジェクトタイプ」リストに「プロジェクト」と表示されている場合は、プロジェクトのネイティブフィールドを選択できますが、タスクに固有のフィールドは選択できません。

カスタムフォームをオブジェクトに添付すると、フィールドはオブジェクトデータから入力されます。 例えば、プロジェクトに添付されたカスタムフォームの「説明」フィールドは、プロジェクトの説明を取り込みます （データが利用できない場合、フィールドには「該当なし」と表示される場合があります）。

カスタムフォームで使用するネイティブフィールドは、designer のフィールドライブラリで再利用できます。これらは、設定／カスタムフォーム／フィールドエリアにも表示されるので、使用しているフォームを確認できます。

この機能は、フォーム designer（Beta）でのみ使用でき、従来のフォームビルダーでは使用できません。

詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

[この機能のデモ動画をご覧ください。](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Adobe IMS に移行した組織で、属性マッピングが使用できるようになりました。

>[!NOTE]
>
>プレビューリリース：2024年2月22日、すべてのお客様向けの本番：2024年2月22日

Workfront システム管理者が、Adobe IMS に移行した組織のユーザー属性マッピングを設定できるようになりました。 これにより、ユーザー情報が組織の SSO（シングルサインオン）プロバイダーから Workfront に渡されるため、ユーザーのデータを Workfront と SSO プロバイダーの両方に入力する必要がなくなります。

以前は、この機能はまだ Adobe IMS にオンボーディングされていない組織でのみ使用できました。

属性マッピングの設定手順について詳しくは、**ユーザー属性の割り当てと新規ユーザーの自動プロビジョニングを実行**&#x200B;の記事の [Adobe Unified Experience でのユーザー属性を割り当て](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience)を参照してください。

## スキップロジックと表示ロジックが、フォーム designer（Beta）で使用できるようになりました。

>[!NOTE]
>
>プレビューリリース：2024年2月8日（PT）。迅速リリース用の実稼動版：24.2 リリース（2024年2月15日（PT））。すべてのお客様向けの実稼動版：24.4（2024年4月11日（PT））

フォーム designer（Beta）で、既存の表示とスキップロジックを編集し、カスタムフォームに新しいロジックを追加できるようになりました。 使いやすいロジックビルダーを使用すると、フォーム内の選択に基づいて、表示またはスキップするフィールドを定義できます。

フォーム designer キャンバスのフィールド上のアイコンは、そのフィールド上でロジックが設定されていることまたは他のフィールド上で設定されているロジックルール内でフィールドが使用されていることを示します。

詳しくは、[フォーム designer を使用した表示ロジックとスキップロジックの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)を参照してください。
