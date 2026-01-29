---
title: レコードタイプを接続
description: 個々のレコードタイプが互いにどのように関連しているかは、レコードタイプを連結するとよくわかります。また、Workfront Planning のレコードタイプを他のアプリケーションのオブジェクトタイプに接続して、ユーザーのエクスペリエンスを向上させ、ユーザーが 1 つのアプリケーションに集中できるようにすることもできます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 665e753880be59cf07062d75c66a7be5f2056aa1
workflow-type: tm+mt
source-wordcount: '2952'
ht-degree: 25%

---


<!--keep the 30 fields limit in yellow till Jan 2026; also the global record type cross-workspace capability information-->

<!--take production and preview references out at prod-->

# レコードタイプを接続

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

レコードタイプを相互に接続することも、レコードタイプを他のアプリケーションのオブジェクトタイプと接続することもできます。

相互に影響を与える複数のタイプの作業オブジェクトがある場合、レコード タイプを接続すると便利です。 例えば、キャンペーンを扱う場合に、各キャンペーンが複数のブランドに対応している可能性があります。 この関係を示すために、キャンペーンをブランドに接続できます。 これにより、キャンペーンレコードにブランド用の接続フィールドが作成されます。

さらに、各キャンペーンの作業は、Workfrontの複数のプロジェクトで計画される可能性があります。 これを示すには、キャンペーンを関連するプロジェクトに接続します。 これにより、キャンペーンレコードにプロジェクト用の接続フィールドが作成されます。

接続フィールドを作成したら、2 つのレコード タイプまたはオブジェクト タイプ間で個々のレコードを接続できます。

>[!NOTE]
>
>1 つのレコードタイプに対して最大 30 個の接続フィールドを持つことができます。

ここでは、2 つのWorkfront Planning レコードタイプまたは 1 つのWorkfront Planning レコードタイプを別のアプリケーションのオブジェクトに関連付ける方法について説明します。

レコード間またはオブジェクト タイプ間の接続を確立すると、接続フィールドが Planning レコード タイプに追加されます。 「接続」フィールドでは、個々のレコードを相互に接続し、リンクされたレコードまたはオブジェクトタイプのフィールドをWorkfront Planning レコードに表示できます。

