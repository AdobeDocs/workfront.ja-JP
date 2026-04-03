---
product-area: projects;templates
navigation-topic: manage-projects
title: プロジェクトをテンプレートとして保存
description: プロジェクトをテンプレートとして保存プロジェクトレベルで「テンプレートとして保存」すると、ユーザーはUIでそれを確認できます。このリンクには、より詳細な別の記事があります（ステップバイステップ）。
author: Alina
feature: Work Management
exl-id: 4b5dfe12-f984-47c6-8e19-78b549f19159
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 55%

---

# プロジェクトをテンプレートとして保存

<!--Audited: 6/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Keep this the way it is in the Managing Projects area because the functionality in the UI is "Save as template" at the project level, so users see that in the UI; there is another article that this links to which is more in depth (step-by-step). This functionality needs to stay in both projects AND templates areas.)</p>
-->

<!--
<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>
-->

プロジェクトが将来再び発生することが決定した場合は、その既存のプロジェクトからテンプレートを作成できます。次に、テンプレートを再度使用して、同様の情報を含む可能性がある、または既存のプロジェクトと同じタイムラインや割り当てを共有する可能性のある今後のプロジェクトを作成できます。

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
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p> /td&gt; 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限またはそれ以上の権限 </p> <p>プロジェクトをテンプレートとして保存した後、テンプレートに対する管理権限を取得します。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p>
   Or 
   <p>Current: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> /td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you save the project as a template</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## プロジェクトをテンプレートとして保存

<!--
Saving a project as a template differs in the Production and the Preview environments. 

### Save a project as a template in the Production environment


1. Go to the project that you want to save as a template. 
1. Click the **More** menu ![More icon](assets/more-icon.png), then **Save as Template**. 
1. Specify the following information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Provide a description for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Yes</strong>: Other users can find the template and attach it to projects.</p> </li> 
        <li><strong>No</strong>: Other users cannot find the template and cannot attach it to projects.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td>Use the drop-down list to select any custom forms to attach to the template. If any custom forms have already been associated with the project, all of the data fields from those custom forms are displayed.<br>You can include up to 10 custom forms on a single template.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Manage Forms** to remove or reorder the forms. For information about how to remove and reorder custom forms on the template, see [Custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

   ![Save as template first step](assets/save-as-template-first-step-350x159.png)

1. Click **Next Step.**
1. In the **Options** section, select the checkbox beside any information you want to clear from the template.

   ![Save as template options step](assets/save-as-template-options-step-350x109.png)

1. Click **Next Step.**
1. In the **Exclude** section, select any tasks that you want to exclude from the project.

   ![Save as template exclude](assets/save-as-template-exclude-350x205.png)

1. Click **Finish and Save Template.**

   Your template now appears in the list of available templates and can either be attached to an existing project or used to create a new one.


<div class="preview">

### Save a project as a template in the Preview environment

-->

1. テンプレートとして保存するプロジェクトに移動します。
1. ヘッダーのプロジェクト名の右側にある&#x200B;**詳細** メニュー![詳細アイコン &#x200B;](assets/qs-more-icon-on-an-object.png)をクリックし、**テンプレートとして保存**&#x200B;します。
1. 「**テンプレートとして保存**」セクションで、テンプレートの次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">テンプレート名</td> 
      <td>テンプレートの名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>テンプレートの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>次のオプションから選択します。</p> 
       <ul> 
        <li> <p><strong>はい</strong>：他のユーザーがテンプレートを見つけてプロジェクトに添付することができます。</p> </li> 
        <li><strong>いいえ</strong>：他のユーザーはテンプレートを見つけることができず、プロジェクトに添付できません。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>ドロップダウンリストを使用して、テンプレートに添付するカスタムフォームを選択します。カスタムフォームがすでにプロジェクトに関連付けられている場合は、それらのカスタムフォームのデータフィールドがすべて表示されます。<br>1 つのテンプレートに最大 10 個のカスタムフォームを含めることができます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 左側のパネルの&#x200B;**カスタム Forms**&#x200B;をクリックして、フォームを削除または並べ替えます。

   フォームを並べ替えるには、フォームを正しい順序でドラッグ&amp;ドロップします。
フォームを削除するには、フォームを選択し、**削除**&#x200B;をクリックします。 **キャンセル**&#x200B;をクリックして、選択したフォームを削除します。

   ![&#x200B; テンプレートとして保存ボックスのカスタムフォーム領域](assets/custom-forms-ara-in-save-as-template-box.png)

1. 必要に応じて、添付されたカスタムフォームの情報を更新します。 情報はテンプレートに転送されます。

1. 左側のパネルで「**オプション**」をクリックし、テンプレートに転送する情報の横にあるチェックボックスを選択します。 選択されていない項目は、テンプレートに転送されません。 デフォルトでは、すべてのオプションの選択が解除されています。

   テンプレートとして保存ボックスの![&#x200B; オプション領域](assets/options-area-in-save-as-template-box.png)

1. 左側のパネルで「**除外**」をクリックし、プロジェクトから除外するタスクを選択します。 デフォルトでは、すべてのタスクの選択が解除されます。

   ![&#x200B; テンプレートとして保存ボックス内の領域を除外](assets/exclude-area-save-as-template-box.png)

1. 画面の右上隅にある「**終了してテンプレートを保存**」をクリックします。

   テンプレートが使用可能なテンプレートのリストに表示され、既存のプロジェクトに添付することも、新しいプロジェクトの作成に使用することもできます。

