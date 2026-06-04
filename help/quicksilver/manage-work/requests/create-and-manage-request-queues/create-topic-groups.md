---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: トピックグループを作成
description: トピックグループはリクエストキューに関連付けられています。 リクエストの性質に応じて、リクエストキューを複数のカテゴリにレイヤー化できます。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/7odH8kf-VPRXoOVlMEiX3dWFLTsDDuy-f4TJgHAUsk8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 466
ht-degree: 83%

---

# トピックグループを作成

<!-- Audited: 2/2024 -->

トピックグループはリクエストキューに関連付けられています。 トピックグループを使用すると、リクエストの性質に応じて、複数のカテゴリでリクエストキューをレイヤー化できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront プラン</p> </td> 
   <td>   
      <p>標準</p>
      <p>プラン</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> プロジェクトの管理権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## トピックグループの概要

例えば、マーケティングリクエストのリクエストキューがある場合、「Mother&#39;s Day Campaign」というトピックグループを作成し、「Digital Media」という第 2 レベルのトピックグループと、「Print Media」という追加の第 2 レベルのトピックグループを含めることができます。 次に、各トピックグループ内に複数のキュートピックを含めることができます。 例えば、「Banner Ad」と「Blog」を、「Digital Media」トピックグループのキュートピックとすることができます。

リクエストキューの作成方法について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

トピックグループを使用する場合は、次の点を考慮してください。

* 1 つのリクエストキュー内に、最大 10 層のトピックグループを作成できます。
* 1 つのトピックグループに関連付けることができるキュートピックの数に制限はありません。
* トピックグループはレポート可能なオブジェクトです。
* プロジェクト間でトピックグループを移動することはできません。

## トピックグループを作成

トピックグループは、キュートピックを作成する前に作成することをお勧めします。 ただし、トピックグループはキュートピックビルダー内で作成できます。 キュートピックの作成について詳しくは、[キュートピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

トピックグループを作成するには：

1. ヘルプリクエストキューとして公開したプロジェクトに移動します。\
   プロジェクトをヘルプリクエストキューとして公開する方法について詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

1. 左側のパネルで「**トピックグループ**」をクリックします。
1. 「**新規トピックグループ**」をクリックします。

   <!--   ![New topic group box](assets/new-topic-group-box-nwe-350x306.png) -->

1. 次の情報を指定します。

   * **名前**：この名前は、このリクエストキューにリクエストを送信するユーザーに表示されます。
   * **説明**：説明は、新しいリクエストの送信処理でトピックグループを選択する際に表示されます。
   * **トピックグループに追加**：新しいトピックグループを既存のトピックグループに追加するか、ヘルプリクエストキューとして公開されたプロジェクトに直接追加できます。

1. 「**保存**」をクリックします。\
   これにより、リクエストキューに新しいトピックグループが作成されます。 リクエストキューの下にある最初のドロップダウンメニューから、追加のカテゴリを選択できるようになりました。\
   リクエストの送信について詳しくは、[Adobe Workfront リクエストの作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。
1. 既存のトピックグループを編集するには、トピックグループリストからトピックグループを選択し、開いたウィンドウで詳細を編集します。 **保存**&#x200B;をクリックして変更を保存します。
