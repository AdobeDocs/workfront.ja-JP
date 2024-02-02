---
title: グループの詳細の表示と管理
description: 管理対象のグループまたはサブグループについて、グループの詳細ページを表示して編集することができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: ht
source-wordcount: '636'
ht-degree: 100%

---

# グループの詳細の表示と管理

管理対象のグループまたはサブグループについて、グループの詳細ページを表示して編集することができます。このページには、以下が含まれます。

* グループの説明
* ビジネスリーダーおよびグループ管理者の名前
* グループとサブグループを公開または非公開にするオプション

  <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

グループを管理するその他の方法について詳しくは、[グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)を参照してください。

グループを非アクティブ化または再アクティブ化する方法については、[グループの非アクティブ化と再アクティブ化](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)を参照してください。

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

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
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>と<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類を確認するには、Workfront 管理者にお問い合わせください。

## グループの詳細の表示と管理

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. 編集する最上位のグループ名をクリックします。
1. グループを非アクティブ化または再アクティブ化する場合は、
1. 左側のメニューで「**グループの詳細**」をクリックし、以下のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td> <p>512 文字まで入力できます。</p> <p>フィールドが空白の場合は、「<strong>追加</strong>」をクリックして説明を入力します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfront インスタンスでグループをアクティブ化します。</p> <p>下図のような先行入力フィールドでは、オブジェクトの関連付けやオブジェクトの共有のために、標準ユーザーがグループを検索しようとすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーが効率的に利用できるようにするには、現在使用していないグループの「アクティブ」オプションを無効にします。</p> <p>このフィールドを使用すると、ステータスがアクティブか非アクティブかに基づいて、グループリストを簡単に表示、フィルタリング、グループ化できます。リストの表示、フィルタリング、グループ化の使用について詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルタリング、表示、グループ化</a>を参照してください。</p> <p>非アクティブなグループについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">カスタムフォームの削除または非アクティブ化</a>の記事の<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">非アクティブなグループに関する考慮事項</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのアクセシビリティ</td> 
      <td> <p>（サブグループではなく、グループの詳細を表示している場合にのみ使用可能。）「<strong>このグループとサブグループをプライベートにする</strong>」オプションを有効または無効にします。</p> <p>パブリックグループの場合、編集ユーザー権限のあるユーザー（グループの内外を問わない）は、他のユーザーのプロファイルにグループを追加できます。これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの最上位階層の親グループでのみ編集できます。すべてのサブグループは親グループの設定を継承します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループの関係者</td> 
      <td> 
       <ul> 
        <li><strong>グループ管理者</strong>：プランナーライセンスを持つユーザーを、グループのグループ管理者として追加または削除します。ユーザーの名前を入力し始め、ドロップダウンメニューに表示されたら、名前をクリックします。</li> 
        <li><strong>ビジネスリーダー</strong>：次のいずれかの操作を行います。
         <ul>
          <li>グループにビジネスリーダーをまだ割り当てていない場合は、「<strong>追加</strong>」をクリックし、割り当てるユーザーの名前を入力し始め、表示されたユーザー名をクリックします。</li>
          <li>グループに既に存在するビジネスリーダーを変更する場合は、既存のビジネスリーダーの名前をダブルクリックします。その名前を削除し、割り当てるユーザーの名前を入力し始めて、表示されたユーザー名をクリックします。</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォームを追加</td> 
      <td>カスタムフォームを管理できるアクセスレベルの場合は、グループにカスタムフォームを追加します。詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">カスタムフォーム</a>を参照してください。</td> 
     </tr> 
    </tbody> 
   </table>
