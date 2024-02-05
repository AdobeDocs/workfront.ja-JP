---
product-area: projects
navigation-topic: manage-tasks
title: タスクのコピーと複製
description: タスクをプロジェクトから別のプロジェクトにコピーしたり、同じプロジェクト内でタスクを複製したりすることができます。
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '1736'
ht-degree: 69%

---

# タスクのコピーと複製

タスクをプロジェクトから別のプロジェクトにコピーしたり、同じプロジェクト内でタスクを複製したりすることができます。

一度に 1 つまたは複数のタスクを、または親タスクをコピーまたは複製できます。

## アクセス要件

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>ワークまたはそれ以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限 </p> <p>プロジェクトに対する参加以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タスクをコピーする際の考慮事項

タスクをコピーする際は、以下の点を考慮してください。

* あるプロジェクトから別のプロジェクトにタスクをコピーすると、タスクの日付が再計算される場合があります。再計算では、新規プロジェクトが使用するスケジュールと、プロジェクトのスケジュールの基点情報が考慮されます。
* カスタムフォームはタスクと共にコピーされます。 カスタムフィールドの情報は、タスクのコピー時に [ カスタムデータのコピー ] を選択した場合にのみ、コピーされたタスクに転送されます。
* コピープロセス中に、タスクに関連付けられた一部の項目をコピー先のタスクにコピーすることを選択できます。 ただし、デフォルトでは、次のオブジェクトはコピーされたタスクに転送されません。
   * イシュー
   * ログに記録された時間数
   * ユーザーコメント <!--not sure about this, enable only if requested by users and verified by Product: System activity comments transfer to the new task if they relate to information that you specifically select to be copied. For example, if you select to copy Expenses to the new task, system comments that identify adding expenses to the task will transfer to the copied task. -->
* デフォルトでは、次の項目はコピーされたタスクに移動します。

   * マイルストーンはコピーされたタスクに転送され、元のタスクから削除されます。
   * サブタスクは新しいタスクに転送されます。

* 一度に 1 つのタスクをコピーすることも、リスト内のタスクを編集する際に複数のタスクを一度にコピーすることもできます。

## リスト内のタスクをコピー {#copy-tasks-in-a-list}

1. コピーする 1 つまたは複数のタスクを含むプロジェクトに移動します。

   または

   タスクレポートに移動します。

