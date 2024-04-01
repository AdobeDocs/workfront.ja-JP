---
title: 2024 年第 2 四半期管理者の機能強化
description: 2024 年第 2 四半期管理者の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 2faa01024a1a174bacb42e9c6e24f528252f49f4
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 4%

---

# 2024 年第 2 四半期管理者の機能強化

このページでは、2024 年第 2 四半期のリリースでプレビュー環境に対しておこなわれた管理者向けの機能強化について説明します。 これらの機能強化は、前述のとおり、実稼動環境で利用できるようになります。

2024 年第 2 四半期のリリースサイクルで現時点で使用可能なすべての変更点のリストについては、 [2024 年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## フォームデザイナーのプレビューモードで、表示ロジックとスキップロジックを使用できるようになりました

>[!NOTE]
>
>プレビューリリース：2024 年 3 月 28 日、すべてのお客様向け実稼動：24.4（2024 年 4 月）

ベータ版のカスタムフォームデザイナーでは、プレビューモードで表示ロジックをテストし、ロジックをスキップできるようになりました。 以前は、ロジックが適用されている場合でも、すべてのフィールドがプレビューに表示されていました。

フォームデザイナーでのカスタムフォームのプレビューについて詳しくは、 [フォームデザイナーを使用したフォームの整理とプレビュー](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## 会社とユーザーが高度なカスタムフォームフィールドをサポートするようになりました

>[!NOTE]
>
>プレビューリリース：2024 年 3 月 14 日、すべてのお客様向けの実稼動環境：24.4（2024 年 4 月）

会社やユーザーにカスタムフォームを添付する際に、外部参照フィールドやWorkfrontネイティブフィールドなどの高度なカスタムフォーム機能を使用できるようになりました。 高度な機能は、会社を編集ダイアログやユーザーを編集ダイアログではなく、会社の詳細ページとユーザーの詳細ページで使用できます。 これらのフィールドタイプを活用するには、新しいフォームデザイナーでカスタムフォームを作成する必要があります。

カスタムフォームフィールドについて詳しくは、 [フォームデザイナーを使用したフォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## 新しいパッケージタイプで JumpSeat 統合が利用できるようになりました。

>[!NOTE]
>
>プレビューリリース：2024 年 2 月 26 日、高速リリース用の実稼動：24.3 リリース（2024 年 3 月 14 日）、すべてのお客様用の実稼動：24.4（2024 年 4 月）

既存の JumpSeat 統合が、新しいパッケージタイプ (Select、Prime、Ultimate) の 1 つを使用してアカウントで使用できるようになりました。 統合を有効にするには、アクティブな JumpSeat サブスクリプションが必要です。

JumpSeat 統合について詳しくは、 [JumpSeat 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Workfrontのネイティブフィールドは、フォームデザイナーベータ版で使用できます。

>[!NOTE]
>
>プレビューリリース：2024 年 2 月 29 日、高速リリース用の実稼動：24.3 リリース（2024 年 3 月 14 日）、すべてのお客様用の実稼動：24.4（2024 年 4 月）

Workfrontネイティブのフィールドをカスタムフォームに追加できるようになりました。 この新しいフィールドタイプを使用すると、カスタムフィールドで既存のデータを再作成する必要なく、データを論理的に整理してユーザーに表示できます。

カスタムフォームのフィールドリストで「ネイティブフィールド」を選択してフィールドをフォームデザイナーに追加した後、フォームのオブジェクトに対して任意のネイティブフィールドを選択できます。 例えば、フォームデザイナーの上部にある「オブジェクトの種類」リストに「プロジェクト」と表示されている場合、プロジェクトのネイティブフィールドを選択できますが、タスクに固有のフィールドは選択できません。

カスタムフォームがオブジェクトに添付されると、そのフィールドにはオブジェクトデータが入力されます。 例えば、プロジェクトに添付されたカスタムフォームの「説明」フィールドが、プロジェクトの説明を取り込みます。 （利用可能なデータがない場合、フィールドに「N/A」と表示される場合があります）。

カスタムフォームで使用されるネイティブフィールドは、Designer のフィールドライブラリで再利用できます。また、設定/カスタムForms/フィールド領域にも表示され、どのフォームで使用されているかを確認できます。

この機能は、フォームデザイナーベータ版でのみ使用でき、レガシーフォームビルダーでは使用できません。

詳しくは、 [フォームデザイナーを使用したフォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[この機能のデモビデオを見る。](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Adobe IMSに移行した組織で、属性マッピングが使用できるようになりました。

>[!NOTE]
>
>プレビューリリース：2024 年 2 月 22 日、全顧客の実稼動環境：2024 年 2 月 22 日

Workfrontシステム管理者は、Adobe IMSに移行した組織のユーザー属性マッピングを設定できるようになりました。 これにより、ユーザー情報が組織の SSO（シングルサインオン）プロバイダーからWorkfrontに渡されるので、ユーザーのデータをWorkfrontと SSO プロバイダーの両方に入力する必要がなくなります。

以前は、この機能はまだAdobe IMSにオンボーディングされていない組織でのみ使用できました。

属性マッピングの設定手順については、 [Unified Experience でのAdobe属性のマッピング](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) 記事内 **ユーザー属性のマッピングと新しいユーザーの自動プロビジョニング**.

## スキップロジックと表示ロジックが、フォームデザイナーベータ版で使用できるようになりました。

>[!NOTE]
>
>プレビューリリース：2024 年 2 月 8 日、高速リリース用の実稼動：24.2 リリース（2024 年 2 月 16 日）、すべてのお客様用の実稼動：TBD

これで、既存の表示を編集し、ロジックをスキップし、フォームデザイナーベータ版でカスタムフォームに新しいロジックを追加できるようになりました。 使いやすいロジックビルダーを使用すると、フォーム内の選択に基づいて、表示またはスキップするフィールドを定義できます。

フォームデザイナーキャンバスのフィールド上のアイコンは、そのフィールド上でロジックが設定されていることまたは他のフィールド上で設定されているロジックルール内でフィールドが使用されていることを示します。

詳しくは、 [フォームデザイナーでの表示ロジックの追加とロジックのスキップ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
