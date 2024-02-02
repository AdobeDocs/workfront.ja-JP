---
product-area: projects
navigation-topic: manage-issues
title: フィードバック待ちから進行中へイシューステータスを自動的に更新する
description: イシューのプライマリ連絡先が、フィールド（カスタムフィールドを含む）の更新またはコメントの追加によってイシューを更新すると、イシューのステータスが自動的に「処理中」に更新されます。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '222'
ht-degree: 100%

---

# フィードバック待ちから進行中へイシューステータスを自動的に更新する

イシューのプライマリ連絡先が、フィールド（カスタムフィールドを含む）の更新またはコメントの追加によってイシューを更新すると、イシューのステータスが自動的に「処理中」に更新されます。

この自動ステータス変更を行うには、次の条件が必要です。

* イシューはリクエストキューを通じて入力する必要があります。

  リクエストキューの作成について詳しくは、[リクエストキューを作成および管理](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md)の節を参照してください。リクエストの作成について詳しくは、[Adobe Workfront リクエストの作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

* リクエストキュー内のキューの詳細で、次の設定を行う必要があります。
   * 「**リクエストが行われる際に自動的に付与する権限**」を「**アクセスに参加**」に設定
   * 「詳細設定」で「**ステータスを変更**」を選択

  ![キューの詳細で「アクセスに参加」と「ステータスを変更」を選択。](assets/queuedetails-contributeaccess-changestatus.png)

  キューの詳細について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

* イシューのステータスが「フィードバック待ち」になっている必要があります。
* システムレベルのイシューで、フィードバック待ち（AWF）ステータスが使用可能である必要があります。

  システムレベルのステータスについて詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。
