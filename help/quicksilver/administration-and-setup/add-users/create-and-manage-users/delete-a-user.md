---
title: ユーザーの削除
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 組織を離れたユーザーは Workfront から削除できますが、削除する代わりにディアクティベートすることをお勧めします。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 77%
---
# ユーザーの削除

>[!IMPORTANT]
>
>このページに記載されている手順は、Admin Consoleにオンボーディングされていない組織にのみ適用されます。 組織はAdobe Admin Consoleにオンボーディングされているため、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>  Adobe Admin Consoleでユーザーを削除する手順については、[ ユーザーを個別に管理](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html)する記事の「ユーザーを完全に削除する」セクションを参照するか、Adobe Admin Console管理者にお問い合わせください。

組織を離れたユーザーは、Adobe Workfront から削除することができます。

ユーザーの削除は、Adobe Admin Consoleを通じて実行する必要があります。 手順については、[ ユーザーを個別に管理](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html)の記事の「ユーザーを完全に削除する」の節を参照するか、Adobe Admin Console管理者にお問い合わせください。

>[!IMPORTANT]
>
>システムからユーザーを削除すると、そのユーザーに関連付けられていて、今後も保持したい情報も削除されます。 ユーザーを削除する代わりに非アクティブ化することをお勧めします。 詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>あなたはAdobe Admin Consoleの管理者でなければなりません。</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーの削除とディアクティベートの違い

ユーザーをディアクティベートすると、次のことが発生します。

* Workfront Proof コンポーネントが Workfront アカウントに関連付けられている場合は、Workfront と Workfront Proof の両方に対するユーザーライセンスが削除されます。 Workfront Proof について詳しくは、[Workfront Proof：記事インデックス](../../../workfront-proof/workfront-proof.md)を参照してください。
* ユーザーに作業を割り当てることができなくなります。
* ユーザーを更新に追加できなくなります。
* ユーザーをチームやグループに追加できなくなります。
* ユーザーにオブジェクトを共有できなくなります。
* 次のオブジェクトとの関連付けはそのまま残ります。

  * タスク、イシュー、プロジェクト、ポートフォリオ
  * ダッシュボード

    >[!NOTE]
    >
    >ユーザーをディアクティベートし、そのユーザーに関連付けられているレポートやダッシュボードを表示できなくなった場合は、「**このレポートを次のアクセス権で実行：**」フィールドを更新する必要がある場合があります。\
    >詳しくは、[ アクティベート解除されたユーザーが所有するレポートにアクセスできない理由を参照してください。](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) [ レポートに関するFAQ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)のセクション。

  * ドキュメント
  * アップデート
  * 時間

* ユーザーがチェックアウトしたドキュメントは、そのユーザーがディアクティベートされてもチェックアウトされたままになります。 再度チェックインできるのは、Workfront 管理者のみです。 ドキュメントのチェックアウトについて詳しくは、[ドキュメントのチェックアウト](../../../documents/managing-documents/check-out-documents.md)を参照してください。

ユーザーを削除すると、次のことが発生します。

* Workfront Proof コンポーネントが Workfront アカウントに関連付けられている場合は、Workfront と Workfront Proof の両方に対するユーザーライセンスが削除されます。 Workfront Proof について詳しくは、[Workfront Proof：記事インデックス](../../../workfront-proof/workfront-proof.md)を参照してください。
* ユーザーに作業を割り当てることができなくなります。
* ユーザーを更新に追加できなくなります。
* ユーザーをチームやグループに追加できなくなります。
* ユーザーにオブジェクトを共有できなくなります。
* ユーザーと次のオブジェクトの関連付けが削除されます。

  * タスク、イシュー、プロジェクト、ポートフォリオ
  * ダッシュボード

<!--

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

-->
* アップデート
* 時間

  >[!NOTE]
  >
  >これらのオブジェクトは Workfront に残りますが、オブジェクトの所有者は空になります。

* ユーザーがグローバルナビゲーションバーのドキュメントエリアでドキュメントをアップロードした場合、そのドキュメントも削除されます。
* ユーザーが自分の所有するドキュメントをチェックアウトし、（メインメニューからアクセスする）メインのドキュメントエリアにドキュメントがアップロードされた場合、そのドキュメントはユーザーと共に削除されます。 ドキュメントのチェックアウトについて詳しくは、[ドキュメントのチェックアウト](../../../documents/managing-documents/check-out-documents.md)を参照してください。

ユーザーの非アクティブ化について詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