接続タイプに関する一般的な情報については、[ 接続されたレコードタイプの概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

レコードまたはレコードを他のアプリケーションのオブジェクトと接続する方法については、「[ レコードを接続する ](/help/quicksilver/planning/records/connect-records.md)」を参照してください。

レコードタイプとレコードの接続例については、[ レコードタイプとレコードの接続例 ](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md) を参照してください。

<!--ensure this last linked article is right; the title and the link should have changed-->


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
<p>同じワークスペースからレコードタイプを接続するには： </p>
<ul> 
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
<li><p>任意のワークフローおよび任意の計画パッケージ</li></ul>

<p>異なるワークスペースからレコードタイプを接続するには、次の手順に従います。</p>

<ul> 
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
<tr> 
<td> 
   <p> その他の製品</p> </td> 
   <td> 
   <p> 以下のアプリケーションのオブジェクトを使用してレコードタイプを関連付ける場合は、Adobe Workfrontに加えて、以下が必要です。</p>
   <ul><li><p>Adobe Experience Manager Assets ライセンス、およびAEM Assets を Planning レコードタイプと統合するためのAEM AssetsとWorkfrontの統合。</p>
   <p>詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials：記事インデックス </a> を参照してください。 </p></li>
   <li><p> レコードタイプとGenStudio ブランドを接続するためのAdobe GenStudio for Performance Marketing ライセンス</p>
   <p>詳しくは、<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketingの基本を学ぶ </a> を参照してください。</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
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
   <li><p> Adobe Experience Manager Assets, if you want to connect AEM assets with Planning record types<p>
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
   <td> <p>Standard</p> 
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p></td> 
  </tr> 
 
</tbody> 
</table> -->

## レコードタイプの接続

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. レコードタイプを接続するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. テーブルビューの右上隅にある **+** アイコンをクリックし、「**新しい接続**」タブをクリックします。

   ![Workfront AEMのオプションを含む新しい「接続」タブ ](assets/new-connection-tab-with-workfront-aem-options-no-buttons.png)

1. レコードタイプを検索するか、次のいずれかを選択します。

   * 現在のワークスペースからのレコードタイプ

     ![ 同じワークスペースレコードタイプの複数選択接続ピッカー ](assets/multi-select-connection-picker-record-type.png)

     >[!TIP]
     >
     > 
     >選択したワークスペースに他のレコードタイプがない場合、ワークスペースセクションは表示されません。

   * 他のワークスペースから接続するように設定された、別のワークスペースからのレコードタイプ。

     >[!TIP]
     >
     >他のワークスペースからレコードの種類にアクセスできるようにするには、[**レコードの種類の編集**] ボックスの [**ワークスペース間の設定**] タブで、**他のワークスペースでこのレコードの種類への接続を許可する** 設定をレコードの種類に対して有効にする必要があります。 他のワークスペースから接続するように設定されているレコードタイプがない場合、「ワークスペース」セクションは表示されません。
     >
     >詳しくは、[ レコードタイプのクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。<!--update screen shot at production-->
     >
     >![ 「レコードタイプを編集」ボックスのクロスワークスペース設定タブ ](assets/edit-record-type-box-advanced-settings-tab.png)

     <!--Old:
        [!TIP]
        The **Allow connecting to this record type in other workspaces** setting must be enabled for a record type in the **Advanced settings** tab of the **Edit record type** box, for a record type to be accessible from other workspaces. If there are no record types that are configured to connect from other workspaces, the workspace section does not display.
        ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
        -->

   詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

   * 「**Workfront オブジェクトタイプ**」セクションからの&#x200B;**プロジェクト、ポートフォリオ、プログラム、会社**&#x200B;または&#x200B;**グループ**。

     ![Workfront プロジェクト連携の選択 ](assets/multi-select-connection-picker-project.png)

   <div class="preview">

   * **2}Workfrontのオブジェクトタイプ** セクションの { 元のリクエスト **オブジェクトタイプ。**

     作成された元のリクエスト接続フィールドには、オブジェクトを作成した送信された Planning リクエストの名前が表示されます。

     >[!NOTE]
     >
     >Workfront Planning でレコードを作成するための Planning リクエストを発行するには、リクエスト・フォームを作成して公開する必要があります。
     >
     >詳しくは、次の記事を参照してください。
     >* [Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md)
     >* [ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md)。

     ![ 元のリクエスト接続の選択 ](assets/original-request-connection-selection.png)

   </div>


   * 「**Adobe アプリケーション**」セクションからの **Experience Manager Assets**。

     ![AEM Assets接続の選択 ](assets/aem-assets-connection-selection.png)

     選択したレコードまたはオブジェクト タイプの [ 新しい接続 ] タブが開きます。

   * **2}Adobe GenStudio** セクションのAdobe GenStudio for Performance Marketingの **ブランド }**

     ![GenStudio Brand 接続の選択 ](assets/brand-genstudio-connection-selection.png)

1. **名前** フィールドを、新しく接続されたフィールドの名前で更新します。この名前は、元のレコードタイプのテーブルビューまたはレコードページに表示されます。 これにより、元のレコードタイプのテーブル表示に接続されたレコード列（またはフィールド）が作成されます。 デフォルトでは、フィールド名は接続先のレコードまたはオブジェクトの名前です。

   >[!TIP]
   >
   >同じレコードまたはオブジェクトタイプへの複数の接続を持つことができます。 連結フィールド名を編集しない場合、Workfrontでは、連結されたレコードの名前の後に数字が追加され、連結されたレコードの種類の数が同じ名前で示されます。

1. 接続レコードフィールドに関する情報を追加して、「**説明**」フィールドを更新します。 フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
1. （条件付き） 2 つの異なるワークスペース（レコードタイプとAdobe Experience Manager アセットオブジェクト、またはレコードタイプとGenStudio ブランド）のレコードタイプを関連付ける場合は、「**複数のレコードを許可**」を選択します。 これを選択すると、元のレコードに「接続されたレコードタイプ」フィールドが表示されたときに、ユーザーが複数のレコードを追加できるように指定できます。 これはデフォルトで選択されています。

   ![ 別のワークスペースからのレコードタイプへの新しい接続 ](assets/new-connection-allow-multiple-records-box.png)

