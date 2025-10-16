---
product-area: projects
navigation-topic: manage-tasks
title: タスクのプロジェクトへの変換
description: プロジェクト内のタスクを完了するために必要な労力が当初の予定よりも多い場合、タスクをプロジェクトに変換できます。
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 80%

---

# タスクをプロジェクトに変換

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

プロジェクト内のタスクを完了するために必要な労力が当初の予定よりも多い場合、タスクをプロジェクトに変換できます。

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
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p>テンプレートを使用してプロジェクトに変換する際の、テンプレートへの表示以上のアクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限</p> <p>テンプレートを使用してプロジェクトに変換する場合、テンプレートへの表示権限</p> <p>プロジェクトを作成すると、プロジェクトへの管理権限が付与されます。</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>View or higher access to&nbsp;Templates, when converting to a project using a template</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>View permissions on a template, if converting to a project using a template</p> <p>After creating the project, you have Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクをプロジェクトに変換する際の考慮事項

* タスクは、空のプロジェクトまたはテンプレートを使用したプロジェクトに変換できます。
* 元のタスクが削除されます。
* すべてのサブタスク、イシュー、メモは、新規プロジェクトにまとめられます。
* ドキュメント、ドキュメントのバージョンおよびプルーフは、新規プロジェクトに移動されます。
* タスクをプロジェクトに変換する場合、処理の制限は 5 分です。 タスクに多数のドキュメントが添付されていて、変換に失敗した場合は、一部のドキュメントを削除して、もう一度試す必要がある可能性があります。
* すべてのサブタスクとイシューのステータスと完了率は保持されます。
* タスクの担当者と、タスクをプロジェクトに変換したユーザーは、プロジェクトの共有ユーザーになります。
* プロジェクトの開始日は、タスクの開始日に設定されます。
* 次の表では、プロジェクト情報およびその情報がテンプレートから転送されるかまたはタスクから転送されるかを示します。

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>説明</td> 
    <td> <p>タスクの説明は、新規プロジェクトに転送されます。 </p> <p> タスクに説明がない場合、テンプレートの説明がプロジェクトに転送されます。 </p> <p>タスクとテンプレートの両方の「説明」フィールドが空の場合、プロジェクトのフィールドは空になります。 </p> </td> 
    </tr> 
    <tr> 
    <td>ステータス</td> 
    <td> テンプレート上のグループに選択されたデフォルトのステータス。テンプレートがグループに関連付けられていない場合、プロジェクトのステータスは、Workfront 管理者が設定のプロジェクト環境設定エリアで設定したデフォルトのステータスに設定されます。詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">システム全体のプロジェクト環境設定の指定</a>を参照してください。

  プロジェクトのステータスを更新するには、次のシナリオがあります。
  <ul>
    <li> タスクのステータスが「新規」の場合、プロジェクトのステータスは「計画」に設定されます。</li>
    <li> タスクのステータスが「処理中」の場合、プロジェクトのステータスは「現在」に設定されます。</li>
    <li> タスクのステータスが「完了」の場合、プロジェクトのステータスも「完了」に設定されます。</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>優先度</td> 
    <td>タスクからプロジェクトに転送するか、変換で使用する場合は、テンプレートから転送します。 </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>タスクから URL が新規プロジェクトに転送されます。 </p> <p> タスクで URL が指定されていない場合、テンプレートから URL がプロジェクトに転送されます。 </p> <p>イシューとテンプレートの両方の「URL」フィールドが空の場合、プロジェクトのフィールドは空になります。 </p> </td> 
    </tr> 
    <tr> 
    <td>プロジェクト状況のタイプ</td> 
    <td>テンプレートから転送します。</td> 
    </tr> 
    <tr> 
    <td>プロジェクト状況</td> 
    <td>設定エリアの Workfront 管理者が決定した、システムレベルのデフォルト環境設定に一致します。詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">カスタム条件をプロジェクトのデフォルトとして設定</a>を参照してください。
    </td> 
    </tr> 
    <tr> 
    <td>スケジュールの基点</td> 
    <td>テンプレートから転送します。</td> 
    </tr> 
    <tr> 
    <td>プロジェクトの日付</td> 
    <td> 
      <ul> 
      <li> <p><b>予定開始日</b>：テンプレートスケジュールのタイムゾーンに従って、テンプレートスケジュールの作業時間に基づく最も近い作業時間を事前に選択する必要があります。「スケジュールの基点」フィールドが「完了日」に設定されている場合、このフィールドは無効になります。 </p> </li> 
      <li> <p><b>完了予定日</b>：テンプレートスケジュールのタイムゾーンに従って、テンプレートスケジュールの作業時間に基づく最も近い作業時間を事前に選択する必要があります。「スケジュールの基点」フィールドが「開始日」に設定されている場合、このフィールドは無効になります。 </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>ポートフォリオ</td> 
    <td>テンプレートから転送します。それ以外の場合、このフィールドは空白になります。</td> 
    </tr> 
    <tr> 
    <td>プログラム</td> 
    <td>テンプレートから転送します。それ以外の場合、このフィールドは空白になります。</td> 
    </tr> 
    <tr> 
    <td>グループ</td> 
    <td><p> 次のシナリオが存在します。</p>
      <ul><li>変換の際にグループが指定された場合、そのグループがプロジェクトのグループになります。</li>
      <li>テンプレートを使用してプロジェクトに変換し、テンプレートにグループが存在し、変換時にグループを指定しない場合、テンプレートのグループが新規プロジェクトのグループになります。</li>
      <li> テンプレートにグループがなく、変換時にグループを指定しない場合、元のイシューのプロジェクトのグループが新規プロジェクトのグループになります。</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>会社</td>    
    <td>  テンプレートから転送します。それ以外の場合、このフィールドは空白になります。</td>

  </tr> 
    <tr> 
    <td>プロジェクト所有者</td> 
    <td>テンプレートの「テンプレート所有者」フィールドから転送します。それ以外の場合は、変換処理を実行するログイン中のユーザーに設定されます。 </td> 
    </tr> 
    <tr> 
    <td>プロジェクトスポンサー</td> 
    <td>テンプレートの「テンプレートスポンサー」フィールドから転送します。それ以外の場合、このフィールドは空白になります。</td> 
    </tr> 
    <tr> 
    <td>リソース管理者</td> 
    <td>テンプレートから転送します。それ以外の場合、このフィールドは空白になります。</td> 
    </tr> 
    <tr> 
    <td>タスク設定</td> 
    <td>テンプレートから転送します。</td> 
    </tr> 
    <tr> 
    <td>イシュー設定</td> 
    <td>テンプレートから転送します。 </td> 
    </tr> 
    <tr> 
    <td>アクセス</td> 
    <td> <p>テンプレートの「アクセス」セクションからの転送。 </p> </td> 
    </tr> 
    <tr> 
    <td>承認</td> 
    <td>テンプレートから転送します。タスクに関連付けられている承認は、変換中に削除されます。 </td> 
    </tr> 
  </tbody> 
  </table>


