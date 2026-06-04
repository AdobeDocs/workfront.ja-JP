---
product-area: projects
navigation-topic: manage-issues
title: 問題のステータスを「フィードバック待ち」から「進行中」に自動更新
description: イシューのプライマリ連絡先が、フィールド（カスタムフィールドを含む）の更新またはコメントの追加によってイシューを更新すると、イシューのステータスが自動的に「処理中」に更新されます。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 56%

---

# フィードバック待ちから進行中へイシューステータスを自動的に更新する

<!--Audited: 109/2025-->

イシューのプライマリ連絡先が、フィールド（カスタムフィールドを含む）の更新またはコメントの追加によってイシューを更新すると、イシューのステータスが自動的に「処理中」に更新されます。

この自動ステータス変更を実行するには、次の手順を実行する必要があります。

* イシューは、リクエストキューを使用して追加する必要があります。

  リクエストキューの作成について詳しくは、「[ リクエストキューの作成と管理](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md)」を参照してください。

  リクエストキューへのリクエストの送信について詳しくは、[Adobe Workfront リクエストの作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

* リクエストキュー内のキューの詳細で、次の設定を行う必要があります。
   * 「**リクエストが行われる際に自動的に付与する権限**」を「**アクセスに参加**」に設定
   * **状態の変更**&#x200B;が選択されています

  ![キューの詳細で「アクセスに参加」と「ステータスを変更」を選択。](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  リクエストキューを設定する際に、送信する問題に対するプライマリコンタクトのアクセス権限を定義できます。
  >
  >リクエストキューを設定する際に「ステータスの変更」設定の選択を解除する場合は、リクエストキュー設定で「ステータスの変更」オプションが選択解除されていても、システム管理者は常に問題のステータスを変更するアクセス権を持っていることを忘れないでください。

  キューの詳細について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

* イシューのステータスが「フィードバック待ち」になっている必要があります。
* システムレベルのイシューで、フィードバック待ち（AWF）ステータスが使用可能である必要があります。

  システムレベルのステータスについて詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。
