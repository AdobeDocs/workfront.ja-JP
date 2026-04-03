---
title: Adobe Workfront計画レコードの自動処理を使用したオブジェクトの作成
description: Adobe Workfront Planningで自動処理を設定してアクティブ化した後、それらを使用してAdobe Workfrontでオブジェクトを作成したり、Adobe Workfront Planningでレコードを作成したりできます。 この記事では、既存のオートメーションを使用してレコードまたはオブジェクトを作成する方法について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 3%

---

# Adobe Workfront計画レコードの自動処理を使用したオブジェクトの作成


<!--you might need to add something about notifications and emails?!-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Adobe Workfront Planningで自動処理を設定してアクティブ化した後、それらを使用してAdobe Workfrontでオブジェクトを作成したり、Adobe Workfront Planningでレコードを作成したりできます。

例えば、既存の自動化機能を使用して、Workfront計画キャンペーンを実行し、Workfrontでプロジェクトを作成して、そのキャンペーンの進行状況を追跡できます。 プロジェクトは、キャンペーンの「接続されたプロジェクト」フィールドのWorkfront計画キャンペーンに接続されます。

ここでは、既存の自動処理を使用して、Workfront Planning レコードまたはWorkfront オブジェクトを作成する方法について説明します。

レコードタイプの自動処理について詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront Planning自動処理の設定](/help/quicksilver/planning/records/configure-automations-to-create-records.md)を参照してください。

自動処理を使用してレコードまたはWorkfront オブジェクトを作成すると、自動処理を実行しているレコードに自動的にリンクされます。

接続されたレコードについて詳しくは、[接続されたレコードの概要](/help/quicksilver/planning/records/connected-records-overview.md)を参照してください。

Workfront Planningの自動化機能を使用して、次の項目を作成できます。

* Workfront計画レコード
* 1つまたは複数のプロジェクト
* グループ
* プログラム
* ポートフォリオ

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
<p>任意のWorkfrontおよびプランニングパッケージ</p> <p>任意のワークフローとプランニングパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>作成するオブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム）に対するWorkfrontの「オブジェクトを作成」へのアクセス権を持つ編集アクセス。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>既存の自動処理を使用してオブジェクトを作成するワークスペースおよびレコードタイプに対して、より高い権限を付与します。 </p>  
   <p>子オブジェクト（プログラムまたはプロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）に対する権限を管理します。</p>
   <p>システム管理者は、作成しなかったワークスペースを含め、すべてのワークスペースに対して管理権限を持っています</p>
   </td> 
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

<!--
Old:

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
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
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and to the record type where you want to create objects using existing automations. </p>  
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (programs or projects).</p>
   <p>System Administrators have Manage permissions to all workspaces, including the ones they did not create</p>
   </td> 
  </tr> 

</tbody> 
</table>
-->

## オートメーションを使用したオブジェクトとレコードの作成に関する考慮事項

* オートメーションによって作成されたオブジェクトまたはレコードの名前は、単一のオブジェクトを作成する際に、そのオブジェクトを作成するレコード名と同じです。

* 複数のプロジェクトを作成する場合は、次のパターンに従って自動的に名前が付けられます。

  `[ Name of the record ] Name of the field choice`

  詳しくは、この記事の「[Workfront Planning Automationを使用したオブジェクトまたはレコードの作成](#use-a-workfront-planning-automation-to-create-an-object-or-a-record)」の節を参照してください。

* 新しいオブジェクトまたはレコードは、同じフィールド内の既存のオブジェクトを上書きしません。 同じレコードに対して同じ自動化を複数回トリガーすると、以前に作成されたオブジェクトに加えて、元のレコードの同じ接続フィールドに新しいオブジェクトまたはレコードが追加されます。



<!--hide this for now; they are trying to remove this limitation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->


## Workfront計画オートメーションを使用したオブジェクトまたはレコードの作成

<!--
For Feb 26 and add Preview disclosure at the top:

<span class="preview">When you choose a Field value change-automation, Workfront Planning creates the objects automatically, when the conditions you define are met. </span>

For information, see [Configure Adobe Workfront Planning automations to create records](/help/quicksilver/planning/records/configure-automations-to-create-records.md).</span>
-->

この節では、ボタンのクリックオートメーションを使用してオブジェクトを作成する方法について説明します。

1. Workfront Planningで、レコードまたはオブジェクトを自動的に作成および接続するために使用する自動処理を含むレコードタイプページを開きます。
1. テーブルビューを開きます。
1. 1つ以上のレコードを選択します。

   テーブルの下部に、オートメーションボタンなどの追加ボタンが表示された青いバーが表示されます。
1. 青いバーの「オートメーション」ボタンをクリックします。

   ![自動化ボタン &#x200B;](assets/automation-custom-button.png)

   次のことが発生します。

   * オートメーションでオブジェクトまたはレコードが正常に作成された場合、確認メッセージが画面の下部に表示されます。

   * 新しいオブジェクトは、オートメーションボタンの設定に示されている接続フィールドに表示されます。 新しいオブジェクトを表示する前に、ページを更新する必要がある場合があります。 新しいオブジェクトの名前は、元のレコードと同じです。

   * 複数の選択フィールドまたは単一選択フィールドの選択肢に基づいて複数のプロジェクトが作成された場合、プロジェクトには次のパターンに従って自動的に名前が付けられます。

     `[ Name of the record ] Name of the field choice`

     例えば、`Summer breeze`という名前のキャンペーンが`EMEA`のフィールド選択からプロジェクトを生成した場合、そのプロジェクトの名前は`[ Summer breeze ] EMEA`になります。

   * オートメーションのトリガー元のレコードが、新しいレコードの接続フィールドに追加されます。

   >[!NOTE]
   >
   >オブジェクトまたはレコードが作成され、期待どおりに接続されていることを確認することをお勧めします。

1. （オプション）接続されたフィールドで新しいオブジェクトをクリックします。 オブジェクトページが開き、新しいオブジェクトに追加の変更を加えることができます。

<!--
ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements. 

You must have the following access to perform the steps in this article:  

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
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
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

