---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: ユーザーのプルーフアクセスの設定
description: Adobe Workfront 管理者または Workfront Proof 管理者は、Workfront と Workfront Proof でプルーフを作成および表示するためのユーザーのアクセス権を設定できます。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 98%
---
# ユーザーのプルーフアクセスの設定

Adobe Workfront 管理者または Workfront Proof 管理者は、Workfront と Workfront Proof でプルーフを作成および表示するためのユーザーのアクセス権を設定できます。

基本プルーフと統合プルーフで利用可能なプルーフ機能について詳しくは、[Workfront でのプルーフ機能へのアクセス](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront 管理者または Workfront Proof 管理者である必要があります。 Workfront 管理者について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## Workfront のメインメニューから Workfront Proof へのアクセスをすべてのユーザーに設定 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

デフォルトでは、[Adobe Workfront から Workfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) で説明されているように、Workfront 内の管理者権限を持つユーザーのみが Workfront Proof にアクセスできます。

Workfront サポートに連絡してリクエストを送信することで、すべてのユーザーに Workfront メインメニュー内の Workfront Proof ボタンへのアクセスを許可できます。

>[!IMPORTANT]
>
> すべての Workfront ユーザーが Workfront グローバルナビゲーションバーから直接 Workfront Proof にアクセスできるようにする場合は、各ユーザーの権限プロファイルが Workfront 内のユーザーのアクセスレベルを超えるアクセスを提供しないようにしてください。 これにより、ユーザーは Workfront 内でアクセスできない Workfront Proof 内のプルーフにアクセスできなくなります。 詳しくは、[ユーザーのプルーフを有効または無効にする（従来のプランのみ）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)を参照してください。

## デスクトッププルーフビューアーへのユーザーアクセスを設定

組織内のユーザーがインタラクティブコンテンツのレビューに web プルーフビューアーではなくデスクトッププルーフビューアーを使用したい場合は、ユーザーがインタラクティブコンテンツのプルーフを開いたときにデスクトッププルーフビューアーが自動的に起動するように設定できます。 デスクトッププルーフビューアーと web プルーフビューアーの違いについては、[デスクトッププルーフビューアーについて理解する](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) および [web プルーフビューアーとデスクトッププルーフビューアーの概要の違い](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)を参照してください。

1. Workfront から、グローバルナビゲーションバーの Workfront Proof アイコンをクリックして、Workfront Proof にアクセスします。

   ![&#x200B; プルーフアイコン &#x200B;](assets/proof-access-proofhq-350x39.png)

1. Workfront Proof の右上隅にある **アカウント設定**&#x200B;をクリックし、「**設定**」タブを選択します。

1. **プルーフのデフォルト**&#x200B;で、**インタラクティブプルーフ用デスクトッププルーフビューアー**&#x200B;行の最後にある&#x200B;**設定**&#x200B;をクリックします。

1. 記事[組織のプルーフ設定を構成](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)の[デスクトップビューアー](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)の説明に従って、デスクトッププルーフビューアーの設定を変更します。

1. 「**保存**」をクリックします。

## インタラクティブなプルーフ用にカスタムデバイスを構成

カスタムデバイスをシステムに追加すると、ユーザーはインタラクティブコンテンツを確認し、デスクトッププルーフビューアーを使用しているときに特定のデバイスでコンテンツがどのように表示されるかをシミュレートできます。 （この機能は、ユーザーがインタラクティブコンテンツをレビューできる web プルーフビューアーでは利用できませんが、さまざまなデバイスではなく、さまざまな解像度で表示される場合に限ります。）

詳しくは、[プルーフビューアーでインタラクティブプルーフ解像度を変更](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)を参照してください。

1. [Adobe Workfront から Workfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) の説明に従って、Workfront から Workfront Proof インターフェイスにアクセスします。
1. 記事[組織のプルーフ設定を構成](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)の[プルーフ用にカスタムデバイスを設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)の説明に従って、デスクトッププルーフビューアーの設定を変更します。
