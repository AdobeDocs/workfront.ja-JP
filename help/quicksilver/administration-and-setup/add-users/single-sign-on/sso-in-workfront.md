---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfrontでのシングルサインオンの概要
description: Workfront は、Workfront を既存の会社の SSO ソリューションと簡単に統合できる、一元的に管理されたシングルサインオン（SSO）設定を提供します。 この設定は、簡単に設定および管理でき、OnDemand と OnPremise の両方のエンタープライズユーザーが利用できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
TQID: https://experienceleague.adobe.com/3Eti-Ucz19uff3H03Go6JuU5hhiTstjg4dbWPLMDl3s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 96%

---

# Adobe Workfront でのシングルサインオンの概要

<!--Audited: 12/2023-->

{{important-admin-console-onboard}}


Workfront は、Workfront を既存の会社の SSO ソリューションと統合できる、一元的に管理されたシングルサインオン（SSO）設定を提供します。 この設定は、OnDemand と OnPremise の両方のエンタープライズのお客様が利用できます。

Workfront で SSO 機能を使用するには、組織で SSO アプリケーションを設定する必要があります。 その後、Workfront を設定して、SSO ソリューションと通信できるようにします。

連合型ソリューションを使用すると、ユーザーは、一元化されたログインポータルにユーザー名とパスワードを入力して、すべてのアプリケーションにログインできます。

![SSO フェデレーテッド &#x200B;](assets/overview-sso-wf-fed-only.png)


## ファイアウォールの設定

SSO ソリューションを使用する場合、Workfront は指定されたポートでサーバーへの接続を開始します。

ファイアウォールやメールサーバーが、特定のベンダーへのアクセスのみを許可するように設定されている場合は、特定の Workfront IP アドレスをファイアウォールの許可リストに追加する必要があります。 詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## シングルサインオンの設定

Workfront は、次の SSO ソリューションと統合されています。

* SAML 2.0 をサポートする連合型ソリューション

  Workfrontと SAML 2.0 の統合について詳しくは、[SAML 2.0 での Adobe Workfront の設定](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)を参照してください。

* ADFS を使用した SAML 2.0 をサポートする連合型ソリューション

  ADFS を使用した Workfrontと SAML 2.0 の統合について詳しくは、[ADFS を使用した SAML 2.0 での Adobe Workfront の設定](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)を参照してください。
