---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのプロジェクトテンプレートの作成と変更
description: '[ グループ ] 領域で管理するグループを表示している場合、そのグループとそのサブグループに関連付けられたプロジェクトテンプレートを表示し、操作できます。'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# グループのプロジェクトテンプレートの作成と変更

[ グループ ] 領域で管理するグループを表示している場合、そのグループとそのサブグループに関連付けられたプロジェクトテンプレートを表示し、操作できます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示および操作するテンプレートに対するアクセス権以上の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループ領域で、グループのテンプレートの表示、操作、作成を行います

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. テンプレートを作成または変更するグループの名前をクリックします。
1. 左側のパネルで、 **テンプレート** グループに関連付けられているテンプレートと、そのグループに含まれているサブグループを一覧表示します。

   このリストに表示するには、テンプレートへの表示アクセス権が必要です。 このアクセスについて詳しくは、 [テンプレートへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">テンプレートを追加</td> 
      <td> <p>クリック <strong>新規テンプレート</strong>を設定し、使用可能なオプションを使用して設定します。 これらのオプションについて詳しくは、 <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">プロジェクトテンプレートの作成</a>.</p> <p>テンプレートはグループに自動的に関連付けられます。</p> <p>新しいテンプレートにグループの環境設定を適用する方法について詳しくは、 <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">テンプレートおよびテンプレートタスクに環境設定を適用する方法</a> 」を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つ以上のテンプレートの編集</td> 
      <td> <p>少なくとも 1 つのテンプレートを選択して、編集アイコンをクリックします。 <img src="assets/edit-icon.png">を設定したら、使用可能な任意のオプションを使用して設定します。 これらのオプションについて詳しくは、 <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">プロジェクトテンプレートの編集</a>.</p> <p>編集アイコンは、選択したすべてのテンプレートに対して編集アクセス権を持っている場合にのみ使用できます。 このアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートへのアクセス権の付与</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つ以上のテンプレートの削除</td> 
      <td> <p>少なくとも 1 つのテンプレートを選択して、削除アイコン <img src="assets/delete.png">.</p> <p>このアイコンは、選択したすべてのテンプレートに対して編集アクセス権を持っている場合にのみ使用できます。 このアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートへのアクセス権の付与</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つ以上のテンプレートを共有する</td> 
      <td> <p>少なくとも 1 つのテンプレートを選択して、共有アイコンをクリックします。 <img src="assets/share-icon.png">をクリックし、ドロップダウンメニューで次のいずれかのオプションをクリックします。</p> 
       <ul> 
        <li> <p><strong>テンプレート</strong>:内 <strong>テンプレートアクセス</strong> 表示されるボックスに、名前を追加して、テンプレート自体にアクセスするユーザーを指定します。</p> <p>詳しくは、 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">テンプレートの共有</a> 記事内 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">プロジェクトテンプレートの共有</a>.</p> </li> 
        <li><strong>プロジェクト</strong>:内 <strong>プロジェクトアクセス</strong> 表示されるボックスに名前を追加して、テンプレートから作成されたプロジェクトにアクセスするユーザーを指定します</li> 
       </ul> <p>「共有」アイコンは、選択したすべてのテンプレートに対して「共有」アクセス権を持っている場合にのみ使用できます。 このアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">テンプレートへのアクセス権の付与</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">テンプレートのリストをエクスポート</td> 
      <td>クリック <strong>書き出し</strong> <img src="assets/export.png">次に、書き出すリストのファイル形式を選択します。</td> 
     </tr> 
    </tbody> 
   </table>

## テンプレートおよびテンプレートタスクに環境設定を適用する方法 {#how-preferences-apply-to-templates-and-template-tasks}

プロジェクトテンプレートを作成する場合、以下の表に示す設定は、関連するプロジェクトまたはタスクのプリファレンスによって自動的に構成されます。

>[!NOTE]
>
>グループレベル、システムレベルのプロジェクトまたはタスクの環境設定は、作成時にテンプレートをグループに関連付けたかどうかに応じて、プロジェクトテンプレートに影響を与えます。
>
>グループに関連付けた場合は、グループレベルの環境設定が有効になります。 これは、次のシナリオで発生します。
>
>* この記事で説明するように、「グループ」領域からテンプレートを作成します。
>* Kickstart ファイルを使用してテンプレートを作成する際にグループを指定します
>* API を使用してテンプレートを作成する際に、グループを指定します
>
>新しいテンプレートをグループに関連付けなかった場合、システムレベルの環境設定が有効になります。 これは、以下のシナリオで発生します。 （後でグループをテンプレートタスクまたはテンプレートタスクに割り当てた場合、グループの環境設定は影響を受けません）。
>
>* テンプレートは、「テンプレート」領域で作成します
>* キックスタートファイルを使用してテンプレートを作成する際に、グループを指定しない
>* API を使用してテンプレートを作成する際に、グループを指定しない
>


* [プロジェクトおよびタスクの環境設定で設定されたプロジェクトテンプレート設定](#project-template-settings-configured-by-project-and-task-preferences)
* [タスクの環境設定で設定されたテンプレートタスク設定](#template-task-settings-configured-by-task-preferences)

### プロジェクトおよびタスクの環境設定で設定されたプロジェクトテンプレート設定 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>パフォーマンス インデックス メソッド</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクトプリファレンス「パフォーマンスインデックスメソッド」で設定し、関連付けない場合は同じシステムレベルのプロジェクトプリファレンスを設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>状況タイプ</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクトプリファレンス「進捗状況ステータスに基づいてプロジェクトの条件を自動的に設定」、関連付けない場合は同じシステムレベルのプロジェクトプリファレンスで設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>スケジュール元</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクトプリファレンス「スケジュール元」で設定し、関連付けない場合は同じシステムレベルのプロジェクトプリファレンスで設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ユーザーのタイムオフ</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクトプリファレンス「ユーザーのタイムオフ」で設定し、関連付けない場合は、同じシステムレベルのプロジェクトプリファレンスで設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>更新タイプ</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は、グループレベルのプロジェクトプリファレンス「プロジェクトタイムラインは自動的に再計算されます」、関連付けない場合は同じシステムレベルのプロジェクトプリファレンスが設定されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>セクション設定にアクセス</p> </td> 
   <td> <p>新しいテンプレートをグループに関連付ける場合は「アクセス」セクションのグループレベルのタスクプリファレンスで設定し、関連付けない場合は同じシステムレベルのプロジェクトプリファレンスで設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表に示すプロジェクトプリファレンスの詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

タスクと問題の環境設定については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* 既存のプロジェクトテンプレートに関連付けられているグループを変更しても、テンプレートの設定は変わりません。
>* 既存のテンプレートタスクを別のテンプレートに移動した場合、新しいテンプレートに関連付けられているグループに関係なく、テンプレートタスクでは次の設定が変更されません。>
   >   * 期間タイプ
   >   * 収益タイプ
   >   * コストの種類
>
>  ただし、テンプレートタスクは、新しいテンプレートの「タスクに割り当てられたとき」の設定の影響を受けます。 詳しくは、 [アクセス](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) 記事内 [プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* 管理者がプロジェクトをテンプレートとして保存すると、そのテンプレートのすべての設定が、グループを含むプロジェクトから継承されます。
>
>  管理者がタスクまたはイシューをテンプレートを使用してプロジェクトに変換すると、テンプレートの設定はすべて、テンプレートに既に保存されている内容によって決まります。

### タスクの環境設定で設定されたテンプレートタスク設定 {#template-task-settings-configured-by-task-preferences}

テンプレートタスクを作成する場合、一部の設定は、関連するタスクの環境設定によって自動的に構成されます。 これらの設定を次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>期間タイプ </p> </td> 
   <td> <p>テンプレートをグループに関連付ける場合は、グループレベルのタスクプリファレンス「期間タイプ」で設定します。関連付けない場合は、同じシステムレベルのタスクと問題のプリファレンスを設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>収益タイプ</p> </td> 
   <td> <p>テンプレートをグループに関連付ける場合は、グループレベルのタスクプリファレンス「収益タイプ」、関連付けない場合は同じシステムレベルのタスクと問題のプリファレンスで設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>コストの種類 </p> </td> 
   <td> <p> テンプレートをグループに関連付ける場合は、グループレベルのタスクプリファレンス「コストタイプ」、関連付けない場合は同じシステムレベルのタスクと問題のプリファレンスで設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表に示すタスクプリファレンスの詳細は、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
