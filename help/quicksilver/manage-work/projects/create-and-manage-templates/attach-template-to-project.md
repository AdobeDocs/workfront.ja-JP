---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトにテンプレートを添付
description: テンプレートは、プロジェクトの最初の作成段階または作成後に、プロジェクトに添付できます。
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 100%

---

# プロジェクトにテンプレートを添付

テンプレートは、プロジェクトの最初の作成段階または作成後に、プロジェクトに添付できます。

テンプレートを使用してプロジェクトを作成する方法について詳しくは、[テンプレートを使用したプロジェクトの作成](../../../manage-work/projects/create-projects/create-project-from-template.md)を参照してください。

## アクセス要件

この記事で説明する手順を実行するには以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集 </p> <p>プロジェクトへのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>を参照してください。</p> <p>テンプレートに対する表示アクセス権</p> <p>テンプレートの権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">テンプレートの共有</a>を参照してください。 </p> <p>テンプレートへのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートへのアクセス権の付与</a>を参照してください。</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの管理権限</p> <p>プロジェクト権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>を参照してください。 </p> <p>テンプレートに対する表示権限以上</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## 既存のプロジェクトにテンプレートを添付 {#attach-a-template-to-an-existing-project}

テンプレートは、プロジェクトページからまたはプロジェクトリストやレポートから Workfront のプロジェクトに添付できます。

1. テンプレートを添付するプロジェクトに移動し、プロジェクト名の右側にある&#x200B;**詳細**&#x200B;アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   または

   プロジェクトリストまたはレポートに移動し、プロジェクトを選択して、リストの上部にある&#x200B;**詳細**&#x200B;アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. 「**テンプレートを添付**」をクリックします。

   「テンプレートを添付」ボックスが表示されます。

1. 添付するテンプレートの名前を「**テンプレートを検索**」フィールドに値を入力し、リストに表示されたらクリックします。

   または

   **その他のテンプレート**&#x200B;エリアでテンプレートの名前をクリックします。

   テンプレートのプレビューが右側に表示され、テンプレートに関する次の情報が示されます。

   * 期間
   * 所有者
   * トップレベルのタスクの数（最初の 3 つのトップレベルのタスクのリストが含まれます）
   * タスクの合計数
   * 添付されたカスタムフォームの名前

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. （オプション）テンプレート名の左側の&#x200B;**お気に入り**&#x200B;アイコン ![](assets/favorites-icon-small.png) をクリックして、お気に入りとしてマークします。これにより、お気に入りリスト内にテンプレートが移動します。

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. （オプション）**お気に入り**&#x200B;アイコン ![](assets/favorites-icon-selected.png) をもう一度クリックして、お気に入りのリストから削除します。
1. 「**カスタマイズと添付**」をクリックします。

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. テンプレートを添付する前に、次のセクションの情報を更新します（またはいつでも「**テンプレートを添付**」をクリックできます）。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">タスクのセクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">以下で選択したテンプレートタスクがプロジェクトに読み込まれます。除外する項目の選択を解除します。 </td> 
      <td>テンプレートをプロジェクトに添付する前に、テンプレートから除外するタスクの選択を解除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">このテンプレートにあるタスクの先行タスクとするプロジェクト タスクを選びます。</td> 
      <td> <p>このフィールドをクリックして、プロジェクトタスクのリストを表示します。テンプレートタスクの開始前に終了する必要があるプロジェクトタスクを選択します。または、この手順をスキップし、テンプレートを添付した後でプロジェクト内で関係を設定することもできます。 </p> <p> 「<strong>依存関係タイプ</strong>」、「<strong>ラグ</strong>」情報および先行タスクを「<strong>強制</strong>」するかどうかを選択します。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このテンプレートで親タスクとするプロジェクト タスクを選びます。</td> 
      <td> すべてのテンプレートタスクの親タスクとして指定するプロジェクトタスクを選択します。選択しない場合は、現在のプロジェクトタスクの終わりにすべてのテンプレートタスクが表示されます。この手順をスキップし、テンプレートを添付した後で、プロジェクト内でタスクを移動することができます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">「オプション」セクション</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下に選択されたアイテムがプロジェクトにインポートされます。除外するものは選択を解除してください。</td> 
      <td> <p>テンプレートをプロジェクトに添付する前にテンプレートからクリアする情報の横にあるチェックボックスの選択を解除します。この情報は、テンプレートからプロジェクトには転送されません。各フィールドについて詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">プロジェクトへのテンプレートの添付の概要</a>を参照してください。 </p> <p>重要：「<strong>キュー プロパティ &amp; 問題設定</strong>」チェックボックスを選択すると、テンプレートのキューの詳細でプロジェクトのキューの詳細が上書きされます。この場合、テンプレートの「ルーティング規則」、「キュートピック」および「トピックグループ」が、プロジェクトの各項目に追加されます。<br>プロジェクトがリクエストキューとして設定され、プロジェクトに添付するテンプレートがリクエストキューとして設定されていない場合は、「<strong>キュー プロパティ &amp; 問題設定</strong>」チェックボックスをオンのままにすると、プロジェクトのキュー情報が削除されます。<br>「<strong>キュー プロパティ &amp; 問題設定</strong>」チェックボックスの選択を解除すると、プロジェクトのキュー設定がすべて保持され、テンプレートのキュー設定は添付されません。 </p> </td> 
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
   >* テンプレートのカスタムフォームのフィールドがプロジェクトに既に存在し、そこに情報が含まれている場合は、既にプロジェクトにある情報が保持されます。テンプレートの添付中はフィールドを編集できません。

1. 「**テンプレートの添付**」をクリックします。
1. 「**添付ファイルをキャンセル**」をクリックして、テンプレートの添付を停止します。

   または

   添付を終了して、プロジェクトにテンプレートを追加できるようにします。

   テンプレートを添付した後、プロジェクトを編集し、必要に応じてタスク、情報または設定を調整できます。

1. （オプション）「**プロジェクト詳細**」に続いて「**概要**」をクリックすると、添付したテンプレートの名前が&#x200B;**プロジェクトの関係**&#x200B;エリアに表示されます。

   >[!TIP]
   >
   >複数のテンプレートをプロジェクトに添付する場合は、最初に添付したテンプレートのみがこのフィールドに表示されます。詳しくは、この記事の[既存のプロジェクトへの複数テンプレートの添付とテンプレート情報の表示](#attach-multiple-templates-to-an-existing-project-and-view-template-information)の節を参照してください。

1. （オプション）テンプレートを添付したプロジェクトからテンプレート情報を削除します。詳しくは、[プロジェクトからのテンプレート情報の削除](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md)を参照してください。

## 既存のプロジェクトへの複数テンプレートの添付とテンプレート情報の表示 {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

この記事の[既存のプロジェクトへのテンプレートの添付](#attach-a-template-to-an-existing-project)の節で説明されている手順に従って、同じプロジェクトに複数のテンプレートを（一度に 1 つずつ）添付できます。これにより、各テンプレートのタスクやその他の情報がプロジェクトに追加されます。

>[!TIP]
>
>複数のテンプレートをプロジェクトに添付する場合、最初に添付したテンプレートのみがプロジェクト詳細エリアに表示されます。

プロジェクトに適用されているテンプレートを把握するには、次の手順に従います。

1. テンプレートが添付されたプロジェクトに移動します。
1. 左パネルの「**プロジェクト詳細**」をクリックします。
1. **プロジェクトの関係**&#x200B;の「**概要**」セクションの下部にある「**テンプレート**」フィールドのプロジェクトに添付されているテンプレートの名前を探します。

   ![](assets/nwe-template-info-on-project-350x356.png)


