---
title: グループの詳細の表示と管理
description: 管理対象のグループまたはサブグループの [ グループの詳細 ] ページを表示および編集できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# グループの詳細の表示と管理

管理対象のグループまたはサブグループの [ グループの詳細 ] ページを表示および編集できます。 このページには、以下が含まれます。

* グループの説明
* ビジネスリーダーおよびグループ管理者の名前
* グループとそのサブグループを公開または非公開にするオプション

   <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

グループを管理するその他の方法について詳しくは、 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

グループを非アクティブ化または再アクティブ化する方法については、 [グループの非アクティブ化または再アクティブ化](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

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

## グループの詳細の表示と管理

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **グループ**.

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. 編集する最上位グループの名前をクリックします。
1. グループを非アクティブ化または再アクティブ化する場合は、
1. 左側のメニューで、 **グループの詳細**&#x200B;次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td> <p>512 文字まで入力できます。</p> <p>フィールドが空白の場合、 <strong>追加</strong> をクリックして、説明を入力します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfrontインスタンスでグループをアクティブにします。</p> <p>以下に示すような先行入力フィールドでは、通常のユーザーがグループを検索してオブジェクトに関連付けたり、オブジェクトと共有したりすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーに対して合理化するには、現在使用中でないグループの「アクティブである」オプションを無効にします。</p> <p>このフィールドを使用すると、アクティブなステータスや非アクティブなステータスに基づいて、グループリストを簡単に表示、フィルタリングおよびグループ化できます。 リストでのビュー、フィルター、グループ化の使用について詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビュー、グループ化</a>.</p> <p>非アクティブなグループについて詳しくは、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">非アクティブなグループに関する考慮事項</a> 記事内 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">カスタムフォームの削除または非アクティブ化</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのアクセシビリティ</td> 
      <td> <p>（サブグループではなく、グループの詳細を表示している場合にのみ使用可能） オプションを有効または無効にします <strong>このグループとサブグループをプライベートにする</strong>.</p> <p>公開グループの場合、編集ユーザーアクセス権を持つ（グループ内またはグループ外の）ユーザーは、他のユーザーのプロファイルにグループを追加できます。 これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの階層の上位の親グループでのみ編集できます。 親グループのすべてのサブグループが設定を継承します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループの関係者</td> 
      <td> 
       <ul> 
        <li><strong>グループ管理者</strong>:Planner ライセンスを持つユーザーを、グループのグループ管理者として追加または削除します。 ユーザーの名前を入力し始め、ドロップダウンメニューに表示されたら、名前をクリックします。</li> 
        <li><strong>ビジネスリーダー</strong>:次のいずれかの操作を行います。
         <ul>
          <li>グループにビジネスリーダーをまだ割り当てていない場合は、 <strong>追加</strong>割り当てるユーザーの名前を入力し、表示されたらユーザーの名前をクリックします。</li>
          <li>グループに既にビジネスリーダーが存在し、変更する場合は、既存のビジネスリーダーの名前をダブルクリックします。 名前を削除し、割り当てるユーザーの名前を入力し、表示されたらユーザー名をクリックします。</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォームを追加</td> 
      <td>アクセスレベルでカスタムフォームを管理できる場合は、カスタムフォームをグループに追加します。 詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">カスタムフォーム</a>.</td> 
     </tr> 
    </tbody> 
   </table>
