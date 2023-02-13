---
title: テンプレートの共有
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront管理者は、アクセスレベルを割り当てる際に、テンプレートの表示や編集に対するアクセス権をユーザーに付与できます。 テンプレートを編集するには、プランライセンスが必要です。
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# テンプレートの共有

Adobe Workfront管理者は、アクセスレベルを割り当てる際に、テンプレートの表示や編集に対するアクセス権をユーザーに付与できます。 テンプレートを編集するには、プランライセンスが必要です。

テンプレートへのアクセス権の付与について詳しくは、 [テンプレートへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

ユーザーは、付与したアクセスレベルに加えて、特定のテンプレートを共有する他のユーザーから、特定のテンプレートを表示または管理する権限を受け取ることもできます。

>[!NOTE]
>
>権限レベルは、アクセスレベル内で機能します。 例えば、ユーザーは、アクセスレベルでテンプレートの表示のみが許可されている場合、テンプレートを管理する権限を受け取ることはできません。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

## テンプレートを共有する際の考慮事項

* 以下の考慮事項に加えて、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* テンプレートの作成者およびテンプレート所有者には、デフォルトでテンプレートに対する管理権限があります。 ユーザーをテンプレート所有者に指定する方法については、 [プロジェクトテンプレートの編集](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* テンプレートを共有する際に、以下を共有できます。

   * テンプレート

      テンプレートの共有方法について詳しくは、 [プロジェクトテンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

      テンプレートには、次の権限を付与できます。

      * ビュー

         ![](assets/view-on-template-262x221.png)

      * 管理

         ![](assets/manage-on-template-225x280.png)
   * このテンプレートを使用して作成される今後のプロジェクト。 個々のプロジェクトと同じレベルの権限を、テンプレートから作成されたプロジェクトに付与できます。 

      テンプレートレベルでテンプレートからプロジェクトを共有する方法については、 [プロジェクトテンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md).


* テンプレートから作成されたテンプレートまたはプロジェクトを共有する場合、ユーザーは、デフォルトで、テンプレートまたはプロジェクトに関連付けられているすべての子オブジェクトに同じ権限を継承します。

   Workfrontのオブジェクトの階層について詳しくは、  [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* テンプレートを共有する場合、特に指定のない限り、テンプレートから作成されるすべてのテンプレートタスクとドキュメント、および今後のプロジェクトの問題は同じ権限を継承します。

   プロジェクトに対するユーザーの権限に基づいて、テンプレートタスクへのアクセスを管理したり、プロジェクトに関する問題を管理したりする方法については、 [アクセス](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) 記事のセクション [プロジェクトテンプレートの編集](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* Workfrontの管理者は、ドキュメントがユーザーのアクセスレベルの上位のオブジェクトから権限を継承するかどうかを指定できます。 ドキュメントに対する継承された権限の制限について詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## テンプレート共有の詳細設定

次の表に、ユーザーにテンプレートの表示または管理を許可する際に付与できる権限を示します。 テンプレートを共有する手順については、 [テンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) 記事内 [プロジェクトテンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アクション</th> 
   <th>管理</th> 
   <th>ビュー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>コピー</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>削除</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレートの詳細を編集</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>テンプレートの表示</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>共有</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>システム全体で共有</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>ドキュメントを追加</p> <p>ヒント：プロジェクトテンプレートにドキュメントを追加する人が、プロジェクトにドキュメントを追加すると考える場合があります。 この設定を無効にすると、受信者に対してこの設定を防ぐことができます。</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

テンプレートから作成されたプロジェクトにユーザーに付与する権限を理解するには、 [Adobe Workfrontでプロジェクトを共有する](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
