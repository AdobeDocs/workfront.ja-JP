---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: レガシーフォームビルダーを使用したカスタムフォームへのセクション区切りの追加
description: カスタムフォームのカスタムフィールドとウィジェットを、見出し付きのセクションにグループ化できます。 これは、フォームに入力するユーザーに、整理されたエクスペリエンスを提示する場合に役立ちます。 また、特定のカスタムフィールドとウィジェットへのアクセスを特定のユーザーに制限する必要がある場合は、それらをセクションに配置し、そのセクションへのアクセス権をそれらのユーザーにのみ付与することができます。
feature: System Setup and Administration
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# レガシーフォームビルダーを使用したカスタムフォームへのセクション区切りの追加

カスタムフォームのカスタムフィールドとウィジェットを、見出し付きのセクションにグループ化できます。 これは、フォームに入力するユーザーに、整理されたエクスペリエンスを提示する場合に役立ちます。 また、特定のカスタムフィールドとウィジェットへのアクセスを特定のユーザーに制限する必要がある場合は、それらをセクションに配置し、そのセクションへのアクセス権をそれらのユーザーにのみ付与することができます。

例えば、システム管理者だけが表示または編集できる機密情報を追跡する必要がある場合は、「管理者のみ」の権限を持つセクション区切りを作成し、そのセクションに機密フィールドを配置できます。

セクションに対して選択するアクセス設定は、カスタムフォームが添付されるWorkfrontオブジェクトに対するユーザーの権限に直接関連付けられます。 ユーザがそのオブジェクトの表示、投稿、管理に対するアクセス権を持っているかどうかに基づいて、セクションの表示/非表示を切り替えることができます。 また、セクションを「管理者のみ」に設定して、システム管理者のアクセスレベルのユーザーのみがアクセスできるようにすることもできます。

オブジェクトに対する権限については、 [オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、 [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) および [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## カスタムフォームのセクションへのアクセスの作成と設定

1. カスタムフォームの作成または編集を開始します ( [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. カスタムフィールドとウィジェットをフォームに追加します。詳しくは、 [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) および [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. カスタムフォームの作成中または編集中に、 **フィールドを追加** タブ、クリック **断面分割**.

   ![](assets/click-section-break.jpg)

1. の **フィールド設定** タブで、セクションに必要なオプションを設定します。

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ラベル</td> 
      <td> <p>（必須）セクションの上に表示する説明的なラベルを入力します。 ラベルはいつでも変更できます。</p> <p><b>重要</b>:このラベルでは特殊文字を使用しないでください。 レポートでは正しく表示されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>ユーザーにセクションの目的を説明する場合は、テキストを入力します。 これは、カスタムフォームのセクションのラベルの下に表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ロジックの追加</td> 
      <td>表示ロジックを使用して、ユーザーがフォームに入力する際に複数選択カスタムフィールドで行った選択に基づいて、セクションをフォームに表示するかどうかを指定します。 詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">表示ロジックの追加とカスタムフォームへのロジックのスキップ</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>アクセスを許可</p> </td> 
      <td> <p> このセクションを表示し、そのフィールド値を編集するために、カスタムフォームが添付されるオブジェクトに対してユーザーが必要とする権限を選択します。 
       <p>以下の権限をで使用できます。 <b>オブジェクトにこのアクセス権を持つユーザーは、フィールド値を表示できます</b>:</p> 
         <ul>  
          <li><p><b>制限付き編集</b>:（オブジェクトがプロジェクト、タスク、タスク、タスクまたはユーザーの場合にのみ使用できます）。</p> 
          <p>プロジェクト、タスクまたはイシューの場合に、ユーザーがオブジェクトに投稿できるようにします。</p>
          <p>ユーザーがプロファイルを編集したり、オブジェクト（ユーザーの場合）に対するプロファイル権限を所有したりできます。</p></li> 
          <li><b>編集</b>:オブジェクトに対する権限の管理 </li> 
          <li><b>管理者のみ</b>:システム管理者のアクセスレベル</li> 
         </ul> </li> 
        <p>以下の権限をで使用できます。 <b>このオブジェクトへのアクセス権を持つユーザーは、フィールド値を編集できます</b>: </p> 
         <ul> 
          <li> <p><b>制限付き編集</b>:（オブジェクトがプロジェクト、タスク、タスク、タスクまたはユーザーの場合にのみ使用できます）。</p> 
           <p>オブジェクトがプロジェクト、タスク、またはイシューの場合は、この権限を持つユーザーがオブジェクトに貢献できます</p>
          <p>オブジェクトがユーザーの場合、この権限を持つユーザーは、プロファイルを編集したり、そのオブジェクトに対するプロファイル権限を所有したりできます。</p> 
          <li><b>編集</b>:オブジェクトに対する権限の管理 </li> 
          <li><b>管理者のみ</b>:システム管理者のアクセスレベル</li> 
         </ul> </li> 
       </ul> 
       <p>オブジェクトに対する権限については、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>.</p> 
       <p><b>メモ</b>:  
       <ul> 
       <li> <p>ここで指定した権限を持たないユーザーは、セクションのカスタムフィールドとウィジェットを表示できません。 </p> <p>これは、フィールドの値をレポートに表示する場合や、テキストモードのレポートで計算フィールドで使用する場合にも当てはまります。</p> </li> 
       <li> <p>複数のオブジェクトタイプをフォームに関連付けると、これらの手順で使用できる表示および編集権限が変更される場合があります。 詳しくは、 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">複数のオブジェクトタイプが、カスタムフォームのセクション区切り権限に与える影響</a> 」を参照してください。</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 1 つ以上のカスタムフィールドまたはウィジェットを新しいセクションにドラッグまたは追加します。

   これは、セクションを保存する前に必要です。

1. クリック **完了**.

   >[!TIP]
   >
   >次をクリックできます。 **適用** カスタムフォームの作成中はいつでも、変更内容を保存し、フォームを開いたままにすることができます。

1. 他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [カスタムフォームのプレビューと完了](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## 複数のオブジェクトタイプが断面の分割権限に与える影響 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

カスタムフォームセクションの改ページに対する制限付き編集権限は、プロジェクト、タスク、問題、ユーザーの各オブジェクトタイプに対してのみ使用できます。

制限付き編集権限を持つセクション区切りを持つカスタムフォームでは、他のオブジェクトタイプ (Portfolio、プログラム、ドキュメント、会社、請求レコード、繰り返し、費用、グループ ) をフォームに追加すると、編集権限に切り替えます。

>[!INFO]
>
>**例：** Project オブジェクトの種類に関連付けられたカスタムフォームでは、セクション区切りは、制限付き編集権限を持つように設定されます。
>
>Portfolioオブジェクトの種類をフォームに追加すると、フォーム内のセクション区切りに対して「制限付き編集」権限オプションを使用できなくなります。
>
>画面上のメッセージで、[ 編集 ] 権限に切り替えるように求められます。この権限は、[ 制限付き編集 ] に最も似ており、[ プロジェクト ] オブジェクトタイプと [Portfolio] オブジェクトタイプの両方に対応しています。
