---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 通知を生成せずにオブジェクトを共有する方法
description: オブジェクトを共有し、この変更に関する通知が送信されないようにする方法を説明します。 これは、オブジェクトを一括共有する場合に特に便利です。
author: Alina
feature: Get Started with Workfront
exl-id: 02106282-addb-4bdd-82d2-9da5a5f6a687
TQID: https://experienceleague.adobe.com/zhNlFwg-1UuNKXxqIj-H62rGdewhbqKHLz4NbzkEqP8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 577
ht-degree: 21%

---

# 通知を生成せずにオブジェクトを共有する方法

<!--Audited: 12/2024-->

Adobe Workfrontでオブジェクトを共有すると、そのオブジェクトを共有しているユーザーには、共有に関するメール通知が届きます。

誰かがオブジェクトを共有したときにメール通知を受け取ることは、この変更を認識しておくことが重要です。 しかし、通知が多すぎると、オーディエンスにとっては混乱しがちです。 一度に多数のオブジェクトをユーザーと共有する場合は、通知を一時的に無効にすると、混乱を避けることができます。

次の設定を同時に有効にすると、ユーザーにメール通知が送信されます。

* システム レベルまたはグループ レベルで、次のイベント通知の一方または両方を有効にします。

   * ユーザー宛オブジェクトの共有
   * グループへのオブジェクト共有は、システムレベルまたはグループレベルで有効になります。
* ユーザーのプロファイルで、次のメール通知の一方または両方が有効になっています。

   * 誰かが私とオブジェクトを共有しました
   * 誰かがマイチームとオブジェクトを共有しました

複数のユーザーと（一括で）複数のオブジェクトを共有する必要があるものの、この変更に関するメール通知を受信したくない場合は、次の操作を行います。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>共有するオブジェクトに対する表示以上の権限</p>
   <p>ユーザーへのアクセスの編集</p>
   <p><b>メモ</b></p>
   <p> システムまたはグループのイベント通知のステータスを確認するには、システムまたはグループ管理者である必要があります</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>共有するオブジェクトに対する表示またはそれ以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 通知を生成せずにオブジェクトを共有

1. 次の&#x200B;**イベント通知**&#x200B;がシステムレベルまたはグループレベルで有効になっていることを確認します。

   * **ユーザーへのオブジェクト共有**
   * **グループへのオブジェクト共有は、システム レベルまたはグループ レベルで有効になっています**。

   詳しくは、[システムの全ユーザーに対するイベント通知の設定](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

   これらのイベント通知が有効になっていない場合、オブジェクトの共有に関する通知はユーザーに送信されません。 どちらか一方または両方が有効になっている場合は、次の手順に進みます。

{{step-1-to-users}}

1. リストで複数のユーザーを選択し、**通知**/**その他**&#x200B;をクリックします。
1. 次の通知の1つまたは両方を無効にします（システムまたはグループレベルで有効な通知に応じて）。

   * **誰かが自分とオブジェクトを共有しています**
   * **誰かが自分のチームとオブジェクトを共有しています**

   選択したすべてのユーザーに、これらの通知が選択されていることを確認してから無効にします。 これにより、オブジェクトを共有した後で、すべてのオブジェクトに対して一括で再度有効にすることができます。

1. 「**変更を保存**」をクリックします。
1. 共有するオブジェクトのリストに移動してオブジェクトを選択し、リストの上部にある「**共有**」アイコンをクリックします。

   オブジェクトの一括共有について詳しくは、[ オブジェクトの共有](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

1. 通知を無効にしたユーザーのリストに戻り、同じユーザーを選択します。
1. リストで同じユーザーを選択し、**通知**/**その他**&#x200B;をクリックします。
1. 次のいずれかの通知または両方を有効にします（システムレベルまたはグループレベルで有効な通知に応じて異なります）。

   * **誰かが自分とオブジェクトを共有しています**
   * **誰かが自分のチームとオブジェクトを共有しています**

1. 「**変更を保存**」をクリックします。

   オブジェクトは選択したユーザーと共有され、この変更に関するメール通知を受け取ったユーザーはいませんでした。
