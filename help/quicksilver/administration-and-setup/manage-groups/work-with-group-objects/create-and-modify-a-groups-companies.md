---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループの会社の作成と変更
description: '[ グループ ] 領域で管理するグループを表示している場合、グループとそのサブグループに関連付けられている会社を表示し、操作できます。'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# グループの会社の作成と変更

[ グループ ] 領域で管理するグループを表示している場合、グループとそのサブグループに関連付けられている会社を表示し、操作できます。

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
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループ領域でグループの会社を表示、操作、作成します

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. 会社を作成または変更するグループの名前をクリックします。
1. 左側のパネルで、 **会社** グループに関連する会社とそのグループに含まれるサブグループを一覧表示します。
1. （オプション）会社を追加するには、 **会社を追加**&#x200B;次に、以下のオプションを使用して会社を設定します。 完了したら、「 **会社を作成**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">「Basic Info」セクション</td> 
      <td> 
       <ul> 
        <li> <p><b>会社名</b>:会社名を入力します。</p> </li> 
        <li> <p><b>アクティブ</b>:このオプションを有効にすると、ユーザーは会社を検索し、作成および編集するプロジェクトに会社を添付できます。 非アクティブな会社はプロジェクトに添付できません。 このオプションは、デフォルトで有効になっています。</p> </li> 
        <li> <p><b>これはプライマリ会社</b>:会社を組織の主要会社として割り当てます。 通常、プライマリ会社は、ほとんどのユーザーが作業するWorkfrontアカウントを表します。</p> <p>ユーザーのアクセスレベルを変更すると、ユーザーに対して他のユーザーの表示を制限できます。</p> 
         <ul> 
          <li>主な会社でのみ</li> 
          <li> <p>関連会社と主要会社</p> <p>ユーザーのアクセスレベルにおける主な企業機能について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> <p>1 つの会社のみを主要な会社として指定できますが、複数の会社を主要な会社として指定することはできません。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>グループ</b>:会社と取引を行うグループがある場合は、ここにグループの名前を追加できます。 これは、グループがビジネスを展開するすべての会社に関するレポートおよび管理を必要とするグループ管理者に役立ちます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">システムが <strong>グループ</strong> 表示しているグループを持つ新しい会社のフィールド。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">アクセスレベルで会社に対する管理者アクセス権を持っている場合、会社からグループを削除して別のグループを割り当てたり、会社をグループなしで終了したりできます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">会社に対する管理者アクセス権がない場合、 <strong>グループ</strong> フィールドは必須です。管理しているグループまたはそのグループの下のサブグループのみを選択できます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">会社への管理アクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </li> 
        <li> <p><b>会社メンバー</b>:会社に既存のユーザーを追加します。 これにより、これらのユーザーをこの会社に関連付けます。</p> <p>1 つの会社と関連付けるユーザー数に制限はありませんが、1 人のユーザーを複数の会社と関連付けることはできません。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">「請求率」セクション</td> 
      <td> <p>会社レベルで、ジョブロールに関連付けられた請求率を上書きできます。 ジョブの役割の作成と請求率との関連付けについて詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">ジョブの役割の作成と管理</a>.</p> <p>会社レベルでの請求率の上書きの詳細は、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">会社レベルでのジョブロール請求率の上書き</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムFormsセクション</td> 
      <td> <p>会社に追加するフィールドがWorkfrontで使用できない場合は、カスタムフォームを作成して会社に関連付けることができます。 このフォームは、ドロップダウンメニューから選択して会社に添付できます。 アクティブな会社のみがドロップダウンメニューに表示されます。 カスタムFormsの作成について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">カスタムフォームの作成または編集</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >アクセスレベルで会社に対する管理者アクセス権を持っている場合は、リストの下部にある「他の会社を追加」をクリックすることもできます。 これにより、新しい会社をすばやく設定できる行が追加されます。

1. （オプション）会社を編集または削除するには、少なくとも 1 つの会社を選択してから、ツールバーのボタンを使用して編集します ![](assets/edit-icon.png) または削除 ![](assets/delete.png) それは。

   会社の編集について詳しくは、 [Workfrontでの会社の作成または編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) 記事内 [会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. （オプション）会社のリストを書き出すには、書き出しアイコン ![](assets/export.png)次に、書き出すリストのファイル形式を選択します。
