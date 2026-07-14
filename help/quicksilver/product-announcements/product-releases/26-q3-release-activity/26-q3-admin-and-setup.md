---
title: 2026年第3四半期：管理者の機能強化
description: 2026年第3四半期：管理者の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: f45c946e48b253018648c414915d53eca5a4de80
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 6%

---

# 2026年第3四半期：管理者の機能強化

このページでは、2026年第3四半期リリースのプレビュー環境に対する管理者の機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2026年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2026年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)を参照してください。

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## Typeahead フィールドタイプを置き換える内部参照フィールド

>[!NOTE]
>
>プレビュー：2026年7月7日（PT）プロダクション高速リリース：2026年7月15日（PT）すべての人のための制作：2026年7月16日

カスタムフォームの新しい&#x200B;**内部検索** フィールドタイプは、動的フィルタリングを提供します。 これはTypeahead フィールドタイプと似ており、名前の一部を入力して既存のWorkfront オブジェクトを検索および選択できます。 内部参照のフィルターは、フォームの別のフィールドの値を参照できますが、これはTypeaheadでは不可能です。

複数選択は内部参照でサポートされており、このフィールドタイプでは、大規模なデータセットのパフォーマンスも向上しています。 次のネイティブ Workfront オブジェクトは、内部参照でサポートされています。プロジェクト、会社、グループ、担当業務、Portfolio、プログラム、チーム、テンプレート、ユーザー、タスク、イシュー、ドキュメント、場所。

内部参照フィールドタイプは、先行入力フィールドタイプに置き換えられます。 右側のフィールドオプションのボタンをクリックすると、既存のTypeahead フィールドを内部参照にすばやく変換できます。 変換すると、履歴データはフィールドに残り、レポートで同じ方法で使用されます。

>[!IMPORTANT]
>
>Workfront FusionのシナリオやAPI ベースの自動化などの外部統合は、従来のフィールド構造を参照し、変換後に更新が必要になる場合があります。 先行入力フィールドを内部参照フィールドに変換する前に、統合を確認する必要があります。

詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## ネイティブ参照フィールドでサポートされるデフォルト値ロジック

>[!NOTE]
>
>プレビュー：2026年7月7日（PT）プロダクション高速リリース：2026年7月15日（PT）すべての人のための制作：2026年7月16日
>
>この機能は、Workflow PrimeまたはUltimate パッケージの組織でのみ使用できます。

カスタムフォームで、ネイティブ参照フィールドでデフォルト値ロジックを追加できるようになりました。

このネイティブ参照フィールドのロジックタイプは、Workfront APIではなく、ユーザーインターフェイスでのみ使用できます。

詳しくは、[ カスタムフォームとフィールドにロジックルールを追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)の記事の[ カスタムフォームにデフォルト値ロジックを追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form)を参照してください。

## カスタムフォームのネイティブフィールドフィルタリングの更新

>[!NOTE]
>
>プレビュー：2026年7月7日（PT）プロダクション高速リリース：2026年7月15日（PT）すべての人のための制作：2026年7月16日

ネイティブフィールドに存在するシステムフィルターが、カスタムフォームのフィールドに適用され、管理者に表示されるようになりました。

システムフィルターが適用されたネイティブ参照フィールドを追加すると、カスタムフォームのフィールドに同じフィルターを適用し、必要に応じてテキストモードボックスでフィルターを変更できます。

フィールドに独自のカスタムフィルターを追加すると、フィールドのシステムフィルターが上書きされます。 カスタムフィルターを入力しない場合、システムフィルターはデフォルトで適用されます。

また、ネイティブ参照フィールドで動的フィルタリングを使用できるようになりました。 ダイナミックフィルターを使用すると、別のフィールドの値に基づいて項目のリストを絞り込むことができます。

例えば、「プロジェクト」フィールドフィルターで`?portfolioID={portfolio}.{ID}`を使用し、Portfolio ネイティブフィールドがカスタムフォーム上にある場合、「プロジェクト」フィールドには、選択したポートフォリオ内のプロジェクトのみが表示されます。 「Portfolio」フィールドが空白のままになっている場合は、「プロジェクト」フィールドにすべてのプロジェクトが表示されます。

詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## 誤った名前の変更からフィールド名を保護する

>[!NOTE]
>
>プレビュー：2026年7月7日（PT）プロダクション高速リリース：2026年7月15日（PT）すべての人のための制作：2026年7月16日

統合とデータの整合性を保護するために、カスタムフォームのフィールド設定パネルでフィールド名を編集する方法を更新しました。

フィールド設定パネルのフィールド名は、デフォルトで読み取り専用になりました。 フィールド名は引き続き編集できますが、名前の変更には明示的な確認手順が必要です。 以前に&#x200B;**Name**&#x200B;という名前のフィールドも、技術的な重要性をより反映させるために&#x200B;**API Name**&#x200B;に更新されました。 **Label** フィールドは編集可能なままです。

詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels)を参照してください。

## Workfront オブジェクトの変更履歴を表示する

