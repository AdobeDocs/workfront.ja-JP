---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのプロジェクトテンプレートを作成および変更
description: グループエリアで管理するグループを表示している場合、そのグループとそのサブグループに関連付けられたプロジェクトテンプレートを表示し、操作できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '1284'
ht-degree: 100%

---

# グループのプロジェクトテンプレートを作成および変更

グループエリアで管理するグループを表示している場合、そのグループとそのサブグループに関連付けられたプロジェクトテンプレートを表示し、操作できます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示や操作を行うテンプレートに対する表示以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループエリアでグループのチームを表示、操作および作成

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ** ![](assets/groups-icon.png)」をクリックします。

1. テンプレートを作成または変更するグループの名前をクリックします。
1. 左側のパネルで「**テンプレート**」をクリックし、グループに関連付けられているテンプレートと、そのグループに含まれているサブグループを一覧表示します。

   このリストに表示するには、テンプレートへの表示アクセス権が必要です。このアクセス権について詳しくは、[テンプレートに対するアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)を参照してください。

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">テンプレートを追加</td> 
      <td> <p>「<strong>新規テンプレート</strong>」をクリックし、使用可能なオプションを使用して設定します。これらのオプションについて詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">プロジェクトテンプレートを作成</a>を参照してください。</p> <p>テンプレートは自動的にグループに関連付けられます。</p> <p>新しいテンプレートにグループの環境設定を適用する方法について詳しくは、<a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">テンプレートおよびテンプレートタスクに環境設定を適用する方法</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つまたは複数のテンプレートを編集</td> 
      <td> <p>少なくとも 1 つのテンプレートを選択して、編集アイコン <img src="assets/edit-icon.png"> をクリックし、使用可能な任意のオプションを使用して設定します。これらのオプションについて詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">プロジェクトテンプレートを編集</a>を参照してください。</p> <p>編集アイコンは、選択したすべてのテンプレートに対して編集アクセス権を持っている場合にのみ使用できます。このアクセス権について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートに対するアクセスの許可</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つまたは複数のテンプレートを削除</td> 
      <td> <p>1 つ以上のテンプレートを選択して、削除アイコン <img src="assets/delete.png"> をクリックします。</p> <p>このアイコンは、選択したすべてのテンプレートに対して編集アクセス権を持っている場合にのみ使用できます。このアクセス権について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートに対するアクセスの許可</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つまたは複数のテンプレートを共有</td> 
      <td> <p>少なくとも 1 つのテンプレートを選択して、共有アイコン <img src="assets/share-icon.png"> をクリックし、ドロップダウンメニューで次のオプションのいずれかをクリックします。</p> 
       <ul> 
        <li> <p><strong>テンプレート</strong>：表示される<strong>テンプレートアクセス</strong>ボックスで、名前を追加して、テンプレート自体にアクセスするユーザーを指定します。</p> <p>詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">プロジェクトテンプレートを共有</a>の記事にある<a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">テンプレートを共有</a>の節を参照してください。</p> </li> 
        <li><strong>プロジェクト</strong>：表示される<strong>プロジェクトアクセス</strong>ボックスで、名前を追加して、テンプレートから作成されたプロジェクトにアクセスするユーザーを指定します。</li> 
       </ul> <p>共有アイコンは、選択したすべてのテンプレートに対して共有アクセス権を持っている場合にのみ使用できます。このアクセス権について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートに対するアクセスの許可</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートのリストを書き出し</td> 
      <td><strong>書き出し</strong> <img src="assets/export.png"> をクリックし、書き出すリストのファイル形式を選択します。</td> 
     </tr> 
    </tbody> 
   </table>

## テンプレートおよびテンプレートタスクに環境設定を適用する方法 {#how-preferences-apply-to-templates-and-template-tasks}

プロジェクトテンプレートを作成する場合、以下の表に示す設定は、関連するプロジェクトまたはタスクの環境設定によって自動的に設定されます。

