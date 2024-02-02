---
user-type: administrator
product-area: system-administration;user-management
keywords: 追加、ユーザー、グループ、追加、別の、割り当て、管理者、削除、ユーザー、表示、役割、メンバー、書き出し、メンバーシップ、データ
navigation-topic: create-and-manage-groups
title: グループのメンバーシップの表示と管理
description: Adobe Workfront 管理者は、管理対象の任意のグループのメンバーの表示、追加、削除、書き出し、アクティブ化、非アクティブ化を行うことができます。また、グループメンバーのプロファイルの編集や更新を行い、グループの追加のグループ管理者としてグループメンバーを割り当てることもできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '753'
ht-degree: 100%

---

# グループのメンバーシップの表示と管理

Adobe Workfront 管理者は、管理対象の任意のグループのメンバーの表示、追加、削除、書き出し、アクティブ化、非アクティブ化を行うことができます。また、グループメンバーのプロファイルの編集や更新を行い、グループの追加のグループ管理者としてグループメンバーを割り当てることもできます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプランまたはライセンスタイプを確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループのメンバーシップの表示と管理

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ**」をクリックします。

   Workfront 管理者は、表示されるリストですべてのグループとサブグループを表示できます。グループ管理者は、管理しているグループとサブグループのみを表示できます。

1. 編集するグループの名前をクリックします。
1. 表示されるページの左側のメニューで&#x200B;**グループメンバー**&#x200B;を選択し、次のいずれかを実行します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">グループにユーザーを追加</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1"><strong>メンバーを追加</strong> <img src="assets/add-icon-plus-in-circle.png"> をクリックし、ユーザーの名前の入力を開始し、表示されたら選択します。</li> 
        <li value="2"> <p>追加する他のユーザーに対して、この手順を繰り返します。</p> <p>ユーザーを追加しない場合は、名前の右側にある「X」をクリックできます。</p> </li> 
        <li value="3">完了したら「<strong>完了</strong>」をクリックします。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループからユーザーを削除</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、「<strong>メンバーを削除</strong><img src="assets/remove-icon---x-in-circle.png">」をクリックします。</li> 
        <li value="2"> <p>表示される警告メッセージで「<strong>削除</strong>」をクリックします。</p> <p>リストから削除するユーザーを検索するには、「<strong>リスト内のユーザーとグループを検索</strong>」をクリックし、ボックスに名前を入力して、表示されたら名前をクリックします。</p> <p><b>メモ</b>：  
          <ul> 
           <li>このグループが削除するユーザーのホームグループの場合は、まずユーザーのプロファイルに別のホームグループを割り当てる必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">ホームグループの概要</a>および<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</li> 
           <li>グループに 1 人のグループ管理者しかいない場合に、グループから別のグループ管理者を削除する必要がある場合は、最初に別のグループ管理者をグループに割り当てる必要があります。</li> 
           <li>ユーザーは、親グループに加えて、個々にサブグループに属することができます。サブグループからユーザーを削除すると、そのユーザーは親グループの一部になります。同様に、親グループから削除すると、サブグループの一部のままになります。ユーザーに親グループへのアクセスを許可しない場合は、サブグループと親グループの両方（両方の場所に個別にリストされている場合）からユーザーを削除する必要があります。</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーのプロファイル情報を編集</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、<strong>編集</strong> <img src="assets/edit-icon.png">をクリックします。</li> 
        <li value="2"> <p>ユーザーのプロファイル情報を変更します。</p> <p>変更について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーメンバーシップデータを書き出し</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、<strong>書き出し</strong> <img src="assets/export.png"> をクリックします。</li> 
        <li value="2"> <p>データを PDF、Excel、またはタブ区切り形式のファイルに書き出します。</p> <p>データの書き出しについて詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">データの書き出し</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">メンバーのグループの役割を表示および編集</td> 
      <td> <p><strong>グループの役割</strong>列には、各メンバーの役割が一覧表示されます。グループ管理者は、メンバーの役割をダブルクリックして変更できます。</p> <p>グループ管理者でないグループのメンバーの場合、この列は編集できません。</p> <p>グループ管理者は常にリストの先頭に表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループメンバーにコメントを送信</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">1 つ以上のユーザー名を選択し、<strong>更新</strong> <img src="assets/comment-icon.png"> をクリックします。</li> 
        <li value="2">コメントを入力します。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront でユーザーをアクティブ化</td> 
      <td>1 人または複数の非アクティブなユーザーを選択し、「<strong>ユーザーをアクティブ化</strong>」をクリックして、Workfront でアクティブ化します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront でユーザーを非アクティブ化</td> 
      <td>1 人または複数のアクティブなユーザーを選択し、「<strong>ユーザーを非アクティブ化</strong><img src="assets/deactivate-user.png">」をクリックして、Workfront で非アクティブ化します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">列で並べ替え</td> 
      <td>列の見出しをクリックすると、その列のコンテンツでリストが並べ替えられます。</td> 
     </tr> 
    </tbody> 
   </table>
