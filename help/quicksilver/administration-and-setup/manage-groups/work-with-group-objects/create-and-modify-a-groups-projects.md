---
user-type: administrator
product-area: system-administration;user-management
keywords: グループ，プロジェクト
navigation-topic: work-with-a-groups-objects
title: グループのプロジェクトの作成と変更
description: '[ グループ ] 領域で管理しているグループを表示しているときは、グループのプロジェクトを作成、編集、書き出し、コピー、削除できます。'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# グループのプロジェクトの作成と変更

[ グループ ] 領域で管理するグループを表示している場合は、次の方法でそのプロジェクトを表示および操作できます。

* グループの新しいプロジェクトを作成します
* プロジェクトの編集、エクスポート、コピー、削除

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td >Workfrontプラン</a>*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfrontライセンス</a>*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <ul> 
     <li> <p>プロジェクトは、グループまたはそのサブグループのいずれかに関連付ける必要があります。 </p> <p>プロジェクトへのグループの割り当てについては、 <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">プロジェクトの概要領域で情報を管理します。</a>.</p> </li> 
     <li> <p>また、プロジェクトを作成したか、自分と共有されていたので、プロジェクトを編集する権限が必要です。</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </li> 
    </ul> <p><b>注意</b>:グループのページからプロジェクトを作成すると、そのプロジェクトがそのグループに割り当てられます。 これは、他のWorkfront領域でプロジェクトを作成する場合とは異なります。この場合、プロジェクトを作成したユーザーのホームグループ（プロジェクト所有者）にプロジェクトが割り当てられます。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## 「グループ」領域で、グループのプロジェクトを表示、操作、作成します

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. プロジェクトを作成、表示、または操作するグループの名前をクリックします。
1. 左側のパネルで、 **プロジェクト** ![](assets/projects-in-main-menu.png) をクリックして、グループに関連付けられたプロジェクトの一覧を表示します。

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>プロジェクトの操作</p> </td> 
      <td> <p>プロジェクトを選択し、ツールバーのボタンを使用して編集します <img src="assets/edit-icon.png">，共有 <img src="assets/share-icon.png">、または削除します。 <img src="assets/delete.png">.</p> <p>これらのアクティビティについて詳しくは、 <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">プロジェクト管理</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>グループの新しいプロジェクトを作成します</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>クリック <strong>新規プロジェクト</strong>をクリックし、ドロップダウンメニューのオプションを選択して、作成方法を指定します。 </p> <p>詳しくは、 <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">プロジェクトの作成方法</a> 記事内 <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">プロジェクトの作成</a>.</p> </li> 
        <li value="2">プロジェクトの名前を入力し、設定します。詳しくは、 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトを編集</a>.</li> 
       </ol> <p> グループに対して設定されたプロジェクト環境設定は、グループ領域で作成するすべてのプロジェクトに影響を与えます。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">グループのプロジェクト環境設定の指定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクトのリストを書き出す</td> 
      <td>書き出しアイコンをクリックします。 <img src="assets/export.png"> 」と入力します。</td> 
     </tr> 
    </tbody> 
   </table>
