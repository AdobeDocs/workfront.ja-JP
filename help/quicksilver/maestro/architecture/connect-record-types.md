---
title: レコードタイプを接続
description: 個々のレコードの種類を相互に関連付ける方法を示すには、レコードの種類を接続します。 また、Maestro レコードタイプを他のアプリケーションのオブジェクトタイプと接続して、ユーザーのエクスペリエンスを向上させ、1 つのアプリケーションにフォーカスを合わせることもできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 98b57b08b87e47a402684428a76576455df664d7
workflow-type: tm+mt
source-wordcount: '1784'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# レコードタイプを接続

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Adobeマエストロを使用すると、組織で必要なレコードの種類を含む完全にカスタマイズ可能なワークスペースをデザインできます。 個々のレコードの種類を相互に関連付ける方法を示すには、レコードの種類を接続します。 また、Maestro レコードタイプを他のアプリケーションのオブジェクトタイプと接続して、ユーザーのエクスペリエンスを向上させ、1 つのアプリケーションにフォーカスを合わせることもできます。

次の項目を接続できます。

* マエストロのオペレーショナルレコードのタイプ
* 分類レコードタイプに対するマエストロオペレーショナルレコードタイプ
* マエストロ分類タイプからオペレーショナルレコードタイプへ
* 他のアプリケーションの操作レコードのタイプとオブジェクトのタイプをマエストロします。

これにより、別の Maestro レコード上に、リンクされたレコードまたはオブジェクトタイプのフィールドを表示できます。

この記事では、2 つの Maestro レコードタイプまたは Maestro レコードタイプを別のアプリケーションのオブジェクトと接続する方法について説明します。

レコードまたはオブジェクトの種類間の接続が確立されたら、個々のレコードを相互に接続できます。

別のアプリケーションからオブジェクトに Maestro レコードを接続する方法については、 [レコードを接続](../records/connect-records.md).

レコードタイプを接続する例については、 [レコードタイプとレコードの接続例](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## レコードタイプの接続に関する考慮事項

次の点に注意してください。

* Maestro では、次のエンティティを接続できます。

   * 2 種類のオペレーショナルレコード
   * 2 つの分類
   * オペレーショナルレコードのタイプと分類
   * 別のアプリケーションのオペレーショナル・レコード・タイプとオブジェクト・タイプ。

     >[!TIP]
     >
     >    分類レコードタイプをオペレーショナルレコードタイプに接続したり、別のアプリケーションからオブジェクトタイプに接続することはできません。

* 次のオブジェクトは、Maestro レコードタイプを使用して、次のアプリケーションから接続できます。

   * ADOBE WORKFRONT:

      * プロジェクト
      * ポートフォリオ
      * プログラム
      * 会社
      * グループ

* レコードタイプを別のレコードタイプに接続するか、別のアプリケーションのオブジェクトタイプに接続すると、次のシナリオが存在します。

   * 2 つのレコードタイプを接続すると、[ リンクされたレコード ] フィールドは、接続元のレコードタイプに対して作成されます。 接続先のレコードタイプに、同様の「リンクされたレコード」フィールドが作成されます。

     例えば、「Campaign」レコードタイプを「Product」レコードタイプに接続すると、「Linked Product」という名前のリンクされたレコードフィールドが「Campaign」レコードタイプに作成され、「Campaign」という名前のリンクされたレコードタイプが「Product」レコードタイプに自動的に作成されます。

   * レコードタイプフィールドを分類に接続する場合：リンクされたレコードフィールドは、接続元のレコードタイプに対して作成されます。 接続先の分類にリンクされたレコードフィールドは作成されません。

     例えば、「キャンペーン」レコードタイプを「オーディエンス」分類のレコードタイプと接続すると、「リンクされたオーディエンス」という名前のリンクされたレコードフィールドがキャンペーンのレコードタイプで作成されます。 オーディエンス分類のレコードタイプで、「キャンペーン」という名前のリンクされたレコードフィールドが自動的に作成されることはありません。 <!--this might be temporary-->

   * レコードタイプフィールドを別のアプリケーションのオブジェクトタイプと接続する場合：リンクされたレコードフィールドは、接続元のレコードタイプに対して作成されます。 WorkfrontのWorkfrontプロジェクトに、リンクされたレコードフィールドが自動的に作成されません。 リンクされたレコードフィールドは、実際のオブジェクトが Maestro レコードに接続されている場合にのみ、Workfrontオブジェクトレコードタイプで作成されます。

     詳しくは、 [レコードを接続](../records/connect-records.md).

* レコードの種類を接続した後で、1 つのレコードの種類から別のレコードの種類に複数のフィールドを接続できます。 これらのフィールドは、「リンクされたフィールド」または「ルックアップフィールド」と呼ばれます。
* リンクされたレコードフィールドの前には関係アイコンが付きます ![](assets/relationship-field-icon.png).
* レコードタイプの個々のレコードを作成した後、リンクされたレコードタイプのフィールドから接続先のレコードを選択できます。 詳しくは、 [レコードを接続](../records/connect-records.md).
* リンク先のレコードタイプからは、リンク先のレコードを選択するとすぐに、そのレコードタイプに属する元のレコードタイプから自動的に入力されるので、リンク先のフィールドの情報を編集することはできません。

## レコードタイプを接続

<!--when changes here, also update the article for "Connect records"-->

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](assets/dots-main-menu.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](assets/lines-main-menu.png) 左上隅で、「 **[!UICONTROL マエストロ]**.

   最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを接続するワークスペースを選択します。
