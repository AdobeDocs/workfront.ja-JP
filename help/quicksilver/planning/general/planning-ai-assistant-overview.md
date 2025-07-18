---
title: Adobe Workfront計画 AI アシスタントの概要
description: AI アシスタントを使用して、現在のページコンテキストとレコード構造に基づいてレコードを生成、更新または削除できます。 ユーザーのコマンドと AI によるコマンドの実行を連携させることで、AI によって行われた変更が環境に正確に反映されるようになります。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: a36968bdae5756f0f8283da04a2afca83b4dd94a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 4%

---


# Adobe Workfront計画 AI アシスタントの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

AI アシスタントを使用して、現在のページコンテキストとレコード構造に基づいてレコードを生成、更新または削除できます。

ユーザーのコマンドと AI によるコマンドの実行を連携させることで、AI によって行われた変更が環境に正確に反映されるようになります。

## AI アシスタントに関する考慮事項

* 会社のユーザーが AI アシスタントを使用できるようにするには、組織で AI アシスタントを有効にする必要があります。 詳しくは、[AI アシスタントの概要 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) を参照してください。
* Workfrontで組織の AI アシスタントが有効になると、メインのWorkfront管理者が使用できるようになります。 詳しくは、[システムの基本情報を設定](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。

* Workfront管理者は、他のすべてのユーザーに対して AI アシスタントを有効にする必要があります。 詳しくは、[AI アシスタントを有効または無効にする ](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

* AI アシスタントは、各ページのコンテキストで機能します。 AI アシスタントに対して送信するリクエストでは、開いているページで使用できる機能を参照する必要があります。

* 計画領域で AI アシスタントが実行するアクションは、Workfront Planning の権限とWorkfrontのアクセスレベルのコンテキストにあります。 詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)

* ユーザーに代わって AI アシスタントが行った変更は、レコードの履歴パネルで追跡されます。

* コマンドを使用してアクションを取り消すことができます。 例えば、「最後の変更を取り消す」と入力して、変更を元に戻すことができます。

* AI Assistant を使用してオブジェクトを作成、更新、または削除する場合、AI Assistant は意図したアクションを表示し、確認を求めます。 その後、アクションを確認またはキャンセルできます。

## 現在、AI アシスタントで使用可能な機能

現在、Workfrontの Planning エリアでは、次のページで AI アシスタントを使用できます。

* Workspaceページ
* レコードタイプページ
* レコードページ

この時点で、AI アシスタントを使用して次の操作を実行できます。

* レコードを検索します。 レコードフィールドに含まれる情報で検索できます。
* レコードを作成します。 新規レコードへのリンクを含む ID は、レコードの作成後に表示されます。 日付や説明など、作成プロセス中に更新するフィールドを指定できます。
* アップロードするドキュメントに基づいてレコードを作成します。 Workfrontは、AI アシスタントで次のドキュメント形式をサポートしています。

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT、およびほとんどの画像形式
* 画面に表示されるレコードのフィールドを更新
* レコードの削除
* 削除したばかりのレコードを復元します


## Workfront Planning で AI アシスタントを見つけます

AI アシスタントは、Workfront計画の次の領域に配置できます。

* 画面の右上隅にあるメインナビゲーションバー。
* プレビューでレコードを開いた後、またはレコードのページを開いた後、レコードの詳細領域内。

## 計画エリアで AI アシスタントにアクセスする

1. Workfrontにログインし、画面の右上隅にある **メインメニュー** アイコン ![ ドットメインメニュー ](assets/dots-main-menu.png) をクリックするか、左上隅にある **メインメニュー** アイコン ![ ラインメインメニュー ](assets/lines-main-menu.png) をクリックします。

.**計画** をクリックします。 計画エリアが開きます。

1. **ワークスペースカード** をクリックします。

1. （任意） **レコードタイプカード** をクリックします。

1. （任意） **レコード** をクリックして、レコードの **詳細** ページを開きます。

1. グローバルナビゲーションバーの画面の右上隅にある **AI アシスタント** アイコン、またはレコードのプレビューまたはページの右上隅をクリックします。

   ![AI アシスタント アイコン ](assets/ai-assistant-icon-highlighted.png)

1. 指定されたスペースで、AI アシスタントのコマンドの入力を開始し、完了したら [Enter] をクリックします。

   ![ 空のコマンドボックスを持つ AI アシスタントパネル ](assets/ai-assistant-panel-with-empty-command-box.png)

   たとえば、次のいずれかを入力できます。

   * 開始日が 7 月 4 日、終了日が 7 月 30 日のキャンペーンを作成します
   * 日付を決定するように、夏物キャンペーンレコードの「説明」フィールドを更新します
   * 最後のレコードを削除
   * レコードを復元

   AI Assistant がコマンドを処理している間に視覚的なインジケータが表示され、応答時間の期待値が設定されます。

   応答が成功したら、提供されたリンクに従うか、左側の変更に注目してください。



