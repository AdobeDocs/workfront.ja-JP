---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 組織をAdobe Admin Consoleにオンボーディングする準備
description: Adobe WorkfrontはAdobe製品なので、Adobe Admin Consoleからアクセスできます。 これにより、Workfrontを、その他のAdobeアカウントや製品と共に、一元的に管理できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# 組織をAdobe Admin Consoleにオンボーディングする準備

<!-- Audited: 12/2023 -->

Adobe WorkfrontはAdobe製品なので、Adobe Admin Consoleからアクセスできます。 これにより、Workfrontを、その他のAdobeアカウントや製品と共に、一元的に管理できます。

Workfrontのすべてのお客様は、最終的にAdobe Admin Consoleに移動されます。 組織がAdobe Admin Consoleに移行すると、Workfront認証はコンソールで管理されます。 この移行の準備と実行は、作業管理の効率化の基盤を早く構築し、将来の迅速なイノベーションのために組織を位置づけます。

Adobe Admin Consoleの概要については、 [Admin Consoleの概要](https://helpx.adobe.com/jp/enterprise/using/admin-console.html).

## 移行チェックリスト

組織がAdobe Admin Consoleに移行できるようにするには、次の操作を実行する必要があります。

1. Workfrontを追加する目的のAdobe Admin Consoleを特定します。

   * 組織が既存のAdobe Admin Consoleを持っていない場合、または既存のAdobe Admin Consoleを使用しない場合、Workfrontサポートが新しいの作成をサポートします。

   * 複数のAdobeAdmin Consoleがあり、Workfrontの追加先として最も適切なものが不明な場合は、Workfrontサポートにお問い合わせください。

1. 既存のAdobe Admin Consoleを使用することをWorkfrontサポートで確認するか、新しく作成してもらいます。

1. Adobe Admin Consoleで ID 管理を設定します。

   >[!IMPORTANT]
   >
   >シングルサインオン (SSO) や非 SSO などの認証設定について、Workfrontサポートおよび IT チームと話す準備をしてください。

   手順については、 [Adobe Admin Consoleのデプロイメントガイド](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. （条件付き）シングルサインオンを使用する場合、新しいAdobe Admin Consoleを既存の SSO プロバイダーに接続します。

   詳しい情報と手順については、 [ID の設定](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >組織がシングルサインオンを使用していない場合、Adobe Admin Consoleに移行されたユーザーには、自分のアカウントとパスワードを作成するための電子メールが送信されます。

1. ユーザーの E メールアドレスを移行する準備が整っていることを確認します。

   1. Workfrontから重複した E メールを削除します。

      手順については、 [Workfrontインスタンスの既存ユーザーの電子メールアドレスを更新する](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [重複するユーザーを防ぐ](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      組織内に重複した E メールアドレスがある場合、そのユーザーは最新の E メールアドレスで表されます `lastLoginDate` がAdobe Admin Console組織に移動されます。 その電子メールアドレスを持つ他のユーザーは、無効化されます。

      >[!NOTE]
      >
      >特定の電子メールアドレスを持つユーザーは 1 人だけアクティブにできるので、現在アクティブなユーザーと同じ電子メールアドレスを持つ別のユーザーをアクティブにする必要がある場合は、非アクティブなユーザーをアクティブにする前に、現在アクティブなユーザーを非アクティブにします。

   1. （条件付き）カスタム API 統合を利用している場合、それらのユーザーがアクセスできる有効な電子メールアドレスを持っていることを確認します。

   1. （オプション）Workfrontへのアクセスを不要にしたユーザーは、Adobe Admin Consoleに追加されなくなった後、非アクティブ化することをお勧めします。

   >[!IMPORTANT]
   >
   >ユーザー電子メールに関するこれらの操作は、組織がAdobe Admin Consoleへの移行を開始する前に実行する必要があります。

1. （オプション）OAuth2 を使用するように、すべてのカスタム統合を更新します。

   OAuth2 統合の設定手順については、 [Workfront統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >この手順はオプションですが、他の形式の API 認証および承認は今後非推奨となるので、強くお勧めします。

Adobe Admin ConsoleとWorkfrontの連携を設定したら、それを使用してユーザーを管理できます。

詳しくは、 [Adobe Admin Consoleでのユーザー管理](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なるその他のアクションのリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
