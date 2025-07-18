---
title: レコードタイプを接続
description: 個々のレコードタイプが互いにどのように関連しているかは、レコードタイプを連結するとよくわかります。また、Workfront Planning のレコードタイプを他のアプリケーションのオブジェクトタイプに接続して、ユーザーのエクスペリエンスを向上させ、ユーザーが 1 つのアプリケーションに集中できるようにすることもできます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '2499'
ht-degree: 37%

---


# レコードタイプを接続

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

レコードタイプを相互に接続することも、レコードタイプを他のアプリケーションのオブジェクトタイプと接続することもできます。

相互に影響を与える複数のタイプの作業オブジェクトがある場合、レコード タイプを接続すると便利です。 例えば、キャンペーンを扱う場合に、各キャンペーンが複数のブランドに対応している可能性があります。 この関係を示すために、キャンペーンをブランドに接続できます。 さらに、各キャンペーンの作業は、Workfrontの複数のプロジェクトで計画される可能性があります。 これを示すには、キャンペーンを関連するプロジェクトに接続します。 レコードタイプを結び付けた後で、個々のレコードを結び付けると、Workfront Planning でこの関係が実現されます。

ここでは、2 つのWorkfront Planning レコードタイプまたは 1 つのWorkfront Planning レコードタイプを別のアプリケーションのオブジェクトに関連付ける方法について説明します。

レコード間またはオブジェクト タイプ間の関連付けを確立した後、個々のレコードを相互に関連付けて、Workfront Planning レコードにリンクされたレコードまたはオブジェクト タイプのフィールドを表示することができます。