>[!NOTE]
>
>作成時にテンプレートをグループに関連付けたかどうかに応じて、グループレベルかシステムレベルのどちらかのプロジェクトまたはタスクの環境設定が、プロジェクトテンプレートに影響を与えます。
>
>グループに関連付けた場合は、グループレベルの環境設定が有効になります。これは、次のシナリオで発生します。
>
>* グループエリアからテンプレートを作成（この記事で説明）
>* キックスタートファイルを使用してテンプレートを作成する際に、グループを指定
>* API を使用してテンプレートを作成する際に、グループを指定
>
>新しいテンプレートをグループに関連付けなかった場合、システムレベルの環境設定が有効になります。これは、次のシナリオで発生します。（後でグループをテンプレートまたはテンプレートタスクに割り当てた場合、グループの環境設定は影響しません。）
>
>* テンプレートエリアからテンプレートを作成
>* キックスタートファイルを使用してテンプレートを作成する際に、グループを指定しない
>* API を使用してテンプレートを作成する際に、グループを指定しない
>

* [プロジェクトおよびタスクの環境設定で指定されたプロジェクトテンプレート設定](#project-template-settings-configured-by-project-and-task-preferences)
* [タスクの環境設定で設定されたテンプレートタスクの設定](#template-task-settings-configured-by-task-preferences)

### プロジェクトおよびタスクの環境設定で指定されたプロジェクトテンプレート設定 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>パフォーマンスインデックスメソッド</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクト環境設定の「パフォーマンスインデックスメソッド」、関連付けない場合は、同じシステムレベルのプロジェクト環境設定で設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>状況タイプ</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクト環境設定の「進行状態に応じて、プロジェクトの状態を自動的に設定する」、関連付けない場合は、同じシステムレベルのプロジェクト環境設定で設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>スケジュールの基点</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクト環境設定の「スケジュール元」、関連付けない場合は、同じシステムレベルのプロジェクト環境設定で設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ユーザーの休暇</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクト環境設定の「ユーザーの休暇」、関連付けない場合は、同じシステムレベルのプロジェクト環境設定で設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>更新タイプ</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクト環境設定の「プロジェクトタイムラインを自動的に再計算する」、関連付けない場合は、同じシステムレベルのプロジェクト環境設定で設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>「アクセス」セクション設定</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、「アクセス」セクションのグループレベルのタスク環境設定、関連付けない場合は、同じシステムレベルのプロジェクト環境設定で設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表に示すプロジェクト環境設定の詳細については、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

タスクとイシューの環境設定について詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

>[!NOTE]
>
>* 既存のプロジェクトテンプレートに関連付けられているグループを変更しても、テンプレートの設定は変わりません。
>* 既存のテンプレートタスクを別のテンプレートに移動した場合、新しいテンプレートに関連付けられているグループに関係なく、テンプレートタスクで次の設定は変更されません。
>   * 期間タイプ
>   * 収益タイプ
>   * コストタイプ
>
>  ただし、テンプレートタスクは、新しいテンプレートの「誰かがタスクに割り当てられたとき」の設定の影響を受けます。詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)の記事の[アクセス](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access)の節を参照してください。
>
>* 管理者がプロジェクトをテンプレートとして保存すると、そのテンプレートのすべての設定が、グループを含むプロジェクトから継承されます。
>
>  管理者が、テンプレートを使用してタスクまたはイシューをプロジェクトに変換すると、テンプレートの設定はすべて、テンプレートに既に保存されている内容によって決まります。
>

### タスクの環境設定で設定されたテンプレートタスクの設定 {#template-task-settings-configured-by-task-preferences}

テンプレートタスクを作成する場合、一部の設定は、関連するタスクの環境設定によって自動的に設定されます。これらの設定を次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>期間タイプ </p> </td> 
   <td> <p>テンプレートをグループに関連付ける場合は、グループレベルのタスク環境設定の「期間タイプ」で設定します。関連付けない場合は、同じシステムレベルのタスクとイシューの環境設定を設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>収益タイプ</p> </td> 
   <td> <p>テンプレートをグループに関連付ける場合は、グループレベルのタスク環境設定の「収益タイプ」、関連付けない場合は、同じシステムレベルのタスクとイシューの環境設定で設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>コストタイプ </p> </td> 
   <td> <p> テンプレートをグループに関連付ける場合は、グループレベルのタスク環境設定の「コストタイプ」、関連付けない場合は、同じシステムレベルのタスクとイシューの環境設定で設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表に示すタスク環境設定については、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。
