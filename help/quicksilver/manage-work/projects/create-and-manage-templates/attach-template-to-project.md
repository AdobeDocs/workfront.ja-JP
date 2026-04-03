---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトにテンプレートを添付
description: テンプレートは、プロジェクトの初期作成段階または作成後にプロジェクトに添付できます。
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 43%

---

# プロジェクトにテンプレートを添付

<!-- Audited: 10/2025 -->

テンプレートは、プロジェクトの初期作成段階または作成後にプロジェクトに添付できます。

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

<!--
 Old:
 
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
</table>
-->

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

プロジェクトページまたはプロジェクトリストまたはレポートから、テンプレートをプロジェクトに添付できます。

{{step1-to-projects}}

1. **プロジェクト** ページで、テンプレートを添付するプロジェクトを選択します。

1. プロジェクト名の右側にある&#x200B;**詳細** アイコン ![詳細ドロップダウン &#x200B;](assets/more-dropdown.png)をクリックします。

   ![その他のアイコン &#x200B;](assets/qs-more-icon-on-an-object.png)

   または

   プロジェクトのリストまたはレポートに移動してプロジェクトを選択し、リストの上部にある&#x200B;**詳細** アイコン ![詳細ドロップダウン &#x200B;](assets/more-dropdown.png)をクリックします。

   ![その他のメニューが展開されました](assets/more-menu-expanded.png)

1. 「**テンプレートを添付**」をクリックします。 「**テンプレートを添付**」ボックスが表示されます。

1. 添付するテンプレートの名前を&#x200B;**テンプレートを検索** フィールドに入力し、リストに表示されたらクリックします。

   または

   **その他のテンプレート**&#x200B;エリアでテンプレートの名前をクリックします。

   テンプレートのプレビューが右側に表示され、テンプレートに関する次の情報が示されます。

   * 期間
   * 所有者
   * 最上位タスクの数（最初の3つの最上位タスクのリストを含む）
   * タスクの合計数
   * 添付されたカスタムフォームの名前

   ![&#x200B; テンプレート ボックスを添付](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. （オプション）テンプレート名の右側にある&#x200B;**お気に入り** アイコン ![お気に入りアイコン &#x200B;](assets/favorites-icon-small.png)をクリックして、お気に入りとしてマークし、**お気に入り** リストに移動します。

1. （オプション） **お気に入り** アイコン ![お気に入りアイコン &#x200B;](assets/favorites-icon-selected.png)をもう一度クリックして、**お気に入り** リストから削除します。
1. 「**カスタマイズして添付**」をクリックします。 **テンプレートを添付** サイドパネルが開きます。

1. （オプション）次のセクションの情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">タスクのセクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">以下の選択したテンプレートタスクがプロジェクトに読み込まれます。 除外するものは選択を解除してください。 </td> 
      <td><p>テンプレートをプロジェクトに添付する前に、テンプレートから除外するタスクの選択を解除します。</p>
      <p><b>ヒント</b></p>
      <p>1つのタスクのみを選択できます。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このテンプレートにあるタスクの先行タスクとするプロジェクト タスクを選びます。</td> 
      <td> <p>フィールドボックス内をクリックしてプロジェクトタスクのリストを表示し、テンプレートタスクを開始する前に終了する必要があるタスクを選択します。 または、この手順をスキップし、テンプレートを添付した後でプロジェクト内で関係を設定することもできます。 </p> <p> 「<strong>依存関係タイプ </strong>、<strong>遅延時間</strong>」の情報を選択します。また、「<strong>先行タスクを適用</strong>」チェックボックスをオンにして先行タスクを適用する場合も選択します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このテンプレートで親タスクとするプロジェクト タスクを選びます。</td> 
      <td> <p>すべてのテンプレートタスクの親タスクとして指定するプロジェクトタスクを選択します。選択しないと、すべてのテンプレートタスクが現在のプロジェクトタスクの最後に表示されます。 この手順をスキップし、テンプレートを添付した後で、プロジェクト内でタスクを移動することができます。</p>
      <p><b>メモ</b></p>
      <p>追加の子を含む親テンプレートタスクを選択した場合、プロジェクトに追加された後は、親のみがプロジェクトタスクを先行タスクとして表示します。 子テンプレートタスクには先行タスクは表示されません。</p>
      <p>子テンプレートタスクのみを選択した場合、プロジェクトタスクはプロジェクトに追加された後に先行タスクとして表示されます。 </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">「オプション」セクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下に選択されたアイテムがプロジェクトにインポートされます。除外するものは選択を解除してください。</td> 
      <td> <p>テンプレートから除外する情報をプロジェクトに添付する前に、チェックボックスの選択を解除します。 各フィールドについて詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">プロジェクトへのテンプレートの添付の概要</a>を参照してください。 </p> <p>重要：「<strong>キュー プロパティ &amp; 問題設定</strong>」チェックボックスを選択すると、テンプレートのキューの詳細でプロジェクトのキューの詳細が上書きされます。この場合、テンプレートの「ルーティング規則」、「キュートピック」および「トピックグループ」が、プロジェクトの各項目に追加されます。<br> プロジェクトがリクエストキューとして設定されていて、プロジェクトに添付したテンプレートがリクエストキューとして設定されていない場合、「<strong> キューのプロパティと問題の設定</strong>」チェックボックスをオンのままにすると、プロジェクトのキュー情報が削除されます。 <br> 「<strong> キューのプロパティと問題の設定</strong>」ボックスの選択を解除すると、プロジェクトのキューの設定設定はすべて保持され、テンプレートのキューの設定設定は添付されません。 </p> </td> 
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
   >* テンプレートのカスタムフォームのフィールドがプロジェクトに既に存在し、そこに情報が含まれている場合は、既にプロジェクトにある情報が保持されます。テンプレートの接続中に編集することはできません。

1. 「**テンプレートの添付**」をクリックします。
1. 「**添付ファイルをキャンセル**」をクリックして、テンプレートの添付を停止します。

   または

   添付を終了して、プロジェクトにテンプレートを追加できるようにします。

   テンプレートを添付した後、プロジェクトを編集し、必要に応じてタスク、情報または設定を調整できます。

1. （オプション）左側のパネルで、**プロジェクトの詳細**&#x200B;をクリックし、**概要**&#x200B;をクリックして、**プロジェクトの関係**&#x200B;領域で添付したテンプレートの名前を表示します。

   >[!TIP]
   >
   >プロジェクトに複数のテンプレートを添付した場合、最初に添付したテンプレートのみが、このフィールドに表示されます。 詳しくは、この記事の[既存のプロジェクトへの複数テンプレートの添付とテンプレート情報の表示](#attach-multiple-templates-to-an-existing-project-and-view-template-information)の節を参照してください。

1. （オプション）テンプレートを添付したプロジェクトからテンプレート情報を削除します。 詳しくは、[プロジェクトからのテンプレート情報の削除](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md)を参照してください。

## 既存のプロジェクトへの複数テンプレートの添付とテンプレート情報の表示 {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

この記事の「[&#x200B; テンプレートを既存のプロジェクトに添付](#attach-a-template-to-an-existing-project)」で説明されている手順に従って、同じプロジェクトに複数のテンプレートを（一度に1つずつ）添付できます。 これにより、各テンプレートのタスクやその他の情報がプロジェクトに追加されます。

>[!TIP]
>
>プロジェクトに複数のテンプレートを添付すると、最初に添付したテンプレートのみがプロジェクトの詳細領域に表示されます。

プロジェクトに適用されているテンプレートを表示するには：

{{step1-to-projects}}

1. **プロジェクト** ページで、テンプレートが添付されているプロジェクトを選択します。

1. 左パネルの「**プロジェクト詳細**」をクリックします。

1. **プロジェクト関係**&#x200B;の&#x200B;**概要** セクションの下部にある&#x200B;**テンプレート** フィールドで、プロジェクトに添付されたテンプレートの名前を探します。

   ![&#x200B; プロジェクトのテンプレート情報](assets/nwe-template-info-on-project-350x356.png)


