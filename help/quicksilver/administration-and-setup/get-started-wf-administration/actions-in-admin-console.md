---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: プラットフォームベースの管理上の違い（Adobe Workfront／Adobe ビジネスプラットフォーム）
description: 組織が Adobe Business Platform にオンボーディングされている場合、ユーザーは Adobe Business Platform を使用して Adobe Workfront にアクセスします。つまり、ユーザー管理は主に Adobe Admin Console を通じて行われ、シングルサインオン（SSO）は Workfront を通じてではなく Adobe Business Platform を通じて処理されます。Adobe Workfront 管理者の管理上の責任と手順は、組織が Adobe Business Platform にオンボーディングされているかどうかで異なります。この記事では、別々の方法で処理する必要がある手順と、Workfront と Adobe Admin Console の両方の手順へのリンクを示します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a84a5a8d-7c2a-4b51-a614-91a6dc9aa4ed
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 56%

---

# プラットフォームベースの管理上の違い（Adobe Workfront／Adobe ビジネスプラットフォーム）

Adobe Workfront管理者の場合、管理上の責任と手順は、組織がAdobeビジネスプラットフォームにオンボーディングされているかどうかによって異なる場合があります。 この記事では、処理方法を説明し、WorkfrontとAdobe Admin Consoleの両方の手順へのリンクを示します。

組織が Adobe Business Platform にオンボーディングされている場合、ユーザーは Adobe Business Platform を使用して Adobe Workfront にアクセスします。つまり、次のようになります。

* システム管理者は、 Adobe Admin Consoleを使用して作成されます
* SAML 証明書の更新は、Adobe Admin Consoleで処理されます。
* シングルサインオン (SSO) は、Workfrontを通じて処理されるのではなく、Adobeビジネスプラットフォームを通じて処理されます

## Adobe Admin ConsoleでのWorkfrontシステム管理者の作成

>[!NOTE]
>
>システム管理者以外のユーザーを直接Workfrontに追加することをお勧めします。 Adobe Admin Consoleでユーザーを追加することはできますが、Workfrontでユーザーを追加すると、ユーザーの作成時にアクセスレベルを設定できるので、時間を節約できます。

Workfrontシステム管理者の作成手順については、 [Adobe Admin Consoleでのシステム管理者の管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Action</th> 
   <th>For instructions in Workfront, see</th> 
   <th>For instructions in the Adobe Admin console, see</th> 
  </tr> 
 </thead> 
 <tbody> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">View information about access levels and licenses for your users</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md" class="MCXref xref">List your users' access levels and licenses</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p>The section "View user list" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Grant a user admin access</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Add a user to Adobe Workfront</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
     <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Add a user to Adobe Workfront Fusion</td> 
    <td> 
     <ul> 
      <li> <p><a href="../../workfront-fusion/organizations/add-user-to-an-organization.md" class="MCXref xref">Add a user to an organization in Adobe Workfront Fusion</a> </p> </li> 
     </ul> </td> 
    <td> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a> </p> </li> 
      <li> <p>The section "Add users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
     </ul> </td> 
   </tr>
  <tr> 
   <td role="rowheader">Deactivate a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Remove users" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Delete a user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">Delete users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Permanently delete users" in <a href="https://helpx.adobe.com/enterprise/using/manage-directory-users.html">Manage directory users</a>
     </p><p>Note: Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Edit a user profile</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in in <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bulk edit user profiles</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">Edit user profiles in bulk</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Edit user details" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Import users </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Import users</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "Add users" in <a href="https://helpx.adobe.com/enterprise/using/bulk-upload-users.html">Bulk CSV upload</a></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log in as another user</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">Log in as another user</a> </p> </li> 
    </ul> </td> 
   <td>Not available</td> 
  </tr> 
  <tr> 
    -->

## SAML 証明書の更新

Adobe Admin Consoleで SAML 証明書を更新する手順については、 [トラブルシューティングFederated ID](https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html?lang=jp)

<!--

   <td role="rowheader">Renew SAML certificate</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Renew the Adobe Workfront SAML 2.0 metadata certificate</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>The section "The digital signature in the SAML response did not validate..." in <a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html">Troubleshooting Federated ID</a></p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

-->

## SSO（シングルサインオン）

Adobe Business Platform は、ユーザーのシングルサインオン（SSO）を制御するので、次のアクションと機能は、Adobe Business Platform を通じて自動的に処理されます。組織がまだ Adobe Business Platform にオンボーディングされていない場合、Workfront でこれらのアクションを実行する必要があります。


* [SAML 2.0 で Adobe Workfront を設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [ADFS を使用した SAML 2.0 で Adobe Workfront を設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Adobe Workfront でシングルサインオンを無効化](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [ID プロバイダーの SAML 2.0 メタデータを更新](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [シングルサインオンのユーザーを更新](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [認証用のパスワードポリシーを設定](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [システムセキュリティの環境設定を指定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