>[!NOTE]
>
>プレビュー：2026年6月11日（PT）プロダクション高速リリース：2026年6月11日（PT）すべての人のための制作：2026年7月16日

一元的なリストで発生した変更を簡単に確認できるように、変更履歴リストを作成しました。 このリストには、オブジェクト、操作、変更のソース（ユーザーやWorkfront システムなど）などの情報が表示されます。

以前は、監査ログは利用できましたが、オブジェクトはカバーしていませんでした。

詳しくは、[変更履歴の表示と管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)を参照してください。

## 従来のストレージポートフォリオをAdobe クラウドストレージに変換する新しいシステム環境設定

>[!NOTE]
>
>プレビュー：2026年6月11日（PT）すべての人のための制作：2026年6月11日スケジュール外]{type=Neutral}

Workfront管理者は、システム環境設定から直接、従来のストレージポートフォリオをAdobe クラウドストレージに変換できるようになりました。 ポートフォリオを変換するには、新しい「エンタープライズストレージに変換するポートフォリオを選択」フィールドでポートフォリオを選択し、ページを保存します。

ポートフォリオがAdobe クラウドストレージに変換される場合：

* 従来の Workfront ストレージを使用するプロジェクトをこのポートフォリオに移動できなくなりました
* このポートフォリオで作成される新しいプロジェクトはすべて、アドビクラウドストレージを使用します
* Frame.ioは、Adobe クラウドストレージを使用するドキュメントのビューアです
* 従来のWorkfront ストレージを使用している子オブジェクトは、従来のストレージに残ります

以前は、Adobe クラウドストレージプロジェクトをレガシーストレージポートフォリオに追加すると、ポートフォリオが自動的にAdobe クラウドストレージに変換されていました。

詳しくは、[ システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

## リッチテキストによるテキストの書式設定フィールドタイプへの置き換え

>[!NOTE]
>
>プレビュー：2026年5月28日（PT）プロダクション高速リリース：2026年6月11日（PT）すべての人のための制作：2026年7月16日

カスタムフォームの新しい&#x200B;**リッチテキスト** フィールドタイプは、堅牢なテキストエディターで、太字、斜体、下付き文字、下線、箇条書き、ハイパーリンク、ブロック引用符などの従来のオプションに加えて、上付き文字や下付き文字、見出し、表などの書式設定オプションを使用できます。 文字数制限は15,000のままです。

リッチテキストフィールドタイプは、テキストを書式設定フィールドタイプに置き換えます。 右側のフィールドオプションのボタンをクリックすると、書式設定フィールドを含む既存のテキストをリッチテキストにすばやく変換できます。 変換すると、履歴データはフィールドに残り、レポートで同じ方法で使用されます。

>[!IMPORTANT]
>
>Workfront FusionのシナリオやAPI ベースの自動化などの外部統合は、従来のフィールド構造を参照し、変換後に更新が必要になる場合があります。 フィールドをリッチテキストに変換する前に、統合を検証する必要があります。

詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

## カスタムフォームでサポートされているネイティブの財務フィールド

>[!NOTE]
>
>プレビュー：2026年5月28日（PT）プロダクション高速リリース：2026年6月11日（PT）すべての人のための制作：2026年7月16日

カスタムフォームにWorkfront ネイティブの金融フィールドを含めることができるようになりました。 以前は、財務フィールドはサポートされていませんでした。

参照できる財務フィールドは、フォームのタイプによって異なります。

詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields)を参照してください。

## カスタムフォームは、システム全体で共有し、添付ファイルへのアクセス権を持つことが可能

>[!NOTE]
>
>プレビュー：2026年5月28日（PT）プロダクション高速リリース：2026年6月11日（PT）すべての人のための制作：2026年7月16日

新しい共有オプション「システム内のすべてのユーザーが表示および添付できる」がカスタムフォームに追加されました。 このオプションを選択すると、システム全体のすべてのユーザーがフォームを他のオブジェクトに添付できます。

システム全体で共有する必要がなくなり、新しいグループが追加されたときに、グループや機関をまたいでフォームを手動で共有し、権限を更新する必要がなくなります。

詳しくは、[カスタムフォームを共有](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)を参照してください。

## 一括編集時に必須フィールドを適用する新しいシステム環境設定

>[!NOTE]
>
>プレビュー：2026年5月28日（PT）プロダクション高速リリース：2026年6月11日（PT）すべての人のための制作：2026年7月16日

現在、オブジェクトを一括編集する場合、必須フィールドはユーザーがフィールドを変更した場合にのみ適用されます。 フィールドが変更されない場合、そのフィールドはオプションとして扱われ、検証されません。

新しいシステム環境設定で、一括編集で必須フィールドを適用できるようになりました。 すべての必須フィールドに値が含まれていない限り、一括編集されたオブジェクトを保存しないようにするには、設定/システム/環境設定ページで「**常に一括編集で必須フィールドを適用**」オプションを選択します。

詳しくは、[ システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。
