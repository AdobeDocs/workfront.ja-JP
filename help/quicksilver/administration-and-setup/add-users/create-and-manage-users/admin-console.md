---
title: Adobe Admin Consoleでのユーザー管理
description: アドビ管理者は、Adobe Admin Console を使用して Adobe Workfront ユーザーおよびシステム管理者を作成できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 14e47364f88b756a2fa25d66ee9f2d85a57c8161
workflow-type: tm+mt
source-wordcount: '1520'
ht-degree: 73%

---

# Adobe Admin Console でのユーザー管理

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>この記事に記載される機能は、Workfront の組織のインスタンスが Adobe Business Platform にオンボーディングされている場合にのみ使用できます。
>
>組織が Adobe Business Platform にオンボーディングされているかどうかによって手順が異なります。手順のリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront／Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

アドビ管理者は、Adobe Admin Console を使用して Adobe Workfront システム管理者を作成できます。Console では、組織全体のアドビ使用権限を一元的に管理できます。詳しくは、[Admin Console の概要](https://helpx.adobe.com/jp/enterprise/using/admin-console.html)を参照してください。

>[!NOTE]
>
>* **Workfront管理者は、Adobe Admin Consoleで設定されている必要があります。** 詳細と手順については、この記事の [Adobe Admin Consoleを使用したWorkfrontでのシステム管理者の作成 ](#create-system-administrators-in-workfront-with-the-adobe-admin-console) を参照してください。
>* **組織がシングルサインオン（SSO）を使用している場合**、Adobe Admin Consoleでユーザーを作成してWorkfrontに割り当てることをお勧めします。 これらのユーザーをWorkfrontで作成することは可能ですが、組織のAdmin Consoleの設定によっては、情報をAdobe Admin Consoleに転送する際に問題が生じる場合があります。
>  &#x200B;>   Adobe Admin Consoleでユーザーを作成したら、Workfrontでユーザーの情報（ロール、グループ、チーム、アクセスレベルの割り当てなど）を設定できます。
>* **組織がシングルサインオン（SSO）を使用していない場合**、システム管理者以外のユーザーをWorkfrontに直接追加できます。 Adobe Admin Console でユーザーを追加することもできますが、Workfront にユーザーを追加すると、ユーザーの作成時にアクセスレベルを設定できるので、時間を節約できます。

Admin Consoleからユーザーのプロファイルに変更を加えると、Workfrontでそのユーザーの「システムアクティビティ」タブに更新が追加されます。 更新は、「システム」によって行われたように表示されます。 これはAdobe Admin Console管理者を指すものであり、Workfrontのメイン管理者を指すものではありません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アドビ管理者権限</td> 
   <td> <p>Adobe製品の製品プロファイル管理者である必要があります</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

Workfront 用に Admin Console を使用する前に、Console への招待メールが届きます。

1. アドビを初めて使用する場合で、組織のアドビソフトウェアおよびサービスの管理者権限があることを知らせるメールを受け取った場合には、メール内のボタンをクリックしてアドビアカウントを作成し、Admin Console を開きます。

   または

   既にアドビアカウントがある場合は、[Adobe Admin Console ページ](https://adminconsole.adobe.com/)に移動します。

## Adobe Admin Console に関するその他の詳細

* Workfront System Administrators は、Workfront 内から Workfront ユーザーを非アクティブ化できますが、Admin Console 内のユーザーは非アクティブ化されません。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* ユーザーの&#x200B;**ホームグループ**&#x200B;は、作成したユーザーに基づいて決定されます。Admin Console 内からカスタマイズすることはできません。
* Workfront システム管理者のアクセスレベルは、Adobe Admin Console 内からのみ編集できます。

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* ユーザーのアクセス権をシステム管理者から他のアクセスレベルに変更するには、まず Admin Console を通じて行う必要があります。

  <!--
   This is not clear
  -->

* Workfront のユーザーからシステム管理者のアクセス権を削除するには、Adobe Admin Console を使用して、製品プロファイル管理者としてユーザーを削除する必要があります。これにより、ユーザーの Workfront アクセスレベルがシステム管理者から依頼者に変更されます。

  >[!IMPORTANT]
  >
  >製品プロファイル自体は変更しないでください。

* Adobe Admin Console管理者は、自動割り当てルールを設定して、Adobe製品を組織内のユーザーに割り当てるプロセスを自動化できます。 この機能を使用するには、組織をAdobe統合エクスペリエンスに移行する必要があります。 詳細と手順については、Adobe ドキュメントの [ 自動割り当てルールの管理 ](https://helpx.adobe.com/enterprise/using/automatic-assignment-rules.html) を参照してください。

  >[!NOTE]
  >
  >自動割り当てを設定するときに信頼できる組織を選択している場合、その組織は「選択したディレクトリまたはドメインのユーザー」領域にあります。 「**ディレクトリを選択** フィールドの横にあるドロップダウン矢印をクリックし、組織を選択します。 信頼できる組織には、信頼できるバッジが付いています。

## Workfront の実稼動インスタンスのユーザーと管理エリアへのアクセス {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. [Adobe Admin Console ページ](https://adminconsole.adobe.com/)で、上部ナビゲーションバーの「**製品**」タブを選択し、「**Workfront**」をクリックします。

   <!--![Admin Console product](assets/admin-product-1.png)-->

1. 表示されるリストで、上部にあるリンクを選択します。

   これは、ユーザーが作業する実稼動インスタンスです。

   <!--![Admin Console instances](assets/instances-1.png)-->

   >[!TIP]
   >
   >リスト内の 2 番目のリンクであるプレビューインスタンスは、実稼動環境を複製するテスト環境です。詳しくは、[Adobe Workfront のプレビューサンドボックス環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。
   >
   >
   >また、リストにサンドボックス環境へのリンクが表示される場合もあります。詳しくは、[Adobe Workfront のプレビューサンドボックス環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。

1. 表示されるリストで「**製品プロファイル**」タブが選択された状態で、Workfront 製品プロファイルリンクの名前をクリックします。

   ![ 製品プロファイル ](assets/prod-profile-1.png)

   このリストには、Workfront の実稼動インスタンスに既に割り当てられているすべてのユーザーが含まれます。

   >[!IMPORTANT]
   >
   >製品プロファイル自体は変更しないでください。

1. この記事では、次のセクションのいずれかに進みます。

   * [Adobe Admin Console で Workfront のユーザーを作成](#create-users-in-workfront-with-the-adobe-admin-console)
   * [Adobe Admin Console で Workfront のシステム管理者を作成](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## Adobe Admin Console で Workfront のシステム管理者を作成 {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

<!--Audited: 12/2023-->

システム管理者のアクセスレベルは、Adobe Admin Console でのみ付与されます。Workfront 内で管理者アクセスを許可または削除することはできません。

ユーザーを Workfront システム管理者にする前に、Workfront の実稼動インスタンスにユーザーを追加する必要があります。

1. この記事の [Workfront の実稼動インスタンスのユーザーおよび管理者エリアにアクセス](#access-the-user-and-admin-area-for-your-production-instance-of-workfront)の節の説明に従って、Admin Console のユーザーおよび管理者エリアに移動します。
1. ユーザーのリストの上にある「**管理者**」タブを選択します。
1. **管理者の追加**&#x200B;を選択します。
1. 「**製品プロファイル管理者の追加**」ボックスに、追加する管理者のメールアドレスまたは名前を入力し、「**保存**」を選択します。

   ![ 管理者を追加 ](assets/add-admin-1.png)

   システム管理者は、Workfront で作成します。

   >[!IMPORTANT]
   >
   >製品プロファイル自体は変更しないでください。


## Adobe Admin Console で Workfront のユーザーを作成 {#create-users-in-workfront-with-the-adobe-admin-console}

>[!NOTE]
>
>システム管理者以外のユーザーは、直接 Workfront に追加することをお勧めします。Adobe Admin Console でユーザーを追加することもできますが、Workfront にユーザーを追加すると、ユーザーの作成時にアクセスレベルを設定できるので、時間を節約できます。

* [Adobe Admin Console で直接 Workfront のユーザーを作成](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [Workfront のユーザーの作成と、Adobe Admin Console に対するユーザーの承認](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### Adobe Admin Console で直接 Workfront のユーザーを作成する

1. この記事内の [Workfront の実稼動インスタンスのユーザーと管理エリアへのアクセス](#access-the-user-and-admin-area-for-your-production-instance-of-workfront)の節で説明されているように、Admin Console のユーザーエリアと管理者エリアに移動します。
1. リストの上部で「**ユーザー**」タブが選択された状態で、「**ユーザーを追加**」をクリックします。
1. 「**この製品プロファイルにユーザーを追加**」ボックスに、追加するユーザーのメールアドレスまたは名前を入力し、「**保存**」をクリックします。

   ユーザーは、Workfront で依頼者のアクセスレベルで作成されます。

   >[!IMPORTANT]
   >
   >製品プロファイル自体は変更しないでください。

1. Workfront で、ユーザーのアクセスレベルを変更します。

   Workfront 管理者がユーザーのアクセスレベルを変更する方法については、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

1. さらにユーザーを追加するには、手順 3 と 4 を繰り返します。

   >[!NOTE]
   >
   >新規アドビユーザーの場合、Admin Console から登録プロセスを完了するための招待メールが送信されます。どのアドビアプリケーションにアクセスするにも、すべてのユーザーが登録プロセスを完了する必要があります。
   >
   >既存のアドビユーザーの場合、Workfront が使用可能になっていることを知らせるメールがユーザーに届く場合と届かない場合があります。これは、製品のアドビ管理者が制御する環境設定です。アドビ管理者は、Workfront 管理者とは異なる場合があります。

### Workfront のユーザーの作成と、Adobe Admin Console に対するユーザーの承認

このワークフローを使用すると、Adobe Admin Console へのアクセス権を持たないグループ管理者でもユーザーを作成できます。

まず、グループ管理者が Workfront のユーザーを作成します。これにより、ユーザーが「非アクティブ化済み」かつ「承認保留中」ステータスで作成されます。

次に、Workfront 管理者がユーザーを承認します。これにより、Workfront のユーザーがアクティブ化され、Adobe Admin Console に追加されます。

#### Workfront のユーザーの作成（グループ管理者）

Workfront のユーザーの作成について詳しくは、[ユーザーの追加](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

#### ユーザーの承認（Workfront 管理者）

ユーザーを承認するには：

{{step-1-to-users}}

1. ユーザーを選択し、**その他** アイコン ![ その他のアイコン ](assets/more-icon.png) をクリックします。

1. ユーザーを承認するには、「**承認**」、「**送信**」の順にクリックします。

   または

   ユーザーを拒否して Workfront から削除するには、「**拒否**」、「**送信**」をの順にクリックします。

   承認されたユーザーは、Adobe Admin Console に自動的に追加されます。

   拒否されたユーザーは、Workfront から自動的に削除されます。


## Adobe Admin Consoleの既存ユーザーの編集

Adobe Admin Consoleで次のユーザー詳細を編集できます。

* ユーザーに関連付けられたユーザーグループと製品
* 管理者権限
* 国

Adobeで 1 人のユーザーを編集する方法については、Adobe Admin Console ドキュメントの「ユーザーを個別に管理する」の [ ユーザーの詳細の編集 ](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#edit-user-details) を参照してください。

Adobe Admin Consoleでのユーザーの一括編集について詳しくは、
Adobe ドキュメントの複数のユーザーの管理の記事 [ ユーザーの詳細を編集 ](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html#edit-user-details)。
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
