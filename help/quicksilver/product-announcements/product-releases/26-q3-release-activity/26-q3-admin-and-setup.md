---
title: 2026年第3四半期：管理者の機能強化
description: 2026年第3四半期：管理者の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 9%

---

# 2026年第3四半期：管理者の機能強化

このページでは、2026年第3四半期リリースのプレビュー環境に対する管理者の機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2026年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2026年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)を参照してください。

## 統一されたレビューと承認のための変更管理

>[!NOTE]
>
>プレビュー：2026年7月7日（PT）プロダクション高速リリース：2026年7月15日（PT）すべての人のための制作：2026年7月16日

Adobe Workfrontの「変更履歴」ページには、統一されたレビューと承認のワークフローをまたいでアクティビティが記録され、管理者はレビューとドキュメントのライフサイクルイベントに関する包括的なガバナンス履歴を確認できます。

承認、ステージ、参加者のアクションが追跡されるようになりました。 こうした行動には下記が含まれる。

* Frame.io ビューアでの承認決定
* 承認の作成または削除
* ドキュメントの更新（名前の変更、移動、削除など）

各エントリには、日付と時刻、操作、ユーザー名（または「システム生成」）、オブジェクト名など、トラッキングされた標準フィールドが含まれます。 Frame.io ビューアコメントは含まれません。

この変更追跡フェーズには、MCP イベントは含まれません。 これらは将来のリリースの一部になります。

詳しくは、[変更履歴の表示と管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)を参照してください。

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

## Workfront オブジェクトの変更履歴を表示する

>[!NOTE]
>
>プレビュー：2026年6月11日（PT）プロダクション高速リリース：2026年6月11日（PT）すべての人のための制作：2026年7月16日

一元的なリストで発生した変更を簡単に確認できるように、変更履歴リストを作成しました。 このリストには、オブジェクト、操作、変更のソース（ユーザーやWorkfront システムなど）などの情報が表示されます。

以前は、監査ログは利用できましたが、オブジェクトはカバーしていませんでした。

詳細については、[変更履歴の表示と管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md)を参照してください。

## 従来のストレージポートフォリオをAdobe クラウドストレージに変換する新しいシステム環境設定

>[!NOTE]
>
>プレビュー：2026年6月11日（PT）すべての人のための制作：2026年6月11日

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
