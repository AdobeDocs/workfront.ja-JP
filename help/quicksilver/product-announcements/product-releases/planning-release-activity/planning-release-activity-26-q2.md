---
content-type: release-notes
title: Adobe Workfront Planning の 2026年第 2 四半期リリースアクティビティ
description: これは、2026年第2四半期のAdobe Workfront計画製品のリリースアクティビティです。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: 79d4ad4a-1dd0-431e-92cd-582b5a1b7ec8
source-git-commit: fa4d8132cecd51b93f26c28803535a84bebad137
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 15%

---

# Adobe Workfront Planning の 2026年第 2 四半期リリースアクティビティ

この記事では、2026年第2四半期リリース中にWorkfront Planningでリリースされる機能について説明します。

<!--keep the sentence below for all future quarterly release pages-->

Adobe Workfront計画でリリースされたすべての機能の一覧については、[Adobe Workfront計画リリースアクティビティ：記事インデックス ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)を参照してください。

## パンくずリストの再設計

>[!NOTE]
>
>プレビュー：2026年3月26日（PT）
>実稼動（迅速リリース）：2026年4月15日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

レコードタイプとレコード全体でパンくずリストを表示する方法を再設計しました。 パンくずリストの「詳細」をクリックすると、レコードとオブジェクトの名前が複数の行に表示されるようになりました。 この機能強化の前は、「詳細」をクリックすると、ドロップダウンメニューにレコードとオブジェクトの名前が表示されていました。

詳しくは、[階層とパンくずリストの概要](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)を参照してください。

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

## 管理者以外のユーザーがレコードタイプを接続可能にできるようにします

>[!NOTE]
>
>プレビュー：2026年3月12日（PT）
>実稼動（迅速リリース）：2026年4月15日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

現在、ワークスペースマネージャーである管理者以外のユーザーでも、特定のワークスペースからレコードタイプを接続可能にすることができます。

この更新の前は、管理者以外のユーザーは、レコードタイプを接続可能にすることができませんでした。 これにより、レコードタイプを特定のワークスペースから接続できるようになります。 レコードタイプをシステム内のすべてのワークスペースから接続可能にすることはできません。

詳しくは、[ レコードタイプのクロスワークスペース機能の設定](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)を参照してください。

## トリガーベースドオートメーション

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

Planning Automationを使用して、レコードフィールドの変更に基づいて、Planning レコードまたはWorkfront オブジェクトを自動的に作成できるようになりました。

この機能強化の前は、事前設定済みボタンをクリックした場合にのみ、Planning レコードまたはWorkfront オブジェクトを自動的に作成できました。

詳しくは、[Adobe Workfront Planningの自動処理の設定](/help/quicksilver/planning/records/configure-automations-to-create-records.md)を参照してください。

## システム全体でワークスペースを共有できるのは、システム管理者のみです

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

ワークスペースを共有する際に、システム管理者のみが次のオプションを選択できるようになりました。

* システム内の全員が表示可能
* 招待されたユーザーのみがアクセス可能

デフォルトでは、ワークスペースは「招待されたユーザーのみがアクセスできる」権限に設定されています。

この変更以前は、これらのワークスペース共有権限を選択する機能は存在しませんでした。

詳しくは、ワークスペースの共有（help/quicksilver/planning/access/share-workspaces.md）を参照してください。

## タイムラインビューでのグループ化の並べ替え

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

タイムラインビューでグループ化を並べ替えることができるようになりました。 詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。

## 接続されたフィールドのユーザー参照をサポート

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

Workfront オブジェクトとWorkfront Planning レコードタイプの間に新しい接続を追加することで、Workfront ユーザーフィールドをWorkfront Planning レコードタイプに接続できるようになりました。

例えば、プロジェクトまたはポートフォリオに接続を追加する際に、Workfront PlanningのルックアップフィールドとしてプロジェクトスポンサーまたはPortfolio オーナーを追加できるようになりました。

詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。


## リアルタイムのプレゼンス指標で、ユーザーがテーブルビューに表示されるようになりました

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

テーブルビューのセルの右上隅にあるリアルタイムプレゼンス指標をクリックすることで、レコードフィールドを更新するユーザーを同時に表示できるようになりました。 レコードテーブルビューの右上隅に表示されるユーザーは、同じビューを開いているユーザーです。

テーブルビューヘッダーの「共同作業者を表示」設定をオンにする必要があります。 他のユーザーは、レコードのテーブルビューまたは詳細領域のフィールドを更新できます。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。


## リストビューの共有エクスペリエンスを更新

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