1. （条件付き）同じワークスペースのレコードタイプを接続する場合、または Planning レコードタイプをWorkfront オブジェクトタイプに接続する場合は、次のいずれかを選択します。

   * **複数選択**：現在のレコードタイプの 1 つのレコードを、接続レコードタイプの複数のレコードに接続できるようにするには、これを選択します。
   * **単一選択**：現在のレコードタイプの 1 つのレコードを、接続レコードタイプの 1 つのレコードと接続する場合に選択します。

1. **リンクされたレコードタイプに対応するフィールドを作成** を選択します。 選択すると、現在のレコードタイプに追加された接続フィールドに加えて、接続先のレコードタイプに接続フィールドが作成されます。 これはデフォルトでは無効になっています。

   >[!TIP]
   >
   >* 1 つのレコードタイプに対して 30 個の接続フィールドという制限に加えて、1 つのレコードタイプに対して 500 個のフィールドという制限があります。 この制限に達するのを避けるために、特に分類レコードタイプでは、この設定をオフにすることをお勧めします。
   >
   >* **リンクされたレコードタイプに対応するフィールドを作成** を選択することは、階層を作成するための前提条件です。

1. （条件付き） **リンクされたレコードタイプに対応するフィールドを作成** を有効にした場合は、次のオプションから選択して、ユーザーが接続できるレコード数と接続できるレコード数を示します。

   * 多対多
   * 1 対多
   * 多対 1
   * 1 対 1

   接続タイプについて詳しくは、[ 接続されたレコードタイプの概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

   >[!NOTE]
   >
   >接続の種類に [ 一対多 ] または [ 一対一 ] を選択した場合、後で他の場所に既に接続されているレコードまたはオブジェクトを接続しようとすると、再度接続すると元の接続から削除されるという警告が表示されます。 削除を許可するか、別のレコードを選択できます。

1. （条件付きおよびオプション）Workfront オブジェクトを接続することを選択した場合は、「**これらの条件に一致するオブジェクトのみをリンク** セクションから **カスタムフォーム** を選択します。 選択したカスタムフォームがアタッチされているオブジェクトのみを、選択したレコードタイプにリンクできます。複数のフォームを選択できます。

   >[!NOTE]
   >
   > このリストに表示される前に、選択したオブジェクトのカスタムフォームを Workfront で作成する必要があります。

1. （条件付き）Experience Manager Assetsへの接続を選択する場合、「**次のリポジトリーからアセットをリンク**」セクションのExperience Manager リポジトリー **ドロップダウンメニューからリポジトリーを選** します。 必須フィールドです。このフィールドには、Experience Manager Assets でアクセス権のあるリポジトリのみが表示されます。

   >[!NOTE]
   >
   >Workfront管理者は、Workfrontのメタデータマッピングを使用して、Workfront Planning フィールドをExperience Manager Assets フィールドにマッピングできます。 詳しくは、[Adobe WorkfrontとExperience Manager Assets間のアセットメタデータのマッピングの設定 ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) を参照してください。


1. （条件付き）Experience Manager Assets、Workfront Planning レコードタイプ、またはGenStudio ブランドに接続する場合は、**レコードの外観** 領域で次のいずれかのオプションを選択します。

   * **名前と画像**：接続されたレコードの名前とサムネールまたはアイコンの両方が「接続されたレコード」フィールドに表示されます。 これはデフォルトのオプションです。
   * **名前**：接続されたレコードの名前のみが、「接続されたレコード」フィールドに表示されます。
   * **画像**：接続されたレコードのサムネールまたはアイコンのみが「接続されたレコード」フィールドに表示されます。

   サムネール画像のないレコードには、代わりにレコードタイプアイコンが表示されます。 接続されたレコードの表示方法の例は、**レコードの外観** 領域に表示されます。

   >[!NOTE]
   >
   >* 複数のレコードをリンクできるようにすると、サムネールのみを表示して、レコードビューなどの小さな領域のスペースを節約できる場合があります。
   >
   >* レコードの名前は、レコードのプライマリフィールドです。 詳しくは、[プライマリフィールドの概要 ](/help/quicksilver/planning/fields/primary-field-overview.md) を参照してください。
   >
   >* Workfront オブジェクトタイプを選択する場合、レコードの外観は使用できません。
   >
   >* 「レコードの外観」領域で選択した内容によって、すべてのビューおよび詳細ページを含む、システム内のすべての接続でのレコードの表示方法が決まります。

1. **参照フィールドを選択** を選択して、接続先のレコードタイプからフィールドを追加します。 ルックアップフィールドは、リンク先のレコードタイプまたはオブジェクトタイプに関連付けられたフィールドです。リンクすると、リンク元のレコード上のリンク先のレコードまたはオブジェクトの情報が表示されます。 これはデフォルトで選択されています。

   >[!TIP]
   >
   >* Workfrontの先行入力フィールド（「プロジェクト所有者」や「プロジェクトスポンサー」などのフィールドを含む）を参照フィールドとして追加することはできません。
   >
   >* Workfront オブジェクトの日付フィールドの情報は、Workfront Planning では、Workfrontでの表示方法に関係なく、24 時間形式で表示されます。
   >
   >   例えば、プロジェクトの予定開始日がWorkfrontで午後 3:00 と表示された場合、Workfront Planning の読み込まれた参照フィールドでは 15:00 と表示されます。
   >* 実稼動環境では、人物フィールドをルックアップフィールドとして追加できません。 <span class="preview"> 人物フィールドをプレビュー環境のルックアップフィールドとして追加できます。</span>
   >

1. 「**作成**」をクリックします。

1. （条件付き）**ルックアップフィールドを選択**&#x200B;設定を選択した場合、「**ルックアップフィールドを追加**」ボックスが開きます。

   **+** アイコンをクリックして、**選択されていないフィールド**&#x200B;エリアからフィールドを追加します。

   または

   **-** アイコンをクリックして、**選択されたフィールド**&#x200B;エリアからフィールドを削除します。

   ![[ 他のレコード タイプのルックアップ フィールドを追加する ] ボックス ](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   レコードやオブジェクトをリンクした後、接続されたフィールドの値が自動的に入力されます。

   >[!IMPORTANT]
   >
   >    ワークスペースに対する表示権限以上の権限を持つユーザーは、リンクされたオブジェクトタイプのアプリケーションでの権限やアクセスレベルに関係なく、リンクされたフィールドの情報を表示できます。

1. （省略可能）リンク レコードまたはオブジェクト タイプからのフィールドの追加をスキップするには、[**スキップ**] をクリックします。 リンクされたレコードの名前またはプライマリフィールドは、リンク元のレコードの種類のテーブル ビューに表示される唯一のフィールドです。

1. 追加する参照フィールドのアグリゲータを選択します。

   >[!NOTE]
   >
   >次のフィールドタイプでは、アグリゲータを追加できません。
   >
   >    * 段落
   >    * チェックボックス

   ユーザーがリンクされたレコードフィールドで複数のリンクされたレコードを選択すると、リンクフィールドの値がコンマで区切られているか、選択したアグリゲータに従った集計値として表示されます。

   集計されていない複数の値がルックアップ フィールドに含まれている場合、このフィールドをビューで並べ替えまたはグループ化で使用する際は、次の点を考慮してください。

   * 並べ替えは最初の値で行われます

   * レコードは、フィールド値の一意の組み合わせごとにグループ化されます

   * タイムラインビューは、接続されたレコードタイプの最初の日付値がビューに表示されるかどうかに基づいて構築されます

   >[!IMPORTANT]
   >
   > 参照日フィールドをタイムライン ビューとカレンダービューの開始日および終了日として追加できるようにする場合は、フィールドを追加するときにアグリゲータ値を選択する必要があります。 例えば、参照日フィールドには、MAXまたは MIN アグリゲータを選択できます。

   ![ リンクされた数値フィールドのアグリゲータドロップダウン ](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > レコードタイプを次に接続する場合、アグリゲータは使用できません。
   >* Experience Manager Assets
   >* GenStudioブランド。
   >

   次の中から選択します。

   * **なし**：複数のレコードから取得された値をコンマで区切って表示します。これはデフォルトの選択です。
   * **最大**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の最大値を表示します。
   * **最小**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の最小値を表示します。
   * **合計**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の合計を表示します。
   * **平均**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の平均を表示します。
   * **UNIQUE**：ルックアップフィールドの値から重複を削除し、一意の値のみを表示します。 これは、次のフィールドタイプでは使用できません。
      * 段落
      * チェックボックス
      * ユーザー

   >[!NOTE]
   >
   >例えば、キャンペーンレコード（元のレコード）から製品レコード（リンクされたレコード）をリンクし、「製品フィールド」という名前を付けることができます。 また、キャンペーンレコードから製品レコードの「予算」フィールドをリンクし、「製品予算」と呼ぶこともできます。 「製品フィールド」で複数のレコードを選択できる場合、「予算$100,000」の製品 1 と「予算$110,000」の製品 2 および「予算$100,000」の製品 3 を選択できます。 選択したアグリゲータに応じて、元のレコードから、リンクされたフィールドに次の予算情報を表示できます。
   >
   >* **なし**: $100,000、$110,000、$100,000
   >* **MAX**: 110,000 ドル
   >* **最小**：100,000 ドル
   >* **合計**:310,000 ドル
   >* **AVG**: 103,000.33 ドル
   >* **一意**:100,000 ドル
   >

1. （オプション） **検索** アイコン ![ 検索アイコン ](assets/search-icon.png) を使用して、フィールドを検索します。

1. 「**フィールドを追加**」をクリックして変更を保存します。

   次のアイテムが追加されます。

   * リンク元のレコードタイプ上のリンクされたレコードフィールド。リンクされたレコードタイプの個別のレコードが手動で追加された後、リンクされたレコードフィールドに表示されます。レコードの追加について詳しくは、[レコードを接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。リンクされたレコードフィールドの名前は、手順 6 で選択した名前です。<!--accurate-->

   * リンク レコード フィールドにレコードまたはオブジェクトを手動で追加した後、リンク レコードまたはオブジェクト タイプに関する情報を表示するリンク （またはルックアップ） フィールド。 ルックアップ フィールドは、接続の作成時に **ルックアップ フィールドを選択** 設定が選択されている場合にのみ作成されます。 参照フィールドには、次のパターンに従って自動的に名前が付けられます。

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     例えば、キャンペーンレコードタイプをプログラムレコードタイプにリンクし、「プログラムリンクされたレコード」フィールドに「プログラム情報」という名前を付け、キャンペーンのテーブルビューにプログラムの「予算」フィールドも表示するように選択した場合、リンクされたフィールドの名前は、キャンペーンのテーブルビューで自動的に `Budget (from Program information)` になります。

   * レコードタイプを相互にリンクさせると、「**リンクされたレコードタイプに対応するフィールドを作成**」設定を有効にした場合にのみ、リンク先のレコードタイプにリンクされたレコードフィールドも追加されます。 リンクされたレコードタイプでのリンクされたレコードフィールドの名前は、リンク元のレコードタイプの名前です。

     例えば、「キャンペーン」レコードタイプから「製品」レコードタイプをリンクし、キャンペーンの「リンクされた製品」の接続フィールドに名前を付けると、製品レコードタイプに対して「キャンペーン」のリンクされたレコードフィールドが作成されます。

     >[!TIP]
     >
     > リンクされたレコードフィールドは、それぞれのアプリケーションの別のアプリケーションのオブジェクトには作成されません。
     > すべてのレコードタイプに対する接続されたフィールドの制限 30 個に加えて、500 個のフィールドに制限があるので、分類レコードタイプへのリンクを作成しないことをお勧めします。


1. （オプションおよび条件付き）元のレコードタイプまたはリンクされたレコードタイプのテーブルビューで、リンクされたレコードフィールドのヘッダーにある下向き矢印をクリックし、次のいずれかをクリックします。

   * **フィールドを編集**：フィールドの **名前** と **説明** 情報を更新します。
   * **ルックアップフィールドを編集**：任意のリンクされたレコードのフィールドを追加または削除します。

   ![ テーブル列のフィールドおよびルックアップフィールドの編集ドロップダウンメニュー ](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   ルックアップ フィールドを追加または削除するには、上記の手順 16 ～ 17 の指示に従います。<!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > リンク元のレコードタイプに属するルックアップフィールドを、別のアプリケーションのオブジェクトタイプに追加することはできません。
   >
   > 例えば、キャンペーンからリンク先の Workfront プロジェクトに「キャンペーンステータス」のルックアップフィールドを追加することはできません。

1. （オプション）リンクされたレコード フィールドのヘッダー、またはリンク元のレコード タイプのルックアップ フィールドのヘッダーにある下向き矢印をクリックし、「**削除**」をクリックします。

   レコードフィールドまたはルックアップフィールドが削除されます。レコードフィールドを削除すると、リンクされたレコードに関連付けられているルックアップフィールドも削除されます。
