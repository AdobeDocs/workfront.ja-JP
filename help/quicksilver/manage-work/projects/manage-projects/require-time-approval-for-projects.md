---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトの承認時間を必要とする
description: プロジェクトに対して記録された時間数についてプロジェクト所有者による承認が必要になるようにプロジェクトを設定できます。このように設定した場合、時間数を請求記録で使用するには、まずプロジェクト所有者によって承認される必要があります。
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 78%

---

# プロジェクトに対する時間の承認の要求

<!--audited: 08/2024-->

プロジェクトに対して記録された時間数についてプロジェクト所有者による承認が必要になるようにプロジェクトを設定できます。このように設定した場合、時間数を請求記録で使用するには、まずプロジェクト所有者によって承認される必要があります。\
請求記録について詳しくは、[請求記録の作成](../../../manage-work/projects/project-finances/create-billing-records.md)を参照してください。

>[!NOTE]
>
>このオプションを有効にしても、タイムシート承認者がタイムシートの時間を承認できなくなるわけではありません。プロジェクト所有者が時間を承認しない、つまり却下した場合でも、タイムシート承認者はタイムシートの時間を承認できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>プロジェクトの承認に要する時間を確認するには、次の手順を実行します。</p>
   <ul><li><p>標準</p></li>
   <li><p>プラン</p></li></ul>

<p>プロジェクトのログ時間を承認するには：</p>
   <ul><li><p>ライト以上</p></li>
   <li><p>レビュー以上</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限またはそれ以上</p>
  </tr> 
  <tr> 
   <td role="rowheader">その他のアクセス</td> 
   <td> <p>プロジェクトに関する時間を承認するには、次の条件の少なくとも 1 つを満たす必要があります。</p> 
    <ul> 
     <li>上記のアクセス権と権限を持つプロジェクト所有者であること。この場合、条件付きで以下が可能です。 
      <ul>
       <li>プロジェクトの管理権限がある場合は、他のユーザーがプロジェクトで記録した時間数を承認または却下できます。</li>
       <li> プロジェクトに対する参加アクセス権または表示アクセス権がある場合は、自分または自分を上司とする他のユーザーが記録した時間数のみを承認または却下できます。<br></li>
      </ul></li> 
     <li>タイムシートおよび時間に管理者アクセス権を持つプランライセンスがあります。 この場合、次のようになります。
      <ul>
       <li>少なくとも表示権限を持つプロジェクトに関する任意の時間数を承認または却下できます。 </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

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
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## プロジェクトに対する時間の承認の要求

プロジェクトの時間数についてプロジェクトマネージャーの承認が必要になるように設定するには、次の手順に従います。

1. 時間数の承認を必要とするプロジェクトに移動します。
1. プロジェクト名の右側にある **その他** アイコン ![ その他のアイコン ](assets/more-icon.png) をクリックし、**編集** をクリックします。\
   プロジェクトの編集ダイアログボックスが表示されます。

1. 「**プロジェクト設定**」セクションで、「**プロジェクト時間の承認**」を選択します。
1. 「**保存**」をクリックします。\
   これで、時間がログに記録され、承認されると、その時間がロックされ、プロジェクトまたはタイムシートに入力したユーザーは変更できなくなります。 記録された時間を調整できるのは Workfront 管理者だけです。

## プロジェクト時間の承認と却下

プロジェクトマネージャーは、タスク、イシューまたはプロジェクトに関して記録される時間数を承認または却下できます。

プロジェクトレベルで時間数を承認しても、時間数を記録したすべてのユーザーのタイムシートには影響はありません。例えば、プロジェクトの時間数がプロジェクトマネージャーによって承認されても、タイムシートが、ユーザーのマネージャーまたはタイムシート承認者によってまだ承認されていない場合があります。

記録された時間数について承認が必要になるようにプロジェクトを設定した場合、プロジェクトマネージャーは時間数を承認して、プロジェクトの請求記録に含めることができるようにする必要があります。請求記録の作成について詳しくは、[請求記録の作成](../../../manage-work/projects/project-finances/create-billing-records.md)を参照してください。

プロジェクトの時間数を承認または却下するには、次の手順に従います。

1. プロジェクトに移動します。
1. 左側のパネルの「**時間**」エリアをクリックします。

1. イシュー、タスク、プロジェクトに関して記録された時間が表示され、ステータスは&#x200B;**送信済み**&#x200B;になります。\
   時間エントリの左側にあるボックスをクリックして、承認する時間を選択します。

1. 時間リストの上部にある **承認** アイコン ![](assets/approve-hours-icon.png) をクリックします。\
   時間のステータスが&#x200B;**承認済み**&#x200B;に変わります。\
   後で承認された時間を却下すると、時間のステータスは&#x200B;**未承認**&#x200B;に変わります。\
   請求記録に承認された時間を含めると、時間のステータスは&#x200B;**請求および承認済み**&#x200B;に変わります。請求記録に追加された時間は削除できません。請求記録の作成について詳しくは、[請求記録を作成](../../../manage-work/projects/project-finances/create-billing-records.md)の記事を参照してください。

1. （任意） **却下** アイコン ![](assets/reject-hours-icon.png) をクリックして、プロジェクトの時間エントリを却下します。\
   時間のステータスが&#x200B;**拒否**&#x200B;に変わります。

   >[!NOTE]
   >
   >   選択した時間が、請求済みまたは請求済みおよび承認済みとしてマークされた請求記録に含まれている場合、「承認」および「却下」アイコンは表示されません。 承認できるのは、請求記録にまだ請求されていない時間のみです。

