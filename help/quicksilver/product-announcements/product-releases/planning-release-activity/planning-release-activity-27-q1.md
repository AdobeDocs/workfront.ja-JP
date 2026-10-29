---
content-type: release-notes
title: Adobe Workfront Planningの2027年第1四半期のリリースアクティビティ
description: これは、2027年第1四半期のAdobe Workfront計画製品のリリースアクティビティです。
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 65b1e818b321dd396720fb791e49e8ae9eb7af92
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 3%
---
# Adobe Workfront Planningの2027年第1四半期のリリースアクティビティ

この記事では、2027年第1四半期リリース中にWorkfront Planningでリリースされる機能について説明します。

Adobe Workfront計画でリリースされたすべての機能の一覧については、[Adobe Workfront計画リリースアクティビティ：記事インデックス ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)を参照してください。

## テーブルビューでのクイック検索の結果の可視性を向上

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

テーブルビューでクイック検索を使用して項目を検索すると、検索に一致しないレコードがすべてビューに表示されなくなり、一致する項目のみが表示されます。

この機能強化の前は、検索結果に一致するレコードがハイライト表示されているすべてのレコードが表示されていました。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

<!--

## Record-level permissions - restricted access to records

PLACEHOLDER: The release note field on the Workfront task points to an anchor story that no longer exists, so there is no description yet. Add the description and help link before unhiding.

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

-->

## クロスワークスペースの接続がオフの場合、セカンダリワークスペースで接続されたグローバルレコードタイプのレコードの接続を許可する

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

2つの接続されたグローバルレコードタイプがセカンダリワークスペースに追加された場合、クロスワークスペース接続をオフにしながら、レコードをローカルにリンクできます。

各セカンダリレコードタイプは、両方のレコードタイプに対して独自のレコードのみを表示し、それらを互いに接続できます。 グローバルワークスペースおよびその他のセカンダリワークスペースのレコードは表示されなくなりました。

この機能強化の前は、接続されたグローバルレコードタイプでワークスペース間の接続がオフになっていると、セカンダリワークスペースで自分のレコードを互いにリンクさせることができませんでした。 このオプションがオンになっている場合、ユーザーはグローバル ワークスペースおよびその他のすべてのセカンダリ ワークスペースからレコードを表示およびリンクできます。

詳しくは、[ クロスワークスペースのレコードタイプの概要](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)を参照してください。

## テーブル、タイムラインおよびリストビューでの合計レコード数の表示

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

テーブル、タイムライン、リストビューにレコードの合計数が表示され、フィルターの適用、検索、またはビューの変更に伴ってカウントが自動的に更新されるようになりました。 レコード数は、常にフルフィルターされた結果を反映し、権限を尊重します。

レコード数は、クイック検索ボックスの左側、テーブル、タイムライン、またはリストビューの右上隅に表示されます。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

<!--

## Field aggregators available for groupings in the table view

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Grouped records in the table views now show a summary row for each grouping, plus a grand total for the full table. Groupings and the grand total use the same summary functions, and nested groupings get their own summaries that include all child records. Aggregators update automatically as you filter, search, regroup, or edit records.

For information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md).

## Add sections to organize Planning views

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now create sections in the Workfront Planning View dropdown menu to organize related views as your list grows. You can name each section when you create it, then move views from My Views and Shared with Me into your custom sections. System views stay fixed in the System section.

For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md).

-->

<!--

## Filters for Workfront objects connected record fields

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

You can now filter for certain Workfront object types that meet a filter criteria when you add them as a connected field in Planning.

Only those Workfront objects that meet your filtering criteria will display as options in connected fields when editing a record.

For this feature, we added a new Record filtering rules option in the New connection tab when connecting the following Workfront object types: projects, portfolios, programs, groups, companies. Prior to this enhancement, filters were available only when connecting two record types.

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

-->

## ルックアップフィールド番号の制限

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

レコードタイプに追加できるルックアップフィールドの数に制限があります。

* レコードタイプごとに最大40個のルックアップフィールド
* レコードタイプごとに最大5つの長テキスト検索フィールド。 接続されたルックアップフィールドは、元のフィールドの制限に対してカウントされます。
* 1つの長いテキストルックアップセルの値に最大50,000文字を含めます。 ルックアップ値の結合コンテンツがこれを超えた場合、値は制限に達するまで接続順に表示されます。 それを超える最初の値と、その後のすべての値は省略されます。 元の接続されたオブジェクトフィールドは変更されません。

最初の2つの制限を超えてルックアップフィールドを作成または編集しようとすると、エラーが表示されます。 既にこれらの制限を超えているレコードタイプは、この変更の影響を受けません。 これらのフィールドは編集できますが、制限に達するまでルックアップフィールドや値を追加することはできません。

詳しくは、[Adobe Workfront計画オブジェクト制限の概要](/help/quicksilver/planning/general/limitations-overview.md)を参照してください。

## 新しいフィールドは、作成したビューにのみ表示されるようになりました

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

