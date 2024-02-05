---
content-type: overview
product-area: documents
keywords: プルーフ, 権限
navigation-topic: proofing-overview
title: プルーフ権限プロファイルの概要
description: プルーフ権限プロファイルは、アカウント内のすべてのプルーフに対してユーザーが持つ全体的な権限を決定するものです。プルーフ権限プロファイルは、ユーザープロファイルのユーザーに割り当てられます。配達確認権限プロファイルは、配達確認の役割とは異なります。
author: Courtney
feature: Digital Content and Documents
exl-id: fb6faa48-d97b-4b7b-83ae-fe39d40b3963
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 75%

---

# プルーフ権限プロファイルの概要

<!--Audited: 12/2023-->

プルーフ権限プロファイルは、アカウント内のすべてのプルーフに対してユーザーが持つ全体的な権限を決定するものです。配達確認権限プロファイルは、ユーザープロファイルのユーザーに割り当てられます。

プルーフ権限プロファイルは、プルーフの役割とは異なります。プルーフの役割について詳しくは、[プルーフの役割の概要](../../../review-and-approve-work/proofing/proofing-overview/proof-roles.md)を参照してください。

>[!NOTE]
>
>管理者は、組織内のユーザーのカスタムプロファイルを作成できます。詳しくは、[Workfront Proof でのカスタムプロファイルの設定](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Consider the following about roles and permissions:</p>
-->

<!--
<ul data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li> <p>Assigned profile permissions relate only to the users and items in your own account. The exception is in the case of Satellite accounts, where the Administrator and Billing Administrator for the main (hub) accounts can access and manage the account settings and billing of those accounts from the hub account level.</p> </li>
<li> <p>Billing Administrators and Administrators can delete users. This can only be done in Account settings.</p> </li>
<li>When Billing Administrators and Administrators view proofs that are owned by other users in their account, they view them with the role of a Reviewer.</li>
<li>Using the Read Only role, Billing Administrators and Administrators can access proofs in folders shared with them or in folders created by them. </li>
</ul>
-->

## プルーフ権限プロファイル

次の表に、各プルーフ権限プロファイルで使用できる権限を示します。

<table>
  <tr>
   <td colspan="1" ><strong></strong>
   </td>
   <td colspan="4" ><strong>自分の項目</strong>
   </td>
   <td colspan="3" ><strong>他のユーザーの項目</strong>
   </td>
   <td><strong>管理</strong>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td><strong>追加</strong>
   </td>
   <td><strong>ビュー</strong>
   </td>
   <td><strong>編集</strong>
   </td>
   <td><strong>削除</strong>
   </td>
   <td><strong>ビュー</strong>
   </td>
   <td><strong>編集</strong>
   </td>
   <td><strong>削除</strong>
   </td>
   <td><strong>編集と削除</strong>
   </td>
  </tr>
  <tr>
   <td>管理者
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
  </tr>
  <tr>
   <td>スーパーバイザ－
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>マネージャー
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>x
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

### 管理者

管理者は、[アカウント設定](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)へのアクセス権、および次の権限があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>管理者が実行できる操作：</td> 
   <td>管理者が実行できない操作：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>プルーフを作成、ファイルをアップロード、およびフォルダーを作成</p> </li> 
     <li> <p>作成したプルーフおよびファイルを表示、編集および削除</p> </li> 
     <li> <p>組織内のすべてのユーザーが作成したプルーフおよびファイルを表示、編集および削除</p> </li> 
     <li> <p>他のユーザーの公開フォルダーを削除する</p> </li> 
     <li> <p>アカウントで作成されたすべてのプルーフを編集</p> </li> 
     <li> <p>ドロップゾーンの所有者として設定*</p> </li> 
     <li> <p>アカウント設定ページにアクセスし、アカウントの詳細を編集します</p> </li> 
     <li> <p>ごみ箱を空にする</p> </li> 
     <li> <p>ユーザーの追加、編集および削除</p> </li> 
     <li> <p>グループの作成と新しい連絡先の追加</p> </li> 
     <li> <p>連絡先を削除</p> </li> 
     <li> <p>返信がない場合は配達確認を編集</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>プルーフの返信を編集</p> </li> 
     <li> <p>他のユーザーのプライベートフォルダーを削除する</p> </li> 
     <li> <p>請求ページにアクセスするか、請求の詳細を編集します</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Workfront Proof スタンドアロン製品でのみ可能です。

### スーパーバイザ－

スーパーバイザーには、次の権限があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>スーパーバイザーが実行できる操作：</td> 
   <td>スーパーバイザーが実行できない操作：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>プルーフを作成、ファイルをアップロード、およびフォルダーを作成</p> </li> 
     <li> <p>作成したプルーフおよびファイルを表示、編集および削除</p> </li> 
     <li> <p>組織内のすべてのユーザーが作成したプルーフおよびファイルを表示、編集および削除</p> </li> 
     <li> <p>他のユーザーの公開フォルダーを削除する</p> </li> 
     <li> <p>アカウントで作成されたすべてのプルーフを編集</p> </li> 
     <li> <p>グループの作成と新しい連絡先の追加</p> </li> 
     <li> <p>連絡先を削除</p> </li> 
     <li> <p>返信がない場合は配達確認を編集</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>プルーフの返信を編集</p> </li> 
     <li> <p>他のユーザーのプライベートフォルダーを削除する</p> </li> 
     <li> <p>請求ページにアクセスするか、請求の詳細を編集します</p> </li> 
     <li> <p>ユーザーの追加、編集または削除</p> </li> 
     <li> <p>ごみ箱を空にする</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### マネージャー

マネージャーには次の権限があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>マネージャーが実行できる操作：</td> 
   <td>マネージャーが実行できない操作：</td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>プルーフを作成、ファイルをアップロード、およびフォルダーを作成</p> </li> 
     <li> <p>作成したプルーフおよびファイルを表示、編集および削除</p> </li> 
     <li> <p>明示的に共有されている他のユーザーのプルーフを表示、レビューおよび承認（共有フォルダー内のすべてに対する読み取り専用権限）</p> </li> 
     <li> <p>アカウントで作成されたすべてのプルーフを編集</p> </li> 
     <li> <p>グループの作成と新しい連絡先の追加</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>組織内の他のユーザーが作成したプルーフやファイルを表示、編集または削除 </p> </li><li><p>プルーフの返信を編集</p> </li> 
     <li> <p>他のユーザーのプライベートフォルダーまたはパブリックフォルダーを削除する</p> </li> 
     <li> <p>請求ページにアクセスするか、請求の詳細を編集します</p> </li> 
     <li> <p>ユーザーの追加、編集または削除</p> </li> 
     <li> <p> 連絡先を削除</p> </li> 
     <li> <p>ごみ箱を空にする</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Observer</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers have the following permissions:</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can see, review, and approve proofs of other users that are explicitly shared with them (Read-only rights to everything in a shared folder). For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create proofs, upload files, and create folders. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md" class="MCXref xref">Upload Files and Web Content to Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot view, edit, or delete proofs and files created by other users in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot edit proofs or replies.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete any items created in the organization.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Billing page or Account settings. For more information, see <a href="../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md" class="MCXref xref">The Workfront Proof Billing Page</a> and <a href="../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md" class="MCXref xref">Account settings in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be set as the Dropzone owner. For more information, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md" class="MCXref xref">Configure the dropzone in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot empty the trash. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md" class="MCXref xref">Restore and Empty the Trash in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot add, edit, or delete users. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot create groups or add new contacts. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot delete contacts. </p>
-->


><!--
><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Menus and functions available to Observers are limited. </p>>
>-->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the Header menu or the green New menu in their Dashboard</li>>
>  -->
>  <!--
>  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Observers do not see the following links in their Settings: Account settings, Billing </li>>
>  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Guest</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Guest profile is used to give access to proofs for reviewers who do not have their own Workfront Proof account. Guests can access proofs shared with them directly via their personal email notifications.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view, review, and approve proofs that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/cleaner2.png">Can view files that are explicitly shared with them.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot access the Dashboard.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot have folders shared with them. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md" class="MCXref xref">Manage Folders in Workfront Proof</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no2.png">Cannot be added as Authors or Moderators to the proofs. For more information, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p>
-->

<!--
<note type="note">
 Guests are not Workfront Proof users, so they cannot see all the proofs shared with them in their own Dashboard.
</note>
-->
