---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトにテンプレートを添付
description: プロジェクトの初期作成段階または作成後に、プロジェクトにテンプレートを添付できます。
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 43%

---

# プロジェクトにテンプレートを添付

<!-- Audited: 10/2025 -->

プロジェクトの初期作成段階または作成後に、プロジェクトにテンプレートを添付できます。

テンプレートを使用してプロジェクトを作成する方法について詳しくは、[テンプレートを使用したプロジェクトの作成](../../../manage-work/projects/create-projects/create-project-from-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
    <p>プラン</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集 </p> <p>テンプレートへのアクセスの表示</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの管理権限</p> <p>テンプレートに対する表示権限以上</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p>
   <p>Or</p>
   <p>Current: Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Share a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create and modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## 既存のプロジェクトにテンプレートを添付 {#attach-a-template-to-an-existing-project}

プロジェクトページまたはプロジェクトリストやレポートから、テンプレートをプロジェクトに添付できます。

{{step1-to-projects}}

1. **プロジェクト** ページで、テンプレートを添付するプロジェクトを選択します。

1. プロジェクト名の右側にある **その他** アイコン ![&#x200B; その他ドロップダウン &#x200B;](assets/more-dropdown.png) をクリックします。

   ![&#x200B; 詳細アイコン &#x200B;](assets/qs-more-icon-on-an-object.png)

   または

   プロジェクトリストまたはレポートに移動してプロジェクトを選択し、リストの上部にある **その他** アイコン ![&#x200B; その他ドロップダウン &#x200B;](assets/more-dropdown.png) をクリックします。

   ![&#x200B; 詳細メニューが展開されました &#x200B;](assets/more-menu-expanded.png)

1. **テンプレートを添付** をクリックします。 **テンプレートを添付** ボックスが表示されます。

1. 添付するテンプレートの名前を「**テンプレートを検索**」フィールドに入力し始め、リストに表示されたらクリックします。

   または

   **その他のテンプレート**&#x200B;エリアでテンプレートの名前をクリックします。

   テンプレートのプレビューが右側に表示され、テンプレートに関する次の情報が示されます。

   * 期間
   * 所有者
   * 最上位タスクの数（最初の 3 つの最上位タスクのリストを含む）
   * タスクの合計数
   * 添付されたカスタムフォームの名前

   ![&#x200B; テンプレートを添付ボックス &#x200B;](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. （オプション）テンプレート名の右側にある **お気に入り** アイコン ![&#x200B; お気に入りアイコン &#x200B;](assets/favorites-icon-small.png) をクリックして、お気に入りとしてマークし、**お気に入り** リストに移動します。

1. （オプション） **お気に入り** アイコン ![&#x200B; お気に入りアイコン &#x200B;](assets/favorites-icon-selected.png) を再度クリックして、**お気に入り** リストから削除します。
1. **カスタマイズと添付** をクリックします。 **テンプレートを添付** サイドパネルが開きます。

1. （任意）次の節の情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">タスクのセクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">以下で選択したテンプレート タスクがプロジェクトにインポートされます。 除外するものは選択を解除してください。 </td> 
      <td><p>テンプレートをプロジェクトに添付する前に、テンプレートから除外するタスクの選択を解除します。</p>
      <p><b>ヒント</b></p>
      <p>選択できるタスクは 1 つだけです。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このテンプレートにあるタスクの先行タスクとするプロジェクト タスクを選びます。</td> 
      <td> <p>フィールド ボックス内をクリックしてプロジェクト タスクの一覧を表示し、テンプレート タスクを開始する前に終了する必要があるタスクを選択します。 または、この手順をスキップし、テンプレートを添付した後でプロジェクト内で関係を設定することもできます。 </p> <p> 「<strong> 依存タイプ </strong>」、「<strong> ラグタイム </strong> 情報、および「<strong> 先行タスクの適用 </strong>」チェックボックスをオンにして先行タスクを適用する場合は、を選択します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このテンプレートで親タスクとするプロジェクト タスクを選びます。</td> 
      <td> <p>すべてのテンプレートタスクの親タスクとして指定するプロジェクトタスクを選択します。何も選択しない場合、すべてのテンプレート タスクが現在のプロジェクト タスクの最後に表示されます。 この手順をスキップし、テンプレートを添付した後で、プロジェクト内でタスクを移動することができます。</p>
      <p><b>メモ</b></p>
      <p>子を追加した親テンプレートタスクを選択した場合、プロジェクトに追加された後、親にのみプロジェクトタスクがその先行タスクとして表示されます。 子テンプレート タスクには先行タスクは表示されません。</p>
      <p>子テンプレートタスクのみを選択した場合、プロジェクトタスクは、プロジェクトに追加された後、その先行タスクとして表示されます。 </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">「オプション」セクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下に選択されたアイテムがプロジェクトにインポートされます。除外するものは選択を解除してください。</td> 
      <td> <p>プロジェクトに添付する前にテンプレートから除外する情報のチェックボックスをオフにします。 各フィールドについて詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">プロジェクトへのテンプレートの添付の概要</a>を参照してください。 </p> <p>重要：「<strong>キュー プロパティ &amp; 問題設定</strong>」チェックボックスを選択すると、テンプレートのキューの詳細でプロジェクトのキューの詳細が上書きされます。この場合、テンプレートの「ルーティング規則」、「キュートピック」および「トピックグループ」が、プロジェクトの各項目に追加されます。<br> プロジェクトが要求キューとして設定され、プロジェクトに添付するテンプレートが要求キューとして設定されていない場合、&lbrack; キューのプロパティと問題の設定 <strong> ボックスをオンにしていると、プロジェクトのキュー情報は削除され </strong> す。 <br> 「<strong> キューのプロパティと問題設定 </strong>」ボックスの選択を解除すると、プロジェクトのキュー設定はすべて保持され、テンプレートのキュー設定は添付されません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">「カスタムフォーム」セクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td> <p>カスタムフォームをテンプレートに添付すると、その名前が左パネルに表示されます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）カスタムフォームの情報を更新します。この情報はプロジェクトに転送されます。

   >[!TIP]
   >
   >* テンプレート上のカスタムフォームに空の必須フィールドが含まれている場合、この手順は必須です。
   >* テンプレートのカスタムフォームのフィールドがプロジェクトに既に存在し、そこに情報が含まれている場合は、既にプロジェクトにある情報が保持されます。テンプレートの添付中は編集できません。

1. 「**テンプレートの添付**」をクリックします。
1. **添付をキャンセル** をクリックして、テンプレートの添付を停止します。

   または

   添付を終了して、プロジェクトにテンプレートを追加できるようにします。

   テンプレートを添付した後、プロジェクトを編集し、必要に応じてタスク、情報または設定を調整できます。

1. （任意）左側のパネルで、「**プロジェクトの詳細**」をクリックしてから **概要** をクリックして、「**プロジェクトの関係**」領域に添付したテンプレートの名前を表示します。

   >[!TIP]
   >
   >プロジェクトに複数のテンプレートを添付する場合、最初に添付したテンプレートのみがこのフィールドに表示されます。 詳しくは、この記事の[既存のプロジェクトへの複数テンプレートの添付とテンプレート情報の表示](#attach-multiple-templates-to-an-existing-project-and-view-template-information)の節を参照してください。

1. （任意）テンプレートを添付したプロジェクトからテンプレート情報を削除します。 詳しくは、[プロジェクトからのテンプレート情報の削除](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md)を参照してください。

## 既存のプロジェクトへの複数テンプレートの添付とテンプレート情報の表示 {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

この記事の「[&#x200B; 既存のプロジェクトにテンプレートを添付する &#x200B;](#attach-a-template-to-an-existing-project)」の節で説明されている手順に従って、複数のテンプレートを同じプロジェクトに（一度に 1 つずつ）添付できます。 これにより、各テンプレートのタスクやその他の情報がプロジェクトに追加されます。

>[!TIP]
>
>複数のテンプレートを 1 つのプロジェクトに添付する場合、最初に添付したテンプレートのみが [ プロジェクトの詳細 ] 領域に表示されます。

プロジェクトに適用されているテンプレートを表示するには：

{{step1-to-projects}}

1. **プロジェクト** ページで、テンプレートが添付されたプロジェクトを選択します。

1. 左パネルの「**プロジェクト詳細**」をクリックします。

1. **プロジェクトの関係** の下の **概要** セクションの下部にある「**テンプレート**」フィールドで、プロジェクトに添付されているテンプレートの名前を見つけます。

   ![&#x200B; プロジェクトのテンプレート情報 &#x200B;](assets/nwe-template-info-on-project-350x356.png)


