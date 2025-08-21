---
title: Adobe Workfront Planning でのGenStudio Workspaceの管理
description: 会社が両方の製品を購入し、GenStudio for Performance MarketingのインスタンスがAdobe Workfrontの会社のインスタンスと統合されている場合、Workfront Workspace はGenStudio Planning で使用できます。 Planning からGenStudioワークスペースを表示し、両方のシステムで情報を更新できます。
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 10%

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

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

会社が両方の製品を購入し、Adobe GenStudio for Performance MarketingのインスタンスがAdobe Workfrontの会社のインスタンスと統合されている場合、Workfront Workspace はGenStudio Planning で使用できます。

Planning からGenStudioワークスペースを表示し、両方のシステムで情報を更新できます。

GenStudio Performance Marketing のGenStudio Workspace の使用と管理については、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

GenStudioとWorkfront Planning の統合に関する一般的な情報については、[Adobe Workfront Planning とAdobe GenStudio for Performance Marketingの統合の基本を学ぶ ](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のAdobe Workfront ワークフローパッケージ</p>
<p>任意のAdobe Workfront Planning パッケージ</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio パッケージ</p></td> 
   <td> 
<p>???GEN STUDIO には、これをサポートするパッケージがありま？??。</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p> 標準</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio ライセンス</p></td> 
   <td><p> ???GEN STUDIO には、これをサポートする特定のライセンスが必要で？??。</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>  
   <p>GenStudioの設定：???GENS に必要なアクセスレベルは？??</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクトの権限*</p></td> 
   <td>  
   <p>Workfrontの計画では、次の操作を行います。 </p>
   <ul>
   <li><p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p> </li> 
   <li><p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p></li>
   </ul>
   <p>Adobe GenStudio for Performance Marketingで： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketingのすべての権限</p></li>
   <li><p> Adobe GenStudio for Performance Marketingでアイテムを作成する権限を作成する</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。
*Adobe GenStudio for Performance Marketingについて詳しくは、[Adobe GenStudio for Performance Marketing ユーザーガイド ](https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/home) を参照してください。

+++   

## Workfront Planning でのGenStudio Workspace の管理に関する考慮事項

* Workfront Planning でAdobe GenStudio for Performance Marketing Workspace を表示するには、GenStudioを購入する必要があります。

* Workfront ユーザーがWorkfront Planning でGenStudio Workspace を表示するには、GenStudioにアクセスできる必要があります。

* Workfront Planning から、GenStudio Workspace の次の情報を更新できます。

   * ワークスペース設定の編集 <!--check to see if this is correct? is this editable or read only from Planning??-->
   * レコードタイプとそのフィールドを編集する <!--check on this-->
   * ビューの共有、編集、追加
   * 新しいレコードタイプを追加
   * レコードの編集、追加、削除

* GenStudio Workspace のワークスペース設定、レコードタイプ、ビュー、フィールドの更新は、Workfront Planning Workspace をその要素で更新する場合と同じです。

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Workfront Planning からのGenStudio レコードタイプの管理

>[!NOTE]
>
>GenStudio Workspace を管理する前に、[Workfront Planning とGenStudio for Performance Marketingの統合の基本を学ぶ ](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md) を参照してください。

1. GenStudioへのアクセス権も持つユーザーとしてWorkfrontにログインします。
1. 左上隅の **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、**[!UICONTROL 計画]** をクリックします。

   Workfront計画のメインページが開きます。

1. **その他のワークスペース** をクリックし、**System** によって作成され、カードに **GenStudio** タグが付いているという表示を持つワークスペースを見つけます。

   ![ タグ付きGenStudio Workspace カード ](assets/genstudio-card-with-tag-highlighted.png)

1. **GenStudio Workspace カード** をクリックして、Workfront Planning でGenStudio Workspace を開きます。
1. デフォルトでは、次のGenStudio レコードタイプが作成され、Workfront Planning から表示されます。

   * キャンペーン
   * 製品
   * アクティベーション
   * チャネル
   * 地域

   GenStudioレコード式のカードには、GenStudioで最初に作成されたことを示す表示があります。

   <!--check screen shot-->

   ![ タグ付きGenStudio レコードタイプカード ](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. レコードタイプカードのいずれかをクリックして、そのタイプのレコードを表示します。

1. 次のいずれかの操作を行います。

   * レコードタイプページの右上隅にある「**共有**」をクリックし、次のいずれかをクリックします。
      * **表示リンクをコピー** して、レコードタイプへのリンクを共有します
      * **現在のビューをエクスポート** して、CSV または Excel ファイルにエクスポートします。
書き出すことができるのは、テーブルビューのみです。<!--check on this later; is this true or are there more options in the Share button-->

   * 「**+ ビュー**」をクリックして、GenStudio レコードタイプのビューを作成します。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * **フルスクリーン** アイコン ![ フルスクリーンでフルビューを開くアイコン ](assets/open-full-screen-icon.png) をクリックして、任意の表示をフルスクリーンモードで開きます。

   * ビューの要素をビューから管理します。

     例えば、ビューのフィルター、グループ化、並べ替え、設定がある場合はそれを変更できます。

     詳しくは、[レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)を参照してください。

   * テーブル表示またはタイムライン表示でレコードを追加します。

     レコードを作成するには、最初から作成するか、CSV ファイルまたは Excel ファイルを読み込む必要があります。

     詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

     レコードは、WorkfrontとGenStudioの両方から表示されます。

   * テーブル表示からレコードをインラインで編集するか、レコードをクリックして詳細ページを開きます。

     詳しくは、[レコードの編集](/help/quicksilver/planning/records/edit-records.md)を参照してください。

   * テーブル表示でレコードを削除します。

     詳しくは、[ レコードの削除 ](/help/quicksilver/planning/records/delete-records.md) を参照してください。

     削除されたレコードは、Workfrontから削除された場合、Workfront Planning のテーブルビューのごみ箱から復元できます。

     詳しくは、[ 削除されたレコードの復元 ](/help/quicksilver/planning/records/restore-deleted-records.md) を参照してください

   * テーブル表示のフィールドの上にマウスポインターを置くと、フィールドの並べ替えや非表示を行うことができます。

     >[!NOTE]
     >
     >GenStudioでの管理権限を持っている場合にのみ、フィールドの設定を編集したり、フィールドを追加したりできます。<!--check to see if this is true??-->
