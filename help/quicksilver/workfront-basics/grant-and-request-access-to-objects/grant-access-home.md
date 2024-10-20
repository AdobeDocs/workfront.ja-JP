---
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
title: ホームエリアのオブジェクトに対するアクセスの許可
description: ユーザーは、Adobe Workfront 内のオブジェクトへのアクセス権をリクエストできます。アクセス権のリクエストについて詳しくは、オブジェクトへのアクセス権のリクエストを参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: e0a69ed5-57c3-47ac-bb7a-65495f93b3e3
source-git-commit: 7b3658e2f13ea75cd7ae09cb7c3486dfc4a0bdb3
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 97%

---

# ホームエリアのオブジェクトに対するアクセスの許可

ユーザーは、Adobe Workfront 内のオブジェクトへのアクセス権をリクエストできます。アクセス権のリクエストについて詳しくは、[オブジェクトへのアクセス権のリクエスト](../../workfront-basics/grant-and-request-access-to-objects/request-access.md)を参照してください。

オブジェクトの所有者は、ホームエリアからアイテムへのアクセス権を付与または拒否できます。

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to projects, tasks, issues, or documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, issues, or documents</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、タスク、イシュー、ドキュメントに対する表示以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシュー、またはドキュメントに対する表示以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ホームエリアのオブジェクトに対するアクセスの許可

1. Adobe Workfront の左上隅にある&#x200B;**ホーム**&#x200B;アイコン ![](assets/home-icon-30x29.png) をクリックします。

   >[!NOTE]
   >
   >Workfront 管理者が、環境内のホームアイコンに次の変更を加える場合があります。
   >
   >* 組織を説明するようにカスタマイズされた画像に置き換える。この場合、アイコンはこの記事に示すものとは異なる外観になります。
   >* リンクされたページを別のページに置き換える。この場合、ページの右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、「**ホーム**」をクリックします。

1. （条件付き）従来のホームエリアで、以下の操作を実行します。

   1. **作業リスト**&#x200B;から、「**承認**」で管理するアクセスリクエストを選択します。

   ![Screen_Shot_2018-07-02_at_11.35.29_AM.png](assets/screen-shot-2018-07-02-at-11.35.29-am-350x242.png)

   このリクエストは作業リストの右側に表示されます。

   1. 右上隅の「アクセス権を付与」のボタンをクリックします。\
      要求されたアクセスのタイプに応じて、ボタン名は変わります。例えば、要求者が表示アクセスを要求した場合、ボタンの表示は「**表示アクセスを許可**」になります。\
      ![Grant_Access_2.png](assets/grant-access-2-350x98.png)

   1. （オプション）要求されたものと異なるレベルのアクセスを許可するには、アクセスを許可のボタンの横にある矢印をクリックして新しいアクセスを選択し、**付与／権限レベル／アクセス**&#x200B;をクリックします。\
      アクセス権が付与されたことを確認するメッセージが表示されます。

   1. （オプション）アクセスを拒否するには、「**無視**」をクリックします。\
      アクセス権が拒否されたことを確認するメッセージが表示されます。

1. （条件付き）新しいホームエリアで、次の操作を実行します。

   1. **自分の承認** ウィジェットに移動して、さらにアクセスするためのリクエストを見つけ、「**アクセスの許可**」をクリックします。

      ![](assets/request-for-access-to-project-in-new-home-approvals-widget.png)

   1. （オプション）要求されたものと異なるレベルのアクセスを許可するには、アクセスを許可のボタンの左側にあるドロップダウンメニューをクリックして新しいアクセスを選択し、「**アクセスを許可**」をクリックします。

      アクセスリクエストが許可され、承認リクエストのリストから消えます。

   1. （オプション）アクセスを拒否するには、「**無視**」をクリックします。アクセスリクエストは許可されず、承認リクエストのリストから消えます。

## リクエストに対するメール通知の設定

アクセス権のリクエストに対して、メール通知を受信するかどうかを設定できます。Workfront 管理者はこの機能を無効にできます。詳しくは、[システムの全員に対するイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 「**環境設定**」をクリックするか、「環境設定」セクションまでスクロールします。
1. 「**次の場合にメールで通知**」ドロップダウンリストで、別のユーザーからアクセス権を要求されたときにメール通知を送るか送らないかに応じて、「**誰かが自分にアクセスを要求**」を選択または選択解除します。

1. 「**変更を保存**」をクリックします。
