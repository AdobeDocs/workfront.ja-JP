---
product-area: projects
navigation-topic: convert-issues
title: イシューのタスクへの変換
description: イシューの送信後にイシューを完了するためにさらに作業が必要な場合は、Adobe Workfrontでイシューをタスクに変換できます。
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 86%

---

# イシューをタスクに変換

<!--Audited: 08/2025-->

イシューの送信後にイシューを完了するためにさらに作業が必要な場合は、Adobe Workfrontでイシューをタスクに変換できます。

イシューの変換に関する一般的な情報については、[Adobe Workfront におけるイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <p>ワークまたはそれ以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>問題、タスクおよびプロジェクトへの編集アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューの表示権限</p> <p>プロジェクトへの投稿権限</p> <p>イシューが変換された後に、タスクに対する管理権限を取得します</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain&nbsp;Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## 考慮事項

* 問題をタスクに変換する際には、処理の制限が 5 分あります。 イシューに多数のドキュメントが添付されていて、変換に失敗した場合は、ドキュメントの一部を削除して、もう一度試す必要がある可能性があります。

## イシューをタスクに変換

1. プロジェクトに移動し、左側のパネルで&#x200B;[!UICONTROL **イシュー**]&#x200B;をクリックします。
1. 変換するイシューをクリックして、イシューのランディングページに移動します。
1. イシューの&#x200B;[!UICONTROL **その他**]&#x200B;メニューをクリックし、[!UICONTROL **タスクに変換**]&#x200B;を選択します。

   ![ 問題の詳細メニュー ](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >イシューが承認プロセスに関連付けられている場合、または既に解決オブジェクトに関連付けられている場合、Workfront の[!UICONTROL プロジェクトに変換]ボックスの上部に警告が表示され、変換中に承認が削除されたか、解決オブジェクトが上書きされたことが通知されます。詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

1. [!UICONTROL タスク名]セクションでタスクの名を前を更新します。デフォルトでは、タスクの名前は元のイシューの名前と同じになります。

   ![ タスクに変換ボックス ](assets/convert-to-task-box-nwe.png)

1. [!UICONTROL **宛先プロジェクト**]&#x200B;をクリックし、新しいタスクを配置するプロジェクトの名前を&#x200B;[!UICONTROL **宛先プロジェクト**]&#x200B;フィールドに入力し始め、リストに表示されたらそれを選択します。デフォルトでは、イシューのプロジェクトが選択されています。

1. [!UICONTROL **概要**]&#x200B;をクリックし、タスクの&#x200B;[!UICONTROL **説明**]&#x200B;を入力します。

   >[!TIP]
   >
   >   システム管理者またはグループ管理者は、レイアウトテンプレートを変更することによって、変換ボックスの左側のパネルセクションの順序を変更することができます。

1. (オプションおよび条件付き) [!UICONTROL **オプション**] をクリックし、以下のオプションのいずれかを選択します。

   Workfront 管理者またはグループ管理者は、これらの設定がイシューの変換時に表示される前に有効にしておく必要があります。

   * [!UICONTROL **元のイシューを保持し、その解決策をこのタスクに関連付ける**]

     選択しない場合、元のイシューは削除されます。

     >[!NOTE]
     >
     >この設定のステータスに関係なく、イシューを削除するアクセス権や権限を持たないユーザーは、イシューを変換する際にイシューを削除できません。イシューに対するアクセス権および権限について詳しくは、次を参照してください。
     >   
     >   * [イシューへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [イシューの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **（ユーザー名）にこのタスクへのアクセスを許可**]

     選択しない場合、イシューのプライマリ連絡先には、新規タスクへのアクセス権がありません。

   * [!UICONTROL **イシューの予定完成日を保持**]

     選択しない場合、新しいタスクの[!UICONTROL 予定完了日]は、タスクの[!UICONTROL 予定開始日]から計算されます。新しいタスクの[!UICONTROL 予定開始日]は、新しいタスクのシステム環境設定に従って設定されます。

     >[!NOTE]
     >
     >
     >ここに表示されるオプションは、Workfront 管理者のシステム内の全員に対する設定によって異なります。詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。
     >
     >または、組織内の最上位グループがそれらを個別に構成した場合、ここに表示されるオプションは、手順 6 で選択したプロジェクトにどのグループが関連付けられているかによって異なります。詳しくは、[グループのタスクとイシューの環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

1. （オプション）[!UICONTROL **カスタムフォーム**] をクリックし、新しいタスクのカスタムフォームを添付します。

   >[!TIP]
   >
   >* イシューに添付された複数のオブジェクトのカスタムフォームをイシューとタスクの両方で使用するように設定すると、イシューとタスクのカスタムフォームの両方にフィールドが存在する場合、フォームに保存されたすべての情報が変換時に保持されます。
   >* 計算フィールドを持つ複数のオブジェクトのカスタムフォームがイシューおよびタスクに添付されている場合、イシューおよびタスクには、フォームの計算カスタムフィールドで参照されているすべてのフィールドとの互換性が必要です。互換性がない場合は、調整を行うように警告するメッセージが表示されます。詳しくは、[ フォームへの計算フィールドの追加 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) を参照してください。
   >* 宛先プロジェクトのタスクデフォルトカスタムフォームフィールドにデフォルトフォームが定義されている場合、プロジェクトの編集時に、それらのタスクフォームも新しいタスクに追加されます。元のイシューとデフォルトのタスクフォームのフィールドに共通するカスタムフィールドには、イシューフィールドの情報が事前に入力されます。


1. [!UICONTROL **タスクに変換**]&#x200B;をクリックします。

   元のイシューを削除した場合、イシューは指定されたプロジェクトのタスクになります。

   または

   元のイシューを保持する場合、イシューは選択したプロジェクトの新しいタスクにリンクされ、タスクが完了するとイシューも完了します。

   一部のイシューフィールドはタスクに転送されます。詳しくは、この記事の[プロジェクトとタスクに関する元のイシュー情報を表示](#view-original-issue-information-on-projects-and-tasks)を参照してください。

1. （オプション）必要に応じてタスクの編集を続けます。

## プロジェクトとタスクに関する元のイシュー情報を表示 {#view-original-issue-information-on-projects-and-tasks}

元のイシューの情報は、プロジェクトとタスクのリストとレポート、またはプロジェクトの詳細領域で表示できます。レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

次の表は、変換されたプロジェクトとタスクのどのイシューフィールドが表示されるかを示しています。

| イシューフィールド | プロジェクトまたはタスクフィールド | プロジェクトリストまたはレポート | プロジェクト詳細領域 | タスクリストまたはレポート | タスク詳細領域 |
|---|---|---|---|---|---|
| [!UICONTROL イシュー名] | [!UICONTROL 変換済みイシュー名] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL プライマリ連絡先] | [!UICONTROL 変換済みイシューの発信元名] | ✔ | ✔ | ✔ |
| [!UICONTROL エントリ日] | [!UICONTROL 変換済みイシューのエントリ日] | ✔ |  | ✔ |


>[!CAUTION]
>
>イシューの[!UICONTROL プライマリ連絡先]が変更された場合、またはイシューが変換された後にプロジェクトまたはタスクからリンクが解除された場合、[!UICONTROL 変換済みイシューの発信元名]は更新されず、イシューが変換されたときの元の[!UICONTROL プライマリ連絡先]が表示されます。
