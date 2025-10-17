---
user-type: administrator
product-area: system-administration;user-management
keywords: 追加、ユーザー、グループ、追加、別の、割り当て、管理者、削除、ユーザー、表示、役割、メンバー、書き出し、メンバーシップ、データ
navigation-topic: create-and-manage-groups
title: グループのメンバーシップの表示と管理
description: Adobe Workfront 管理者は、管理対象の任意のグループのメンバーの表示、追加、削除、書き出し、アクティブ化、非アクティブ化を行うことができます。また、グループメンバーのプロファイルの編集や更新を行い、グループの追加のグループ管理者としてグループメンバーを割り当てることもできます。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 89%

---

# グループのメンバーシップの表示と管理

Adobe Workfront 管理者は、管理対象の任意のグループのメンバーの表示、追加、削除、書き出し、アクティブ化、非アクティブ化を行うことができます。また、グループメンバーのプロファイルの編集や更新を行い、グループの追加のグループ管理者としてグループメンバーを割り当てることもできます。

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
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループのメンバーシップの表示と管理

{{step-1-to-setup}}

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
       <ol> 
        <li><strong>メンバーを追加</strong> <img src="assets/add-icon-plus-in-circle.png"> をクリックし、ユーザーの名前の入力を開始し、表示されたら選択します。</li>
        <li> <p>追加する他のユーザーに対して、この手順を繰り返します。</p> <p>ユーザーを追加しない場合は、名前の右側にある「X」をクリックできます。</p> </li>
        <li>完了したら「<strong>完了</strong>」をクリックします。</li>
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループからユーザーを削除</td> 
      <td> 
       <ol> 
        <li>1 つ以上のユーザー名を選択し、「<strong>メンバーを削除</strong><img src="assets/remove-icon---x-in-circle.png">」をクリックします。</li> 
        <li> <p>表示される警告メッセージで「<strong>削除</strong>」をクリックします。</p> <p>リストから削除するユーザーを検索するには、「<strong>リスト内のユーザーとグループを検索</strong>」をクリックし、ボックスに名前を入力して、表示されたら名前をクリックします。</p> <p><b>メモ</b>：  
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
       <ol> 
        <li>1 つ以上のユーザー名を選択し、「<strong> 編集 </strong>」 <img src="assets/edit-icon.png"> をクリックします。</li> 
        <li> <p>ユーザーのプロファイル情報を変更します。</p> <p>変更について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーメンバーシップデータを書き出し</td> 
      <td> 
       <ol> 
        <li>1 つ以上のユーザー名を選択し、「<strong> 書き出し </strong>」 <img src="assets/export.png"> タンをクリックします。</li> 
        <li> <p>データを PDF、Excel、またはタブ区切り形式のファイルに書き出します。</p> <p>データの書き出しについて詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">データの書き出し</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">メンバーのグループの役割を表示および編集</td> 
      <td> <p><strong>グループの役割</strong>列には、各メンバーの役割が一覧表示されます。グループ管理者は、メンバーの役割をダブルクリックして変更できます。</p> <p>グループ管理者でないグループのメンバーの場合、この列は編集できません。</p> <p>グループ管理者は常にリストの先頭に表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループメンバーにコメントを送信</td> 
      <td> 
       <ol> 
        <li>1 人以上のグループメンバーを選択し、ツールバーの <strong> ユーザーに更新を送信 </strong> をクリックしてください。</li> 
        <li><p>ユーザーに送信するコメントと、ユーザープロファイルの更新エリアに入力します。</p>
        <p>詳しくは、<a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md"> 他のユーザーへのダイレクトメッセージの送信 </a> を参照してください。</p></li> 
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
