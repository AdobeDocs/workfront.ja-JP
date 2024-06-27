---
title: 'Adobe Workfront Planning AI Assistant の概要'
description: AI アシスタントを使用して、現在のページコンテキストとレコード構造に基づいてレコードを生成、更新または削除できます。 ユーザーのコマンドと AI によるコマンドの実行を連携させることで、AI によって行われた変更が環境に正確に反映されるようになります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 64f187ed78b69db9b9ac0259e96ef0bf47abf4f4
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 8%

---


# Adobe Workfront計画 AI アシスタントの概要

<!-- update TOC and miniTOC when making this live-->

>[!IMPORTANT]
>
>この記事では、Adobe Workfront Planning と、Adobe Workfrontの新機能である AI アシスタントについて説明します。
>
>現在、Workfrontプランニングと AI アシスタントは、限られた数のお客様に開放されている早期アクセス段階にあります。
>
>これらの機能を使用するには、Workfront の顧客である必要があります。
>
>このステージに参加している場合は、アカウント担当者からお知らせします。
>
>詳しくは、[Adobe Workfront Planning の概要](/help/quicksilver/planning/general/planning-overview.md)を参照してください。

AI アシスタントを使用して、現在のページコンテキストとレコード構造に基づいてレコードを生成、更新または削除できます。

ユーザーのコマンドと AI によるコマンドの実行を連携させることで、AI によって行われた変更が環境に正確に反映されるようになります。

## AI アシスタントに関する考慮事項

* AI アシスタントは、Workfront管理者がデフォルトで使用できます。

* Workfront管理者は、他のすべてのユーザーに対して AI アシスタントを有効にする必要があります。 詳しくは、を参照してください [AI アシスタントを有効または無効にする](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* AI アシスタントは、各ページのコンテキストで機能します。 AI アシスタントに対して送信するリクエストでは、開いているページで使用できる機能を参照する必要があります。

* AI アシスタントが実行するアクションは、Workfront Planning の権限とWorkfrontのアクセスレベルに応じて異なります。 詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* ユーザーに代わって AI アシスタントが行った変更は、レコードの履歴パネルで追跡されます。

* コマンドを使用してアクションを取り消すことができます。

## 現在、AI アシスタントで使用可能な機能

現在、Workfrontの Planning エリアでは、次のページで AI アシスタントを使用できます。

* レコードタイプページ
* レコードページ

この時点で、AI アシスタントを使用して次の操作を実行できます。

* レコードを作成します。 新規レコードへのリンクを含む ID は、レコードの作成後に表示されます。
* アップロードするドキュメントに基づいてレコードを作成します。 Workfrontは、AI アシスタントで次のドキュメント形式をサポートしています。

  .pptx、.pdf、.docx、.xlsx、.ppt、.doc、.txt、およびほとんどの画像形式
* 画面に表示されるレコードのフィールドを更新
* レコードの削除
* 削除したばかりのレコードを復元します

## AI アシスタントへのアクセス

1. Workfrontにログインし、 **計画** 領域。

1. をクリック **ワークスペースカード** > **レコードタイプカード**.

1. （任意） **レコード** レコードを開く **詳細** ページ。

1. 「」をクリックします **AI アシスタント アイコン** をグローバルナビゲーションバーの画面の右上隅に表示します。

   ![](assets/ai-assistant-icon-highlighted.png)

1. 指定されたスペースで、AI アシスタントのコマンドの入力を開始し、完了したら [Enter] をクリックします。

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   たとえば、次のいずれかを入力できます。

   * レコードを作成
   * 日付を決定するように、夏物キャンペーンレコードの「説明」フィールドを更新します
   * 最後のレコードを削除
   * レコードを復元

   AI Assistant がコマンドを処理している間に視覚的なインジケータが表示され、応答時間の期待値が設定されます。

   応答が成功したら、提供されたリンクに従うか、左側の変更に注目してください。
