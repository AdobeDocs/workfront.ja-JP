---
title: 2026 年第 2 四半期レポートの機能強化
description: 2026 年第 2 四半期レポートの機能強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 8bcea5cec9f68deacc5f89ca7703303a1b00769f
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 23%

---

# 2026 年第 2 四半期レポートの機能強化

このページでは、2026 年第 2 四半期リリースでプレビュー環境に対して行われたレポートの機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2026年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)を参照してください。

## レポートの構築時に表示されるカスタムフィールドラベル

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

レポート作成ツールのフィールド名およびオブジェクトの前にカスタムフィールドラベルが表示されるようになり、フィールドを見つけやすくなりました。 フィールドラベルは、リストでフィルター、ビュー、グループ化を定義する際にも表示されます。

カスタムフィールドラベルはシステムインターフェイス用ですが、フィールド名は API やバックエンドのストレージ目的で頻繁に使用され、フィールドを見つける際にはそれほど役に立たない場合があります。

詳しくは、[カスタムレポートを作成](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

<!--

## Shareable Report Folders

>[!NOTE]
>
>Preview: February 26, 2026
>Production fast release: March 12, 2026
>Production for everyone: April 16, 2026

You can now organize and share reports using shareable report folders. This new feature helps teams that manage large volumes of reports maintain scalable and consistent access control:

* **Create organized folder structures**: System administrators can create top-level folders, and users with manage access can create subfolders up to 4 levels deep.
* **Granular permission controls**: Share folders with two permission levels:
   * View: Users can open reports and share folders
   * Manage: Users can edit folder details, add/remove items, and automatically receive manage access to all reports within the folder
* **Inherited permissions**: Permissions cascade from parent folders to all subfolders and reports within the folder tree
* **Enhanced list experience**: When you enable sharable folders, you will have access to the enhanced list experience. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


For more information, see [Use shareable report folders](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

-->

## キャンバスダッシュボードのグラフのグループ化の日付ラベルを改善しました

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

データを日付別にグループ化するグラフで、より明確で読みやすい日付ラベルが表示されるようになりました。 この更新により、日付ラベルは、選択した「グループ化の基準」オプション（日、週、月、年など）に基づいて動的に調整されるようになり、グラフを一目で読みやすく、解釈しやすくなりました。

<table> <tbody> <tr> <td>日</td> <td>完全な日付が表示されます。 例：3/12/2026</td> </tr> <tr> <td>週</td> <td>書式設定された週の開始日を表示します。 例、2026 年 3 月 8 日</td> </tr> <tr> <td>月</td> <td>月と年が表示されます。 2026 年 3 月の例</td> </tr> <tr> <td>年</td> <td>年のみを表示します。 例：2026</td> </tr> </tbody> </table>

以前は、グラフのグループ化には、選択した期間の開始日が常に数値形式で表示されていました。


