---
user-type: administrator
product-area: system-administration;user-management
keywords: 追加，ユーザー，グループ，追加，別の，割り当て，管理者，削除，ユーザー，表示，役割，メンバー，書き出し，メンバーシップ，データ
navigation-topic: create-and-manage-groups
title: グループのメンバーシップを表示および管理する
description: Adobe Workfront管理者は、管理対象の任意のグループのメンバーの表示、追加、削除、書き出し、アクティブ化および非アクティブ化をおこなうことができます。 また、プロファイルの編集、プロファイルへの更新の追加、グループの追加のグループ管理者として割り当てることもできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# グループのメンバーシップを表示および管理する

Adobe Workfront管理者は、管理対象の任意のグループのメンバーの表示、追加、削除、書き出し、アクティブ化および非アクティブ化をおこなうことができます。 また、プロファイルの編集、プロファイルへの更新の追加、グループの追加のグループ管理者として割り当てることもできます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループのメンバーシップを表示および管理する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ**.

   表示されるリストで、Workfront管理者はすべてのグループとサブグループを表示できます。 グループ管理者は、管理しているグループとサブグループのみを表示できます。

1. 編集するグループの名前をクリックします。
1. 表示されるページで、を使用します。 **グループメンバー** 左側のメニューで選択した状態で、次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">グループにユーザーを追加する</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">クリック <strong>メンバーを追加</strong> <img src="assets/add-icon-plus-in-circle.png">をクリックし、ユーザーの名前の入力を開始し、表示されたら選択します。</li> 
        <li value="2"> <p>追加する他のユーザーに対して、この手順を繰り返します。</p> <p>ユーザーを追加しない場合は、名前の右側にある X をクリックできます。</p> </li> 
        <li value="3">クリック <strong>完了</strong> 完了したら、</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループからユーザーを削除する</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、「 <strong>メンバーを削除</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>クリック <strong>削除</strong> が表示される警告メッセージ。</p> <p>リストから削除するユーザーを検索するには、 <strong>リスト内のユーザーとグループを検索</strong>をクリックし、ボックスに名前を入力して、表示されたら名前をクリックします。</p> <p><b>メモ</b>:  
          <ul> 
           <li>このグループが、削除するユーザのホームグループの場合は、まずユーザのプロファイルに別のホームグループを割り当てる必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">ホームグループの概要</a> および <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>.</li> 
           <li>グループに 1 人のグループ管理者しかいない場合、グループから別のグループ管理者を削除する必要がある場合は、最初に別のグループ管理者をグループに割り当てる必要があります。</li> 
           <li>ユーザは、親グループに加えて、個々にサブグループに属することができます。 サブグループから誰かを削除すると、その人は親グループの一部になります。 同様に、親グループから削除すると、それらはサブグループの一部になります。 ユーザーが親グループに対するアクセスを許可しない場合は、サブグループと親グループの両方（両方の場所に個別にリストされている場合）からユーザーを削除する必要があります。</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーのプロファイル情報の編集</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、「 <strong>編集</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>ユーザーのプロファイル情報を変更します。</p> <p>変更について詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーメンバーシップデータのエクスポート</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、「 <strong>書き出し</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>データをPDF、Excel またはタブ区切りファイルとしてエクスポートします。</p> <p>データのエクスポートについて詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">データを書き出し</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">メンバーのグループロールの表示と編集</td> 
      <td> <p>この <strong>グループの役割</strong> 列には、各メンバーの役割が一覧表示されます。 グループ管理者は、メンバーの役割をダブルクリックして変更できます。</p> <p>グループ管理者でないグループのメンバーの場合、この列は編集できません。</p> <p>グループ管理者は常にリストの先頭にいます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループメンバーにコメントを送信</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、「 <strong>更新</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">コメントを入力します。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfrontでのユーザーのアクティベート</td> 
      <td>1 人または複数の非アクティブなユーザーを選択し、 <strong>ユーザーをアクティベート</strong> をクリックして、Workfrontでアクティブ化します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfrontでのユーザーの非アクティブ化</td> 
      <td>1 人または複数のアクティブなユーザーを選択し、「 <strong>ユーザーを非アクティブ化</strong><img src="assets/deactivate-user.png"> をクリックして、Workfrontで非アクティブ化します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">列で並べ替え</td> 
      <td>列の見出しをクリックすると、その列のコンテンツでリストが並べ替えられます。</td> 
     </tr> 
    </tbody> 
   </table>
