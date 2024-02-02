---
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront でのグループ化の作成
description: カスタムグループを最初から作成することも、既存のグループ化をカスタマイズすることもできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 64cc52b7-d97b-4b41-9101-530e7db2d26e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '496'
ht-degree: 100%

---

# Adobe Workfront でのグループ化の作成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is a third part of an article split in 3 about creating and customizing groupings (2 how-tos and one reference) </p>
-->

レポートまたはリストの結果は、グループ化を使用して整理できます。グループ化では、特定の情報に基づいて情報が分類されます。

カスタムグループを最初から作成することも、既存のグループ化をカスタマイズすることもできます。最初からグループ化を作成するには、次の手順に従います。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>リクエスト以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへの編集アクセス権（レポートでグループ化を作成するため）</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>レポートへの管理権限でレポート内のグループ化を編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## グループ化を作成

1. カスタムグループ化を作成するレポートまたはリストに移動します。
1. **グループ化**&#x200B;アイコンをクリックします。

   ![新規グループ化の選択](assets/newgrouping-nwe-standard-350x304.png)

1. 「**新規グループ化**」をクリックします。
グループ化を作成するためのインターフェイスビルダーが起動します。

1. 「**グループ化のプレビュー**」セクションで、「**グループ化の追加**」をクリックして、レポート内の情報の整理方法を定義します。レポート内のグループ化の表示についてプレビューを次に示します。

1. レポート内の情報を整理する方法を表すフィールドの名前を入力し、ドロップダウンリストに表示されたらクリックします。
1. （オプションおよび条件付き）更新されたリストでグループ化を作成する場合、グループ化の結果を展開された状態ではなく折りたたまれた状態で表示するには、「**既定としてこのグループ化を折りたたむ**」を選択します。この設定はデフォルトでは無効になっており、グループ化の結果は常に展開されたリストで表示されます。

   更新されたリストと従来のリストについては、[Adobe Workfront のリストの基本を学ぶ](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)の記事の[更新されたリストと従来のリストの違い](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated)の節を参照してください。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Edit existing grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* リストを表示しているときにグループ化を手動で調整すると、ログアウトするまで Workfront に手動の設定が記憶されます。再度ログインすると、この設定に従ってリストが表示されます。
   >* グループ化の結果は、グラフ要素または従来のリストからアクセスした後で常に展開されて表示されます。この場合、この設定は無視されます。

1. 手順 4、5 および 6 を繰り返して、追加のグループ化を定義します。\
   情報を整理するために、最大 3 つのグループを定義できます。マトリックスレポートを作成すると、最大 4 つのグループに分けて情報を整理できます。マトリックスレポートについて詳しくは、[マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)を参照してください。

1. 「**グループ化の保存**」をクリックします。

## 追加情報

関連トピック：