1. （条件付き）クリック **タスク** タスクを含むプロジェクトを開いた場合は、左側のパネルで。
1. 次をクリック： **プランモード** アイコン ![](assets/qs-list-mode-or-save-mode-icon-small.png)をクリックし、 **自動保存** 」オプションが有効になっている。

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >変更を自動的に保存する場合にのみ、リスト内のタスクをコピーすることができます。タスク編集時の保存オプションについて詳しくは、[リスト内のタスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

1. コピーするタスクを選択し、以下のいずれかを行います。

   * タスクリストの上部で、**その他メニュー**&#x200B;をクリックし、続いて&#x200B;**コピー先**&#x200B;をクリックします。
   * 選択したタスクを右クリックし、**コピー先**&#x200B;をクリックします。
   * 1 つのタスクを選択する場合、 **その他** メニュー ![](assets/more-icon-task-list.png) リスト内のタスク名の横にあるをクリックし、 **コピー先**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. 「[タスクレベルでタスクをコピー](#copy-a-task-at-the-task-level)」の節の説明に従って、ステップ 4 からタスクのコピーを続行します。

   <!--
      (NOTE: is this still accurate?!)
   -->

## タスクレベルでのタスクのコピー {#copy-a-task-at-the-task-level}

タスクリスト内のタスクをコピーするだけでなく、タスクを開いてからコピーすることもできます。

1. Workfront システム内のタスクを検索して見つけます。
1. タスクの名前をクリックして開きます。
1. 次をクリック： **その他** ドロップダウンメニュー ![](assets/qs-more-menu.png) タスク名の横にあるをクリックし、 **コピー先**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   「タスクをコピー」ボックスが表示されます。

1. （オプション）**タスク名**&#x200B;を更新します。

   >[!TIP]
   >
   >リスト内の複数のタスクをコピーする場合、このフィールドはグレー表示になり、編集できません。タスク名フィールドにポインタを合わせると、選択したすべてのタスクのリストが表示されます。
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. 名前を入力 **宛先プロジェクト** タスクをコピーする場所： **宛先プロジェクトを選択** フィールドに入力します。

   >[!TIP]
   >
   >* プロジェクトの名前では、大文字と小文字が区別されます。
   >* 参照番号を入力したり、プロジェクトの ID を入力したりすることもできます。これは、同じ名前のプロジェクトを区別するのに役立ちます。
   >* リストには 100 個のプロジェクトのみが表示されます。

   デフォルトでは、現在のプロジェクト名が表示されます。同じプロジェクト内のタスクをコピーする場合は、このフィールドを変更しないでください。

1. （条件付き）クリック **アクセスを要求** 選択したプロジェクトへのアクセス権を持っていない場合に、プロジェクトへのアクセス権を要求します。
1. （条件付き）対象プロジェクトのタスクの 1 つにタスクを追加するアクセス権がある場合は、アクセスをリクエストせずに、引き続き選択した対象プロジェクトにタスクをコピーします。

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Workfront管理者がタスクをプロジェクトに追加できない場合、選択したプロジェクトが承認待ち、完了または無効の場合にも、同様のメッセージが表示されます。 詳しくは、[システム全体のプロジェクト環境の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. クリック **オプション** 左側のパネルで、タスクと共にコピーしないタスク属性の選択を解除します。 デフォルトでは、すべてのオプションが選択されています。

   >[!TIP]
   >
   >「**すべて選択**」を選択してから選択を解除すると、すべてのオプションの選択を解除できます。

   次のオプションの選択を解除すると、コピーしたタスクに転送されません。次の表は、オプションの選択を解除した場合の動作を示しています。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">制約</td> 
      <td> <p>タスク制約は、プロジェクトのスケジュールモードの設定に応じて、「できるだけ早く」または「できるだけ遅く」に設定されます。</p> <p> 選択すると、タスクの現在の制約がコピーされたタスクに転送されます。 </p> <p>注意：日付固有の制約を含むタスクを別のプロジェクトに移動またはコピーし、タスクの制約日が新しいプロジェクトの日付の外にある場合、タスク制約は「可能な限り早く」、「遅く」に変わるか、プロジェクトの計画開始日または計画完了日が調整されます。 日付固有の制約の例としては、「開始日」、「終了日」、「次の日より前に開始」、「次の日より後に開始」などがあります。 タスク制約と、タスク制約やプロジェクト日付がどのように影響を受けるかについて詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>で具体的な制約を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">割り当て</td> 
      <td> <p>すべての割り当てがタスクから削除されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td>すべての承認プロセスがタスクから削除されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況</td> 
      <td>タスクのステータスは「新規」です。それ以外の場合、コピーされたタスクは既存のタスクのステータスを維持します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">財務情報</td> 
      <td>タスクの財務情報が削除されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての先行タスク</td> 
      <td> <p>つまり、依存関係はコピーされたタスクに引き継がれません。 </p> <p>選択すると、コピーされたタスクのグループ内の先行タスクは保持され、その他は削除されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td> <p>タスクに添付されたドキュメントは、コピーされたタスクには転送されません。これには、バージョン、プルーフ、およびリンクされたドキュメントが含まれます。</p> <p>これにはドキュメントの承認は含まれません。タスクをコピーする際にドキュメントの承認をコピーすることはできません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知</td> 
      <td>タスクのリマインダーは、コピーされたタスクには転送されません。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>タスクに記録された費用は、コピーされたタスクには転送されません。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">権限</td> 
      <td>Workfront は、タスクの共有リストに表示されているすべてのエンティティの名前を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムデータ</td> 
      <td> <p>カスタムフィールドの値はクリアされ、カスタムフォームはコピーされたタスクに転送されます。 </p> <p>選択すると、カスタムフィールドのフォームと値の両方がコピーされたタスクに転送されます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「 **親を選択** 左側のパネルで、コピーしたタスクの親にするタスクを、コピー先のプロジェクトで選択します。

   >[!TIP]
   >
   >リスト内の複数のタスクをコピーするように選択すると、選択したすべてのタスクが、選択した親の子になります。

   次のいずれかの操作を行って、親を選択します。

   * タスクリストのプロジェクト計画で親の 1 つを選択します。
   * 検索アイコン ![検索アイコン](assets/search-icon.png) をクリックし、名前で親タスクを検索します。

   タスクがリストに表示されます。

   ![検索機能によるタスク移動時の親タスクの選択](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 親が見つかったら、その親のラジオボタンを選択します。

   親タスクを選択しない場合、タスクはサブタスクではなくメインタスクとしてコピーされ、コピー先プロジェクトのタスクリストの最後に配置されます。

1. 「**タスクをコピー**」をクリックします。

   または

   リスト内の複数のタスクを選択する場合、**タスクをコピー**をクリックします。
コピーされたタスクは、指定したプロジェクト上に存在し、選択した親タスクのサブタスク、またはプロジェクト上の最後のタスクのいずれかになります。

## タスクを複製

同じプロジェクトで同一のタスクが必要な場合は、タスクリスト内のタスクをすばやく複製できます。

* [タスクを複製する際の考慮事項](#considerations-for-duplicating-tasks)
* [タスクを複製](#duplicate-tasks)

### タスクを複製する際の考慮事項 {#considerations-for-duplicating-tasks}

* タスクリスト内のタスクを複製できるのは、タスク番号で並べ替えられている場合のみです。
* 新しいタスクは元のタスクと同じ名前になります。
* 新しいタスクに複製する情報を選択することはできません。デフォルトでは、元のタスクの親関係を含むほとんどの情報が、複製されたタスクに転送されます。
* 次の項目は、新しいタスクには転送されません。

   * ログに記録された時間数
   * メモ
   * イシュー
   * コピーされたタスクの同じグループに属する先行タスクのみが、その後続タスクと共にコピーされます。

     **例**

     たとえば、Task 2 とその先行タスク 1 を同時にコピーした場合、Task 2 のコピーと Task 1 のコピーが作成されます。 タスク 1 のコピーは、タスク 2 のコピーの先行タスクとなります。ただし、タスク 2 だけをコピーしてその先行タスクをコピーしない場合、そのコピーには先行タスクがありません。

* 親タスクを複製すると、子タスクを選択していない場合でも、すべての子タスクが複製されます。
* 同時に 1 つまたは複数のタスクを複製できます。

  ただし、連続していない複数のタスクを同時に複製することはできません。

* マイルストーンは新しいタスクに移動され、元のタスクから削除されます。

### タスクを複製

1. 複製する 1 つまたは複数のタスクを含むプロジェクトに移動します。
1. 左側のパネルの「**タスク**」をクリックします。
1. 次のいずれかの操作を行います。

   * （条件付き） **プランモード** アイコン ![](assets/qs-list-mode-or-save-mode-icon-small.png) そして **自動保存** 「 」オプションが有効な場合は、複製するタスクを選択し、 **その他のメニュー** ![](assets/qs-more-menu-29x11.png) > **複製**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * （条件付き） **プランモード** アイコン ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **手動で保存** > **標準** または **タイムライン計画**&#x200B;次に、以下の手順を実行します。

      1. 複製する 1 つまたは複数のタスクを選択し、「**複製**」をクリックします。
      1. （オプション）「**取り消し**」をクリックして変更を元に戻し、タスクを複製しないようにします。
      1. （オプションおよび条件付き）以前に「**取り消し**」をクリックした場合は、「**やり直し**」をクリックして変更を保存し、タスクを複製します。

      1. 「**保存**」をクリックして変更を保存します。

         タスクは複製され、元のタスクと同じプロジェクトに追加されます。
