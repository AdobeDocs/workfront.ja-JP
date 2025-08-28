---
content-type: release-notes
title: Adobe Workfront Planning の 2025 年第 4 四半期リリースアクティビティ
description: これは、2025 年第 4 四半期のAdobe Workfront Planning 製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 4e1761f9-bf73-4355-925a-9136f2787a3f
source-git-commit: f7dcae5e6bcc8674ef37ef94282c50dc9ffe951d
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 11%

---

# Adobe Workfront Planning の 2025 年第 4 四半期リリースアクティビティ

この記事では、2025 年第 4 四半期リリースでWorkfront Planning に対してリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront Planning 用にリリースされたすべての機能の一覧については、[Adobe Workfront Planning リリース アクティビティ：記事一覧 ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md) を参照してください。

## 式フィールドの新しい制限

>[!NOTE]
>
>* プレビュー：2025 年 8 月 28 日（PT）
>* 実稼動高速リリース：2025 年 9 月 11 日（PT）
>* 実稼動版（すべてのお客様向け）：2025年10月16日（PT）

式フィールドには次の制限があります。

* レコードタイプあたり 20 個の式フィールドという制限があります
* 数式には、50,000 文字までの制限があります

詳しくは、[ 式フィールドの概要 ](/help/quicksilver/planning/fields/formula-fields.md) を参照してください。

## 数式の値を解決できない場合にエラーを表示する

>[!NOTE]
>
>* プレビュー：2025 年 8 月 28 日（PT）
>* 実稼動高速リリース：2025 年 9 月 11 日（PT）
>* 実稼動版（すべてのお客様向け）：2025年10月16日（PT）

式フィールドの解決で問題が発生したことを示すために、フィールドには「#ERROR!」と表示されるようになりました。 次のいずれかの場合：

* 式で使用されているフィールドが削除されたとき。

* 集計参照フィールドで使用されているフィールドが#ERROR！と表示されている場合。

* 選択した形式で式の値を表示できない場合。

詳しくは、[数式フィールドの概要](/help/quicksilver/planning/fields/formula-fields.md)を参照してください。

## Planning の式フィールドに追加された新しい式

>[!NOTE]
>
>プレビュー：2025 年 8 月 7 日（PT）
>>すべてのお客様の実稼動環境 :August、2025 年
>>[!BADGE 予定外 ]{type=Neutral}

Workfront Planning の式フィールドとWorkfrontの計算カスタムフィールドに、次のように使用する新しい式を追加しました。

* **REMOVEACCENTS （string）**：入力文字列内のすべてのアクセント付き文字から発音区別符号を削除します。
* **REPLACEPATTERN （文字列、パターン、置換文字列）**：指定したパターンの一致を置換文字列で置き換えます。
* **PASCAL （string）**：各単語の最初の文字を大文字にし、すべてのスペースを削除して、入力文字列を PascalCase に変換します。

詳しくは、[計算データ数式の概要](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)を参照してください。

## 式フィールドの作成ウィンドウへの「最大化」および「最小化」ボタンの追加

>[!NOTE]
>
>プレビュー：2025 年 7 月 31 日（PT）
>>実稼動版（すべてのお客様向け）：2025年7月31日（PT）
>>[!BADGE 予定外 ]{type=Neutral}

レコードテーブルビューで式フィールドを作成または編集する際に、式フィールドを拡大するための「最大化」ボタンを追加しました。 さらに、拡大された新しいウィンドウに「最小化」ボタンを追加して、フィールド作成ボックスに戻しました。

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

## 接続されたレコード ページがレコードのプレビュー領域で使用できるようになりました

>[!NOTE]
>
>* プレビュー：2025 年 7 月 31 日（PT）
>* 実稼動迅速リリース：2025 年 8 月 14 日（PT）
>* 実稼動版（すべてのお客様向け）：2025年10月16日（PT）

プレビューボックスの接続されたレコードページのエクスペリエンスを、レコードの詳細領域の完全なページのページと一致させました。

この機能強化が行われるまで、接続されたレコード ページで接続されたレコードを表示することができたのは、レコードの詳細領域の全ページでした。

詳しくは、[ レコードページレイアウトの管理 ](/help/quicksilver/planning/records/manage-the-record-page.md) を参照してください。

<!--## Updates to Requesting experience 

>[!NOTE]
>
>* Preview: July 31, 2025
>* Production fast release: August 14, 2025
>* Production for all customers: October 16, 2025

