---
title: 2026 年第 1 四半期リクエストの機能強化
description: 2026 年第 1 四半期リクエストの機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d8f563bdbde76ae86b5e130a07d2dc66c8d2e034
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 4%

---

# 2026 年第 1 四半期リクエストの機能強化

このページでは、2026 年第 1 四半期のリリースで行われた、プレビュー環境に対するリクエストの機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第 1 四半期リリースサイクルの現時点で利用可能なすべての変更のリストについて詳しくは、[2026年第 1 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)を参照してください。

## リクエストエリアとマイリクエストウィジェットで作成済みのオブジェクトリンクを使用できるようになりました

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

特定のリクエストで作成されたオブジェクトに簡単に移動できるように、「作成されたオブジェクト」列へのリンクを追加しました。 これで、この列のリンクをクリックして、作成したオブジェクトのページに直接移動できます。

このリンクは、要求自体がオブジェクトを作成した場合に、Planning 要求に対してのみ使用できます。 Workfront リクエストがプロジェクトまたは他のオブジェクトに変換された場合、その変換後のオブジェクトへのリンクは、新しいリクエスト環境のリクエストリストで使用できません。

以前は、この列にはオブジェクトの名前のみが含まれており、リンクは含まれていませんでした。

これらのリンクの場所については、以下を参照してください。

* [送信されたリクエストを見つける](/help/quicksilver/manage-work/requests/create-requests/locate-submitted-requests.md)
* [自分のリクエスト ウィジェットの使用](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)

<!--

## Create groupings in the Requests list and My Requests widget

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026  
>Production for everyone: January 15, 2026  

To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.

For more information on creating views for the Request list and My Requests widget, including adding groupings, see [Create or edit views in the Requests area and My Requests widget](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).

-->

## リクエスト エリアとマイリクエストウィジェットでのビューの共有

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

必要な情報を確実に表示しやすくするために、新しいリクエスト用エクスペリエンスにビューを共有する機能を追加しました。 他のユーザー、チーム、グループとビューを共有できるようになりました。

共有を含むリクエストビューについて詳しくは、[ リクエストエリアでのビューの作成と管理 ](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md) を参照してください。

## リクエストリストとマイリクエストウィジェットにカスタムフィールドを追加

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

必要な情報を見やすくするために、ホームのリクエスト リストとマイリクエストウィジェットに列としてカスタムフィールドを追加する機能を追加しました。 これで、カスタムフォームのフィールドを列として追加でき、そのフィールドに情報が含まれるリクエストは、その情報をリストまたはウィジェットに表示します。

この機能は、新しいリクエスト エクスペリエンスでのみ使用できます。

以前は、リクエストリストやマイリクエストウィジェットではカスタムフィールドを使用できませんでした。

列の追加手順については、以下を参照してください。

* [リクエスト エリアでのビューの作成または編集](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md)
* [自分のリクエスト ウィジェットの使用](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)

## 現在のユーザーワイルドカードを要求フィルターで使用できるようになりました

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

自分に適用されるリクエストをフィルタリングしやすくするために、現在のユーザーワイルドカードを作成しました。 これで、フィルタリング時に「自分（ログインしたユーザー）」を選択できます。 その後、フィルターはリクエストリストを表示しているユーザーに適用されます。

これは、複数のユーザーが使用するビューにフィルターを追加する場合に便利です。 各ユーザーに適用されるフィルター結果が表示されます。

ワイルドカードは、値がユーザーであるフィールドで使用できます。

フィルターを含む、リクエストリストでのビューの設定について詳しくは、「[ リクエスト領域でのビューの作成または編集 ](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md) を参照してください。

## AI を活用したフォーム入力がリクエストに使用できるようになりました

>[!NOTE]
>
>プレビュー：2025 年 12 月 11 日（PT）
>実稼動高速リリース：2025 年 12 月 11 日（PT）\
>すべてのユーザー向けの実稼動：2025 年 12 月 11 日（PT）

リクエストの作成を容易にするために、AI を活用したフォーム入力を作成しました。 これで、プロンプトに貼り付けたり、リクエストフォームにドキュメントをアップロードしたりするだけで、AI が関連情報を取り出してフォームに入力します。

この機能にアクセスするには、組織の AI が有効になっている必要があります。

組織の AI を有効にするために必要なことなど、AI を利用したフォーム入力について詳しくは、[AI を利用したフォーム入力を使用してプロンプトやドキュメントを使用してリクエストを入力する ](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md) を参照してください。


## リクエストのドラフトを新しいリクエストエクスペリエンスに保存

>[!NOTE]
>
>プレビュー：2025 年 11 月 20 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

リクエストの作成と送信を簡単にするために、新しいリクエスト用エクスペリエンスにドラフトを保存する機能が追加されました。 リクエストの入力を開始して閉じると、リクエストはドラフト ステータスで保存され、ドラフトの作成に使用したリクエストフォームに表示されます。 その後、必要に応じてドラフトを再度開き、更新して送信できます。

以前は、この機能は、新しいリクエストエクスペリエンスでは使用できませんでした。

リクエストドラフトについて詳しくは、「[ ドラフトからのリクエストの作成 ](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md)」を参照してください。

## 新しい要求エクスペリエンスで送信済み要求を削除

>[!NOTE]
>
>プレビュー：2025 年 11 月 20 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

リクエストを整理し整頓しやすくするために、新しいリクエスト用エクスペリエンスにリクエストを削除する機能が追加されました。 送信したリクエストを削除できるようになりました。 Workfront管理者とWorkfront Planning Workspace管理者は、リクエストを削除することもできます。

以前は、この機能は、新しいリクエストエクスペリエンスでは使用できませんでした。

詳細と手順については、[ 送信されたリクエストまたはリクエストドラフトの削除 ](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md) を参照してください。


## 以前に送信したリクエストを新しいリクエストエクスペリエンスにコピーして、新しいリクエストを作成します

>[!NOTE]
>
>プレビュー：2025 年 11 月 20 日（PT）
>実稼動高速リリース：2025 年 12 月 11 日（PT）\
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

リクエストを送信しやすくするために、新しいリクエスト用エクスペリエンスにリクエストをコピーする機能を追加しました。 これで、リクエストをコピーし、フィールドを編集して、新しいリクエストとして送信できます。

以前は、この機能は、新しいリクエスト用エクスペリエンスでは使用できませんでした。

リクエストのコピーと送信について詳しくは、[ リクエストのコピーと送信 ](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md) を参照してください。







