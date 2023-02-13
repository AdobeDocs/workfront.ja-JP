---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: デフォルトの配達確認電子メール通知設定を構成する
description: Adobe Workfrontの校正ユーザーは、配達確認に対するコメントや決定を行ったときに、WorkfrontとWorkfrontの両方の配達確認から電子メール通知を受け取ることができます。 ユーザーが既にWorkfront配達確認から電子メール通知を受け取っている場合、Workfrontから送信される通知を無効にして、重複する通知電子メールが送信されないようにすることをお勧めします。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: ed97b8a6-54db-42f8-afee-d76c2df53a94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 1%

---

# デフォルトの配達確認電子メール通知設定を構成する

Adobe Workfrontの校正ユーザーは、配達確認に対するコメントや決定を行ったときに、WorkfrontとWorkfrontの両方の配達確認から電子メール通知を受け取ることができます。 ユーザーが既にWorkfront配達確認から電子メール通知を受け取っている場合、Workfrontから送信される通知を無効にして、重複する通知電子メールが送信されないようにすることをお勧めします。

Workfront Proof から送信される通知設定について詳しくは、 [Workfront Proof での電子メール通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront管理者である。 Workfront管理者について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## デフォルトの配達確認電子メール通知設定を構成する

Workfrontから送信される配達確認の E メール通知を設定するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **電子メール**&#x200B;を選択し、「 **レビューと承認**.

1. 内 **Workfrontの配達確認通知** 「配達確認にコメントが付けられたらWorkfrontから E メールを送信する」オプションを有効または無効にするかどうかを決定します。

   * この設定を有効にすると、配達確認にコメントが加えられたときに、Workfrontから電子メールがユーザーに送信されます。
   * この設定を無効にした場合、配達確認に対するコメントが行われても、Workfrontから電子メールが送信されません。

1. 「**保存**」をクリックします。
