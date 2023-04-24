---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Workfront for G Suite のプライバシーと権限
description: Workfront for G Suite のプライバシーと権限
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: a156092bf2b6cca70d09b76a65d755fbe05ec8da
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Workfront for G Suite のプライバシーと権限

顧客のプライバシーは重要なので、Adobe Workfrontは、Googleプラグインアプリのサードパーティ認証によって生じる、識別する顧客データを保存または収集しません。 Workfront for G Suite の使用と、Google API から受け取った情報の他のアプリへの転送は、Google API Services のユーザーデータポリシー（使用制限の要件を含む）に従います。

Workfront for G Suite プラグインが最大値を提供できるように、次の権限が必要です。

* **アドオンの実行時に電子メールメッセージを表示する**:Workfront for G Suite プラグインは、E メールをWorkfrontの新しいタスクに変換し、タスクのタイトルと説明に E メールの件名と本文を自動的に入力することで、ユーザーの重複作業を数え切れないほど時間を節約できます。 また、このプラグインを使用すると、E メールを新しいコメントとしてWorkfrontに投稿することもできます。 プラグインは、この値を配信するためにアドオンが実行されているときに、電子メールメッセージを表示する必要があります。
* **Gmail アドオンとして実行/機密性なし**:Gmail 環境で G Suite アドオンが機能するには、Workfrontの権限が必要です。 プラグインを使用するには Gmail 環境が必要なので、 `Run as a Gmail add-on / non-sensitive` 権限。
* **アドオンの実行時に電子メールメッセージのメタデータを表示する**:ワークフローを改善するために、Workfront for G Suite プラグインは、電子メールがWorkfront通知であるかどうかを確認し、Workfront通知のタイプ（新しい作業リクエスト、承認リクエスト、新しいコメントなど）を識別します。 プラグインを使用するには、 `View your email message metadata when the add-on is running` この値を配信する権限。
* **プラグインは、カレンダーアドオンとして実行する必要がある/機密性が低い**:Workfront for G Suite プラグインは、カレンダーに接続するので、タスクがスケジュールに与える影響を視覚化できます。 プラグインには `Run as a Calendar add-on / non-sensitive` 権限を持っています。
* **外部サービスに接続する権限：** 最終的に、プラグインはWorkfront API に接続する必要があります。これは、プラグイン値のバックボーンです。 Workfront API はGoogleの外部にあるサービスなので、このプラグインには `Connect to an external service permission` を使用してプラグインを動作させる。

顧客のプライバシーに対するAdobe Workfrontの取り組みについて詳しくは、 [Workfrontのプライバシーに関するお知らせ](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

詳しくは、 [Google API Services ユーザーデータポリシー](https://developers.google.com/terms/api-services-user-data-policy).