1. レコードタイプのカードをクリックして、レコードタイプのページを開きます。
1. 次をクリック： **+** アイコンをクリックし、 **新しい接続** タブをクリックします。

   ![](assets/new-connection-tab-with-workfront-option.png)
1. Adobe Analytics の **レコードタイプ** 「 」フィールドで、次のいずれかを選択します。 <!--is the field name spelled right? lowercase "t"?-->

   * 別のオペレーショナルレコードタイプ
   * 分類
   * Workfrontプロジェクト、Portfolio、プログラム、会社、またはグループ。

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)

   >[!TIP]
   >
   > 選択したワークスペースのレコードタイプと分類のみを選択できます。

1. 次の情報を更新します。

   * **名前**：テーブル表示または元のレコードタイプの詳細ページに表示される、接続されたフィールドの名前。 これにより、元のレコードの種類のテーブルビューまたは元のレコードのリンクされたレコードフィールドに、リンクされたレコード列が作成されます。 <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >リンク先のレコードの名前を、接続されたレコードフィールドの名前に含めて、新しいフィールドのレコードの種類を取り込むことをお勧めします。 リンクされたレコードの名前は、新しくリンクされたレコードフィールドまたはリンクされたフィールドには表示されません。

   * **説明**:「接続されたレコード」フィールドに関する追加情報。 フィールドの説明は、テーブルのフィールドの列にカーソルを合わせると表示されます。
   * **複数のレコードを許可**：リンクされたレコードタイプのフィールドが元のレコードに表示される場合に、ユーザーが複数のレコードを追加できるようにするには、このオプションを選択します。 これはデフォルトで選択されています。
   * **参照フィールドを選択**：選択したレコードタイプからフィールドを追加するには、このオプションを選択します。 これはデフォルトで選択されています。

1. 「**作成**」をクリックします。

1. （条件付き）前の手順でルックアップフィールドを選択設定を選択した場合、 **参照フィールドを追加** ボックスが開きます。

   次をクリック： **+** アイコンをクリックして、 **未選択のフィールド** 領域。

   または

   次をクリック： **-** アイコンを使用して、次の場所からフィールドを削除します。 **選択したフィールド** 領域

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   >[!NOTE]
   >
   >どのフィールドも選択しない場合、 **名前** リンクされたレコードのフィールドは、元のレコードのテーブルビューに表示される唯一のフィールドです。 The **名前** フィールドは削除できません。