To create a better user experience when making requests in Workfront and Workfront Planning, we've updated the requesting experience. Now you can:

* View Workfront and Workfront Planning requests in a single list.
* Filter submitted requests based on criteria you specify.
* Search for and select Workfront request queues and Workfront Planning forms in a consolidated experience.
* Hide and reorder columns in the submitted requests list.

This update also features changes to the look and feel of the page.

Previously, Workfront and Workfront Planning requests were on separate tabs, and filters were not customizable.

For more information on creating requests see:

* For Workfront: [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)
* For Workfront Planning: [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md) -->

## タイムラインビューでのレコードの作成

>[!NOTE]
>
>プレビュー：2025 年 7 月 24 日（PT）
>>実稼動迅速リリース：2025 年 8 月 14 日（PT）
>>実稼動版（すべてのお客様向け）：2025年10月16日（PT）

タイムライン上の任意の場所をダブルクリックすることで、レコードタイプのタイムライン表示でレコードを作成できるようになりました。

レコードの日付範囲を選択するか、レコードのページを開いてその詳細をすべて編集できます。

この機能強化が行われるまで、新しいレコードを追加するには、「新規レコード」ボタンを使用するか、テーブル表示でインライン化する必要があります。

詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

## レコードタイプのカードの詳細メニューに「共有」オプションを追加する

>[!NOTE]
>
>プレビュー：2025 年 7 月 24 日（PT）
>>実稼動迅速リリース：2025 年 8 月 14 日（PT）
>>実稼動版（すべてのお客様向け）：2025年10月16日（PT）

ワークスペースページのレコードタイプカードの「詳細」メニューからレコードタイプを共有できるようになりました。 この機能強化の前は、共有オプションはレコードタイプページ内でのみ使用できました。

詳しくは、[ レコードタイプの共有 ](/help/quicksilver/planning/access/share-record-types.md) を参照してください。

## すべてのWorkfront Planning ビューをフルスクリーン・モードで表示します

>[!NOTE]
>
>プレビュー：2025 年 7 月 24 日（PT）
>>実稼動迅速リリース：2025 年 8 月 14 日（PT）
>>実稼動版（すべてのお客様向け）：2025年10月16日（PT）

すべてのWorkfront Planning ビュー（テーブル、タイムライン、カレンダー）をフルスクリーンモードで表示できるようになりました。 ビュー機能は維持され、フルスクリーンでビューを変更することもできます。

この機能強化の前は、この機能は存在しませんでした。

詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

## Planning リクエスト・フォームの承認者としてのチームの追加

>[!NOTE]
>
>プレビュー：2025 年 7 月 22 日（PT）
>>迅速リリース用の実稼動版： 2025年8月14日（PT）
>>実稼動版（すべてのお客様向け）：2025年10月16日（PT）

承認プロセスの柔軟性を高めるために、Planning のリクエストフォームに承認者としてチームを追加する機能を追加しました。 現在は、承認者を設定する際に、チーム名を入力および選択できます。 チームメンバーは誰でも決定を行うことができます。これは、チーム全体の承認決定としてカウントされます。

以前は、個々のユーザーのみを承認者として割り当てることができました。

詳しくは、[Adobe Workfront Planning のリクエストフォームへの承認の追加 ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) を参照してください。

## レコードの承認情報を表示する新しいフィールド

>[!NOTE]
>
>プレビュー：2025 年 7 月 17 日（PT）
>>迅速リリース用の実稼動版： 2025年8月14日（PT）
>>実稼動版（すべてのお客様向け）：2025年10月16日（PT）

次のフィールドを導入して、承認を伴うリクエストを送信することで作成されたレコードの承認情報を取得しています。

* 承認者
* 承認日

詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

## 適用されたグループ化に基づいてフィールドを自動入力

>[!NOTE]
>
>プレビュー：2025 年 7 月 10 日（PT）
>>実稼動迅速リリース：2025 年 8 月 14 日（PT）
>>実稼動版（すべてのお客様向け）：2025年10月16日（PT）


現在、テーブルビューに適用されたグループ化が存在する場合、テーブルにレコードを追加すると、レコードの追加先のグループ化に関連するフィールドが自動入力されるようになりました。

複数のグループ化を適用した場合、最後のグループ化条件内のリストの最後にレコードを追加した場合にのみ、すべてのグループ化に関連付けられたフィールドが自動的に入力されます。

この機能強化の前は、グループ化に関連付けられたフィールドを手動で更新する必要がありました。

詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
