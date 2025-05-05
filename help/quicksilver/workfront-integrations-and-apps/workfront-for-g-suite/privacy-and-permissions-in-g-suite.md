---
product-area: workfront-integrations
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Workfront for Google Workspaceのプライバシーと権限
description: Workfront for Google Workspaceのプライバシーと権限
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 43%

---

# Workfront for Google Workspaceのプライバシーと権限

顧客のプライバシーは重要なので、Adobe Workfront は、Google プラグインアプリのサードパーティ認証に起因する、顧客を特定する顧客データを保存または収集しません。Google Workspace用Workfront Google API から受け取った情報の使用および他のアプリへの転送は、使用制限を含む [&#128279;](https://developers.google.com/terms/api-services-user-data-policy)0&rbrace;Google API サービスユーザーデータポリシー &rbrace; に従います。

Workfront for Google Workspace プラグインが最大限の価値を引き出せるように、次の権限が必要です。

* **アドオンの実行中にメールメッセージを表示**:Workfront for Google Workspace プラグインを使用すると、Workfront内の新しいタスクにメールを変換し、タスクのタイトルと説明にメールの件名と本文を自動入力することで、ユーザーの重複する作業を何時間も省くことができます。 また、このプラグインを使用すると、メールを新しいコメントとして Workfront に投稿することもできます。この価値を提供するために、プラグインはアドオンの実行時にメールメッセージを表示する必要があります。
* **Gmail として実行アドオン /機密**:Workfront for Google Workspace アドオンが Gmail 環境で機能するには、権限が必要です。 プラグインが Gmail 環境で機能するには、`Run as a Gmail add-on / non-sensitive` 権限を必要とします。
* **アドオンの実行中にメールメッセージメタデータを表示**：ワークフローを改善するために、Workfront for Google Workspace プラグインはメールがWorkfront通知かどうかを確認し、Workfront通知のタイプ（新規作業要求、承認要求、新規コメントなど）を特定します。 プラグインには、この値を提供するために `View your email message metadata when the add-on is running` 権限が必要となります。
* **プラグインは、カレンダーアドオンとして実行/非機密にする必要があります**:Workfront for Google Workspace プラグインはカレンダーに接続し、タスクがスケジュールに与える影響を視覚化できます。 プラグインには、`Run as a Calendar add-on / non-sensitive` 権限が必要です。
* **外部サービスに接続する権限：**&#x200B;プラグインは最終的に、プラグインの値のバックボーンである Workfront API に接続する必要があります。Workfront API は Google の外部にあるサービスなので、プラグインを動作させるには `Connect to an external service permission` が必要です。

顧客のプライバシーに対する Adobe Workfront の取り組みについて詳しくは、[Workfront のプライバシーに関するお知らせ](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf)を参照してください。

詳しくは、[Google API サービスのユーザーデータに関するポリシー](https://developers.google.com/terms/api-services-user-data-policy)を参照してください。
