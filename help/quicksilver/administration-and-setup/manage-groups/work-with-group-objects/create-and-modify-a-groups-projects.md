---
user-type: administrator
product-area: system-administration;user-management
keywords: グループ、プロジェクト
navigation-topic: work-with-a-groups-objects
title: グループのプロジェクトの作成と変更
description: グループエリアで管理しているグループを表示しているときは、グループのプロジェクトを作成、編集、書き出し、コピー、削除できます。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 86%

---

# グループのプロジェクトを作成および変更する

グループエリアで管理するグループを表示している場合は、次の方法でそのプロジェクトを表示および操作できます。

* グループの新しいプロジェクトの作成
* プロジェクトを編集、書き出し、コピー、または削除する

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

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
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr>
  <tr>
   <td>アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr>
  <tr> 
   <td>オブジェクト権限</td>
   <td> 
    <ul> 
     <li> <p>プロジェクトは、グループまたはそのサブグループのいずれかに関連付ける必要があります。 </p> <p>プロジェクトへのグループの割り当てについて詳しくは、<a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">プロジェクトの概要エリアで情報を管理</a>を参照してください。</p> </li> 
     <li> <p>また、プロジェクトを作成したか、自分と共有されていたので、プロジェクトを編集する権限が必要です。</p></li> 
    </ul>
    <p><b>メモ</b>：グループのページからプロジェクトを作成すると、システムによってプロジェクトがそのグループに割り当てられます。これは、他の Workfront エリアでプロジェクトを作成する場合とは異なります。この場合、システムはプロジェクトを、プロジェクトを作成したユーザー（プロジェクト所有者）のホームグループに割り当てます。</p> </td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループエリアで、グループのプロジェクトを表示、操作、作成します。

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![&#x200B; グループ &#x200B;](assets/groups-icon.png)」をクリックします。

1. プロジェクトを作成、表示、または操作するグループの名前をクリックします。
1. 左側のパネルで、**メインメニューのプロジェクト**![&#x200B; プロジェクト &#x200B;](assets/projects-in-main-menu.png) をクリックして、グループに関連付けられているプロジェクトのリストを表示します。

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>プロジェクトを操作する</p> </td> 
      <td> <p>プロジェクトを選択し、ツールバーボタンを使用して編集 <img src="assets/edit-icon.png">、共有 <img src="assets/share-icon.png">、削除 <img src="assets/delete.png"> を行います。</p> <p>これらのアクティビティについて詳しくは、<a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">プロジェクトの管理：記事インデックス</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>グループの新しいプロジェクトの作成</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p>「<strong>新規プロジェクト</strong>」をクリックし、ドロップダウンメニューからオプションを選択してプロジェクトの作成方法を指定します。 </p> <p>詳しくは、<a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">プロジェクトの作成</a>の記事の<a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">プロジェクトを作成する方法</a>の節を参照してください。</p> </li> 
        <li value="2"><a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトの編集</a>で説明されているように、プロジェクトの名前を入力して設定します。</li> 
       </ol> <p> グループに対して設定されたプロジェクト環境設定は、グループエリアで作成するすべてのプロジェクトに影響を与えます。詳しくは、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">グループのプロジェクト環境設定を指定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクトのリストを書き出す</td> 
      <td>リストの上にあるツールバーの書き出しアイコン <img src="assets/export.png"> をクリックします。</td> 
     </tr> 
    </tbody> 
   </table>
