---
title: レコードを接続
description: レコードタイプ間の接続を作成したら、個々のレコードを相互に接続できます。 あるレコードの情報を別のレコードに接続すると、それらのレコードの情報を表示できます。
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 9a7ab1928bfd25c197fca65eddfba1bc01977ea7
workflow-type: tm+mt
source-wordcount: '3421'
ht-degree: 36%

---


# レコードの接続

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。 あるレコードの情報を別のレコードに接続すると、それらのレコードの情報を表示できます。

この記事では、レコードを接続する方法について説明します。 レコードの接続に関する一般的な情報については、[ 接続されたレコードの概要 ](/help/quicksilver/planning/records/connected-records-overview.md) を参照してください。

まず、2 つのレコードタイプを相互に接続するか、レコードタイプを別のアプリケーションのオブジェクトタイプに接続する必要があります。これにより、接続されたレコードフィールドが作成されます。 その後、接続されたレコードフィールドで、レコードを相互に接続したり、他のアプリケーションからレコードを他のオブジェクトに接続したりできます。

レコードの接続は、レコードを別のアプリケーションのオブジェクトに接続することと似ています。

レコードタイプの相互の接続や、レコードタイプの他のアプリケーションのオブジェクトタイプへの接続について詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

レコードタイプを連結する例については、[レコードタイプとレコードの連結例](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)を参照してください。

以下を連結することができます。

* Adobe Workfront計画レコード同士
* 他のアプリケーションからのオブジェクトを含む Adobe Workfront Planning レコード。

  次のアプリケーションから、レコードを以下に示すタイプのオブジェクトに接続できます。

   * Adobe Workfront

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * 会社
      * グループ

   * Adobe Experience Manager Assets

      * 画像ファイル
      * フォルダー

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <p> 以下のアプリケーションのオブジェクトを使用してレコードを関連付ける場合、Adobe Workfrontに加えて、以下が必要です。</p>
   <ul><li><p>Adobe Experience Manager Assets ライセンス、およびAEM Assets を Planning タイプと統合するためのAEM AssetsとWorkfrontの統合。</p>
   <p>詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials：記事インデックス </a> を参照してください。 </p></li>
   <li><p> レコードタイプとGenStudio ブランドを接続するためのAdobe GenStudio for Performance Marketing ライセンス</p>
   <p>詳しくは、<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketingの基本を学ぶ </a> を参照してください。</p></li></ul>
   </td> 
  </tr>   
<tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>WorkfrontおよびAEM Assetsで、接続先のオブジェクトのオブジェクトタイプを表示または上位アクセス権にする。 </p>  
</td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する投稿以上の権限と、レコードを接続するためのレコードタイプ。 </p>  
   <p>ワークスペースおよびレコードタイプに対する表示以上の権限。他のアプリケーションでのアクセス権に関係なく、他のアプリケーションからのオブジェクトおよびフィールドに対するすべての接続を表示します。 </p>
   <p>WorkfrontまたはExperience Manager Assetsからリンクするオブジェクトに対する表示以上の権限。 </p>
   <p>システム管理者は、自分が作成したものでないものも含めて、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li>
   <li><p>Adobe Experience Manager Assets, if you want to connect AEM assets with Planning records<p>
   <p>You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p>
   </li>  
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning objects</p> 
   <p>View or higher permissions to the object types you want to link from Workfront.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type to connect records </p>  
   <p>View or higher permissions to a workspace and record type to view all connections to objects and fields from other applications, regardless of your access in the other application. </p>
   <p>View or higher permissions to the objects you want to link from Workfront or Experience Manager Assets. </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p> </td> 
  </tr> 
</tbody> 
</table> -->

## レコードを接続する際の考慮事項

* レコードを他のレコードまたはオブジェクトと接続するには、次の条件を満たす必要があります。

   * 少なくとも 1 つのワークスペース、レコードタイプおよびレコード。

     詳しくは、次の記事を参照してください。

      * [ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)
      * [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)
      * [レコードの作成](/help/quicksilver/planning/records/create-records.md)

   * レコードタイプ間の接続や、レコードタイプと他のアプリケーションからのオブジェクト間の接続。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

