---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループの会社を作成および変更
description: グループエリアで管理するグループを表示している場合、グループとそのサブグループに関連付けられている会社を表示して操作できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: ab7877c048ea87180dd518c978b258d266e0f95c
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 100%

---

# グループの会社を作成および変更

グループエリアで管理するグループを表示している場合、グループとそのサブグループに関連付けられている会社を表示して操作できます。

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
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプランまたはライセンスタイプを確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループエリアからグループの会社を表示、操作および作成

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、**グループ** ![](assets/groups-icon.png) をクリックします。

1. 会社を作成または変更するグループの名前をクリックします。
1. 左側のパネルで「**会社**」をクリックし、グループとそのグループに含まれるサブグループに関連付けられている会社を一覧表示します。
1. （オプション）会社を追加するには、「**会社を追加**」をクリックし、以下に示すオプションを使用して会社を設定します。完了したら、「**会社を作成**」をクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">「基本情報」セクション</td> 
      <td> 
       <ul> 
        <li> <p><b>会社名</b>：会社の名前を入力します。</p> </li> 
        <li> <p><b>アクティブ</b>：このオプションを有効にすると、ユーザーは会社を見つけて、作成および編集するプロジェクトに参加させることができます。非アクティブな会社はプロジェクトに添付できません。このオプションは、デフォルトで有効になっています。</p> </li> 
        <li> <p><b>これがプライマリ会社です</b>：会社を組織のプライマリ会社として割り当てます。通常、プライマリ会社は、ほとんどのユーザーが作業する Workfront アカウントを表します。</p> <p>ユーザーのアクセスレベルを変更することで、ユーザーに対して他のユーザーの表示を次のように制限できます。</p> 
         <ul> 
          <li>プライマリ会社内のみ</li> 
          <li> <p>関連付けられた会社内とプライマリ会社内</p> <p>ユーザーのアクセスレベル内でのプライマリ企業の機能について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> <p>1 つの会社のみをプライマリ会社として指定することも、プライマリ会社を指定しないこともできますが、複数の会社をプライマリ会社として指定することはできません。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルを作成または変更</a>を参照してください。</p> </li> 
         </ul> </li> 
        <li> <p><b>グループ</b>：会社と取引を行うグループがある場合、ここにグループの名前を追加できます。これは、グループがビジネスを展開するすべての会社に関するレポートおよび管理を必要とするグループ管理者に役立ちます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">システムにより、新しい会社の<strong>グループ</strong>フィールドに、表示しているグループが入力されます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">現在のアクセスレベルで会社に対する管理者アクセス権がある場合、会社からグループを削除して別のグループを割り当てたり、会社をグループがないままにしたりできます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">会社に対する管理者アクセス権がない場合、<strong>グループ</strong>フィールドは必須で、管理しているグループまたはそのグループの下のサブグループのみを選択できます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">会社への管理アクセス権については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">特定のエリアに対する管理者アクセス権のユーザーへの付与</a>を参照してください。</p> </li> 
        <li> <p><b>会社メンバー</b>：会社に既存のユーザーを追加します。これにより、これらのユーザーをこの会社に関連付けます。</p> <p>1 つの会社と関連付けるユーザー数に制限はありませんが、1 人のユーザーを複数の会社と関連付けることはできません。</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">「カスタムフォーム」セクション</td> 
      <td> <p>会社に追加するフィールドが Workfront で使用できない場合は、カスタムフォームを作成して会社に関連付けることができます。このフォームは、ドロップダウンメニューから選択して会社に添付できます。アクティブな会社のみがドロップダウンメニューに表示されます。カスタムフォームの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">カスタムフォームの作成または編集</a>を参照してください。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >アクセスレベルで会社に対する管理者アクセス権を持っている場合は、リストの下部にある「他の会社を追加」をクリックすることもできます。これにより、新しい会社を素早く設定できる行が追加されます。

1. （オプション）会社を編集または削除するには、少なくとも 1 つの会社を選択してから、ツールバーのボタンを使用して編集 ![](assets/edit-icon.png) または削除 ![](assets/delete.png) します。

   会社の編集について詳しくは、[会社の作成または編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)の記事の[Workfront での会社の作成または編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront)の節を参照してください。

1. （オプション）会社のリストを書き出すには、書き出しアイコン ![](assets/export.png) をクリックしてから、書き出すリストのファイル形式を選択します。
