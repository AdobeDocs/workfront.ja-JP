---
title: 接続されたレコードページのレコードへの追加
description: 接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 48bfeb3b950ca1149a919aa204d77db6aa501e01
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 4%

---


# 接続されたレコード ページをレコードに追加する

接続されたレコード ページのタブをレコードに追加すると、接続されたレコードまたはオブジェクトの情報を表示できます。 これにより、テーブル表示の接続されたレコードがタブに追加されます。

「接続済みレコード」ページをレコードに追加する場合は、次の点を考慮してください。

* レコード タイプのテーブル ビューからレコード タイプにレコード タイプまたはオブジェクト タイプを接続した後に、[ 接続されたレコード ] ページをレコードに追加できます。

* レコードのプレビュー領域またはレコードのページから、「接続済みレコード」ページを追加できます。

* 接続されたレコード・ページには、接続されたオブジェクトまたは 1 つのオブジェクトまたはレコード・タイプのレコードのみがテーブル・ビューに表示されます。 ページには、そのタイプのすべてのレコードが表示されるわけではありません。

* 以下の接続されたレコードまたはオブジェクト タイプに対して、接続されたレコード ページを追加できます。

   * Workfront計画レコードタイプ
   * Workfront プロジェクト、プログラム、ポートフォリオ、グループまたは会社。 Connected Workfront オブジェクトは、Workfrontでアクセスする権限を持っていない場合でも表示できます。

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
   <p> 以下のアプリケーションのオブジェクトに接続済みレコードページを追加する場合は、Adobe Workfrontに加えて、以下が必要です。</p>
   <ul><li><p>Adobe Experience Manager Assets ライセンス、およびAEM Assets を Planning レコードタイプと統合するためのAEM AssetsとWorkfrontの統合。</p>
   <p>詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials：記事インデックス </a> を参照してください。 </p></li>
   <li><p> レコードタイプとGenStudio ブランドを接続するためのAdobe GenStudio for Performance Marketing ライセンス</p>
   <p>詳しくは、<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketingの基本を学ぶ </a> を参照してください。</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <p>ワークスペースおよびレコードタイプへの投稿以上の権限 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> 
  </td>
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   


## 接続されたレコード ページをレコードに追加する

1. レコード名をクリックすると、レコードタイプページの任意のビューからレコードが開きます。
1. 次のいずれかの領域で **ページを追加** をクリックします。

   * レコードのプレビューウィンドウ
   * レコードの詳細ページ。プレビューページの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで詳細を開くアイコン ](assets/open-details-in-a-new-tab-icon.png) をクリックします。

   **ページを作成** ボックスが開きます。

   ![ 接続されたレコードを追加ページモーダル ](assets/add-connection-view-page-modal.png)

1. **ページ名** を追加し、「**接続されたレコードページ**」をクリックしてから、「**作成**」をクリックします。

   新しく接続されたレコードページが、新しいタブとしてレコードのページに追加されます。

   現在のレコードに接続されているレコードがテーブルビューに表示されます。

   >[!TIP]
   >
   >接続レコード ページに表示するには、レコードのテーブル領域または詳細領域に接続レコードを追加する必要があります。

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   接続されたレコードの最初の 5 つのフィールドは、デフォルトで表示されます。<!--No lookup fields display by default.-->

   ![ キャンペーンの詳細のオーディエンスに接続されたテーブル表示 ](assets/audience-connected-table-view-under-campaign-details-page.png)

1. （オプション）リスト内の接続されたレコードまたはオブジェクトタイプの名前を検索またはクリックします。

1. （オプションおよび条件付き）接続された Planning レコードまたはプロジェクト以外のWorkfrontオブジェクトを表示する場合は、接続されたレコード・ページのテーブル・ビューで、次のいずれかの操作を行います。<!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * レコードの名前をクリックします。 レコードのページが新しいタブで開きます。

   * テーブル ビューの下部にある [**接続**] をクリックしてさらにレコードを接続し、接続ボックスの外側をクリックしてレコードを閉じます。 新しいレコードが自動的にテーブルに追加されます。

     詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
   * テーブル表示で、接続されたレコードからの情報をインラインで編集します。

   * 接続されているレコードの名前にポインタを合わせ、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックします

     または

     レコードの 1 つを選択し、リストの下部にある青いバーで次のいずれかのオプションをクリックします。

      * **表示**：レコードページを新しいタブで開きます
      * **リンクをコピー** レコードページへのリンクをコピーする
      * **サムネールを編集** して「サムネールを記録 **ボックスを開き、レコードのサムネール画像を編集します**
      * **複製**：接続されたレコードを複製します。 複製されたレコードは、現在のレコードにも接続されます。
      * 接続されたレコードタイプに新しいレコードを追加するには、**上または下にレコードを挿入** します。 ここに追加された新しいレコードも、現在のレコードに接続されます。 このオプションは、テーブルでレコードを選択する際に青いバーでは使用できません。
      * **削除**：レコードを削除します。 接続されたレコードを削除すると、そのレコードの種類と、レコードが接続されているすべての場所からレコードが削除されます。

     テーブルビューでのレコードの編集については、[ レコードの編集 ](/help/quicksilver/planning/records/edit-records.md) を参照してください。

     >[!TIP]
     >
     >複数のレコードまたはオブジェクトを選択して削除できます。

   * 接続されたレコード ページのテーブル内の任意の Planning レコードをインライン編集します。

     その他のWorkfront オブジェクトは、読み取り専用のテーブルビューで表示され、編集することはできません。

1. （オプションおよび条件付き）接続されたレコードページのテーブルビューで、接続されたWorkfront プロジェクトを表示する際に、次のいずれかの操作を行います。

   * 接続されたレコードページの右上隅にある「**レコードを接続**」をクリックして、既存のプロジェクトを接続します。

   詳しくは、[レコードを接続する](/help/quicksilver/planning/records/connect-records.md)を参照してください。
   * テーブル内のインライン編集プロジェクト情報。
   * **新しい行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードにすぐに接続されます。

     詳しくは、[ レコードに関連付ける際に、Workfront Planning からWorkfront オブジェクトを作成する ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。
   * プロジェクトの上にマウスポインターを置き、**詳細** メニュー [ 詳細メニュー ](assets/more-menu.png) をクリックしてください

     または

     1 つ以上のプロジェクトを選択し、リストの下部にある青いバーに注目して、次のいずれかをクリックします。

      * **削除**：プロジェクトを削除します。 プロジェクトを削除すると、レコードから切断され、Workfrontのごみ箱に移動されます。
      * **切断**：レコードからプロジェクトを切断します。 プロジェクトの接続を解除すると、プロジェクトとその参照フィールドのすべての値が現在のレコードから削除されます。

1. （オプション）「**接続されたレコード」ページ** タブの名前をダブルクリックします

   または

   タブの名前にポインタを合わせて、**その他** ![ その他メニュー ](assets/more-menu.png) をクリックしてから、**名前を変更** をクリックして、新しい [ 接続されたビュー ] タブに名前を変更します。
1. （オプション）接続されたレコードページのツールバーで次のビュー要素のいずれかを使用して、テーブルビューを管理します。

   * フィルター
   * 並べ替え
   * グループ化
   * フィールド（フィールドの表示、非表示、並べ替えを行う）
   * 行の高さ
   * 検索

   詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

   >[!NOTE]
   >
   >接続されたレコードのタブのテーブル表示のフィールドを作成、編集、削除することはできません。

1. （オプション）接続されたレコードページのタブの名前にポインタを合わせ、「**詳細**![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、「**削除**」をクリックしてタブを削除します。