---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Adobe Workfrontドメインの変更
description: Adobe Workfrontの管理者で、認証済みのWorkfrontサポート担当者は、Workfrontサポートチームに支援を依頼して、組織のWorkfrontドメインを変更することができます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: b9e088a0cdb32f3e8c565ea17f4613dda104bd7b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Adobe Workfrontドメインの変更

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Workfrontドメインを変更することはできません。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfrontの管理者で、認証済みのWorkfrontサポート担当者は、Workfrontサポートチームに支援を依頼して、組織のWorkfrontドメインを変更することができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ドメインの変更をリクエスト

1. 次をクリック： **サポート** 「 Workfront One 」ページの「 」タブで、サポートケースの作成を開始します。
1. 内 **説明** ボックスに、新しいドメインを追加し、新しいドメインを有効にする期間を追加します。
1. サポートケースのボックスへの入力を完了し、「 **送信**.

また、Workfrontサポートに連絡して、ドメインの変更に関するヘルプを受け取ることもできます。

## SSO のお客様の場合は、新しいドメインを更新します。

会社が SSO を使用している場合は、Workfrontドメインを変更した後に、次の手順を実行する必要があります。

>[!NOTE]
>
>組織のWorkfrontインスタンスで「Adobe IMS」が有効になっている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のサイドバーで、 **システム** > **顧客情報** お客様のドメインが顧客情報ページで更新されていることを確認します。

1. 左側のサイドバーで、 **システム** > **シングルサインオン (SSO)**.

1. クリック **SAML 2.0 メタデータのダウンロード**.
1. ファイルがダウンロードされたら、ファイルを開き、次の点を確認します。

   1. **entityID** が新しいドメインを指している。
   1. 内のすべての場所 **`<md:AssertionConsumerService>`** 新しいドメインを指します。

1. ダウンロードしたメタデータファイルを ID プロバイダーに提供し、プロバイダーが最後に更新できるようにします。
1. 組織で使用されるすべてのWorkfront統合で、ドメインが更新されていることを確認します。
