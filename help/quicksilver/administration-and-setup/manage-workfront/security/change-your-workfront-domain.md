---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe Workfront ドメインを変更
description: Adobe Workfront の管理者であり、認定 Workfront サポート担当者である場合は、組織の Workfront ドメインを変更するために、Workfront サポートチームにヘルプをリクエストできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: 22ea9b623d7bc7b216511538cf88e4d020529bd3
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 98%

---

# Adobe Workfront ドメインを変更

>[!IMPORTANT]
>
>このページで説明する手順は、Admin Console にまだ登録されていない組織にのみ適用されます。組織が Adobe Admin Console にオンボーディング済みの場合、Workfront ドメインを変更することはできません。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについて詳しくは、[プラットフォームベースの管理上の違い（Adobe Workfront/Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

Adobe Workfront の管理者であり、認定 Workfront サポート担当者である場合は、組織の Workfront ドメインを変更するために、Workfront サポートチームにヘルプをリクエストできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ドメインの変更をリクエスト

1. Experience Leagueでサポートチケットを作成し始めます。
1. 「**説明**」ボックスに、必要な新しいドメインと、新しいドメインを稼動させる時期を記入します。
1. サポートケースのボックスへの記入を完了したら、「**送信**」をクリックします。

また、Workfront サポートに連絡して、ドメインの変更に関するヘルプを受けることもできます。

## 新しいドメインを更新（SSO のお客様の場合）

会社が SSO を使用している場合は、Workfront ドメインを変更した後に、次の手順を実行する必要があります。

>[!NOTE]
>
>組織の Workfront インスタンスが Adobe IMS によって有効化されている場合は使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 左側のサイドバーで、**システム**／**顧客情報**&#x200B;をクリックし、お客様のドメインが顧客情報ページで更新されていることを確認します。

1. 左側のサイドバーで、**システム**／**シングルサインオン（SSO）**&#x200B;をクリックします。

1. 「**SAML 2.0 メタデータのダウンロード**」をクリックします。
1. ファイルがダウンロードされたら、ファイルを開き、次の点を確認します。

   1. **entityID** が新しいドメインを指している。
   1. **`<md:AssertionConsumerService>`** 内のすべての場所が新しいドメインを指している。

1. ダウンロードしたメタデータファイルを ID プロバイダーに提供し、プロバイダー側で更新できるようにします。
1. 組織で使用されるすべての Workfront 統合で、ドメインが更新されていることを確認します。