* [Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
* [レポート要素：フィルター、ビューおよびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)
* [既存のグループを編集](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h1>Create or edit groupings in Adobe Workfront</h1>
<p class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.</p>
<p>You can organize the results of a report or list with a grouping. Groupings categorize data based on a particular piece of information. For more information on groupings, see <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Groupings overview in Adobe Workfront</a>.</p>
<p>You can create groupings in lists and reports in the following ways:</p>
<ul>
<li> <p>From scratch</p> </li>
<li> <p>Edit an existing grouping that you originally created or that was shared with you</p> </li>
<li> <p>Copy an existing grouping</p> <p>To copy an existing grouping, you can edit it and save it as a new grouping.</p> </li>
</ul>
<h2>Types of grouping-building interfaces</h2>
<p>You can create groupings using the types of grouping builders described in the table below.</p>
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td><strong>Builder type</strong> </td>
<td><strong>Grouping object</strong> </td>
<td><strong>Where available</strong> </td>
</tr>
<tr>
<td><strong>Standard builder</strong> </td>
<td>All objects</td>
<td>Reports and lists</td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td rowspan="2">
<div class="preview">
<p><strong>Beta builder</strong> </p>
</div> </td>
<td>
<div class="preview">
<p>Projects</p>
<p>Tasks</p>
<p>Issues</p>
</div> </td>
<td>
<div class="preview">
<p>Lists</p>
</div> </td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<td colspan="2"> <note type="note">
<span class="preview">Beta builders for groupings are not available in reports.</span>
</note> </td>
</tr>
</tbody>
</table>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Consider the following when creating groupings using the different builders:
</div>
<ul data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<li>
<div class="preview">
You can switch back and forth between the standard builder and the beta builder, where the beta option is available.
</div> </li>
<li>
<div class="preview">
After you have enabled the beta builder in one area, it is the default experience for all areas where it is available.
</div> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span class="preview">If you enable the beta builder in a project list, it is the default experience for building task and issue groupings in lists as well.</span> </p> </li>
<li> <p><span class="preview">Groupings are available in both builders, regardless of which experience you used to originally build them.</span> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span class="preview">If you created a grouping using the standard builder, you can find and modify it in the beta builder interface as well.</span> </p> </li>
</ul>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Request or higher</p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to&nbsp;filters, views, and groupings</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage access to a grouping to be able to modify or copy it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
<h2>Create a grouping in the standard builder</h2>
<p>Regardless of the method you use to create groupings, creating a grouping from scratch or from an existing grouping is similar.</p>
<ol>
<li value="1"> <p>Go to a list or a report where you want to create a grouping or that contains the grouping that you want to customize.</p> </li>
<li value="2"> <p>Click the <strong>Grouping</strong> icon .</p> <p> <img src="assets/newgrouping-nwe-standard-350x304.png" alt="Select New Grouping" style="width: 350;height: 304;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>New Grouping</strong> at the top of the list of groupings.</p>
<p>Or</p>
<p>Hover over the grouping you want to modify and click the <strong>Edit</strong> icon <img src="assets/edit-icon.png">.</p>
</div> <p>The builder for customizing the grouping opens.</p> </li>
<li value="4"> <p>In the <strong>Grouping Preview</strong> section, click <strong>Add Grouping</strong> to define how you want information in the report to be organized. A preview of what the grouping looks like in the report is shown below.</p> </li>
<li value="5"> <p>Begin typing the name of the field that represents the way that you want to organize information in the report, then click it when it appears in the drop-down list.</p> </li>
<li value="6"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional and conditional) When customizing a grouping in an updated list, select <strong>Collapse this grouping by default</strong> if you want the results in the grouping to display collapsed rather than expanded.&nbsp;This setting is disabled by default and the results of the grouping always display in the expanded list.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> For information about updated and legacy lists, see the section <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated" class="MCXref xref">The difference between the updated and the legacy lists</a>&nbsp;in the article <a href="../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md" class="MCXref xref">Get started with lists in&nbsp;Adobe Workfront</a>.</p>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Edit existing grouping article and Common uses of text mode)</p>
<note type="tip">  
<ul>
<li>When you manually adjust groupings when viewing a list, Workfront remembers your manual preference until you log out. When you log back in, the list displays according to this setting.</li>
<li> <p>The results of a grouping always display expanded after accessing them from a chart element or in a legacy list. In these cases, this setting is ignored.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Legacy lists in classic do NOT have this option; legacy lists in NWE DO have this option but it's not functional; this is conditioned only for QS)</p>
</li>
</ul>
</note> </li>
<li value="7"> <p>Repeat Steps  4, 5, and 6  to define additional groupings.</p> <p>You can define up to three groupings for organizing information. You can further organize your information with up to four groupings by creating a matrix report. For more information on matrix reports, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Create a matrix report</a>.</p> </li>
<li value="8"> <p>(Optional) Click <strong>Switch to Text Mode</strong> to add a grouping using the Text Mode interface.</p> <p>For more information about creating a grouping using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>.</p> </li>
<li value="9"> <p>Click <strong>Save Grouping</strong> to create a new grouping.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Save as New Grouping</strong> to create a new grouping from the selected one.</p> <p>The new grouping displays in the list of groupings.</p> </li>
<li value="10"> <p>(Optional) Remove groupings you no longer want to display in the list.</p> <p>For information, see <a href="../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md" class="MCXref xref">Remove filters, views, and groupings</a>.</p> </li>
</ol>
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Create a grouping in the beta builder</h2>
<h3>Enable the beta builder</h3>
<p>The beta builder toggle is disabled by default. You must enable it to use the beta builder.</p>
<ol>
<li value="1">Go to a project, task, or issue list.</li>
<li value="2"> <p>Click the <strong>Grouping</strong> icon <img src="assets/groupingicon.png" alt="Grouping icon">, then enable the beta builder toggle.</p> <p>The beta builder interface opens.</p> <note type="tip">
The header of the grouping builder interface is blue when the beta builder is enabled. This enables the beta builder for all areas of Workfront where it is available.
</note> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replace shot below!)</p>
<p> <img src="assets/beta-toggle-groupings-nwe-350x300.png" alt="Beta toggle for groupings" style="width: 350;height: 300;"> </p> </li>
<li value="3"> <p>Continue with <a href="#create-a-grouping-in-the-beta-builder" class="MCXref xref">Create a grouping in the beta builder</a>, below.</p> </li>
</ol>
<p><strong>Create a grouping in the beta builder</strong></p>
<ol>
<li value="1"> <p>Go to a project, task, or issue list where you want to create a grouping, and click the <strong>Grouping</strong> icon <img src="assets/groupingicon.png" alt="Grouping icon">.</p> </li>
<li value="2"> <p>Click <strong>New Grouping</strong> to create a new grouping.</p> <p>Or</p> <p>Hover over an existing grouping in the My groupings area, then click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> to edit an existing grouping.</p> <p>Or</p> <p>Hover over an existing grouping in the My groupings area, select the <strong>More</strong> icon <img src="assets/more-icon.png" alt="More icon">, and select <strong>Duplicate</strong> to copy a grouping.</p> </li>
<li value="3"> <p>Start typing the name of a field in the Group by area, then select it when it displays in the list.</p> <p>You can also select <strong>Search all fields</strong> to view a list of all fields to group by. The fields in the advanced search are grouped by object category.</p> <note type="tip">
As you build the grouping, the results appear immediately in the list.
</note> </li>
<li value="4"> <p>(Optional) Click <strong>Add grouping</strong> to add a second or third grouping.</p> <p> <img src="assets/gouping-groupby-options-350x202.png" alt="Group by options" style="width: 350;height: 202;"> </p> </li>
<li value="5"> <p>(Optional) To reorder the groupings, select a grouping and drag it to the new position.</p> <p>Or</p> <p>Select a grouping and use the keyboard arrow keys to change the order.</p> </li>
<li value="6"> <p>(Optional) Make other selections for the groupings as needed:</p>
<ul>
<li> <p>When grouping by date you must choose a date option such as week, month, or quarter.</p> </li>
<li> <p>Select <img src="assets/grouping-expandicon.png" alt="Expand grouping icon"> to set a grouping to be expanded by default.</p> </li>
<li> <p>Select <img src="assets/delete.png" alt="Delete icon"> to delete a grouping.</p> </li>
</ul> <p> <img src="assets/grouping-editgrouping-350x409.png" alt="Edit grouping" style="width: 350;height: 409;"> </p> </li>
<li value="7"> <p>(Optional) Select <strong>Text Mode</strong> to continue building the grouping using the Text Mode interface.</p> <p>For more information about creating a grouping using the text mode interface, see <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md" class="MCXref xref">Edit text mode in a grouping</a>.</p> </li>
<li value="8"> <p>(Optional) To use the grouping as an ad hoc grouping without saving it:</p>
<ul>
<li> <p>When working in a new grouping, close the beta builder.</p> </li>
<li> <p>When editing an existing grouping, select <strong>Apply</strong>.</p> </li>
</ul> </li>
<li value="9"> <p>Select <strong>Save as new</strong> for a new grouping, or <strong>Save</strong> for an existing grouping.</p> </li>
<li value="10"> <p>Type a name for the grouping.</p> </li>
<li value="11"> <p>(Optional) Select an icon for the grouping to represent the field type.</p> </li>
<li value="12"> <p>(Optional) Type a description of the grouping.</p> </li>
<li value="13"> <p>Select <strong>Save</strong>.</p> <p>The grouping is saved in the My groupings list.</p> </li>
</ol>
</div>
</div>
-->
