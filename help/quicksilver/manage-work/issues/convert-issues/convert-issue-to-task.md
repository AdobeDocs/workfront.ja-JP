---
product-area: projects
navigation-topic: convert-issues
title: Adobe Workfront でのイシューのタスクへの変換
description: イシューの送信後、イシューを完了するために必要な作業が他にもある場合は、そのイシューをタスクに変換することができます。
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 44f01128ef4e6581dc8eaca318a999f2e7274f2a
workflow-type: ht
source-wordcount: '1048'
ht-degree: 100%

---

# Adobe Workfront でのイシューのタスクへの変換

イシューの送信後、イシューを完了するために必要な作業が他にもある場合は、そのイシューをタスクに変換することができます。

イシューの変換に関する一般的な情報については、[Adobe Workfront におけるイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>問題、タスクおよびプロジェクトへの編集アクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューの表示権限</p> <p>プロジェクトへの投稿権限</p> <p>イシューの変換後、タスクに対する管理権限を取得します</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## イシューをタスクに変換

1. プロジェクトに移動し、左側のパネルで&#x200B;[!UICONTROL **イシュー**]&#x200B;をクリックします。
1. 変換するイシューをクリックして、イシューのランディングページに移動します。
1. イシューの&#x200B;[!UICONTROL **その他**]&#x200B;メニューをクリックし、[!UICONTROL **タスクに変換**]&#x200B;を選択します。

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >イシューが承認プロセスに関連付けられている場合、または既に解決オブジェクトに関連付けられている場合、Workfront の[!UICONTROL プロジェクトに変換]ボックスの上部に警告が表示され、変換中に承認が削除されたか、解決オブジェクトが上書きされたことが通知されます。詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

1. [!UICONTROL タスク名]セクションでタスクの名を前を更新します。デフォルトでは、タスクの名前は元のイシューの名前と同じになります。

   ![](assets/convert-to-task-box-nwe.png)

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
     >   * [イシューへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
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
   >* 計算フィールドを持つ複数のオブジェクトのカスタムフォームがイシューおよびタスクに添付されている場合、イシューおよびタスクには、フォームの計算カスタムフィールドで参照されているすべてのフィールドとの互換性が必要です。互換性がない場合は、調整を行うように警告するメッセージが表示されます。詳しくは、[レガシーフォームビルダーを使用した計算データのカスタムフォームへの追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)の「マルチオブジェクトカスタムフォームの計算カスタムフィールド」を参照してください。
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