* 1 つまたは複数のレコードまたはオブジェクトを相互に接続できます。 これは、レコードまたはオブジェクトの種類を接続するときに選択した接続の種類によって異なります。 詳しくは、[ レコードタイプの接続の概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

## Workfront Planning からレコードを接続

計画レコードの次の領域で、Workfront Planning のレコードを関連付けることができます。

* テーブル表示の接続されたレコードフィールド
* [ 詳細 ] タブの [ 接続されたレコード ] フィールドのレコードのプレビューボックスまたはページ。
* [ 接続 ] タブのレコードのプレビューボックスまたはページ。
* 接続されたレコードページタブのレコードのページ。

### テーブル表示またはレコードの詳細領域からWorkfront Planning レコードを接続します

{{step1-to-planning}}

1. レコードを接続するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. テーブルビューの名前をクリックして開きます。
1. （オプション）テーブルに新しい行を追加して、選択したレコードタイプにレコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプを別のレコードタイプに接続した後、レコードの接続されたフィールドに移動し、フィールド内をクリックするか、**接続** をクリックしてレコードを追加します。

   ![ 他のレコードをテーブル表示で接続 ](assets/connect-other-records-smaller-box-in-table-view.png)

1. 次のいずれかの操作を行います。

   * リストから接続されているレコードの名前をクリックして、選択したレコードに追加します。レコードは自動的に追加されます。
   * レコードの名前の入力を開始し、リストに名前が表示されたら選択します。レコードは自動的に追加されます。

   >[!TIP]
   >
   >レコードタイプが接続されたときにレコードの画像のみを表示するように選択した場合、接続されたフィールドにはサムネールまたはレコードのアイコンのみが表示されます。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
   >

1. （条件付き）レコードタイプを接続した際に、接続タイプとして「1 対多」または「1 対 1」を選択した場合、他の場所で接続されているレコードまたはオブジェクトを接続しようとすると、再度接続すると元の接続から削除されるという警告が表示されます。 **接続** をクリックして削除を許可してレコードを接続するか、**キャンセル** をクリックしてフィールドに戻って別のレコードを選択します。
1. （オプション）接続するオブジェクトが見つからず、追加する場合は、「**+追加」をクリックし** す。

   または

   オブジェクトの名前の入力を開始し、「**+追加**」をクリックしてオブジェクトを作成および追加します。

   詳細については、「レコードを作成する」の「他のレコードから接続する際にレコードを作成する [ を参照し ](/help/quicksilver/planning/records/create-records.md) ください。

   >[!TIP]
   >
   >    テーブル ビューで次の操作を行うと、レコードのページを開き、他のレコードを接続できます。
   >1. ビューでレコードの名前をクリックします。
   >1. リンクされたレコードフィールドを見つけ、フィールドをダブルクリックします（既に接続されているレコードがある場合）
   >または
   >**レコードを接続** （フィールドが空の場合）をクリックして、接続されたレコードまたはオブジェクトタイプからレコードを追加します。
   >
   >![ レコードページからレコードを接続フィールド ](assets/connect-records-from-record-page-field.png)

1. （任意）すべてのレコードを表示するには、「**すべて表示**」をクリックします。

1. （条件付き）前の手順で「**すべて表示**」をクリックした場合、「**オブジェクトを接続**」ボックスが表示されます。

   ![ レコード用の接続オブジェクト テーブル ](assets/connected-objects-table-for-records.png)

1. 検索ボックスにレコード名を入力していき、リストに表示されたら選択します

   または

   ボックス内の 1 つまたは複数のレコードの名前を選択し、[**オブジェクトを接続**] をクリックします。

   以下が追加されます。

   * リンクされたレコードは、前の手順で選択したレコードの「リンクされたレコード」フィールドに表示されます。
   * レコードタイプを接続したときにリンクされたルックアップフィールドを追加した場合、リンクされたフィールドには、リンクされたレコードからの情報が入力されます。

   リンクされたレコードを更新すると、リンク元のレコードのリンクされたフィールドも自動的に更新されます。リンクされたフィールドは手動で編集できません。

   >[!TIP]
   >
   >* 「リンクされたフィールド」と「ルックアップフィールド」は同じ意味で使用されます。
   >
   >* レコードタイプを接続したときに複数のレコードを接続するように選択した場合、複数のオブジェクトからのフィールド値は、コンマで区切って表示されるか、レコードタイプの接続時に選択した集計に従って集計されます。
   >* Workfrontの先行入力フィールド（「プロジェクト所有者」や「プロジェクトスポンサー」などのフィールドを含む）を参照フィールドとして追加することはできません。
   >
   >* Workfront オブジェクトの日付フィールドの情報は、Workfront Planning では、Workfrontでの表示方法に関係なく、24 時間形式で表示されます。
   >
   >   例えば、プロジェクトの予定開始日がWorkfrontで午後 3:00 と表示された場合、Workfront Planning の読み込まれた参照フィールドでは 15:00 と表示されます。

1. （オプション）レコードタイプページを閉じて、選択したワークスペースに移動します。
1. リンク先のレコードタイプのカードをクリックします。

   例えば、**キャンペーン**&#x200B;レコードを製品レコードに接続した場合は、**製品**&#x200B;カードをクリックします。

   レコードタイプカードがテーブル表示で開きます。 そうでない場合は、テーブルビューを選択します。

   **キャンペーン**&#x200B;にリンクされたレコードフィールドには、製品レコードタイプのページで製品にリンクしたキャンペーンの名前が表示されます。キャンペーン情報を更新すると、製品レコードタイプのキャンペーンにリンクされたレコードフィールドが自動的に更新されます。

### レコードのテーブル表示または詳細領域から、Workfront Planning レコードをWorkfront オブジェクトに接続します

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

レコードタイプとWorkfront オブジェクトタイプの間の関連付けを作成したら、個々のレコードをWorkfrontのオブジェクトに関連付けることができます。 接続した Workfront フィールドは、オブジェクトのリンク元のレコードに自動的に入力されます。

>[!NOTE]
>
>Workfront オブジェクトタイプをWorkfrontのWorkfront Planning レコードタイプに関連付けることはできません。


{{step1-to-planning}}

1. レコードを接続するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。
1. レコードタイプのカードをクリックして、レコードタイプページを開きます。
1. **ビュー**&#x200B;ドロップダウンメニューから&#x200B;**テーブル**&#x200B;ビューを選択します。

1. 「**新規レコード**」をクリックして、選択したレコードタイプに個別のレコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。

1. （条件付き）選択したレコードタイプをWorkfront オブジェクトタイプに関連付けた後、レコードの接続されたフィールドに移動して、フィールドをクリックするか、「**接続**」をクリックしてWorkfront オブジェクトを追加します。

   ![ テーブル表示でのプロジェクトの接続 ](assets/connect-projects-smaller-box-in-table-view.png)

1. 次のいずれかの操作を行います。

   * リストからオブジェクトをクリックして、選択したレコードに追加します。オブジェクトはアルファベット順にリストされます。オブジェクトは自動的に追加されます。
   * オブジェクトの名前の入力を開始し、リストに名前が表示されたらクリックします。オブジェクトは自動的に追加されます。

   >[!TIP]
   >
   >ビューからレコードのページを開き、リンクされたレコードフィールドをダブルクリックするか、フィールドの **接続** をクリックして、接続されたオブジェクトタイプからオブジェクトを追加できます。

1. （オプション）接続するオブジェクトが見つからず、追加する場合は、「**+追加」をクリックし** す。

   または

   オブジェクトの名前の入力を開始し、「**+追加」をクリックして** 新しいプロジェクト、ポートフォリオまたはプログラムを作成して追加します。

   詳しくは、[Workfront計画からのWorkfront オブジェクトの作成 ](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md) を参照してください。

1. （オプション）「**すべて表示**」をクリックすると、少なくとも表示権限を持つすべてのオブジェクトが表示されます。

   前の手順で「**すべて表示**」をクリックすると、「**オブジェクトを接続** ボックスが表示されます。

   ![ プロジェクトを選択するには「オブジェクトを接続」ボックス ](assets/connect-objects-box-to-select-projects.png)

1. 検索ボックスに Workfront オブジェクト名を入力していき、リストに表示されたら選択します

   または

   ボックス内の 1 つまたは複数のオブジェクトの名前を選択し、**オブジェクトを接続** をクリックします。

   >[!IMPORTANT]
   >
   >* 表示のアクセス権限のある Workfront オブジェクトのみを追加できます。
   >
   >* Workfront オブジェクトを追加すると、ワークスペースに対する表示権限以上の権限を持つすべてのユーザーは、Workfront での権限やアクセス権に関係なく、Workfront オブジェクトとそのフィールド情報を表示できるようになります。

   次のものが追加されます。

   * 選択した Workfront オブジェクトが、リンクされたレコードフィールドに追加されます。
   * レコードタイプを Workfront に接続するときにこれらを追加した場合、Workfront オブジェクトのリンクされたフィールド（またはルックアップフィールド）には、Workfront からの情報が自動的に入力されます。

   レコードタイプと別のアプリケーションのオブジェクトの接続について詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

1. （オプション）テーブルビューのリンクされたフィールド、またはレコードページのリンクされたフィールドで、Workfront Planning レコードに接続されている Workfront オブジェクトの名前をクリックします。

   少なくともオブジェクトに対する表示権限がある場合、これによりWorkfrontにWorkfront オブジェクトが開きます。

   >[!TIP]
   >
   >* レコードタイプを接続するときに複数のレコードを接続することを選択した場合、ルックアップフィールドの値は、コンマで区切って表示されるか、選択したアグリゲータに従って集計されます。
   >
   >* Workfront のリンクされた Workfront オブジェクトに対して、リンクされたレコードフィールドは作成されません。

1. （オプション）レコードタイプのテーブルビューで、リンクされた Workfront オブジェクトの列ヘッダーにポインタを合わせ、ドロップダウンメニューをクリックして、「**ルックアップフィールドを編集**」をクリックします。

1. **選択されていないフィールド**&#x200B;エリアから Workfront オブジェクトフィールドを追加します。

   または

   **選択されたフィールド**&#x200B;エリアから、Workfront オブジェクトフィールドを削除します。

   これにより、リンクされたフィールドが Workfront Planning レコードに追加または削除されます。削除されたフィールドに関連付けられた情報は Workfront に残ります。


### レコードのテーブル表示または詳細領域から、Workfront Planning レコードをAdobe Experience Manager オブジェクトに接続します

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Workfront Planning レコードを Adobe Experience Manager Assets に接続するには、Adobe Experience Manager Assets ライセンスが必要であり、組織の Workfront インスタンスが Adobe Business Platform または Adobe Admin Console にオンボーディングされている必要があります。
>
>Adobe Admin Console のオンボーディングについて質問がある場合は、[Adobe Unified Experience の FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md) を参照してください。

レコードタイプと Adobe Experience Manager Assets 間の接続を作成した後、個別のレコードを Experience Manager Assets に接続できます。接続の作成時に Experience Manager Assets から接続したアセットフィールドは、リンク元のレコードタイプで自動的に入力されます。

>[!NOTE]
>
>Planning レコードとそのフィールドには、Experience Manager AssetsとAdobe Experience Manager Assets間の統合を通じてWorkfront管理者がメタデータ・マッピングを構成する際に、Workfrontからアクセスできます。 詳しくは、[Adobe WorkfrontとExperience Manager Assets間のアセットメタデータのマッピングの設定 ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) を参照してください。

レコードをExperience Manager Assets に接続するには：

{{step1-to-planning}}

1. レコードを接続するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプが表示されます。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. レコードタイプページの右上隅にある&#x200B;**ビュー**&#x200B;ドロップダウンメニューから、**テーブル**&#x200B;ビューを選択します。

1. （オプション）「**新規レコード**」をクリックして、選択したレコードタイプに新規レコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
1. （条件付き）選択したレコードタイプをExperience Manager Assetsに関連付けた後、レコードの接続されたフィールドに移動して、フィールドをクリックするか、**接続** をクリックしてExperience Manager アセットをレコードに追加し、**+** アイコンをクリックします。

   >[!TIP]
   >
   >  レコードページのリンクされたオブジェクトフィールドにある **+** アイコンをクリックして、アセットをレコードに接続できます。

   「**アセットを選択**」ボックスが表示されます。<!--we might change this to Connect assets-->

   ![AEM レコード接続用の「アセットを選択」ボックス ](assets/select-assets-box-for-aem-record-connections.png)

1. 次のタイプのアセットのいくつかをクリックして選択します。

   * 画像
   * フォルダー

   複数のアセットを選択できます。

   >[!IMPORTANT]
   >
   > 接続できるのは、Experience Manager で表示するアクセス権のあるアセットのみです。接続すると、すべての Workfront Planning ユーザーは、Experience Manager Assets へのアクセス権に関係なく、Workfront Planning でアセットを表示できます。

1. 「**選択**」をクリックします。<!-- we might change this to Connect-->

   次のものが追加されます。

   * 選択した Experience Manager Assets が、リンクされたレコードフィールドに追加されます。
   * リンクされたフィールド（またはルックアップフィールド）には、Experience Manager に接続されたアセットからの情報が入力されます。

     Experience Manager Assets のフィールドからのすべての既存の情報は、リンクされたフィールドまたはルックアップフィールドに自動的に表示されます。

     >[!TIP]
     >
     >* レコードタイプを接続するときに複数のレコードを接続することを選択した場合、複数のオブジェクトの値がコンマで区切られているか、選択したアグリゲータに従って集計されて表示されます。
     >
     >* Workfront Planning にリンクされたレコードへのリンクされたレコードフィールドは、Experience Manager Assets アプリケーションのリンクされた Experience Manager アセットに対しては作成されません。

1. （オプション）Experience Manager Assets にリンクしたレコードタイプに移動し、リンクされたレコードフィールド内のアセットの名前をクリックします。アセットのExperience Managerの詳細がポップアップウィンドウに表示されます。

   ![AEMの詳細とサムネールを含むアセットポップアップウィンドウ ](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   画像ファイルには、次のフィールドが表示されます。

   * 画像のサムネール
   * 画像ファイル名
   * 寸法
   * サイズ
   * 説明
   * Experience Manager のファイルパス
   * アセットタイプ
   * 作成日
   * 変更日時

1. （オプション）Experience Manager Assets のレコードページをExperience Managerで開くには、リンク元のレコードのレコードタイプページに移動し、「リンクされたレコード」フィールドでアセットの名前をクリックしてポップアップウィンドウを開き、**AEMで開く** アイコン ![AEMでアセットを開く ](assets/open-asset-icon.png) をクリックしてアセットを開きます。

   これにより、Adobe Experience Manager Assets で Experience Manager のアセットが開きます。

1. （オプション）レコードタイプのテーブルビューで、リンクされた Experience Manager のアセットの列ヘッダーにポインタを合わせ、ドロップダウンメニューをクリックし、「**ルックアップフィールドを編集**」を選択します。

1. **選択されていないフィールド**&#x200B;エリアから、Experience Manager Assets オブジェクトフィールドを追加します。

   または

   **選択されたフィールド**&#x200B;エリアから、Workfront オブジェクトフィールドを削除します。

   これにより、リンクされたフィールドがレコードに追加または削除されます。削除されたフィールドに関連付けられた情報は、Adobe Experience Assets に残ります。

### レコードページの「接続」タブで、Workfront Planning レコードと他のレコードまたはオブジェクトを接続します

1. 他の Planning レコード・タイプまたは他のアプリケーションのオブジェクト・タイプに接続されているレコード・タイプの任意のビューに移動します。
1. 他のレコードまたはオブジェクトと接続するレコードをビューで検索するには、前のサブセクションで説明した手順に従います。
1. レコードの名前をクリックします。

   プレビューページが開きます。
1. （オプション） **新しいタブで開く** アイコン ![ 詳細を新しいタブアイコンで開く ](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを新しいブラウザータブで開きます。
1. （オプションおよび条件付き）レコードページヘッダーのパンくずリストにあるレコードタイプの名前をクリックして、同じ階層内の別のレコードタイプにアクセスします。 階層は、接続しているレコードのレコードタイプに対して存在する必要があります。階層は、パンくずリストで表示できるようになります。 詳しくは、[ ワークスペース階層の作成 ](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) を参照してください。
1. レコードのプレビューまたはページで、「**接続**」タブをクリックします。

   ![Workfront Planning のレコードの「接続」タブ ](assets/connections-tab-on-record-in-workfront-planning.png)

   選択したレコードタイプにリンクされているすべてのレコードタイプまたはオブジェクトタイプがセクションとして表示されます。 接続されたレコードまたはオブジェクトは、カード上のレコードまたはオブジェクトタイプの名前の下に表示されます。

   >[!TIP]
   >
   >    デフォルトでは、個々のレコードが接続されている接続レコードのみが表示されます。

1. （省略可能） [**すべての接続を表示**] をクリックすると、接続されたすべてのレコードの種類（接続されていないレコードを含む）が表示されます。

1. （オプション）セクションを折りたたむには、セクションの左側にある下向き矢印をクリックします。

1. （条件付き）同じタイプのレコードまたはオブジェクトをさらに追加するには、「**接続**」をクリックします。
1. （オプション）接続するレコードまたはオブジェクトが見つからず、追加する場合は、[**+追加 ] をクリックします**

   または

   オブジェクトの名前の入力を開始し、「**+追加**」をクリックしてオブジェクトを作成し、レコードに追加します。

   詳細については、「レコードを作成する」の「他のレコードから接続する際にレコードを作成する [ を参照し ](/help/quicksilver/planning/records/create-records.md) ください。
1. 前の節で説明した手順に従って、Workfront Planning のレコードまたはWorkfrontやExperience Manager Assetsのオブジェクトを接続します。
レコードとオブジェクトが直ちに追加されます。
1. （オプション）レコードまたはオブジェクトの接続されたカードにポインタを合わせ、「**レコードを切断**」アイコン ![ レコードを切断 ](assets/disconnect-icon-with-tooltip.png) をクリックして、選択したレコードとの接続を切断します。

   ![ 「接続」タブのレコードを切断アイコンとツールチップ ](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   レコードは、Workfront Planning のすべての領域、または接続済みと表示される可能性のある他のアプリケーションから直ちに切断されます。 参照フィールドの値も削除されます。

### レコードの接続されたレコード ページからレコードを接続

1. 他の Planning レコード・タイプまたは他のアプリケーションのオブジェクト・タイプに接続されているレコード・タイプの任意のビューに移動します。
1. 他のレコードまたはオブジェクトと接続するレコードをビューで検索するには、前のサブセクションで説明した手順に従います。
1. レコードの名前をクリックします。

   プレビューページが開きます。
1. （オプション） **新しいタブで開く** アイコン ![ 詳細を新しいタブアイコンで開く ](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを開きます。
1. レコードのページで、既存の **接続されたレコードページ** タブをクリックします。 最初に **接続されたレコードページ** を作成する必要があります。

   接続されたレコードタイプのページがテーブル表示に表示されます。

   1 つのタイプの接続レコードがすべてテーブルに表示されます。

   >[!TIP]
   >
   >接続レコード ページに表示するには、接続レコードをカレント レコードに追加する必要があります。

1. レコードのリストの **接続** またはプロジェクトのリストの **レコードの接続** をクリックして、既存のレコードまたはプロジェクトを追加または削除します。

   ![ 接続されたレコードの詳細タブでハイライト表示された「接続」ボタン ](assets/connect-button-highlighted-in-connected-record-details-tab.png)

   詳しくは、[ 接続されたレコードページのレコードへの追加 ](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) を参照してください。
1. プロジェクトのリストで **新規行** をクリックして、テンプレートを使用せずにプロジェクトを作成します。 新しいプロジェクトは、現在のレコードに自動的に接続されます。
1. （オプション）接続されたレコードが見つからない場合は、「**+追加**」をクリックして作成し、接続します。

## Workfront オブジェクトからのレコードの接続

Workfront オブジェクトからWorkfront計画レコードを接続するには、次のものが必要です。

* Workfront Planning で確立されたレコード・タイプとWorkfrontオブジェクト・タイプ間の関連付け。
* Workfrontまたはグループ管理者が、Workfront オブジェクトタイプに次のいずれかを追加する必要があります。

   * 計画セクションは、レイアウトテンプレート内のWorkfront プロジェクト、ポートフォリオおよびプログラムに適用されます。

   * Planning 接続のカスタム・フィールドは、次のいずれかのオブジェクトのカスタム・フォームに対して使用します。

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * グループ
      * 会社

  詳しくは、[Workfront オブジェクトからのレコード接続の管理 ](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。