新しいフィールドをレコードタイプに追加すると、作業中のビューにのみ表示され、他のすべての既存のビューでは非表示になります。 他のビューは設定通りに表示され、必要に応じて新しいフィールドを再表示できます。

この機能強化の前は、すべてのビューに新しいフィールドが非表示に追加されていましたが、新しいフィールドに慣れていないユーザーが混乱を起こすことがありました。

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

## 任意のビューからレコードの詳細をエクスポートします

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

すべてのフィールドビューに切り替えることなく、任意の詳細ビューからレコードの詳細を書き出せるようになりました。

以前は、「すべてのフィールド」ビューが選択されている場合にのみ、「書き出し」オプションを使用していました。

詳しくは、[ レコードの詳細の書き出し](/help/quicksilver/planning/records/export-the-record-page.md)を参照してください。

<!--

## Cancel and revert changes when editing records when business rules are violated

>[!NOTE]
>
>Preview: October 29, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

To ensure data integrity, when a business rule is violated while you edit a record, the change is blocked, the value reverts, and a toast notification explains why the edit is not allowed. The warning is visible in all areas where you are editing records, including the table view or details page.

If multiple rules are violated, each violation issues its own toast notification.

For more information, see [Configure business rules](/help/quicksilver/planning/architecture/configure-business-rules.md).

-->

## テーブルビューとタイムラインビューでの増分データの読み込みによるパフォーマンスの向上

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

多数のレコードのパフォーマンスを向上させるために、テーブルとタイムラインビューに次の改善を加えました。

* テーブルビューでは、最初に最初の500件のレコードが読み込まれ、500件のバッチでスクロールすると、追加のレコードが自動的に読み込まれるようになりました。
* タイムラインビューは同様の動作を持ちますが、スクロールしながら次の1000が読み込まれると、一度に1000件のレコードが読み込まれます。
* クイック検索は、現在のビューに表示されるレコードだけでなく、すべてのレコードに適用されます。 タイムラインビューとテーブルビューの両方でスクロールすると、より多くのレコードが読み込まれます。
* タイムラインビューにクイック検索を適用すると、1000以上の項目が見つかり、タイムラインの下部にある「さらに読み込む」をクリックすると、検索に一致するレコードをさらに表示できます。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)および[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。

<!--

## Additional permissions for users other than requestors to submitted requests

>[!NOTE]
>
>Preview: October 28, 2026
>Production fast release: November 12, 2026
>Production for everyone: January 21, 2027

Workspace managers can now define what access to submitted requests users other than requestors have.

By editing the Permissions area of a request form, you can define additional access for other users to requests submitted using the form.

You can grant permissions to workspace users or any other users, groups, teams, job roles or companies in the system. Once defined in the request queue, the permissions are granted automatically when the request is submitted, and any permission changes apply only to new requests.

Prior to this enhancement, you could only grant permissions to requestors.

For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

-->

## タイムラインビューでの手動によるグループ化の並べ替え

>[!NOTE]
>
>プレビュー：2026年10月29日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

グループ、サブグループ、レコードをドラッグ&amp;ドロップして、タイムラインビューでカスタム順序を作成できるようになりました。 手動での並べ替えはセッション間で保持され、計画のニーズの変化に応じて、手動による並べ替えとフィールドベースの並べ替えをシームレスに切り替えることができます。

ドラッグ&amp;ドロップ機能は、タイムラインビューのスイムレーンと積み重ねバージョンの両方で使用できます。

詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。

## グローバルレコードタイプのビジネスルール

>[!NOTE]
>
>プレビュー：2026年10月28日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

Workspace マネージャーは、プライマリワークスペースとセカンダリワークスペースの両方で、グローバルレコードタイプにビジネスルールを設定できるようになりました。 ルールは、追加されたすべてのワークスペース内の同じタイプのすべてのレコードに適用されます。

グローバルワークスペースに追加されたビジネスルールは、レコードタイプが読み込まれたセカンダリワークスペースに読み取り専用として表示されます。 セカンダリワークスペースに追加されたビジネスルールは、レコードタイプが最初に作成されたプライマリワークスペースに読み取り専用として表示されます。 ルールは、作成されたワークスペースでのみ編集できます。

詳しくは、[ レコードタイプのビジネスルールの設定](/help/quicksilver/planning/architecture/configure-business-rules.md)を参照してください。

## Planning リクエストの入力フォーム機能のデフォルトのプロンプト設定を設定します

>[!NOTE]
>
>プレビュー：2026年10月21日（PT）
>プロダクション高速リリース：2026年11月12日（PT）
>すべての人のための制作：2027年1月21日

Planning リクエストの送信時にAIを活用した入力フォーム機能を使用する場合にユーザーに表示されるプロンプトをカスタマイズできるようになりました。

Planning リクエストのリクエストフォームを作成する際に、デフォルトのプロンプトを作成できます。

詳しくは、[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)でのリクエストフォームの作成と管理を参照してください。