ビュー権限を持つレコードのプロジェクト接続レコードページでリストビューを共有すると、ビューを共有するユーザーはビュー要素を変更でき、それらの変更はユーザーの個人設定に保存されます。 変更内容を含むビューのコピーを保存したり、共有ビューを元の設定にリセットしたりするオプションが表示されます。 コピーしたビューをさらに他のユーザーと共有できます。

この更新は、プロジェクトを表示する際に、レコードの接続されたレコードページのリストビューでのみ使用できます。

詳しくは、[ リスト表示の管理](/help/quicksilver/planning/views/manage-the-list-view.md)を参照してください。

## リスト表示に条件付き書式を適用する

>[!NOTE]
>
>プレビュー：2026年2月26日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

レコードの接続されたレコードページのリストビューで、プロジェクトに条件付き書式設定を適用できるようになりました。 この機能は、この機能強化の前にリストビューに存在しませんでした。

詳しくは、[ リスト表示の管理](/help/quicksilver/planning/views/manage-the-list-view.md)を参照してください。

## セカンダリワークスペースのグローバルレコードタイプの改善

>[!NOTE]
>
>プレビュー：2026年2月5日（PT）
>実稼動（迅速リリース）：2026年3月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

プライマリワークスペースからセカンダリワークスペースに追加されたグローバルレコードタイプの可視性が向上しました。 改善点は次のとおりです。

* レコードタイプが別のワークスペースから追加されたことを示す、わずかに変更されたグローバルアイコン。

* 新しいアイコンのツールチップが改善され、レコードタイプが作成されたワークスペースが明確に識別されるようになりました。

詳しくは、[別のワークスペースから既存のレコードタイプを追加](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)を参照してください。

## レコードの「詳細」プレビューボックスに表示されるフィールドを設定します

>[!NOTE]
>
>プレビュー：2026年1月29日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

テーブルビューに表示されるフィールドに基づいて、レコードの詳細プレビューボックスでレコードフィールドを表示または非表示にできる設定を導入しました。 

この新しい設定では、レコードの詳細プレビュー領域からテーブルビューで非表示になっているフィールドを含めるか除外するかを選択できます。

詳しくは、[ レコードページレイアウトの管理](/help/quicksilver/planning/records/manage-the-record-page.md)を参照してください。

## 元のリクエストの新しいプランニング接続フィールド

>[!NOTE]
>
>プレビュー：2026年1月29日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

「オリジナルリクエスト」接続フィールドをレコードタイプに追加できるようになりました。 Planning リクエストフォームを送信してレコードを作成すると、元のリクエストの名前が「元のリクエスト接続」フィールドに入力されます。

この機能強化を行う前は、レコードを作成した元のリクエストをリクエスト領域からのみ表示してアクセスできました。

詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

## Workfront Planningでのリクエストの承認ルールの作成

>[!NOTE]
>
>プレビュー：2026年1月29日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

リクエストの承認をより動的かつ柔軟にするために、承認ルールを作成する機能を追加しました。 これらのルールにより、リクエストをリクエスト内のフィールド値に基づいて異なる承認者にルーティングできます。

例えば、リクエストフォームに「Campaign type」フィールドがある場合、そのフィールドに「Digital」という値がある場合は1人に、そのフィールドに「Print」という値がある場合は別のユーザーにリクエストを送信するルールを作成できます。

承認ルールは、リクエストフォームで作成されます。

詳しくは、「[ リクエストフォームに承認ルールを追加する](/help/quicksilver/planning/requests/add-approval-to-request-form.md#add-approval-rules-to-a-request-form)」を参照してください。Adobe Workfront Planningの「リクエストフォームに承認を追加する」を参照してください。

## Workfront Planningのユーザー先行入力フィールドにメールを表示する

>[!NOTE]
>
>プレビュー：2026年1月22日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

ユーザーを次の領域に追加すると、ユーザーの電子メールが表示されるようになりました。

* 人物タイプ計画フィールド
* Planning オブジェクトを共有する場合の「共有」ボックス

この機能強化を行う前は、ユーザーの名前に加えて、ユーザーのプライマリロールのみが表示されていました。
詳しくは、次の記事を参照してください。

* [フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)
* [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

## 人物フィールドは、Planning接続のルックアップフィールドとして有効になります

>[!NOTE]
>
>プレビュー：2026年1月14日（PT）
>実稼動（迅速リリース）：2026年2月12日（PT）
>実稼動（全ユーザー）：2026年4月16日（PT）

2つのプランニングレコードタイプを接続する際に、ルックアップフィールドに「人物」フィールドを追加できるようになりました。

詳しくは、[ レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
