---
title: Adobe Admin Consoleでのユーザー管理
description: Adobe管理者は、Adobe Admin Consoleを使用してAdobe Workfrontユーザーおよびシステム管理者を作成できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 1224ecc73ed333a5296b23735ad4e899f15f544b
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Adobe Admin Consoleでのユーザー管理

>[!IMPORTANT]
>
>この記事の機能は、組織のWorkfrontインスタンスがAdobeビジネスプラットフォームにオンボーディングされている場合にのみ使用できます。
>
>組織がAdobeビジネスプラットフォームにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe管理者は、Adobe Admin Consoleを使用してAdobe Workfrontユーザーおよびシステム管理者を作成できます。 コンソールでは、組織全体のAdobe使用権限を一元的に管理できます。 詳しくは、 [Admin Consoleの概要](https://helpx.adobe.com/jp/enterprise/using/admin-console.html).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe管理者権限</td> 
   <td> <p>組織の製品製品のAdobe構成管理者である。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件

Workfront用のAdmin Consoleを使用する前に、コンソールに招待する電子メールが届きます。

1. Adobeを初めておこない、組織のAdobeソフトウェアとサービスを管理する権限が与えられたことを知らせる電子メールが届いた場合は、電子メールの「 」ボタンをクリックしてAdobeアカウントを作成し、Admin Consoleを開きます。

   または

   既にAdobeアカウントがある場合は、 [Adobe Admin Consoleページ](https://adminconsole.adobe.com/).

## Adobe Admin Consoleのその他の詳細

* Workfront System Administrators は、Workfront内からWorkfrontユーザーを非アクティブ化できますが、Admin Console内のユーザーは非アクティブ化されません。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* ユーザー **ホームグループ** は、作成したユーザーに基づいて決定されます。 これは、Admin Console内からはカスタマイズできません。
* Workfrontシステム管理者のアクセスレベルは、Adobe Admin Console内からのみ編集できます。

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* ユーザーのアクセスをシステム管理者から他のアクセスレベルに変更する場合は、まずAdmin Consoleを通じて行う必要があります。

  <!--
   This is not clear
  -->

* Workfrontのユーザーからシステム管理者のアクセス権を削除するには、Adobe Admin Consoleを使用して、製品プロファイル管理者としてユーザーを削除する必要があります。 これにより、ユーザーのWorkfrontアクセスレベルがシステム管理者から要求者に変更されます。

  >[!IMPORTANT]
  >
  >製品プロファイル自体は変更しないでください。

## Workfrontの実稼動インスタンスのユーザーと管理領域にアクセスする {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. 次から： [Adobe Admin Consoleページ](https://adminconsole.adobe.com/)を選択し、 **製品** タブをクリックし、 **Workfront**.

   <!--![](assets/admin-product-1.png)-->

1. 表示されるリストで、上部にあるリンクを選択します。

   これは、ユーザーが作業する実稼動インスタンスです。

   <!--![](assets/instances-1.png)-->

   >[!TIP]
   >
   >リスト内の 2 つ目のリンクであるプレビューインスタンスは、実稼動環境を複製するテスト環境です。 詳しくは、 [Adobe Workfrontプレビューサンドボックス環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >また、リストにサンドボックス環境へのリンクが表示される場合もあります。 詳しくは、 [Adobe Workfrontプレビューサンドボックス環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. 表示されるリストで、 **製品プロファイル** 「 」タブが選択されている場合は、「 Workfront Product Profile 」リンクの名前をクリックします。

   ![](assets/prod-profile-1.png)

   このリストには、Workfrontの実稼動インスタンスに既に割り当てられているすべてのユーザーが含まれます。

   >[!IMPORTANT]
   >
   >製品プロファイル自体は変更しないでください。

1. この記事では、次のセクションのいずれかに進みます。

   * [Adobe Admin Consoleを使用したWorkfrontでのユーザー作成](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Adobe Admin Consoleを使用したWorkfrontでのシステム管理者の作成](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Adobe Admin Consoleを使用したWorkfrontでのユーザー作成 {#create-users-in-workfront-with-the-adobe-admin-console}

WorkfrontユーザーをAdobe Admin Consoleに追加する必要があります。 管理者は、Adobe Admin Consoleで直接ユーザーを作成できます。 グループ管理者は、Workfrontでユーザーを作成し、承認用に送信します。 承認されると、ユーザーがAdobe Admin Consoleに追加されます。

* [Adobe Admin Consoleで直接Workfrontにユーザーを作成](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Workfrontでユーザーを作成し、Adobe Admin Consoleで承認する](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Adobe Admin Consoleで直接Workfrontにユーザーを作成

1. の節で説明されているように、Admin Consoleの「ユーザー」および「管理者」領域に移動します。 [Workfrontの実稼動インスタンスのユーザーと管理領域にアクセスする](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 」を参照してください。
1. を使用 **ユーザー** リストの上で選択したタブで、「 」を選択します。 **ユーザーを追加**.
1. Adobe Analytics の **この製品プロファイルにユーザーを追加** ボックスに、追加するユーザーの電子メールアドレスまたは名前を入力し、 **保存**.

   ユーザーは、Workfrontで要求者のアクセスレベルで作成されます。

   >[!IMPORTANT]
   >
   >製品プロファイル自体は変更しないでください。

1. Workfrontで、ユーザーのアクセスレベルを変更します。

   Workfront管理者がユーザーのアクセスレベルを変更する方法については、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 手順 3 と 4 を繰り返して、さらにユーザーを追加します。

   >[!NOTE]
   >
   >新規Adobeユーザーの場合、Admin Consoleは登録プロセスを完了するよう招待する電子メールを配信します。 すべてのユーザーが登録プロセスを完了して、任意の登録アプリケーションにアクセスするAdobeが必要です。
   >
   >既存のAdobeユーザーの場合、Workfrontが使用可能になっていることを知らせる電子メールをユーザーが受け取る場合と受け取らない場合があります。 これは、製品のAdobe管理者が制御するプリファレンスです。 Adobe管理者が、Workfront管理者とは異なるユーザーである場合があります。

### Workfrontでユーザーを作成し、Adobe Admin Consoleで承認する

Adobe Admin Consoleへのアクセス権を持たないグループ管理者は、このワークフローでユーザーを作成できます。

まず、グループ管理者がWorkfrontでユーザーを作成します。 これにより、「非アクティブ」ステータスと「承認待ち」ステータスのユーザーが作成されます。

次に、Workfront管理者がユーザーを承認します。 これにより、Workfrontのユーザーがアクティベートされ、Adobe Admin Consoleに追加されます。

#### Workfrontでのユーザーの作成（グループ管理者）

Workfrontでユーザーを作成する手順については、 [ユーザーを追加](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### ユーザーを承認する (Workfront管理者 )

ユーザーを承認するには、次の手順に従います。

{{step-1-to-users}}

1. ユーザーを選択し、 **その他** アイコン ![](assets/more-icon.png).

1. ユーザーを承認するには、以下をクリックします。 **承認**&#x200B;を選択し、次に **送信**.

   または

   ユーザーを拒否し、Workfrontから削除するには、 **拒否**&#x200B;を選択し、次に **送信**.

   承認されたユーザーは、Adobe Admin Consoleに自動的に追加されます。

   拒否されたユーザーはWorkfrontから自動的に削除されます。



## Adobe Admin Consoleを使用したWorkfrontでのシステム管理者の作成 {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

システム管理者のアクセスレベルは、Adobe Admin Consoleでのみ付与されます。 Workfront内で管理者アクセスを許可または削除することはできません。

ユーザーをWorkfrontシステム管理者にする前に、Workfrontの実稼動インスタンスにユーザーを追加する必要があります。 手順については、「 [Adobe Admin Consoleを使用したWorkfrontでのユーザー作成](#create-users-in-workfront-with-the-adobe-admin-console) 」を参照してください。

1. の節で説明されているように、Admin Consoleの「ユーザー」および「管理者」領域に移動します。 [Workfrontの実稼動インスタンスのユーザーと管理領域にアクセスする](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 」を参照してください。
1. を選択します。 **管理者** タブを使用して、ユーザーのリストの上に表示されます。
1. 選択 **管理者を追加**.
1. Adobe Analytics の **製品プロファイル管理者の追加** ボックスに、追加する管理者の電子メールアドレスまたは名前を入力し、「 」を選択します。 **保存**.

   ![](assets/add-admin-1.png)

   システム管理者はWorkfrontで作成します。

   >[!IMPORTANT]
   >
   >製品プロファイル自体は変更しないでください。



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
