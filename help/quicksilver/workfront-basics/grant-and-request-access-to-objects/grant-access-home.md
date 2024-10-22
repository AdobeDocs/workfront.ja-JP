---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: ホームエリアのオブジェクトに対するアクセスの許可
description: ユーザーは、Adobe Workfront 内のオブジェクトへのアクセス権をリクエストできます。アクセス権のリクエストについて詳しくは、オブジェクトへのアクセス権のリクエストを参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 60%

---

# ホームエリアのオブジェクトに対するアクセスの許可

<!--Audited: 10/2024-->

ユーザーは、Adobe Workfront内のオブジェクトへのアクセスをリクエストできます。

アクセスのリクエストについて詳しくは、[ オブジェクトへのアクセスのリクエスト ](../../workfront-basics/grant-and-request-access-to-objects/request-access.md) を参照してください。

オブジェクトの所有者は、ホームエリアからアイテムへのアクセス権を付与または拒否できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準</p> 
   <p>現在：ワーク以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスク、イシュー、ドキュメントに対する表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシュー、またはドキュメントに対する表示以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ホームエリアのオブジェクトに対するアクセスの許可

1. 画面の右上隅にある **メインメニュー**![](assets/dots-main-menu.png) をクリックするか、左上隅にある **メインメニュー**![](assets/lines-main-menu.png) をクリックし（使用可能な場合）、**ホーム** をクリックします
または
Adobe Workfrontの左上隅にある **ホーム** アイコン ![](assets/home-icon-30x29.png) をクリックします。

   >[!NOTE]
   >
   >Workfront 管理者が、環境内のホームアイコンに次の変更を加える場合があります。
   >
   >* 組織を説明するようにカスタマイズされた画像に置き換える。この場合、アイコンはこの記事に示すものとは異なる外観になります。
   >* リンクされたページを別のページに置き換える。この場合、ページの右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、「**ホーム**」をクリックします。

1. 次の操作を実行します。

   1. **自分の承認** ウィジェットに移動して、さらにアクセスするためのリクエストを見つけ、「**アクセスを許可**」をクリックします。

      ![](assets/request-for-access-to-project-in-new-home-approvals-widget.png)

   1. （オプション）要求されたものと異なるレベルのアクセスを許可するには、アクセスを許可のボタンの左側にあるドロップダウンメニューをクリックして新しいアクセスを選択し、「**アクセスを許可**」をクリックします。

      アクセスリクエストが許可され、承認リクエストのリストから消えます。

1. （オプション）アクセスを拒否するには、「**無視**」をクリックします。アクセスリクエストは許可されず、承認リクエストのリストから消えます。

## アクセスリクエストのメール通知の設定

アクセス権のリクエストに対して、メール通知を受信するかどうかを設定できます。Workfront 管理者はこの機能を無効にできます。詳しくは、[システムの全員に対するイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

1. 次のいずれかの操作を行って、ユーザープロファイルに移動します。

   * 画面の右上隅にある **メインメニュー**![](assets/dots-main-menu.png) をクリックしてから、自分の名前をクリックします。
   * 右上隅のAdobe **メインメニュー**![](assets/adobe-blue-main-menu.png) をクリックし、**Workfront プロファイル** をクリックします（使用可能な場合）。

1. ヘッダーの名前の右 ![](assets/more-icon.png) にある **その他** メニューをクリックし、**編集** をクリックします。
1. 「**通知**」をクリックし、別のユーザーが自分からのアクセスを要求したときにメール通知を受け取るかどうかに応じて、「**必要なアクション**」セクションの **自分からアクセスを要求するユーザー** を選択または選択解除します。

   日別またはインスタントの通知を有効にできます。

1. 「**変更を保存**」をクリックします。

<!--1. (Conditional) From the legacy Home area, do the following: 
   
   1. In the **Work List**, select the access request you want to manage in the **Approvals** section.  

   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

   The request displays on the right of the Work List. 

   1. In the upper-right corner, click the grant access button.  
   Depending on the type of access requested, the button name changes. For example, if the requestor asks for View access, the button says **Grant View Access**.  
   ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

   1. (Optional) To grant a different level of access than requested, click the arrow next to the grant access button and select the new access, then click **Grant < Permission level > Access >**.  
   A message appears confirming access was granted.  
   
   1. (Optional) Click **Ignore** to deny access.  
   A message appears confirming access was ignored.-->
