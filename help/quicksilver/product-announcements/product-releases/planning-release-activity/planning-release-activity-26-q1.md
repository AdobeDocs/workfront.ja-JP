---
content-type: release-notes
title: Adobe Workfront Planning の 2026 年第 1 四半期リリースアクティビティ
description: これは、2026 年第 1 四半期のAdobe Workfront Planning 製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: a58e7da96c43dd308a213c6d7ef74d5085a2e1ba
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 2%

---

# Adobe Workfront Planning の 2026 年第 1 四半期リリースアクティビティ

この記事では、2026 年第 1 四半期のリリースでWorkfront Planning に対してリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront Planning 用にリリースされたすべての機能の一覧については、[Adobe Workfront Planning リリース アクティビティ：記事一覧 &#x200B;](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md) を参照してください。

## プロジェクトの接続されたレコードページでビューを共有

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

必要な情報を確実に表示できるように、プロジェクトの接続されたレコード ページにビューを共有する機能を追加しました。 他のユーザー、チーム、グループとビューを共有できるようになりました。

共有を含むリクエストビューについて詳しくは、[&#x200B; リクエストエリアでのビューの作成と管理 &#x200B;](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md) を参照してください。

## 現在のユーザーワイルドカードをプロジェクト接続表示フィルターで使用できるようになりました

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

自分に適用されるプロジェクト接続をフィルターしやすくするために、現在のユーザーワイルドカードを作成しました。 これで、フィルタリング時に「自分（ログインしたユーザー）」を選択できます。 その後、フィルターはリクエストリストを表示しているユーザーに適用されます。

これは、複数のユーザーが使用するビューにフィルターを追加する場合に便利です。 各ユーザーに適用されるフィルター結果が表示されます。

ワイルドカードは、値がユーザーであるフィールドで使用できます。

フィルターを含むプロジェクト接続ビューの設定について詳しくは、[&#x200B; 接続されたレコードのページのレコードへの追加 &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) を参照してください。

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Workspaceのメインページの改善

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動の高速化：2026 年 1 月 14 日（PT）
>全員の実稼動：2026 年 1 月 15 日（PT）

Workfront Planning の「Workspaces」メインページが次のように改善されました：

* より高速で動的なスクロール機能。 これは、組織に多数のワークスペースがある場合や、システム管理者が使用する場合に特に目立ちます。

* 検索ボックスが追加され、特定のワークスペースを名前で検索できるようになりました。

* 「**その他のワークスペース**」タブの名前は、「**すべてのワークスペース** に変更されました。これには、作成したワークスペースを含む、少なくとも表示権限を持つすべてのワークスペースが含まれます。

詳しくは、[&#x200B; ワークスペースの編集 &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) を参照してください。

<!--

## Improvements to connected records pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

To give you more flexibility when working with connected records pages, we have enhanced the functionality of views in this area of Workfront Planning. The following are improvements in the connected records pages of a record that are coming with this release:

* You can now add a timeline and a calendar view to a record's connected records page.
* You can now share views from a connected records page. The views shared from these pages are visible system-wide by all users you share them with in any other area of Workfront Planning. All views shared in any other areas of Planning are also visible in the connected records page for the same users they are shared with.
* We have added a restriction to only allow one connected records page per each record or object type. Prior to this enhancement, you could add multiple pages for the same record or object type. Now, you can use multiple views for the same record type in one connected records page.
* We have added a **New row** link at the bottom of a table view and a **Connect records** button in the upper-right area of the connected records page. Prior to this enhancement, the **New row** link and the **Connect records** button existed only on a project connected page. 

For information, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

-->

## GenStudio Workspace でのデフォルトの「ブランド接続」フィールドの製品およびペルソナへの追加

>[!NOTE]
>
>プレビュー：2025 年 12 月 11 日（PT）
>実稼動高速リリース：2025 年 12 月 11 日（PT）
>すべてのユーザー向けの実稼動：2025 年 12 月 11 日（PT）

GenStudio for Performance Marketing Brand の接続フィールドが、Workfront Planning のGenStudio Workspace の Products および Personas レコードタイプにデフォルトで追加されるようになりました。

組織には、Workfront Planning とAdobe GenStudio for Performance Marketingの両方が必要です。

この機能強化の前は、ブランド接続フィールドを、製品やペルソナを含む任意のレコードタイプに手動でのみ追加できました。 Brand GenStudio レコードタイプをWorkfront Planning の他のレコードタイプに手動で接続することはできます。

詳しくは、[Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの統合の基本を学ぶ &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。

## GenStudio for Performance Marketing ユーザーの権限の Planning からの削除の制限

>[!NOTE]
>
>プレビュー：2025 年 12 月 11 日（PT）
>実稼動高速リリース：2025 年 12 月 11 日（PT）
>すべてのユーザー向けの実稼動：2025 年 12 月 11 日（PT）

Workfront Planning オブジェクトからGenStudio for Performance Marketing ユーザーの権限を削除しないようにするガードレールが追加されました。 この機能強化により、GenStudio ユーザーが含まれている場合、Planning のGenStudio Workspace からGenStudio ユーザーを削除することや、GenStudio Workspace のレコードタイプに対する継承された権限を無効にすることができなくなります。 この機能強化が行われるまで、Planning のGenStudioワークスペースからこれらのユーザーを削除すると、GenStudioでもレコードタイプを使用する権限が失われていました。

組織には、Workfront Planning とAdobe GenStudio for Performance Marketingの両方が必要です。

詳しくは、[Adobe Workfront Planning と Adobe GenStudio for Performance Marketingの統合の基本を学ぶ &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。


## セカンダリワークスペースのグローバルレコードタイプに対するビューの公開共有を削除しました


>[!NOTE]
>
>プレビュー：2025 年 12 月 3 日（Pt）
>実稼動高速リリース：2025 年 12 月 4 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）


セカンダリワークスペースでグローバルレコードのビューを共有する際の、「公開共有」タブを削除しました。 既存のグローバルレコードタイプから別のワークスペースに追加されたグローバルレコードタイプからビューを公開して共有することはできません。 グローバルレコードタイプのビューは、元のワークスペースから公開で共有できます。

詳しくは、[&#x200B; ビューの共有 &#x200B;](/help/quicksilver/planning/access/share-views.md) を参照してください。


## GenStudio for Performance Marketing Brands とWorkfront Planning レコードタイプの連携

>[!NOTE]
>
>プレビュー：2025 年 11 月 13 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2025 年 11 月 13 日（PT）

Workfrontの計画レコードタイプをAdobe GenStudio for Performance Marketingのブランドと関連付けられるようになりました。 組織には、Workfront Planning とAdobe GenStudio for Performance Marketingの両方が必要です。

詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。


## Planning ビューの「フィルタ」、「フィールド」、「行の色」アイコンの新規フィールド検索ボックス

>[!NOTE]
>
>プレビュー：2025 年 11 月 6 日（PT）
>実稼動高速リリース：2025 年 12 月 11 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

レコードタイプビューでビュー要素を作成する際に、特定のフィールドを検索できるようになりました。 フィルター、並べ替え、グループ化を作成する際や、フィールドや行のカラーを設定する際に、検索ボックスを追加しました。 この機能強化の前は、使用可能なフィールドのリストをスクロールするだけで済みます。

この機能強化は、すべてのレコードタイプのビューで利用できます。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。


## グローバルレコードタイプと、既存のレコードタイプとして他のワークスペースに追加する機能

>[!NOTE]
>
>プレビュー：2025 年 10 月 16 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

共通のワークフローを持つマルチチーム組織にWorkfront プランニングを実装する場合、各チームのワークスペースに追加できる主要なレコードタイプ（キャンペーンや成果物など）の包括的な構造とメタデータを定義して、チームの作業をキャプチャおよび管理する必要がある場合があります。

また、各チームの作業を中央レベルに展開する必要がある場合もあります。

このようなワークフローでは、組織内の全員をすべてのワークスペースに追加しなくても、チーム間の表示をロック解除しながら、チームが一貫して作業をキャプチャできるようにします。 グローバルレコードタイプを使用すると、これを実現できます。

レコードタイプをグローバルに指定し、複数のワークスペースで使用できるようになりました。 ユーザーは、中央のワークスペースで既に設定されているのと同じフィールド構造および接続を使用できます。

詳しくは、次の記事を参照してください。

* [&#x200B; クロスワークスペースレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [&#x200B; レコードタイプのワークスペース間機能の設定 &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [別のワークスペースからの既存のレコードタイプの追加](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## 1 つのレコードタイプの接続フィールドに対する新しい制限

>[!NOTE]
>
>プレビュー：2025 年 10 月 16 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

各レコードタイプに対して 30 個の接続フィールドという制限が導入されました。

注意：現在、組織に 1 つのレコードタイプに対して 30 を超える接続フィールドがある場合は、30 の制限を超える追加フィールドを保持できます。 ただし、制限を超えるレコードタイプに接続フィールドを追加することはできません。 今後、新しい制限の 30 個の接続フィールドが適用されます。

詳しくは、[&#x200B; 接続されたレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

## 選択タイプのフィールドの選択肢に対して、ユーザーにわかりやすい値を設定します

>[!NOTE]
>
>プレビュー：2025 年 10 月 16 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

フィールドの選択肢を 1 つまたは複数選択のフィールドに追加する際に、Workfrontで、各選択肢に一意のわかりやすい値を割り当てるようになりました。 この機能向上が行われる前は、Workfrontが生成した英数字の ID は、API 呼び出しやその他の統合環境では理解および使用が困難でした。

この改善により、次の点が考慮されます。

* 新しい値は、新しいフィールドの選択肢に追加されます。 既存のフィールドの選択肢では、英数字の ID が保持されます。

* 選択肢の値は、1 つのフィールドに対して一意ですが、異なるフィールド間で繰り返すことができます。

* 選択肢の名前を変更しても、元の値は更新されません。

* 複数の単語を選択した場合、選択値は小文字で表示され、アンダースコアで区切られます。 同じフィールドに別の選択名として既に使用されているラベルを使用する場合、Workfrontは値に連番を追加します。

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。






