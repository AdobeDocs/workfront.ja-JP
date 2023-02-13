---
product-area: projects
navigation-topic: manage-issues
title: フィードバック待ちから進行中へ問題ステータスを自動的に更新
description: 問題のプライマリ連絡先は、フィールド（カスタムフィールドを含む）の更新またはコメントの追加によって問題を更新すると、問題のステータスが自動的に「処理中」に更新されます。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# フィードバック待ちから進行中へ問題ステータスを自動的に更新

問題のプライマリ連絡先は、フィールド（カスタムフィールドを含む）の更新またはコメントの追加によって問題を更新すると、問題のステータスが自動的に「処理中」に更新されます。

この自動ステータス変更を行うには、次の操作が必要です。

* 問題はリクエストキューを通じて入力する必要があります。

   リクエストキューの作成について詳しくは、 [リクエストキューの作成と管理](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) 」セクションに入力します。 リクエストの作成について詳しくは、 [Adobe Workfront要求の作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md).

* リクエストキュー内のキューの詳細には、次の設定が必要です。
   * **がリクエストをおこなうと、自動的にを付与します** が **Contribute へのアクセス**
   * **ステータスの変更** が「詳細設定」で選択されている場合は、

   ![[ キューの詳細 ] で [Contribute へのアクセス ] が表示され、[ ステータスの変更 ] が選択されています。](assets/queuedetails-contributeaccess-changestatus.png)

   キューの詳細について詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* 問題のステータスは「フィードバック待ち」になっている必要があります。
* システムレベルの問題に対しては、フィードバック待ち (AWF) ステータスが使用可能である必要があります。

   システムレベルのステータスについて詳しくは、 [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
