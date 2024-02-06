---
product-area: reporting
navigation-topic: reporting-elements
title: フィルター、ビュー、グループの共有
description: 表示アクセス権のあるフィルター、ビューおよびグループを、他のユーザーと共有できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 97%

---

# フィルター、ビュー、グループの共有

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにオブジェクトの表示や編集のアクセス権を付与します。オブジェクトへのアクセス権の付与について詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

ユーザーに付与されるアクセスレベルに加えて、自分が作成した特定のオブジェクトや、自分が共有のアクセス権を持つ特定のオブジェクトを表示または編集する権限をユーザーに付与することもできます。アクセスレベルと権限について詳しくは、[アクセスレベルと権限の連携方法](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

表示アクセス権のあるフィルター、ビューおよびグループを、他のユーザーと共有できます。

フィルター、ビュー、またはグループが共有されている場合、そのフィルター、ビューまたはグループをリストに適用できます。自分に付与されているアクセス権によっては、変更したり、他のユーザーと共有できる場合があります。

フィルター、ビューまたはグループの作成方法については、次の記事を参照してください。

* [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront でのグループの概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループに対する表示以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ビュー、フィルター、またはグループに対する共有アクセス権を持つ表示以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## フィルター、ビュー、グループの共有

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

選択リストでのフィルターの共有方法は、フィルターを共有する際に使用するインターフェイス（標準またはレガシー）によって異なります。フィルター構築インターフェイスの種類については、[Adobe Workfront でフィルターを作成または編集する](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

ビューとグループは、レガシーインターフェイスでのみ共有できます。

### 標準ビルダーインターフェイスを使用してフィルターを共有する

標準インターフェイスでは、プロジェクト、タスク、イシュー、ポートフォリオ、プログラム、ユーザー、テンプレート、グループのリストからフィルターを共有できます。フィルターの標準ビルダーインターフェイスは、他のオブジェクトや、ビューおよびグループでは使用できません。

標準ビルダーインターフェイスを使用してフィルターを共有します。

1. プロジェクト、タスクまたはイシューのリストに移動します。
1. **フィルター** アイコン ![フィルターアイコン](assets/filter-nwepng.png) をクリックします。

   ![標準フィルタービルダー](assets/new-filters-all-filter-types.png)

1. 次のフィルターリストを確認します。

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>お気に入りに登録済み</strong></td>
   <td>お気に入りとしてマークしたフィルターです。フィルターをお気に入りに登録すると、元の場所がフィルター名の下に表示されます。また、お気に入りから削除しない限り、このフィルターは元のリストでは非表示になります。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>保存済み</strong></td>
   <td>自分で作成し、保存したフィルター。デフォルトでは、このリストには保存済みのフィルターが、保存日時が新しい順に表示されますが、フィルター名をドラッグして手動でリストを並べ替えることもできます。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>システムデフォルト</strong></td>
   <td>Workfront システムのデフォルトのフィルター、および Workfront 管理者がシステムレベルまたはレイアウトテンプレートでフィルターのリストに追加したフィルター。</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>自分と共有</strong></td>
   <td>他のユーザーが作成して自分と共有したフィルター、またはシステム全体で共有されているフィルター。</td>
   </tr>
   </tbody>
   </table>

1. 少なくとも表示および共有アクセス権を持つフィルターにポインタを合わせて、**その他**&#x200B;メニュー ![その他メニュー](assets/more-icon-spectrum.png)、「**共有**」の順にクリックします。

   ![その他メニューのオプション](assets/new-filters-more-menu-options-with-delete.png)

   「フィルターの共有」ボックスが表示されます。

1. で共有するユーザー、チーム、役割、グループまたは会社の名前の入力を開始します **へのアクセス権を付与** フィールドに入力します。

   ![フィルター共有ボックス](assets/new-filters-share-filter.png)

1. （オプション）フィルターに対する権限を編集するエンティティの名前の横にある右向き矢印をクリックし、「**表示**」オプションまたは「**管理**」オプションを有効にします。「**表示**」がデフォルトです。

   ![権限の共有](assets/new-filters-sharing-permissions.png)

1. （オプション）以下のいずれかの操作を行って、エンティティに対する追加の権限を有効または無効にします。

   1. 「**表示**」をクリックし、「**共有**」オプションを無効にします。これはデフォルトで有効になっています。
   1. 「**管理**」をクリックし、「**共有**」オプションまたは「**削除**」オプションを無効にします。これらは、デフォルトで有効になっています。

      >[!NOTE]
      >
      >「削除」オプションを使用して管理アクセス権を有効にした場合、ユーザーはフィルターを所有していなくても、すべてのユーザーからフィルターを削除できます。

   >[!TIP]
   >
   >ユーザーは、自分のアクセスレベルより高い権限を受け取ることはできません。アクセスレベルでフィルターを編集するアクセス権がない場合、フィルターを管理する権限を受け取ることはできません。Workfront はこれらのユーザーの「管理」オプションを無効にし、無効になったオプションはグレー表示になります。

1. 「**共有**」をクリックします。フィルターは、指定したエンティティと共有されます。

   >[!TIP]
   >
   >グループと共有すると、グループおよびすべてのサブグループのメンバーに対して、フィルター権限が与えられます。

   共有したフィルターが、指定したエンティティのフィルターパネルの「**自分と共有**」セクションに表示されます。

   ![自分と共有されたフィルター](assets/new-filters-shared-with-me.png)

### 従来のインターフェイスを使用したフィルター、表示、グループ化の共有

従来のインターフェイスを使用したフィルター、表示、グループ化の共有は同じです。

1. オブジェクトのリストまたはレポートに移動します。
1. （条件付き）リストから、**フィルター**、**表示**&#x200B;または&#x200B;**グループ化**&#x200B;アイコンをクリックし、共有するフィルター、表示またはグループ化にポインタを合わせて、**その他**&#x200B;アイコン ![その他アイコン](assets/more-icon.png)、「**共有**」の順にクリックします。

   レポートで、**フィルター**、**表示**&#x200B;または&#x200B;**グループ化**&#x200B;ドロップダウンメニューをクリックし、共有するフィルター、表示またはグループ化を選択します。

1. （条件付き）レポートから共有する場合、**フィルター**、**表示**&#x200B;または&#x200B;**グループ化**&#x200B;ドロップダウンメニューを再度クリックし、「**フィルターの共有**」、「**ビューを共有**」または「**グループを共有**」を選択します。\
   **アクセスをフィルター**、**アクセスを表示**&#x200B;または&#x200B;**アクセスをグループ化**&#x200B;ダイアログボックスが表示されます。

   ![フィルターを共有](assets/share-filter-people-box-nwe-350x458.png)

1. 誰と共有するかに応じて、以下のいずれかの操作を完了します。

   **個々のユーザー、チーム、役割、グループや会社と共有するには、**&#x200B;表示されたフィールドに、共有するユーザー、チーム、役割、グループや会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。\
   複数のユーザー、チーム、役割、グループや会社とアクセスを共有するには、この処理を繰り返します。

   >[!TIP]
   >
   >グループと共有すると、グループのメンバーとすべてのサブグループのメンバーに対して、フィルター、表示、またはグループ化の権限が与えられます。

   **システム内のすべてのユーザーと共有するには、****設定**&#x200B;アイコン、「**この機能をシステム全体で表示**」の順にクリックします。\
   このオプションを使用するには、管理者が「システム全体で共有」オプションを選択する必要があります。詳しくは、[カスタムアクセスレベルを作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の記事と、[レポート、ダッシュボード、カレンダーを共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)の記事を参照してください。

1. （条件付き）個々のユーザー、チーム、役割、グループや会社と共有している場合は、ドロップダウンメニューをクリックして、付与するアクセスレベルを定義します。

   以下のオプションから選択できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>それを表示</strong></td> 
      <td> <p>共有受信者のみが共有フィルター、共有表示や共有グループ化を使用できるようにするには、このオプションを選択します。このオプションを選択した場合、受信者は共有項目を変更できません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>それを管理</strong></td> 
      <td> <p>このオプションを選択すると、共有受信者は共有フィルター、共有表示や共有グループ化の使用および変更が行えます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>共有する</strong></td> 
      <td> <p>「<strong>詳細設定</strong>」をクリックし、受信者が他のユーザーと共有できるようにするかどうかに応じて「<strong>共有</strong>」オプションを選択またはクリアします。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

   フィルター、ビューやグループを共有したユーザーは、**フィルター**、**表示**&#x200B;または&#x200B;**グループ化**&#x200B;のドロップダウンメニューまたはアイコンをクリックし、「**自分と共有**」セクションまで下向きにスクロールすることにより、共有項目にアクセスすることができます。


