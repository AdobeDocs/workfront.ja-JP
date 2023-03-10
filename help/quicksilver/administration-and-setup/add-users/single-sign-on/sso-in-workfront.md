---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfrontでのシングルサインオンの概要
description: Workfrontは、Workfrontを既存の会社の SSO ソリューションと簡単に統合できる、一元的に管理されたシングルサインオン (SSO) 設定を提供します。 この設定は、簡単に設定および管理でき、OnDemand と OnPremise の両方のエンタープライズユーザーが利用できます。
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 87f1b6c0-6b74-4eac-87cd-899b1c74af25
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Adobe Workfrontでのシングルサインオンの概要

{{important-admin-console-onboard}}


Workfrontは、Workfrontを既存の会社の SSO ソリューションと簡単に統合できる、一元的に管理されたシングルサインオン (SSO) 設定を提供します。 この設定は、簡単に設定および管理でき、OnDemand と OnPremise の両方のエンタープライズユーザーが利用できます。

Workfrontで SSO 機能を使用するには、組織で SSO アプリケーションを設定する必要があります。 その後、Workfrontを設定して、SSO ソリューションと通信できるようにします。

フェデレーテッドソリューションを使用すると、ユーザーは、一元化されたログインポータルにユーザー名とパスワードを入力して、すべてのアプリケーションにログインできます。

![](assets/overview-sso-wf.png)


## ファイアウォールを設定

SSO ソリューションを使用する場合、Workfrontは指定されたポートでサーバーへの接続を開始します。

Workfront On-demand を購読し、特定のベンダーへのアクセスのみを許可するようにファイアウォールまたはメールサーバーを設定した場合は、特定のWorkfront IP アドレスをファイアウォールに追加する必要がありま許可リストす。 詳しくは、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## シングルサインオンの設定

Workfrontは、次の SSO ソリューションと統合されます。

* SAML 2.0 をサポートするフェデレーテッドソリューション

   Workfrontと SAML 2.0 の統合について詳しくは、 [SAML 2.0 でのAdobe Workfrontの設定](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

* ADFS を使用した SAML 2.0 をサポートするフェデレーテッドソリューション

   ADFS を使用したWorkfrontと SAML 2.0 の統合について詳しくは、 [ADFS を使用した SAML 2.0 でのAdobe Workfrontの設定](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
