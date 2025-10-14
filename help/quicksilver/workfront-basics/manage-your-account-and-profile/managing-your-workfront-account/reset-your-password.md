---
product-area: user-management
navigation-topic: manage-your-workfront-account
title: パスワードをリセット
description: ' [!DNL Adobe Workfront]  パスワードをリセットできます。重要なセキュリティ対策として、これを定期的に行うことをお勧めします。'
author: Courtney
feature: Get Started with Workfront
exl-id: 571cd77d-4f63-40c2-8a21-9646e924e75e
source-git-commit: 1a81c1becfc0866b92dbd1358af23671e5302266
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 68%

---

# パスワードをリセット

{{important-not-on-aec}}

[!DNL Adobe Workfront] パスワードをリセットできます。重要なセキュリティ対策として、これを定期的に行うことをお勧めします。

>[!NOTE]
>
>[システムセキュリティの環境設定の設定](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)および[認証用のパスワードポリシーの設定](../../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)で説明されるように、[!DNL Workfront] 管理者は、カスタムパスワード制限を設定できます。
>
><!-- [!DNL Workfront] administrator can also reset your password in an Enhanced Authentication enabled environment. For more information, see [Reset a user's password with Enhanced Authentication](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-user-password-eauth.md).-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>投稿者以上</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>リクエスト以上</p></li>
         </ul>
   </td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Adobe Workfront] でパスワードをリセットする

{{step1-click-profile-pic}}

![メインメニューを開き、ユーザー名を選択します。](assets/main-menu-options-350x481.png)

1. **[!UICONTROL その他メニュー]**![&#x200B; その他アイコン &#x200B;](assets/more-icon.png) をクリックしてから、**[!UICONTROL 編集]** をクリックします。

1. **[!UICONTROL 個人情報]** の下に表示される **[!UICONTROL ユーザーの編集]** ボックスで、[**[!UICONTROL パスワードの変更]**] をクリックします。

   ![[ パスワードの変更 ] をクリック &#x200B;](assets/edit-user-change-password.png)

   組織が [!DNL Workfront] を SSO ソリューションと統合している場合、「**[!UICONTROL パスワードを変更]**」をクリックすると、SSO システムを通じてパスワードをリセットするようにルーティングされる場合があります。 これにより、SSO パスワードがリセットされ、組織内での他のすべてのアプリケーションへのログインに影響します。

1. 古いパスワードを入力し、新しいパスワードを 2 回入力します。

   パスワードは 8 文字以上で、次の 2 種類の文字を含む必要があります。

   * 大文字
   * 小文字
   * 数字
   * 特殊文字（など） @ # $ %）

   パスワードの規則は、[!DNL Workfront] 管理者が指定する設定によって、これより厳しくなる場合があります。

1. **[!UICONTROL 保存]**&#x200B;をクリックします。
