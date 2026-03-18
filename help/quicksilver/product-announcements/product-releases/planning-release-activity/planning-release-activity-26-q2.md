---
content-type: release-notes
title: Adobe Workfront Planning の 2026年第 2 四半期リリースアクティビティ
description: これは、2026 年第 2 四半期のAdobe Workfront Planning 製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 79d4ad4a-1dd0-431e-92cd-582b5a1b7ec8
source-git-commit: 50ee9ac593e230e6f869f4158a67e4c3113aed45
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 15%

---

# Adobe Workfront Planning の 2026年第 2 四半期リリースアクティビティ

この記事では、2026 年第 2 四半期のリリースでWorkfront Planning に対してリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront Planning 用にリリースされたすべての機能の一覧については、[Adobe Workfront Planning リリース アクティビティ：記事一覧 &#x200B;](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md) を参照してください。

<!--

## New field type for Record ID  

>[!NOTE]
>
>Preview: March 12, 2026
>Production fast release: April 15, 2026
>Production for everyone: April 16, 2026

We have added a new field type for Record ID. This is a system-generated alpha-numeric indicator which uniquely identifies each record. The field displays in any record view as well as the record details area.  

For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).

-->

## 管理者以外のユーザーがレコードタイプを接続可能にすることを許可

>[!NOTE]
>
>プレビュー：2026 年 3 月 12 日（PT）
>実稼動（迅速リリース）：2026年4月15日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

現在、ワークスペース管理者である非管理者が、特定のワークスペースからレコードタイプを接続可能にできるようになりました。

この更新以前は、管理者以外のユーザーは、レコードタイプを接続可能にすることができませんでした。 特定のワークスペースからレコードタイプに接続できるようになりました。 システム内のすべてのワークスペースからレコードタイプを接続可能にすることはできません。