1. （オプションおよび条件付き）数値、通貨、割合または日付タイプのフィールドをリンクする場合は、集計値も選択します。 ユーザーがリンクされたレコードフィールドで複数のリンクされたレコードを選択する場合、リンクされたフィールドの値は、コンマで区切るか、選択した集計に従って集計値として表示されます。

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   次の中から選択します。

   * **なし**：複数のレコードから取得された値をコンマで区切って表示します。 これはデフォルトの選択です。
   * **MAX**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の最大値を表示します。
   * **最小**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の最小値を表示します。
   * **SUM**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の合計を表示します。
   * **AVG**：リンクされたレコードフィールドで選択された複数のレコードから取得されたすべての値の平均を表示します。

   >[!NOTE]
   >
   >例えば、キャンペーンレコード（元のレコード）から製品レコード（リンクされたレコード）をリンクし、「製品フィールド」という名前を付けることができます。 また、キャンペーンレコードから製品レコードの「予算」フィールドをリンクし、「製品の予算」と呼ぶこともできます。 「製品」フィールドで複数のレコードを選択できる場合は、予算が$120,000 の製品 1 と、予算が$100,000 の製品 2 を選択できます。 選択した集約に応じて、元のレコードから、リンクされたフィールドに次の予算情報を表示できます。
   >
   >* **なし**:120,000 ドル、100,000 ドル
   >* **MAX**:120,000 ドル
   >* **最小**:100,000 ドル
   >* **SUM**:220,000 ドル
   >* **AVG**:110,000 ドル
   >

1. （オプション） **検索** アイコン ![](assets/search-icon.png) をクリックしてフィールドを検索します。

1. （オプション）「 **スキップ** 接続されたレコードタイプのフィールドを追加しない場合。

1. クリック **フィールドを追加** をクリックして変更を保存します。

   次の項目が追加されます。

   * 手動で追加した後に、リンクされたレコードタイプのレコードを表示する、リンクされたレコードフィールド。 リンクされたレコードフィールドの名前は、手順 6 で選択した名前です。 <!-- ensure this is still accurate-->

   * リンクされたレコードフィールドに手動でレコードを追加した後に、リンクされたレコードタイプのフィールドの情報を表示する、リンクされたフィールド（複数可）。 リンクされたフィールドは、 **参照フィールドを選択** 接続を作成する際に設定が選択されます。 リンクされたフィールドの名前は、次のパターンに従って付けられます。

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * リンク先のレコードタイプ上のリンクされたレコードフィールド。 リンクされたレコードタイプのリンクされたレコードフィールドの名前は、リンク元のレコードタイプの名前です。

     例えば、「Campaign」レコードタイプから「Product」レコードタイプをリンクし、「Linked Product」キャンペーンの接続済みフィールドに名前を付けた場合、「Campaign」リンク済みレコードタイプに対して「Campaign」リンク済みレコードフィールドが作成されます。

1. （オプション）元のレコードの種類またはリンクされたレコードの種類のテーブルビューで、リンクされたレコードフィールドのヘッダーにある下向き矢印をクリックし、次のいずれかをクリックします。

   * **フィールドを編集**：更新できるのは **名前** そして **説明** フィールドの情報。
   * **参照フィールドの編集**：リンクされているレコードのフィールドを追加または削除します。

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   参照フィールドを追加または削除するには、上記の手順 7～12 の指示に従います。 <!--ensure these step numbers stay accurate-->

1. （オプション）リンク元のレコードタイプから、リンクされたレコードフィールドのヘッダーにある下向き矢印をクリックし、 **削除**.

   レコードフィールドと、リンクされているその他の参照フィールドは削除され、フィールドとその情報は復元できません。

   >[!TIP]
   >
   >    リンク先のレコードタイプのリンクされたレコードフィールドは削除されません。 <!-- is this still accurate?! -->
