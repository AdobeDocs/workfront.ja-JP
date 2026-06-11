---
title: 2026年第3四半期：管理者の機能強化
description: 2026年第3四半期：管理者の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: cc0067cb2f64eae79647881ab30355b6832073d1
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 3%

---

# 2026年第3四半期：管理者の機能強化

このページでは、2026年第3四半期リリースのプレビュー環境に対する管理者の機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2026年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2026年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)を参照してください。

## Workfront オブジェクトの変更履歴を表示する

>[!NOTE]
>
>プレビュー：2026年6月11日>実稼動用の高速リリース：2026年6月11日>全員の実稼動環境：2026年7月16日

一元的なリストで発生した変更を簡単に確認できるように、変更履歴リストを作成しました。 このリストには、オブジェクト、操作、変更のソース（ユーザーやWorkfront システムなど）などの情報が表示されます。

以前は、監査ログは利用できましたが、オブジェクトはカバーしていませんでした。

<!--

For more information see [View and manage change history](help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

<!--

## New system preference to convert legacy storage portfolios to Adobe cloud storage

>[!NOTE]
>
>Preview: June 11, 2026
>Production for everyone: June 11, 2026

Workfront administrators can now convert legacy storage portfolios to Adobe cloud storage directly from System Preferences. To convert portfolios, select them in the new Select portfolios to convert to enterprise storage field and save the page.

When a portfolio is converted to Adobe cloud storage:

* You can no longer move projects that use legacy Workfront storage to this portfolio
* All new projects created in this portfolio use Adobe cloud storage
* Frame.io is the viewer for documents using Adobe cloud storage
* Child objects using legacy Workfront storage stay on legacy storage

Previously, adding an Adobe cloud storage project to a Legacy storage portfolio automatically converted the portfolio to Adobe cloud storage.

For more information, see [Configure system preferences](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

-->

## リッチテキストは、テキストを書式設定フィールドタイプに置き換えます

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

カスタムフォームの新しい&#x200B;**リッチテキスト** フィールドタイプは、堅牢なテキストエディターで、太字、斜体、下付き文字、下線、箇条書き、ハイパーリンク、ブロック引用符などの従来のオプションに加えて、上付き文字や下付き文字、見出し、表などの書式設定オプションを使用できます。 文字数制限は15,000のままです。

リッチテキストフィールドタイプは、テキストを書式設定フィールドタイプに置き換えます。 右側のフィールドオプションのボタンをクリックすると、書式設定フィールドを含む既存のテキストをリッチテキストにすばやく変換できます。 変換すると、履歴データはフィールドに残り、レポートで同じ方法で使用されます。

>[!IMPORTANT]
>
>Workfront FusionのシナリオやAPI ベースの自動化などの外部統合は、従来のフィールド構造を参照し、変換後に更新が必要になる場合があります。 フィールドをリッチテキストに変換する前に、統合を検証する必要があります。

詳しくは、[&#x200B; カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## カスタムフォームでサポートされているネイティブ財務フィールド

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

カスタムフォームにWorkfront ネイティブの金融フィールドを含めることができるようになりました。 以前は、財務フィールドはサポートされていませんでした。

参照できる財務フィールドは、フォームのタイプによって異なります。

詳しくは、[&#x200B; カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)を参照してください。

## カスタムフォームは、システム全体で共有し、添付するためのアクセス権を持つことができます

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

新しい共有オプション「システム内のすべてのユーザーが表示および添付できる」がカスタムフォームに追加されました。 このオプションを選択すると、システム全体のすべてのユーザーがフォームを他のオブジェクトに添付できます。

システム全体で共有する必要がなくなり、新しいグループが追加されたときに、グループや機関をまたいでフォームを手動で共有し、権限を更新する必要がなくなります。

詳しくは、[カスタムフォームを共有](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)を参照してください。

## 一括編集で必須フィールドを適用するための新しいシステム環境設定

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

現在、オブジェクトを一括編集する場合、必須フィールドはユーザーがフィールドを変更した場合にのみ適用されます。 フィールドが変更されない場合、そのフィールドはオプションとして扱われ、検証されません。

新しいシステム環境設定で、一括編集で必須フィールドを適用できるようになりました。 すべての必須フィールドに値が含まれていない限り、一括編集されたオブジェクトを保存しないようにするには、設定/システム/環境設定ページで「**常に一括編集で必須フィールドを適用**」オプションを選択します。

詳しくは、[&#x200B; システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。