接続タイプに関する一般的な情報については、[ 接続されたレコードタイプの概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

レコードまたはレコードを他のアプリケーションのオブジェクトと接続する方法については、「[ レコードを接続する ](/help/quicksilver/planning/records/connect-records.md)」を参照してください。

レコードタイプとレコードの接続例については、[ レコードタイプとレコードの接続例 ](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md) を参照してください。

<!--ensure this last linked article is right; the title and the link should have changed-->

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li>
   <li><p> Adobe Experience Manager Assets（AEM アセットを Planning レコードタイプと関連付ける場合）<p>
   <p>Adobe Experience Manager Assets ライセンスと、AEM AssetsとWorkfrontの統合が必要です。
    詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials：記事インデックス </a> を参照してください。 </p>
   </li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> <p>標準</p> 
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する管理権限</a> </p>  
   <p>システム管理者は、自分が作成したものでないものも含めて、すべてのワークスペースに対する権限を持っています。</p></td> 
  </tr>

</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードタイプの接続

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. レコードタイプを接続するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. テーブルビューの右上隅にある **+** アイコンをクリックし、「**新しい接続**」タブをクリックします。

   ![Workfront AEMのオプションを含む新しい「接続」タブ ](assets/new-connection-tab-with-workfront-aem-options.png)

1. 「**レコードタイプ**」フィールドでレコードタイプを検索するか、次のいずれかを選択します。

   * 現在のワークスペースの別のレコードタイプ

     ![ 多対多の接続ピッカー ](assets/many-to-many-connection-picker.png)

     >[!TIP]
     >
     > 
     >選択したワークスペースに他のレコードタイプがない場合、ワークスペースセクションは表示されません。


   * 他のワークスペースから接続するように設定された、別のワークスペースからのレコードタイプ。

     >[!TIP]
     >
     >他のワークスペースからレコードの種類にアクセスするには、[**&#x200B;** レコードの種類の編集 **] ボックスの [** 詳細設定 **] タブで、レコードの種類に対して &lbrack; 他のワークスペースでこのレコードの種類への接続を許可する** 設定を有効にする必要があります。 他のワークスペースから接続するように設定されているレコードタイプがない場合、「ワークスペース」セクションは表示されません。
     > ![ レコードタイプを編集ボックスの「詳細設定」タブ ](assets/edit-record-type-box-advanced-settings-tab.png)

     詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

     ![ 複数レコードを許可する新しい接続ボックス ](assets/new-connection-allow-multiple-records-box.png)

   * 「**Workfront オブジェクトタイプ**」セクションからの&#x200B;**プロジェクト、ポートフォリオ、プログラム、会社**&#x200B;または&#x200B;**グループ**。

     ![Workfront プロジェクト連携の選択 ](assets/workfront-project-connection-selection.png)

   * 「**Adobe アプリケーション**」セクションからの **Experience Manager Assets**。

     ![AEM Assets接続の選択 ](assets/aem-assets-connection-selection.png)

1. 次の情報を更新します。

   * **名前**：テーブルビューまたは元のレコードタイプのレコードページに表示される、接続されたフィールドの名前。これにより、元のレコードタイプのテーブル ビュー、または元のレコードのリンクされたレコードフィールドに、リンクされたレコード列が作成されます。 デフォルトでは、フィールド名は接続先のレコードまたはオブジェクトの名前です。

   >[!TIP]
   >
   >同じレコードまたはオブジェクトタイプへの複数の接続を持つことができます。 連結フィールド名を編集しない場合、Workfrontでは、連結されたレコードの名前の後に数字が追加され、連結されたレコードの種類の数が同じ名前で示されます。

   * **説明**：接続されたレコードのフィールドに関する追加情報。フィールドの説明は、テーブル内でフィールドの列にポインタを合わせると表示されます。
   * **複数レコードを許可**：元のレコードに「リンクされたレコードタイプ」フィールドが表示されたときにユーザーが複数のレコードを追加できるようにするときに、このオプションを選択します。 これはデフォルトで選択されています。

     このオプションは、2 つの異なるワークスペース、またはレコードとAdobe Experience Manager アセットオブジェクトからレコードを接続する場合にのみ使用できます。

     ![ 複数レコードを許可する新しい接続ボックス ](assets/new-connection-allow-multiple-records-box.png)

   * **接続タイプ**：次のいずれかのオプションを選択して、接続先および接続先のレコードの数を指定します。

      * 多対多
      * 一対多
      * 多対 1
      * 一対一

     このオプションは、同じワークスペースのレコードまたはレコードとWorkfront オブジェクトタイプを接続する場合にのみ使用できます。

     ![ 多対多の接続ピッカー ](assets/many-to-many-connection-picker.png)

     接続タイプについて詳しくは、[ 接続されたレコードタイプの概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

     >[!NOTE]
     >
     > 接続の種類に [ 一対多 ] または [ 一対一 ] を選択した場合、後で他の場所に既に接続されているレコードまたはオブジェクトを接続しようとすると、再度接続すると元の接続から削除されるという警告が表示されます。 削除を許可するか、別のレコードを選択できます。

   * **ルックアップフィールドを選択**：選択したレコードタイプからフィールドを追加するには、このオプションを選択します。ルックアップフィールドは、リンク先のレコードタイプまたはオブジェクトタイプに関連付けられたフィールドです。リンクすると、リンク元のレコード上のリンク先のレコードまたはオブジェクトの情報が表示されます。 これはデフォルトで選択されています。

   >[!TIP]
   >
   >* Workfrontの先行入力フィールド（「プロジェクト所有者」や「プロジェクトスポンサー」などのフィールドを含む）を参照フィールドとして追加することはできません。
   >
   >* Workfront オブジェクトの日付フィールドの情報は、Workfront Planning では、Workfrontでの表示方法に関係なく、24 時間形式で表示されます。
   >
   >   例えば、プロジェクトの予定開始日がWorkfrontで午後 3:00 と表示された場合、Workfront Planning の読み込まれた参照フィールドでは 15:00 と表示されます。

1. （条件付きおよびオプション）Workfront オブジェクトの接続を選択した場合、「**これらの条件に一致するオブジェクトのみをリンク**」セクションから「**カスタムフォーム**」を選択します。選択したカスタムフォームがアタッチされているオブジェクトのみを、選択したレコードタイプにリンクできます。複数のフォームを選択できます。

   >[!NOTE]
   >
   > このリストに表示される前に、選択したオブジェクトのカスタムフォームを Workfront で作成する必要があります。

1. （条件付き）Experience Manager Assets への接続を選択した場合、「**次のリポジトリからアセットをリンク**」セクションの **Experience Manager リポジトリ**&#x200B;ドロップダウンメニューからリポジトリを選択します。必須フィールドです。このフィールドには、Experience Manager Assets でアクセス権のあるリポジトリのみが表示されます。

   >[!NOTE]
   >
   >Workfront管理者は、Workfrontのメタデータマッピングを使用して、Workfront Planning フィールドをExperience Manager Assets フィールドにマッピングできます。 詳しくは、[Adobe WorkfrontとExperience Manager Assets間のアセットメタデータのマッピングの設定 ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) を参照してください。

1. （条件付き）Experience Manager AssetsまたはWorkfront Planning レコードタイプへの接続を選択した場合は、「レコードの外観 **領域で次のいずれかのオプションを選択し** す。

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
   > レコードタイプを Experience Manager Assets に接続した場合、アグリゲータは使用できません。

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

   * レコードタイプを相互にリンクすると、リンク先のレコードタイプにも、リンクされたレコードフィールドが追加されます。リンクされたレコードタイプでのリンクされたレコードフィールドの名前は、リンク元のレコードタイプの名前です。

     例えば、「キャンペーン」レコードタイプから「製品」レコードタイプをリンクし、キャンペーンの「リンクされた製品」の接続フィールドに名前を付けると、製品レコードタイプに対して「キャンペーン」のリンクされたレコードフィールドが作成されます。

     >[!TIP]
     >
     > 別のアプリケーションから Workfront Planning でのリンク元のレコードタイプへのオブジェクトには、リンクされたレコードフィールドは作成されません。

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