## タスクをプロジェクトに変換

1. プロジェクトに変換するタスクに移動します。
1. **その他**&#x200B;アイコン ![](assets/more-icon.png)、「**プロジェクトに変換**」の順にクリックします。
1. 次のいずれかのオプションを選択します。

   * **新規プロジェクト**：テンプレートを使用せずにプロジェクトを作成します。
   * 「**テンプレートから選択**」セクションのテンプレート

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. 表示される通知で「**続行**」をクリックします。
1. **プロジェクトに変換**&#x200B;ボックスで、次の情報を指定します。

   * **名前**：プロジェクトに名前を付けます。デフォルト名はタスクの名前です。 必須フィールドです。
   * **説明**：このプロジェクトの目的を説明します。
   * （条件付き）テンプレートからプロジェクトを作成することを選択した場合は、「**プロジェクトに変換**」ボックスの使用可能なフィールドを更新します。

     プロジェクトのフィールドの編集について詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

     >[!TIP]
     >
     >「プロジェクトに変換」ボックスの「財務」セクションのフィールドを更新するには、アクセスレベルの財務データに対する編集アクセス権が必要です。 アクセスレベルで財務データへの表示アクセス権を持っている場合、テンプレートからのすべての財務情報は新しいプロジェクトに転送され、問題を変換している間は編集できません。 詳しくは、[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)および[テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。

   * （オプション）**カスタムフォーム**&#x200B;を新規プロジェクトに追加します。

     >[!TIP]
     >
     >タスクに添付された複数オブジェクトのカスタムフォームをタスクとプロジェクトの両方で使用するように設定すると、フォームに保存されたすべての情報が変換時に保持されます。
     >
     >
     >変換用のテンプレートを使用していて、テンプレートに添付されたカスタムフォームに、タスクに添付されたカスタムフォームにもカスタムフィールドが含まれている場合は、タスクのフィールド値が新規プロジェクトで使用されます。ただし、タスクのカスタムフィールドが空の場合は、テンプレートの値が使用されます。

1. **プロジェクトに変換** をクリックします。
