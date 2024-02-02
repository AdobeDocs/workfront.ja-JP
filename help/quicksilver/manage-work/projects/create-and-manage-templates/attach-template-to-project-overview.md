---
content-type: overview
product-area: templates
keywords: 上書き,フィールド,上書きされた
navigation-topic: templates-navigation-topic
title: プロジェクトへのテンプレート添付の概要
description: テンプレートを既存のプロジェクトに添付する場合、テンプレートの情報に応じて、プロジェクトの情報の一部が修正されます。プロジェクトの情報で変更されないものもあります。
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '1247'
ht-degree: 100%

---

# プロジェクトへのテンプレート添付の概要

テンプレートを既存のプロジェクトに添付する場合、テンプレートの情報に応じて、プロジェクトの情報の一部が修正されます。プロジェクトの情報で変更されないものもあります。

テンプレートをプロジェクトに添付する方法について詳しくは、[プロジェクトへのテンプレートの添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

## テンプレートをプロジェクトに追加する際の考慮事項

プロジェクトにテンプレートを追加する際は、次の点を考慮してください。

* アクティブなテンプレートのみをプロジェクトに添付できます。
* プロジェクトのステータスが完了、無効または承認待ちの場合は、Adobe Workfront 管理者またはグループ管理者がプロジェクト環境設定エリアでこの機能を有効にしている場合にのみ、プロジェクトにテンプレートを添付できます。プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
* 特定のテンプレートタスクを添付プロセスでの追加から除外しない限り、すべてのテンプレートタスクが既存のプロジェクトに追加されます。
* ほとんどのテンプレート設定がプロジェクトに追加されます。一部のプロジェクト設定は保持されます。詳しくは、この記事の[テンプレートを添付する際のプロジェクトフィールドの変更について](#understand-changes-to-project-fields-when-attaching-a-template)の節を参照してください。

## テンプレートを添付する際のプロジェクトフィールドの変更について {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>プロジェクトにテンプレートを添付する方法は、テンプレートからプロジェクトを作成する方法とは異なります。テンプレートからプロジェクトを作成すると、すべてのテンプレートフィールドが新しいプロジェクトに転送されます。テンプレートを添付しても、既存のプロジェクトフィールドの一部は変更されません。

一部のテンプレート設定は、テンプレートの添付プロセス中に除外するよう特にマークしない限り、自動的にプロジェクトに転送されます。除外するようマークすると、プロジェクトフィールドの値が保持されます。

ただし、プロジェクトにテンプレートを添付する際に、管理できないプロジェクトフィールドもあります。詳しくは、[プロジェクトへのテンプレートの添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

次の表は、テンプレートを添付する際にプロジェクトフィールドに適用されるデフォルトの動作と、添付プロセス中にデフォルトの動作を上書きするよう管理できるフィールドを示しています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>フィールド</td> 
   <td>テンプレートの添付プロセスでの動作（デフォルト）</td> 
   <td>添付プロセスでフィールドの更新の管理が可能 </td> 
  </tr> 
  <tr> 
   <td>説明</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>ステータス</p> </td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>プロジェクトでフィールドが空の場合は、テンプレートから転送されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>優先度</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>状況タイプ</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>スケジュールモード</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予定日</td> 
   <td>追加されたタスクに応じて変更される場合があります</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>実際の日付</td> 
   <td>追加されたタスクに応じて変更される場合があります</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>会社</td> 
   <td>プロジェクトでフィールドが空の場合は、テンプレートから転送されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予定時間数</td> 
   <td>追加されたタスクに応じて変更される場合があります</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト所有者</td> 
   <td>プロジェクトでフィールドが空の場合は、テンプレートから転送されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>プロジェクトスポンサー</td> 
   <td>プロジェクトでフィールドが空の場合は、テンプレートから転送されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リソース管理者</td> 
   <td>プロジェクト上の既存のリソースマネージャーのリストに追加されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>カスタムフォーム</td> 
   <td>既にプロジェクトに存在するフォームに加えて、プロジェクトに追加されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予算</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>通貨</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>PIM</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予定利益</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>実際のメリット</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>マイルストーンパス</td> 
   <td>プロジェクトでフィールドが空の場合は、テンプレートから転送されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>完了モード</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>概要完了モード</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新タイプ</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>スケジュール</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ユーザーの休暇</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リソースの標準化モード</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスク（プロジェクトフィールド）</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リソースプール</td> 
   <td>プロジェクト上の既存のリソースプールのリストに追加されました</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時間タイプ</td> 
   <td> <p>添付プロセス中に選択を解除しても、プロジェクトの時間タイプの設定は変更されません。 </p> <p>選択した場合、テンプレート設定がプロジェクトに転送されます。プロジェクトとテンプレートの両方で時間タイプフィルターが「はい」に設定されている場合、テンプレートの時間タイプがプロジェクトの時間タイプに追加されます。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>リマインダー通知</td> 
   <td> <p>プロジェクト上の既存のリマインダーのリストに追加されます。 </p> <p>添付プロセス中に選択を解除しても、プロジェクトのリマインダー通知は変更されません。 </p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>デフォルトのタスク承認プロセス</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>デフォルトのタスクカスタムフォーム</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>作業量</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>ユーザーによるインラインでのイシューの追加を許可</span> </td> 
   <td><span>プロジェクト情報は保持されます</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>すべての設定</td> 
   <td>テンプレート設定によってプロジェクトの設定が上書きされます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>既存のプロジェクトタスクに加えて、タスクリストの下部に追加されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>ドキュメント</td> 
   <td>既存のプロジェクトドキュメントに加えて、プロジェクトに追加されました</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>リスク（プロジェクトのリスク領域のオブジェクト）</td> 
   <td>既存のプロジェクトリスクに加えて、プロジェクトに追加されました </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>承認プロセス</td> 
   <td>テンプレートから転送済み</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>請求レート</td> 
   <td> <p>プロジェクトの既存の請求率に加えて、テンプレートから転送されました。 </p> <p>プロジェクトとテンプレートの両方で同じ担当業務の請求率が異なっても、プロジェクトの請求率は変更されません。 </p> </td> 
   <td> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>請求記録</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>プロジェクトの既存の費用に加えて、テンプレートから転送済み</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>財務情報</td> 
   <td> <p>添付プロセスでこれを選択すると、次のフィールドがプロジェクトに転送または追加されます。</p> 
    <ul> 
     <li> <p>固定コスト</p> <p>このオプションを選択すると、プロジェクトの更新された固定コストが次の式で計算されます。</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>固定収益</p> <p>このオプションを選択すると、プロジェクトの更新された固定収益が次の数式で計算されます。</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>タスクのコストタイプ</p> <p>テンプレートから転送済み</p> </li> 
     <li> <p>タスクの収益タイプ</p> <p>テンプレートから転送済み</p> </li> 
    </ul> <p>添付プロセス中にこのフィールドの選択を解除すると、次の処理が行われます。</p> 
    <ul> 
     <li> <p>プロジェクトの固定コストと固定収益は保持されます。</p> </li> 
     <li> <p>テンプレートから追加されたタスクのコストタイプと収益タイプが、「コストなし」と「請求不可」に設定されます</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>時間</td> 
   <td>プロジェクト情報は保持されます</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>キューの詳細、トピックグループ、キューのトピック、ルーティングルール</td> 
   <td> <p>テンプレートから転送済み</p> <p>添付プロセス中に「<strong>キューのプロパティとイシューの設定</strong>」オプションを選択すると、テンプレートのキューの詳細によってプロジェクトのキューの詳細が上書きされます。この場合、テンプレートの「ルーティング規則」、「キュートピック」および「トピックグループ」が、プロジェクトの各項目に追加されます。<br>プロジェクトがリクエストキューとして設定されており、プロジェクトに添付したテンプレートがリクエストキューとして設定されていない場合、「<strong>キューのプロパティとイシューの設定</strong>」チェックボックスがオンになっていると、プロジェクトのキュー情報は削除されます。<br>「<strong>キューのプロパティとイシューの設定</strong>」ボックスの選択を解除すると、プロジェクトのすべてのキュー設定が保存されますが、テンプレートのキュー設定は添付されません。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>タスクの制約</td> 
   <td> <p>テンプレートから転送済み </p> <p>添付プロセス中に選択を解除すると、プロジェクトの「スケジュールの基点」設定に応じて、タスク制約が「できるだけ早く」か「できるだけ遅く」に設定されます。 </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓</p> </td> 
  </tr> 
  <tr> 
   <td>タスク先行タスク</td> 
   <td> <p>テンプレートから転送済み</p> <p>添付プロセス中に選択を解除すると、テンプレートタスク間の先行タスク接続がすべて削除されます。</p> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>共有オプション</td> 
   <td> <p>添付プロセス中に選択を解除しても、プロジェクトの権限は変更されません。</p> <p>添付プロセス中に選択した場合、テンプレート権限はプロジェクトの権限に追加または上書きされます。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>ユーザー A がプロジェクトに対する表示権限を持ち、テンプレートに対する管理権限を持っている場合、テンプレートを添付すると、ユーザー A はプロジェクトに対する管理アクセス権を取得します。</p> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

 

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p>&nbsp;</p>
</div>
-->

 
