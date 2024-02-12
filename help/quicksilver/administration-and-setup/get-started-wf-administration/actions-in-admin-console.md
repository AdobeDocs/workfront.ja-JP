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
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 86%

---

# プラットフォームベースの管理上の違い（Adobe Workfront／Adobe ビジネスプラットフォーム）

組織が Adobe Business Platform にオンボーディングされている場合、ユーザーは Adobe Business Platform を使用して Adobe Workfront にアクセスします。つまり、次のようになります。

* システム管理者は、 Adobe Admin Consoleを使用して作成されます
* シングルサインオン（SSO）は、Workfront を通じてではなく、Adobe Business Platform を通じて処理される

Adobe Workfront 管理者の管理上の責任と手順は、組織が Adobe Business Platform にオンボーディングされているかどうかで異なります。この記事では、処理方法を説明し、WorkfrontとAdobe Admin Consoleの両方の手順へのリンクを示します。

## ユーザー



>[!NOTE]
>
>システム管理者以外のユーザーを直接Workfrontに追加することをお勧めします。 Adobe Admin Consoleでユーザーを追加することはできますが、Workfrontでユーザーを追加すると、ユーザーの作成時にアクセスレベルを設定できるので、時間を節約できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクション</th> 
   <th>Workfront での手順の参照先</th> 
   <th>AdobeAdmin Console での手順の参照先</th> 
  </tr> 
 </thead> 
 <tbody> <!--
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
  --> 
  <tr> 
   <td role="rowheader">ユーザーに管理者アクセス権を付与</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html">ユーザーを個別に管理</a>の「ユーザーの詳細の編集」の節</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront にユーザーを追加</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">ユーザーを追加</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Adobe Admin Console でのユーザー管理</a> </p> </li> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html">ユーザーを個別に管理</a>の「ユーザーの追加」の節</p> </li> 
    </ul> </td> 
  </tr> <!--
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
  --> 
  <tr> 
   <td role="rowheader">ユーザーの非アクティブ化</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html">ユーザーを個別に管理</a>の「ユーザーの削除」の節</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザーを削除</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md" class="MCXref xref">ユーザーの削除</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/manage-directory-users.html">ディレクトリユーザーを管理</a>の「ユーザーを完全に削除」の節
     </p><p>メモ：[!DNL Adobe Admin Console] からユーザーを削除すると、ユーザーは [!DNL Workfront] で非アクティブ化されますが、[!DNL Workfront] からは削除されません。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザープロファイルを編集</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html">ユーザーを個別に管理</a>の「ユーザーの詳細の編集」の節</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザープロファイルを一括編集</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md" class="MCXref xref">ユーザープロファイルを一括編集</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html">CSV の一括アップロード</a>の「ユーザーの詳細の編集」の節</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザーの読み込み </td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">ユーザーの読み込み</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/jp/enterprise/using/bulk-upload-users.html">CSV の一括アップロード</a>の「ユーザーの追加」の節</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">別のユーザーとしてのログイン</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md" class="MCXref xref">別のユーザーとしてのログイン</a> </p> </li> 
    </ul> </td> 
   <td>利用不可</td> 
  </tr> 
  <tr> 
   <td role="rowheader">SAML 証明書を更新</td> 
   <td> 
    <ul> 
     <li> <p><a href="../../administration-and-setup/manage-workfront/security/renew-wf-saml-2-certificate.md" class="MCXref xref">Adobe Workfront SAML 2.0 メタデータ証明書を更新</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="https://helpx.adobe.com/enterprise/kb/tshoot-fed-id.html?lang=jp">Federated ID のトラブルシューティング</a>内の「SAML 応答のデジタル署名が検証されませんでした...」の節</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## SSO（シングルサインオン）

Adobe Business Platform は、ユーザーのシングルサインオン（SSO）を制御するので、次のアクションと機能は、Adobe Business Platform を通じて自動的に処理されます。組織がまだ Adobe Business Platform にオンボーディングされていない場合、Workfront でこれらのアクションを実行する必要があります。


* [SAML 2.0 で Adobe Workfront を設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)
* [ADFS を使用した SAML 2.0 で Adobe Workfront を設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)
* [Adobe Workfront でシングルサインオンを無効化](../../administration-and-setup/add-users/single-sign-on/deactivate-sso.md)
* [ID プロバイダーの SAML 2.0 メタデータを更新](../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)
* [シングルサインオンのユーザーを更新](../../administration-and-setup/add-users/single-sign-on/update-users-sso.md)
* [認証用のパスワードポリシーを設定](../../administration-and-setup/manage-workfront/security/configure-password-policies-authentication.md)
* [システムセキュリティの環境設定を指定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)
