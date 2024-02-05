---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 組織の Adobe Admin Console 導入の準備
description: Adobe Workfront は Adobe 製品なので、Adobe Admin Console からアクセスできます。これにより、ユーザーのための他の Adobe アカウントや製品と Workfront を一か所で管理できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 75%

---

# 組織の Adobe Admin Console 導入の準備

<!-- Audited: 12/2023 -->

Adobe Workfront は Adobe 製品なので、Adobe Admin Console からアクセスできます。これにより、ユーザーのための他の Adobe アカウントや製品と Workfront を一か所で管理できます。

Workfront のすべてのお客様が、最終的に Adobe Admin Console に移行します。組織がAdobe Admin Consoleに移行すると、Workfront認証はコンソールで管理されます。 この移行をより早く準備して実行することで、作業管理の効率化の基礎が築かれ、将来の迅速なイノベーションに備えることができます。

Adobe Admin Console の概要については、[Admin Console の概要](https://helpx.adobe.com/jp/enterprise/using/admin-console.html)を参照してください。

## 移行チェックリスト

組織がAdobe Admin Consoleに移行できるようにするには、次の操作を実行する必要があります。

1. Workfront を追加する Adobe Admin Console を指定します。

   * 組織に既存の Adobe Admin Console がない場合や既存の Adobe Admin Console を使用しない場合は、Workfront サポートが新しい Adobe Admin Console の作成をサポートします。

   * 複数のAdobeAdmin Consoleがあり、Workfrontの追加先として最も適切なものが不明な場合は、Workfrontサポートにお問い合わせください。

1. 既存の Adobe Admin Console を使用するか、新しい Adobe Admin Console を作成するかについて、Workfront サポートと一緒に決定できます。

1. Adobe Admin Console で Identity Management を設定します。

   >[!IMPORTANT]
   >
   >シングルサインオン（SSO）や非 SSO などの認証設定について、Workfront サポートおよび組織の IT チームに伝えられるようにしておきます。

   手順については、 [Adobe Admin Consoleのデプロイメントガイド](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. （条件付き）シングルサインオンを使用する場合、新しいAdobe Admin Consoleを既存の SSO プロバイダーに接続します。

   詳しい情報と手順については、[ID の設定](https://helpx.adobe.com/enterprise/using/set-up-identity.html)を参照してください。

   >[!NOTE]
   >
   >組織がシングルサインオンを使用していない場合、Adobe Admin Console に移行したユーザーには、自分のアカウントとパスワードを作成するためのメールが送信されます。

1. ユーザーのメールアドレスを移行する準備ができていることを、次の手順で確認します。

   1. Workfrontから重複した E メールを削除します。

      手順については、 [Workfrontインスタンスの既存ユーザーの電子メールアドレスを更新する](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [重複するユーザーを防ぐ](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      組織内に重複するメールアドレスがある場合は、最新の `lastLoginDate` を持つメールアドレスで表されるユーザーが、Adobe Admin Console の組織に移動されます。そのメールアドレスを持つ他のユーザーは、ディアクティベートされます。

      >[!NOTE]
      >
      >特定の電子メールアドレスを持つユーザーは 1 人だけアクティブにできるので、現在アクティブなユーザーと同じ電子メールアドレスを持つ別のユーザーをアクティブにする必要がある場合は、非アクティブなユーザーをアクティブにする前に、現在アクティブなユーザーを非アクティブにします。

   1. （条件付き）カスタム API 統合を利用している場合は、アクセスできる有効なメールアドレスをそれらのユーザーが持っていることを確認します。

   1. （オプション）Workfront へのアクセスが不要になったユーザーはディアクティベートして、Adobe Admin Console に追加されないようにすることをお勧めします。

   >[!IMPORTANT]
   >
   >ユーザーのメールに関するこれらの操作は、組織が Adobe Admin Console への移行を開始する前に完了する必要があります。

1. （オプション）OAuth2 を使用するように、すべてのカスタム統合を更新します。

   OAuth2 統合の設定手順については、[Workfront 統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

   >[!NOTE]
   >
   >この手順はオプションですが、他の形式の API 認証や承認が今後非推奨となるため、実行することを強くお勧めします。

Adobe Admin Console と Workfront を連携させたら、Adobe Admin Console でユーザーを管理できるようになります。

詳しくは、[Adobe Admin Console でのユーザーの管理](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください。

その他のアクションは、組織が Adobe Admin Console にオンボーディングされているかどうかによって異なります。それらのアクションのリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront / Adobe Business Platform）](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。
