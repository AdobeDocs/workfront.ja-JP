---
product-area: projects
navigation-topic: manage-tasks
title: リスト内のタスクを編集
description: リストに表示されるフィールドを編集することで、タスクのリスト内のタスク情報を編集できます。変更内容をWorkfrontに保存する方法を指定するには、タスクのリストでプランモードを定義する必要があります。 変更は、手動または自動で保存できます。
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '2764'
ht-degree: 69%

---

# リスト内のタスクを編集 {#edit-tasks-in-a-list}

<!-- Audited: 5/2025 -->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

リストに表示されるフィールドを編集することで、タスクのリスト内のタスク情報を編集できます。タスクを編集するその他の方法について詳しくは、[タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

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
   <td> <p>標準<p>
   <p>ワークまたはそれ以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクとプロジェクトに参加権限か、それ以上の権限を付与</p></td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## リスト内のタスクの編集に関する考慮事項 {#considerations-about-editing-tasks-in-a-list}

リストでタスクを編集すると、変更がプロジェクトのタイムラインに与える影響を明確に把握しながら、複数のタスクに対して同時に変更を加えることができます。

リスト内のタスクを編集する際は、以下の点に注意してください。

* 「編集」ボックスでタスクを編集する際にタスクに対する管理権限が必要な場合とは異なり、タスクに対する参加権限を持つリスト内のタスクのみを編集できます。これにより、タスクに関する以下の制限付き情報を編集できます。

   * 説明
   * ステータス
   * 完了率
   * カスタムフォームの情報

     >[!NOTE]
     >
     >リスト内のタスクのカスタムフィールドは、フィールドをアップデートする権限を持っている場合にのみ編集できます。

   * 時間の記録
   * 割り当てを変更
   * 財務情報を表示
   * 費用、タスクまたはイシューを追加

* 以下のリストでタスクを編集できます。

   * プロジェクトのタスクセクション
   * プロジェクトのサブタスクセクション
   * タスクレポート

     >[!NOTE]
     >
     >デフォルトでは、Workfront は、タスクに対する変更をサブタスクセクションまたはタスクレポートに自動的に保存します。

* タスクの編集を開始する前に計画モードを定義することで、Workfrontでリスト内のタスクに加えた変更をいつ保存するかを制御できます。

  変更内容を保存するWorkfrontは、次のどちらかを選択できます。

      *すべての変更の後に自動的に 
    *手動で、保存をクリックした後にのみ 
  
  Workfrontがリスト内のタスクに加えた変更をいつ保存するかについての詳細は、この記事の「リスト内のタスクを編集する前にプラン モードを変更する [&#x200B; を参照してください &#x200B;](#modify-plan-mode-before-editing-tasks-in-a-list)。

* 他のユーザーは、タスクに対して行った更新を表示する前に、ページを更新する必要があります。

## リストでタスクを編集する前にプランモードを変更

リスト内のタスクに加えた変更を、発生時に自動的に保存するか、または各変更を手動で保存するかを指定できます。 これを行うには、タスクを編集する前に、タスクのリストでプランモードを変更する必要があります。

>[!IMPORTANT]
>
>タスクを自動で保存するか手動で保存するかに応じて、リストのタスクを編集する際に他のユーザーの情報を上書きする場合があります。詳しくは、[&#x200B; タスクリスト内の同時変更の保存の概要 &#x200B;](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md) を参照してください。

更新の種類として「自動」または「自動・変更時」が選択されているプロジェクトのリストに変更を保存すると、Workfront はプロジェクトのタイムラインと、プロジェクト内およびプロジェクト間のすべての依存関係をアップデートします。プロジェクトが大きい場合や、依存関係が多い場合は、タイムラインの計算に時間がかかる場合があります。タスクリストの編集方法の中には、変更を保存する方法に応じて、他の方法よりも速く編集できるものがあります。

タスクに加えた変更を Workfront がリストに保存するタイミングを制御できます。次のシナリオが存在します。

* アップデートのたびに、Workfront で自動的に変更を保存することができます。

  詳しくは、この記事の [&#x200B; 変更を自動的に保存するようにプランモードを設定する &#x200B;](#set-the-plan-mode-to-automatically-save-changes) の節を参照してください。

* 「保存」ボタンを使用して、手動で複数の変更を一度に適用するタイミングを制御できます。

  詳しくは、この記事の [&#x200B; 手動で変更を保存するようにプランモードを設定 &#x200B;](#set-the-plan-mode-to-manually-save-changes) 節を参照してください。

### 変更が自動的に保存されるように計画モードを設定します。

>[!TIP]
>
>プロジェクトに 2000 を超えるタスクがある場合や、多くの依存関係がある場合には、変更内容とすべてのプロジェクトの依存関係を保存するのに時間がかかる可能性があります。

タスクリストの変更を自動的に保存する場合は、以下の点に注意してください。

* カスタムビューをタスクリストに適用し、アップデートするためのアクセス権があるタスク関連フィールドを編集することができます。
* 自動保存された変更を元に戻すことはできません。これはデフォルトの設定です。
* プロジェクトの更新の種類が自動または自動で、「変更時」の場合、Workfrontでは、変更のたびに、プロジェクトのタイムラインと、プロジェクト内およびプロジェクト間のすべての依存関係が自動的に再計算されます。 プロジェクトの更新の種類について詳しくは、[プロジェクトの更新の種類を選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。

リスト内のタスクを編集し、変更を自動的に保存するには、以下のように行います。

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。
1. 左側のパネルで、「**タスク**」セクションをクリックします。

1. リストの上部にある **プランモード** アイコン ![&#x200B; プランモードアイコン &#x200B;](assets/plan-mode-icon.png) をクリックし、「**自動保存**」オプションが選択されていることを確認します。

   ![&#x200B; 自動保存設定を有効にする &#x200B;](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. 手動でアップデートする権限を持つフィールドを編集します。

1. （オプション）**Escape** を押して、変更をキャンセルします。
1. キーボードの **Enter** （Windows）または **Return** （Mac）を押して、タスクとプロジェクトタイムラインに対する変更を保存します。
1. （オプション）変更するタスクを右クリックします。

   または

   タスク名の右にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-icon-task-list.png) をクリックします。

1. （オプション）以下のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新しいタブで開く</td> 
      <td>タスクが新しいブラウザータブで開きます。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">タスクを上に挿入</td> 
      <td>選択したタスクの上にタスクを挿入します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクを下に挿入</td> 
      <td>選択したタスクの下にタスクを挿入します</td> 
     </tr>
     <tr> 
      <td role="rowheader">編集</td> 
      <td><p>タスクを編集できる「タスクを編集」ボックスを開きます。</p><p>タスクの編集について詳しくは、<a href="#edit-tasks-in-a-list" class="MCXref xref">リスト内でタスクを編集</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">削除</td> 
      <td><p>タスクを削除します。</p><p>タスクの削除について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">タスクを削除</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">インデント</td> 
      <td><p>タスクが 1 レベルインデントします。 </p><p>このオプションは、スタンドアロンタスクでのみ表示されます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">アウトデント</td> 
      <td><p>タスクが 1 レベルアウトデントします。 </p><p>このオプションは、子タスクにのみ表示されます。 </p></td> 
     </tr>  
     <tr> 
      <td role="rowheader">複製</td> 
      <td><p>同じプロジェクト内にタスクの複製バージョンを作成します。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">指定の場所にコピー...</td> 
      <td><p>タスクを別のプロジェクトにコピーします。</p><p>タスクのコピーと複製について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">タスクをコピーおよび複製</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">指定の場所に移動...</td> 
      <td><p>タスクを別のプロジェクトに移動します。</p><p>タスクの移動について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">タスクを移動</a>を参照してください。</p></td> 
     </tr> 
    </tbody> 
   </table>

### 変更を手動で保存するように計画モードを設定します。 {#edit-tasks-in-a-list-and-manually-save-changes}

リスト内のタスクに加えた変更を手動で保存できます。この方法で変更を保存する場合、保存する前に変更を元に戻すことができる自由度があります。

>[!TIP]
>
>* サブタスクセクションまたはタスクレポートでタスクを編集している場合、リスト内のタスクに加えた変更を元に戻すことはできません。
>* 元に戻すことができる変更の数に制限はありません。タスクの元の状態に達するまで、それらをすべて 1 つずつ元に戻すことができます。
>

タスクリスト内の変更を手動で保存する場合は、以下の点を考慮してください。

* タスクリストの変更を手動で保存するには、タスクとプロジェクトの両方を管理する権限が必要です。
* プロジェクトは編集できません。プロジェクトを編集するオプションは無効になっています。
* プロジェクトのヘッダー内の情報をアップデートすることはできません。タスクリストの変更を手動で保存する場合には、以下の操作のみを実行できます。

   * プロジェクトに登録します。
   * プロジェクトをお気に入りのリストに追加します。
   * リストでタスクの名前をクリックして、タスクを開きます。

* タスクを一括編集します。 複数のタスクを選択すると、「編集」アイコンが無効になります。
* Workfront は、変更を保存した後にのみ、タスクに加えた変更に関する通知をトリガーします。

リスト内のタスクに対する変更を手動で保存する方法は 2 つあります。

* [「手動保存標準」オプションを選択すると、タスクリストの変更を手動で保存](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [「タイムライン計画を手動保存」オプションを選択すると、タスクリストの変更を手動で保存](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### 「手動保存標準」オプションを選択すると、タスクリストの変更を手動で保存 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>プロジェクトに 2000 を超えるタスクがある場合、またはプロジェクトに多くの依存関係がある場合には、タスクに加えた変更と、それらの変更がプロジェクトのすべての依存関係に与える影響を視覚的に識別するのに時間がかかることがあります。この場合、変更の保存に予想以上の時間がかかる可能性があります。

「手動保存標準」オプションを選択した後にリスト内のタスクをアップデートする場合は、以下の点に注意してください。

* タスクリストにカスタムビューを適用し、管理する権限を持つタスク関連のフィールドを、そのビュー内で編集できます。
* プロジェクトの「更新の種類」が「自動」または「自動」で、「変更時」の場合、「保存」をクリックすると、Workfrontはプロジェクトのタイムラインと、プロジェクト内およびプロジェクト間のすべての依存関係を計算します。 プロジェクトの更新タイプについて詳しくは、[プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。

「手動保存標準」オプションを選択する際に、リスト内のタスクを編集するには、次の手順に従います。

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。

1. 左側のパネルで、「**タスク**」セクションをクリックします。

1. リストの上部にある **プランモード** アイコン ![&#x200B; プランモードアイコン &#x200B;](assets/plan-mode-icon.png) をクリックします。

1. **プランモード** ダイアログで、**手動保存** を選択し、**標準** をクリックします。

   ![&#x200B; 手動保存の設定を有効にする &#x200B;](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. **適用** をクリックします。 ツールバー設定が表示され、変更の取り消し、やり直し、保存のオプションが表示されます。

   ![&#x200B; 手動保存ツールバー &#x200B;](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 手動で更新する権限を持つフィールド内をクリックします。フィールドが編集可能になり、変更を加えることができます。

1. キーボードの **Enter** （Windows）または **Return** （Mac）を押して、変更内容を一時的に保存します。

1. （オプション） **取り消し** アイコン ![&#x200B; 取り消しアイコン &#x200B;](assets/undo-icon-on-task-list.png) をクリックして、変更を元に戻し、フィールドを元の状態に戻します。

1. （オプションおよび条件付き） **やり直し** アイコン ![&#x200B; やり直しアイコン &#x200B;](assets/redo-icon-on-task-list.png) をクリックして、取り消した変更を復元します。

1. （オプション）変更するタスクを右クリックします。

   または

   **詳細**&#x200B;メニュー ![](assets/more-icon-task-list.png) をクリックします。

1. （オプション）以下のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新しいタブで開く</td> 
      <td>タスクが新しいブラウザータブで開きます。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">タスクを上に挿入</td> 
      <td>選択したタスクの上にタスクを挿入します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクを下に挿入</td> 
      <td>選択したタスクの下にタスクを挿入します</td> 
     </tr> 
     <tr> 
      <td role="rowheader">削除</td> 
      <td>タスクの削除について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">タスクを削除</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">インデント</td> 
      <td> <p>タスクが 1 レベルインデントします。 </p> <p>このオプションは、スタンドアロンタスクでのみ表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">アウトデント</td> 
      <td> <p>タスクが 1 レベルアウトデントします。 </p> <p>このオプションは、子タスクにのみ表示されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製</td> 
      <td> <p>同じプロジェクト内にタスクの複製バージョンを作成します。 </p> <p>タスクのコピーと複製について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">タスクをコピーおよび複製</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront は、タスクのタイムラインに変更を加えると、プロジェクト内およびプロジェクト間のすべての依存関係を更新します。
1. タスクの変更を完全に保持し、プロジェクトのタイムラインを保存する場合は、「**保存**」をクリックします。

#### 「タイムライン計画を手動保存」オプションを選択すると、タスクリストの変更を手動で保存 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

変更およびすべてのプロジェクトの依存関係を保存する方がより迅速です。2,000 個を超えるタスクがあるプロジェクトでは使用できません。

>[!IMPORTANT]
>
>多数の依存関係がある数百を超えるタスクの大量のリストを編集する場合は、このオプションを使用することをお勧めします。このオプションを使用すると、「手動保存」オプションを使用する場合よりも、非常に速く変更を視覚的に確認することができます。

タスクリストで「タイムライン計画を手動保存」オプションを使用する際は、次の点に注意してください。

* 2,000 個を超えるタスクがあるプロジェクトには、「タイムライン計画を手動保存」オプションを適用できません。
* タスクリストにカスタムビュー、フィルター、またはグループ化を適用することはできません。表示、フィルター、グループ化の各ドロップダウンメニューとアジャイルビューアイコンは無効になっています。デフォルトで適用されるビューは、フィールドの数が制限されています。
* プロジェクトの更新タイプが「自動」または「自動・変更時」の場合、プロジェクトのタイムラインとすべてのプロジェクト内依存関係は、変更後に自動的に計算されます。
* プロジェクトの [ 更新の種類 ] が [ 自動 ] または [ 自動 ] で、[ 変更時 ] の場合、[ 保存 ] をクリックすると、プロジェクト間の依存関係が計算されます。 プロジェクトの更新タイプについて詳しくは、[プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。

「タイムライン計画を手動保存」オプションを使用する際にリスト内のタスクを編集する手順は、次のとおりです。


{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。

1. 左側のパネルで、「**タスク**」セクションをクリックします。

1. リストの上部にある **プランモード** アイコン ![&#x200B; プランモードアイコン &#x200B;](assets/plan-mode-icon.png) をクリックします。

1. **プランモード** ダイアログで、**手動保存** を選択し、**タイムライン計画** をクリックします。

   ![&#x200B; タイムライン計画設定の適用 &#x200B;](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >タスクの数が 2000 を超えるプロジェクトでは、「**時間計画**」オプションはグレー表示されます。

1. 「**適用**」をクリックします。

   リストでは、次の変更が行われます。

   * 表示、グループ化、およびフィルターのドロップダウンメニューが削除され、ビューが次のフィールドに置き換えられます。

      * タスク番号
      * タスク名
      * 制約タイプ
      * 期間
      * 予定開始日
      * 予定完了日
      * 先行タスク
      * 割り当て
      * ステータス
      * 完了率

   * アジャイルビューアイコンが削除されます。
   * ツールバー設定が表示され、変更の取り消し、やり直し、保存のオプションが表示されます。

     ![&#x200B; 手動保存ツールバー &#x200B;](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 手動でアップデートする権限を持つフィールドを編集します。

1. キーボードの **Enter** （Windows）または **Return** （Mac）を押して、変更内容を一時的に保存します。
1. （オプション） **取り消し** アイコン ![&#x200B; 取り消しアイコン &#x200B;](assets/undo-icon-on-task-list.png) をクリックして、変更を元に戻し、フィールドを元の状態に戻します。
1. （オプションおよび条件付き） **やり直し** アイコン ![&#x200B; やり直しアイコン &#x200B;](assets/redo-icon-on-task-list.png) をクリックして、取り消した変更を元に戻します。

1. （オプション）変更するタスクを右クリックします。

   または

   **詳細**&#x200B;メニュー ![](assets/more-icon-task-list.png) をクリックします。

1. 次のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新しいタブで開く</td> 
      <td>タスクが新しいブラウザータブで開きます。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">タスクを上に挿入</td> 
      <td>選択したタスクの上にタスクを挿入します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクを下に挿入</td> 
      <td>選択したタスクの下にタスクを挿入します</td> 
     </tr> 
     <tr> 
      <td role="rowheader">削除</td> 
      <td>タスクの削除について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">タスクを削除</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">インデント</td> 
      <td> <p>タスクが 1 レベルインデントします。 </p> <p>このオプションは、スタンドアロンタスクでのみ表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">アウトデント</td> 
      <td> <p>タスクが 1 レベルアウトデントします。 </p> <p>このオプションは、子タスクにのみ表示されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製</td> 
      <td> <p>同じプロジェクト内にタスクの複製バージョンを作成します。 </p> <p>タスクのコピーと複製について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">タスクをコピーおよび複製</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront は、タスクのタイムラインに変更を加えると、プロジェクト内およびプロジェクト間のすべての依存関係を更新します。
1. タスクの変更を完全に保持し、プロジェクトのタイムラインを保存する場合は、「**保存**」をクリックします。

## 概要を使用してリスト内のタスクを編集

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。

1. 左側のパネルで、「**タスク**」セクションをクリックします。 プロジェクトのタスクのリストが表示されます。

1. 編集するタスクを選択し、リストの右上隅にある **概要を開く** アイコン ![&#x200B; 概要を開くアイコン &#x200B;](assets/task-summary-icon.png) をクリックします。 **タスクの概要** パネルが開きます。

1. （オプション）**更新**&#x200B;エリアでタスクの更新を入力します。
1. 次のアイコンまたはエリアのいずれかをクリックしてタスクに移動し、タスクレベルで情報を編集します。

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td>ドキュメントをタスクに追加します。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>カスタムフォームを追加または削除したり、フォームに関する情報を更新したりします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間</td> 
      <td>時間を記録します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認</td> 
      <td>タスク承認を追加します。</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. パネルの右上隅にある「**X**」をクリックして閉じます。

## タスクを一括編集

一度に複数のタスクを編集できます。タスクを編集するには、タスクに対する管理権限を持っていることを確認します。

{{step1-to-projects}}

1. **プロジェクト** ページで、プロジェクトを選択します。
1. 左側のパネルで、「**タスク**」セクションをクリックします。

1. リストの上部にある **プランモード** アイコン ![&#x200B; プランモードアイコン &#x200B;](assets/plan-mode-icon.png) をクリックし、「**自動保存**」オプションが選択されていることを確認します。

   ![&#x200B; 自動保存設定を有効にする &#x200B;](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >タスクを手動で保存する際に、タスクを一括編集することはできません。

1. タスク リストで複数のタスクを選択します。
1. **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/qs-edit-icon.png) をクリックします。 **タスクを編集**&#x200B;ダイアログボックスが開きます。

1. 選択したすべてのタスクに対して変更する情報を指定します。

   すべてのタスクに関する情報の編集は、1 つのタスクに関する情報の編集と同じです。タスク期間を編集する場合、選択したタスクは同じタスクの制約を持つ必要があります。同じでない場合は、**期間**&#x200B;フィールドに値が入力されません。

   タスクの編集について詳しくは、[タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

   >[!NOTE]
   >
   >選択したすべてのタスクに関して変更中の情報は、「**割り当て**」フィールドを除き、個々のタスクに関する既存の情報を上書きします。一括編集で新しい担当者を追加すると、その担当者は選択したすべてのタスクに追加されます。選択したタスクに他の担当者が割り当てられている場合、一括編集で追加された担当者に加えて、割り当てられたままになります。

1. 「**カスタムフォーム**」をクリックして、選択したすべてのタスクに添付されているカスタムフォームを編集します。アクティブなカスタムフォームのみがリストに表示されます。

   選択したタスクに共通するカスタムフォームがない場合、このセクションにはフォームが表示されません。

   選択したすべてのタスクに添付され、編集権限を持つフォーム上のフィールドのみを編集できます。

   <!--1. (Optional and conditional) Depending what environment you use to edit the tasks, do one of the following to recalculate custom expressions for all tasks:
   1. In the Production environment, ADD THE SENTENCE FROM THE NEXT STEP HERE:-->

1. （オプション）カスタムフォームセクションで、「**カスタム式を再計算**」オプションを選択し、選択したタスクに添付されたカスタムフォーム上にあるすべての計算済みカスタムフィールドが最新であることを確認します。

   <!--
   <div class="preview">

   1. In the Preview environment, with all the tasks selected in the list, click the **More** menu ![More menu](assets/more-icon.png) at the top of the task list, then click **Recalculate Expressions**. This is only available when you automatically save your changes. 

   -->
1. 「**変更を保存**」をクリックします。これで、行ったすべての変更が、選択したすべてのタスクに表示されます。

カスタムフォームの一括編集について詳しくは、「[&#x200B; オブジェクトに添付されたカスタムフォームの管理 &#x200B;](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)」を参照してください。
