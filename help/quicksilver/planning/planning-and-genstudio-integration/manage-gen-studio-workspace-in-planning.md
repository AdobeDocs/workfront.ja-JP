---
title: Adobe Workfront Planning でのGenStudio Workspaceの管理
description: 会社が両方の製品を購入し、GenStudio for Performance MarketingのインスタンスがAdobe Workfrontの会社のインスタンスと統合されている場合、Workfront Workspace はGenStudio Planning で使用できます。 Planning からGenStudioワークスペースを表示し、両方のシステムで情報を更新できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 3%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# Adobe Workfront Planning でのGenStudio Workspace の管理

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

会社が両方の製品を購入し、Adobe GenStudio for Performance MarketingのインスタンスがAdobe Workfrontの会社のインスタンスと統合されている場合、Workfront Workspace はGenStudio Planning で使用できます。

Planning からGenStudioワークスペースを表示し、両方のシステムで情報を更新できます。

GenStudio Performance Marketing のGenStudio Workspace の使用と管理については、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

GenStudioとWorkfront Planning の統合に関する一般的な情報については、[Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの統合の基本を学ぶ &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。

>[!IMPORTANT]
>
>ここでは、管理権限を持っている場合にWorkfront Planning からGenStudio Workspace を更新する手順について説明します。
> GenStudio Workspace に対する投稿権限を持っている場合、すべての機能が使用できるわけではありません。
>
>会社にWorkfrontの複数のインスタンスがある場合、すべてのユーザーはWorkfront Planning のGenStudio Workspace で投稿権限を取得します。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontと任意の Planning パッケージ</p>
<p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
   <tr> 
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing ユーザーの役割</p></td> 
   <td><p><ul><li>キャンペーン、製品およびペルソナにアクセスするためのGenStudio ユーザーロール</li>
   <li>アクティベーションにアクセスするための GenSudio System Manager <!--and Events--></li></ul>
   詳しくは、<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles"> ユーザーの役割と権限 </a> を参照してください。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  
   <p>Workfrontの計画では、次の操作を行います。 </p>
   <ul>
   <li><p>GenStudio Workspace に新しいフィールドまたはレコードタイプを追加するためのGenStudio Workspace に対する権限を管理します</p></li>
   <li><p>GenStudio Workspace に対するレコードの追加、更新、削除の権限の投稿GenStudio Workspace</p> </li>  
   </ul>
   <p>Workfront Planning のGenStudio Workspace からGenStudio for Performance Marketing レコードタイプまたはフィールドを削除することはできません</p>
   <p>Adobe GenStudio for Performance Marketingで： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketingのすべての権限</p></li>
   <li><p> Adobe GenStudio for Performance Marketingでアイテムを作成する権限を作成する</p></li></ul>
   </td>  
</tbody> 
</table>

Adobe Workfront Planning へのアクセスについて詳しくは、[Adobe Workfront Planning へのアクセスの概要 &#x200B;](/help/quicksilver/planning/access/access-overview.md) を参照してください。

Adobe GenStudio for Performance Marketingについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド &#x200B;](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****** and Events*********</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Workfront Planning でのGenStudio Workspace の管理に関する考慮事項

* Workfront Planning でAdobe GenStudio for Performance Marketing Workspace を表示するには、GenStudioを購入する必要があります。

* 組織のWorkfront インスタンスの数に応じて、Planning のGenStudio Workspace に対して自動的に次の権限が付与されます。

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>Workfrontの 1 つのインスタンス</p></td> 
      <td> 
   <p>GenStudio Workspace は、Workfront Planning のインスタンスに表示されます</p>
   <p>Workfront管理者には、Planning のGenStudio Workspace に対する管理権限があります</p>
   <p>他のすべてのユーザーは、Planning のGenStudioワークスペースへの Contribute アクセス権を持っています</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Workfrontの複数のインスタンス</p> </td> 
      <td> 
      <p>GenStudio Workspace は、すべてのWorkfront インスタンスから表示されます</p>
   <p>GenStudio for Performance MarketingおよびWorkfront Planning へのアクセス権を持つすべてのユーザーには、Planning のGenStudioに対する投稿権限があります</p> </td> 
   </tr>
      </tbody> 
   </table>

* GenStudio Workspace のワークスペース設定、レコードタイプ、ビュー、フィールドの更新は、Workfront Planning Workspace をその要素で更新する場合と同じです。
<!--Is this just preview?? * You can build hierarchies for the record types in the GenStudio workspace. For more information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* You cannot include GenStudio Brands in a hierarchy. -->

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Workfront Planning からのGenStudio Workspace の管理

>[!NOTE]
>
>GenStudio Workspace を管理する前に、[Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの統合の基本を学ぶ &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。
>

1. GenStudioへのアクセス権も持つユーザーとしてWorkfrontにログインします。
1. 左上隅の **[!UICONTROL メインメニュー]** アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、**[!UICONTROL 計画]** をクリックします。

   Workfront計画のメインページが開きます。

1. **その他のワークスペース** をクリックし、**System** によって作成され、カードに **GenStudio** タグが付いているという表示を持つワークスペースを見つけます。

   ![&#x200B; タグ付きGenStudio Workspace カード &#x200B;](assets/genstudio-card-with-tag-highlighted.png)

1. **GenStudio Workspace カード** をクリックして、Workfront Planning でGenStudio Workspace を開きます。
1. デフォルトでは、次のGenStudio レコードタイプが作成され、Workfront Planning から表示されます。

   * キャンペーン
   * 製品
   * ペルソナ
   * アクティベーション
   * チャネル
   * 地域

   GenStudioレコード式のカードには、GenStudioで最初に作成されたことを示す表示があります。

   <!--check screen shot-->

   ![&#x200B; タグ付きGenStudio レコードタイプカード &#x200B;](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. ワークスペース名の右側にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックし、次のいずれかをクリックします。

   * **編集**

     詳しくは、[&#x200B; ワークスペースの編集 &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) を参照してください。
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. 右上隅の **共有** をクリックして、他のユーザーとワークスペースを共有します。

   詳しくは、「ワークスペースの共有 [&#x200B; を参照してください &#x200B;](/help/quicksilver/planning/access/share-workspaces.md)

   >[!NOTE]
   >
   >共有に関する次の制限があります。
   >
   >* GenStudio ユーザーとGenStudio Workspace を共有した後は、そのユーザーを Workspace から削除することはできません。
   >* ユーザーがGenStudioの権限を持っている場合、そのユーザーのアクセス権をWorkfront Planning の「表示」に変更することはできません。 少なくとも Planning のGenStudioワークスペースで投稿権限が付与されている必要があります。
   >* GenStudio Workspace のGenStudio レコードタイプに対して、継承された権限を無効にすることはできません。

1. レコードタイプカードのいずれかをクリックして、そのタイプのレコードを表示します。

   レコードタイプ、ビュー、フィールドを管理するには、この記事の [Workfront Planning からのGenStudio レコードタイプの管理 &#x200B;](#manage-genstudio-record-types-from-workfront-planning) の節を参照してください。


## Workfront Planning のGenStudio Workspace からレコードタイプ、ビューおよびレコードを管理します

>[!NOTE]
>
>GenStudio Workspace を管理する前に、[Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの統合の基本を学ぶ &#x200B;](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。
>

1. この記事の [Workfront Planning からのGenStudio Workspace の管理 &#x200B;](#manage-the-genstudio-workspace-from-workfront-planning) の説明に従って、Workfront Planning のGenStudio Workspace に移動し、レコードタイプ ページを開きます。

1. レコードタイプ名の右側にある **その他** メニュー ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックし、次のいずれかをクリックします。

   * **編集**

     詳しくは、[&#x200B; レコードタイプの編集 &#x200B;](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。
   * **自動化の管理**

     詳しくは、[Adobe Workfront Planning の自動設定の構成 &#x200B;](/help/quicksilver/planning/records/configure-automations-to-create-records.md) を参照してください。
   * **リクエストフォームの管理**

     複数のリクエストフォームを作成できます。 リクエストフォームは、Workfrontの「リクエスト」エリアで利用できます。また、リクエストフォームを公開したり、リンクで共有したりすることもできます。

     詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

1. ビューまたはレコードの種類を共有するには、次の操作を行います。

   * レコードタイプページの右上隅にある「**共有**」をクリックし、次のいずれかをクリックします。
      * **レコードタイプの共有**
詳しくは、[&#x200B; レコードタイプの共有 &#x200B;](/help/quicksilver/planning/access/share-record-types.md) を参照してください。
      * **現在のビューを共有**
詳しくは、[&#x200B; ビューの共有 &#x200B;](/help/quicksilver/planning/access/share-views.md) を参照してください。
      * **ビューリンクのコピー**
ビューへのリンクがクリップボードにコピーされました。
      * **現在のビューをエクスポート**
詳しくは、[&#x200B; テーブルビューからのレコードのエクスポート &#x200B;](/help/quicksilver/planning/records/export-records-from-the-table-view.md) を参照してください。

        >[!NOTE]
        >
        >GenStudio ユーザーまたはレコードタイプをGenStudio Workspace と共有した後で、そのワークスペースのレコードタイプからユーザーを削除することはできません。

1. レコードタイプのビューを管理するには、次の手順を実行します。

   * 「**+ ビュー**」をクリックして、GenStudio レコードタイプのビューを作成します。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * **フルスクリーン** アイコン ![&#x200B; フルスクリーンでフルビューを開くアイコン &#x200B;](assets/open-full-screen-icon.png) をクリックして、任意の表示をフルスクリーンモードで開きます。

   * ビューの要素をビューから管理します。

     例えば、ビューのフィルター、グループ化、並べ替え、設定がある場合はそれを変更できます。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

1. レコードを追加するには、次のいずれかの操作を行います。

   * 任意のビューで **新規レコード** をクリックすると、レコードを最初から作成できます

   * テーブル表示での Excel または CSV ファイルを使用したレコードの読み込み

   * レコードを追加するには、タイムラインビューまたはカレンダービューの任意の場所をクリックします。

     詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

     レコードは、WorkfrontとGenStudioの両方から表示されます。

     >[!NOTE]
     >
     >有効化レコードタイプのレコードは追加できません。

1. レコードを編集するには、次のいずれかの操作を行います。

   * テーブル表示からレコードをインラインで編集

   * 任意のビューからレコードをクリックすると、その詳細ページが開きます。

     詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

     Planning のGenStudioワークスペースから行った変更は、GenStudioからただちに表示されます。

1. テーブル表示でレコードを選択し、「**削除**」をクリックします。

   詳しくは、[&#x200B; レコードの削除 &#x200B;](/help/quicksilver/planning/records/delete-records.md) を参照してください。

   削除されたレコードは、GenStudioからすぐに削除されます。

   >[!TIP]
   >
   >削除されたレコードは、Workfront Planning のテーブルビュー「最近削除されたレコード」ビンから復元できます。 GenStudioから削除されたレコードは、Workfront Planning の「最近削除された項目」ビンからも復元できます。

   詳しくは、[&#x200B; 削除されたレコードの復元 &#x200B;](/help/quicksilver/planning/records/restore-deleted-records.md) を参照してください

1. 以下を作成するには、テーブルビューの右上隅にある「+」アイコンをクリックします。

   * フィールド

     詳しくは、[&#x200B; フィールドの作成 &#x200B;](/help/quicksilver/planning/fields/create-fields.md) を参照してください。

   * 接続

     詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

     GenStudio Workspace から作成されたフィールドは、次の領域に表示されます。

      * Workfront計画ビュー
      * Workfront計画レコードの詳細
      * GenStudio レコードの詳細

     >[!NOTE]
     >
     >* フィールドの追加は、GenStudioでの管理権限を持っている場合にのみ行えます。
     >* Workfront Planning で作成されたフィールドは、GenStudioのリストビューには表示されません。
     >
     >* 任意のGenStudio レコードタイプを Brands GenStudio レコードタイプに関連付けることができます。
     >  製品とペルソナは、デフォルトでブランドに接続されています。

1. テーブル表示のフィールドの上にマウスポインターを置き、ドロップダウンメニューをクリックして、次のいずれかの操作を行います。

   * 基準：
   * 非表示にする
   * 設定の編集

   <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

   <!--GenStudio-native fields are note removed from GenStudio. -->

   >[!NOTE]
   >
   >* GenStudio フィールドの設定を編集できるのは、GenStudioでの管理権限を持っている場合のみです。
   >* GenStudio フィールドは削除できません。

<!--Is this just Preview?? Or direct to Prod?? 

## Create workspace hierarchies in the GenStudio workspace

Creating hierarchies in the GenStudio workspace is similar to creating hierarchies in any workspace. 

>[!NOTE]
>
>You cannot add GenStudio Brands to a hierarchy in the GenStudio workspace.

For information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)
-->
