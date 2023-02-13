---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: ドキュメントフォルダーの共有
description: 「ドキュメント」領域で、フォルダーとそのコンテンツを共有できます。
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# ドキュメントフォルダーの共有

「ドキュメント」領域で、フォルダーとそのコンテンツを共有できます。

>[!NOTE]
>
>* このフォルダーは、オブジェクト上のフォルダー階層の上位 5 レベルに存在する必要があります。 6 番目以下のフォルダーは、そのすぐ上のフォルダーから共有設定を継承します。
>
>  サブフォルダーを追加してフォルダー階層を作成する方法について詳しくは、 [フォルダーとサブフォルダーの作成](../../documents/organizing-documents/create-documents-folder.md#creating-folders) 記事内 [ドキュメントフォルダーの作成](../../documents/organizing-documents/create-documents-folder.md).
>
>* スマートフォルダーは共有できません。
>* テンプレート内のドキュメントフォルダーの共有オプションを設定し、そのテンプレートからプロジェクトを作成した場合、共有設定は新しいプロジェクトのドキュメントフォルダーに転送されません。
>* 作業項目内のドキュメントフォルダの共有オプションを設定し、作業項目をコピーした場合、共有設定は新しい作業項目のドキュメントフォルダに転送されません。
>


## アクセス要件

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## フォルダーの共有

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ドキュメント**.

   または

   Workfrontオブジェクトを開いた状態で、 **ドキュメント** をクリックします。

1. フォルダーを選択して、共有アイコンをクリックします。 ![](assets/share-icon.png) 」と入力します。

   このフォルダーは、オブジェクト上のフォルダー階層の上位 5 レベルに存在する必要があり、スマートフォルダーにはできません。

1. 表示されるボックスの下に、 **フォルダーへのアクセス権を付与**&#x200B;で、フォルダーを共有するユーザー、チーム、ジョブの役割、グループまたは会社の名前を入力し、 **入力** 名前が表示されたら、
1. 先ほど追加したユーザー、チーム、ジョブの役割、グループまたは会社のアクセスを調整するには、名前の右にあるドロップダウンメニューをクリックし、次の使用可能なオプションのいずれかと、その詳細設定を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">それを表示</td> 
      <td> <p>フォルダーとそのコンテンツを表示できます。</p> <p>クリック <strong>詳細設定</strong> を使用して、次のことを許可するかどうかを指定します。</p> 
       <ul> 
        <li><strong>ダウンロード</strong>:フォルダーとそのコンテンツを ZIP ファイルとしてダウンロードする機能</li> 
        <li> <p><strong>共有</strong>:システム内の他のユーザーとフォルダーを共有する機能</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">それを管理</td> 
      <td> <p>フォルダーとそのコンテンツを表示および編集する機能</p> <p>クリック <strong>詳細設定</strong> を使用して、ユーザーに対して次の操作を許可するかどうかを指定します。</p> 
       <ul> 
        <li><strong>削除</strong>:システムからフォルダーとそのコンテンツを削除します</li> 
        <li><b>ダウンロード</b>:フォルダーとそのコンテンツを ZIP ファイルとしてダウンロードします。</li> 
        <li><strong>共有</strong>:システム内の他のユーザーとフォルダーとそのコンテンツを共有します</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）手順 3 ～ 4 を繰り返して、他の名前をリストに追加し、そのオプションを設定します。
1. （オプション）システムの全員がフォルダーとその内容を表示できるようにするには、歯車アイコンをクリックします ![](assets/gear-icon-settings-with-dn-arrow.jpg) 共有ボックスの右上隅にあるをクリックし、 **システム全体で表示できるようにします。**

   気が変わったら、 **システム全体のアクセスを削除** （デフォルトのオプション）。

## ユーザーが自分と共有しているフォルダーのコンテンツにアクセスする方法

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

現在、フォルダーを共有している場合、受信者の「ドキュメント」領域にそのフォルダーは表示されません。 ただし、ドキュメントレポートを実行すると、ドキュメントにアクセスできます。

レポートの実行について詳しくは、 [オブジェクトのレポート](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 記事内 [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). 関連トピック [カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## フォルダーを含むオブジェクトを共有する際の継承された権限

ドキュメントフォルダーを持つオブジェクトを共有すると、受信者はそのフォルダーにもアクセスできます。

* 受信者に親オブジェクトへの表示アクセス権を付与すると、その受信者はフォルダーに対する表示アクセス権を持ちます。
* 受信者に投稿または管理で親オブジェクトへのアクセス権を付与した場合、その受信者はフォルダへのアクセス権を管理できます。
* 親オブジェクトに 1 つのタイプのアクセス（表示、投稿、管理）を付与し、別のタイプのアクセス（フォルダに別のタイプ）を付与した場合、受信者は、フォルダ内のドキュメントに対して最も高いアクセス権を持ちます

   例えば、親オブジェクトを表示アクセス権で共有し、フォルダーを管理アクセス権で共有すると、受信者はフォルダー内のドキュメントに対して「管理」を持ちます。

   >[!NOTE]
   >
   >添付されたドキュメントは、添付されたオブジェクトからのみ権限を継承します。 オブジェクト上にフォルダーを作成し、ドキュメントをフォルダーに移動すると、そのフォルダーの権限が継承されます。 ただし、親オブジェクトまたは親オブジェクト上にフォルダを作成し、ドキュメントをそのフォルダに移動した場合、そのフォルダの権限は継承されません。

* 受信者のアクセスレベルで「プロジェクト、タスク、問題などからドキュメントアクセスを継承しない」オプションが有効になっている場合、ユーザーが共有するフォルダー内のドキュメントに対する権限は継承されません。 フォルダー内のドキュメントへのアクセス権を付与するには、ドキュメントを共有する必要があります。

   「継承しない」オプションについて詳しくは、 [Adobe Workfrontへのアクセスの設定](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

   ドキュメントの共有について詳しくは、 [ドキュメントの共有](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