詳しくは、[&#x200B; レコードタイプのクロスワークスペース機能の設定 &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

## トリガーベースの自動処理

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

Planning の自動化を使用して、レコード・フィールドの変更に基づいて Planning レコードまたはWorkfrontオブジェクトを自動作成できるようになりました。

この機能強化の前は、事前設定されたボタンをクリックした場合にのみ、Planning レコードまたはWorkfrontオブジェクトを自動作成できました。

詳しくは、[Adobe Workfront Planning の自動設定の構成 &#x200B;](/help/quicksilver/planning/records/configure-automations-to-create-records.md) を参照してください。

## システム管理者のみが、システム全体でワークスペースを共有できます

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

ワークスペースを共有する際に、システム管理者が次のいずれかのオプションを選択できるようになりました。

* システム内の全員が表示可能
* 招待されたユーザーのみがアクセス可能

デフォルトでは、ワークスペースは「招待されたユーザーのみがアクセスできる」権限に設定されています。

この変更以前は、これらのワークスペース共有権限を選択する機能は存在しませんでした。

詳しくは、ワークスペースの共有（help/quicksilver/planning/access/share-workspaces.md）を参照してください。

## タイムラインビューでのグループ化の並べ替え

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

タイムライン表示でグループ化を並べ替えられるようになりました。 詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。

## 接続されたフィールドのユーザー参照のサポート

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

Workfront オブジェクトとWorkfront Planning レコードタイプの間に新しい接続を追加することで、Workfront ユーザーフィールドをWorkfront Planning レコードタイプに接続できるようになりました。

例えば、プロジェクトまたはポートフォリオへの接続を追加する際に、プロジェクトスポンサーまたはPortfolio オーナーをWorkfront Planning のルックアップフィールドとして追加できるようになりました。

詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。


## リアルタイムプレゼンス指標で、テーブル表示にユーザーが表示されるようになりました

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

テーブル表示のセルの右上隅にあるリアルタイムプレゼンスインジケーターをクリックして、ユーザーが同時にレコードフィールドを更新するのを確認できるようになりました。 レコードテーブルビューの右上隅にリストされているユーザーは、同じビューを開いているユーザーです。

テーブルビューヘッダーで「共同作業者を表示」設定をオンにする必要があります。 他のユーザーは、テーブル表示またはレコードの詳細領域のフィールドを更新できます。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。


## リストビューの共有エクスペリエンスの更新

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

表示権限を持つレコードの、プロジェクトに接続されたレコードページでリストビューを共有する場合、ビューを共有するユーザーはビュー要素を変更でき、それらの変更はユーザーの個人環境設定に保存されます。 変更を含むビューのコピーを保存するか、共有ビューを元の設定にリセットするオプションが追加されました。 コピーしたビューを他のユーザーと共有することもできます。

この更新は、プロジェクトの表示時にレコードの接続されたレコードページのリスト表示でのみ使用できます。

詳しくは、「[&#x200B; リスト表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-list-view.md)」を参照してください。

## リスト表示への条件付き書式の適用

>[!NOTE]
>
>プレビュー：2026 年 2 月 26 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

レコードの接続されたレコード ページのリストビューで、プロジェクトに条件付き書式を適用できるようになりました。 この機能は、この機能強化の前はリスト表示には存在しませんでした。

詳しくは、「[&#x200B; リスト表示の管理 &#x200B;](/help/quicksilver/planning/views/manage-the-list-view.md) を参照してください。

## セカンダリワークスペースのグローバルレコードタイプの改善

>[!NOTE]
>
>プレビュー：2026 年 2 月 5 日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

プライマリワークスペースからセカンダリワークスペースに追加されたグローバルレコードタイプの表示が改善されました。 改善点は次のとおりです。

* レコードタイプが別のワークスペースから追加されたことを示す、少し変更されたグローバルアイコン。

* レコードタイプが作成されたワークスペースを明確に識別する、新しいアイコンのツールチップを改善しました。

詳しくは、[&#x200B; 別のワークスペースから既存のレコードタイプを追加する &#x200B;](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md) を参照してください。

## レコードの詳細プレビューボックスに表示されるフィールドを設定する

>[!NOTE]
>
>プレビュー：2026 年 1 月 29 日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

レコードの「詳細」プレビューボックスで、テーブル表示に表示されるフィールドに基づいてレコードフィールドの表示/非表示を切り替えることができる設定を導入しました。 

この新しい設定では、レコードの詳細プレビューエリアから、テーブル表示で非表示になっているフィールドを含めるか除外するかを選択することができます。

詳しくは、[&#x200B; レコードページレイアウトの管理 &#x200B;](/help/quicksilver/planning/records/manage-the-record-page.md) を参照してください。

## 元の要求の新しい Planning 接続フィールド

>[!NOTE]
>
>プレビュー：2026 年 1 月 29 日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

レコードタイプに「元のリクエスト」接続フィールドを追加できるようになりました。 Planning 要求フォームを送信してレコードを作成すると、元の要求の名前が「元の要求接続」フィールドに移入されます。

この機能強化の前は、リクエスト エリアからのみ、レコードを作成した元のリクエストを表示してアクセスできました。

詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

## Workfront Planning での要求の承認ルールの作成

>[!NOTE]
>
>プレビュー：2026 年 1 月 29 日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

リクエストの承認をより動的かつ柔軟にするために、承認ルールを作成する機能を追加しました。 これらのルールを使用すると、リクエスト内のフィールド値に基づいて、リクエストを様々な承認者にルーティングできます。

例えば、リクエストフォームに「キャンペーンタイプ」フィールドがある場合、フィールドの値が「デジタル」の場合は 1 人のユーザーにリクエストを送信し、値が「印刷」の場合は別のユーザーにリクエストを送信するルールを作成できます。

承認ルールはリクエストフォームで作成されます。

詳細および手順については、「Adobe Workfront Planning の要求フォームに承認を追加する [」の &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md#add-approval-rules-to-a-request-form) 要求フォームに承認ルールを追加する」を参照してください。

## Workfront Planning のユーザー先行入力フィールドにメールを表示する

>[!NOTE]
>
>プレビュー：2026 年 1 月 22 日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

ユーザーを次のエリアに追加すると、ユーザーのメールが表示されるようになりました。

* 人物タイプの計画フィールド
* Planning オブジェクトを共有する場合の「共有」ボックス

この機能強化の前は、これらのエリアにユーザーを追加する際に、ユーザー名に加えて、ユーザーのプライマリロールのみが表示されていました。
詳しくは、次の記事を参照してください。

* [フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)
* [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

## 人物フィールドは、Planning 接続の参照フィールドとして使用可能です

>[!NOTE]
>
>プレビュー：2026 年 1 月 14 日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

2 つの Planning レコードタイプを接続する際、ルックアップフィールドに人物フィールドを追加できるようになりました。

詳しくは、[&#x200B; レコードタイプの接続 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md) を参照してください。
