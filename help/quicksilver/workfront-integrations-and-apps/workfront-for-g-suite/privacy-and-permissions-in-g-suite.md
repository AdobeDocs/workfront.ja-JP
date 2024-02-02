---
product-area: workfront-integrations
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Workfront for G Suite のプライバシーと権限
description: Workfront for G Suite のプライバシーと権限
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: bd9fb14b99886f4a514c4d37ad9d93be7a051858
workflow-type: ht
source-wordcount: '384'
ht-degree: 100%

---

# Workfront for G Suite のプライバシーと権限

顧客のプライバシーは重要なので、Adobe Workfront は、Google プラグインアプリのサードパーティ認証に起因する、顧客を特定する顧客データを保存または収集しません。Workfront for G Suite による Google API から受け取った情報の使用および他のアプリへの転送は、[Google API サービスのユーザーデータに関するポリシー](https://developers.google.com/terms/api-services-user-data-policy)（使用制限要件を含む）に準拠します。

Workfront for G Suite プラグインが最大限の価値を提供できるように、次の権限が必要です。

* **アドオンの実行時にメールメッセージを表示する**：Workfront for G Suite プラグインを使用すると、メールを Workfront の新しいタスクに変換し、タスクのタイトルと説明にメールの件名と本文を自動的に入力することで、重複作業に費やすユーザーの時間を節約できます。また、このプラグインを使用すると、メールを新しいコメントとして Workfront に投稿することもできます。この価値を提供するために、プラグインはアドオンの実行時にメールメッセージを表示する必要があります。
* **Gmail アドオンとして非機密で実行する**：Workfront for G Suite アドオンが Gmail 環境で機能するためには、権限が必要です。プラグインが Gmail 環境で機能するには、`Run as a Gmail add-on / non-sensitive` 権限を必要とします。
* **アドオンの実行時にメールメッセージのメタデータを表示する**：ワークフローを改善するために、Workfront for G Suite プラグインは、メールが Workfront 通知であるかどうかを確認し、Workfront 通知のタイプ（新規作業リクエスト、承認リクエスト、新規コメントなど）を識別します。プラグインには、この値を提供するために `View your email message metadata when the add-on is running` 権限が必要となります。
* **プラグインはカレンダーアドオンとして非機密で実行する必要がある**：Workfront for G Suite プラグインは、カレンダーに接続するので、タスクがスケジュールに与える影響を視覚化できます。プラグインには、`Run as a Calendar add-on / non-sensitive` 権限が必要です。
* **外部サービスに接続する権限：**&#x200B;プラグインは最終的に、プラグインの値のバックボーンである Workfront API に接続する必要があります。Workfront API は Google の外部にあるサービスなので、プラグインを動作させるには `Connect to an external service permission` が必要です。

顧客のプライバシーに対する Adobe Workfront の取り組みについて詳しくは、[Workfront のプライバシーに関するお知らせ](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf)を参照してください。

詳しくは、[Google API サービスのユーザーデータに関するポリシー](https://developers.google.com/terms/api-services-user-data-policy)を参照してください。
