---
product-area: projects
navigation-topic: manage-tasks
title: タスクの移動
description: Adobe Workfront では、様々なプロジェクトや様々な親タスクにタスクを移動できます。
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 48%

---

# タスクの移動

<!--Audited: 5/2025-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Adobe Workfront では、次のオブジェクト間でタスクを移動できます。

* プロジェクトに対するアドホックタスク。
* プロジェクトから別のプロジェクトへのタスク。
* 別のプロジェクトの別の親の下にあるプロジェクトのタスク。
* 同じプロジェクト内の別の親の下のタスク。

タスクは、タスクレベルで移動することも、タスクのリストから移動することもできます。

1 つのタスクを移動することも、タスクのリストから複数のタスクを一度に移動することもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：標準 </p> 
 <p>または</p>  
<p>現在：ワーク以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する権限を管理</p> <p>タスクの追加が可能な、プロジェクトに対する参加以上の権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タスクを移動する際の考慮事項

タスクを移動する際は、以下の点を考慮してください。

* システム管理者またはグループ管理者は、設定エリアの「ユーザーがログ時間に関するタスクおよび問題を移動することを許可する」環境設定の設定方法に応じて、ログ時間を持つタスクを移動できないようにすることができます。 詳しくは、[システム全体のタスクおよびイシューの環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

* あるプロジェクトから別のプロジェクトにタスクを移動すると、タスクの日付が再計算される場合があります。再計算では、新規プロジェクトが使用するスケジュールと、プロジェクトのスケジュールの基点情報が考慮されます。

* 移動プロセス中に、タスクに関連付けられた一部の項目を移動タスクに移動できます。 ただし、デフォルトでは、次のオブジェクトは移動されたタスクに転送されます。

   * イシュー
   * ログに記録された時間数
   * ユーザーコメント
   * カスタムフォームとカスタムフィールド情報
   * サブタスク

* デフォルトでは、次の項目はタスクと一緒に移動しません。

   * マイルストーン

## リスト内のタスクを移動

{{step1-to-projects}}

1. **プロジェクト** ページで、移動する 1 つ以上のタスクが含まれているプロジェクトを選択します。
1. 左パネルの「**タスク**」をクリックしてタスクリストを表示します。
1. **プランモード** アイコン ![&#x200B; プランモード &#x200B;](assets/plan-mode.png) アイコンをクリックし、「**自動保存**」切替スイッチが有効になっていることを確認して、移動する 1 つ以上のタスクを選択します。

   ![&#x200B; 自動保存オプション &#x200B;](assets/autosave-icon.png)

   >[!IMPORTANT]
   >
   >「**自動保存**」切り替えスイッチが無効な場合は、タスクを移動できません。

1. （オプションおよび条件付き）選択したタスクを同じプロジェクト内で移動する場合は、選択したタスクをクリックし、プロジェクト上で移動先にドラッグ&amp;ドロップします。 タスクの階層の変更は直ちに保存され、各タスクに関連付けられた情報がタスクと共に移動されます。

1. （条件付き）移動する 1 つ以上のタスクを選択し、次のいずれかの操作を行います。

   * タスクリストの上部にある **その他** メニュー ![&#x200B; その他のアイコン &#x200B;](assets/main-more-icon.png) をクリックしてから、**移動先** をクリックします。
   * 選択したタスクを右クリックし、[**移動先**] をクリックします。
   * 1 つのタスクを選択する場合、リスト内のタスク名の横にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-icon-task-list.png) をクリックし、続いて「**指定の場所に移動**」をクリックします。

   **タスクを移動** ボックスが表示されます。

1. この記事の [&#x200B; タスクレベルでのタスクの移動 &#x200B;](#move-a-task-at-the-task-level) の節で説明しているように、タスクの移動を続行します。

   <!--
   is this still accurate?!
   -->

## タスクレベルでタスクを移動 {#move-a-task-at-the-task-level}

タスクのリストからタスクを移動する以外に、タスクを開いた後にタスクレベルでタスクを移動することもできます。

1. Workfront システム内のタスクを検索して見つけます。
1. タスクの名前をクリックして開きます。
1. タスク名の横にある **その他** ドロップダウンメニュー ![&#x200B; その他アイコン &#x200B;](assets/main-more-icon.png) をクリックし、「**移動先**」をクリックします。 **タスクを移動** サイドパネルが表示されます。

1. （オプション）**タスク名**&#x200B;を更新します。タスクが新しい名前で新しい場所に移動します。

   >[!TIP]
   >
   >リスト内の複数のタスクを移動するように選択すると、「**タスク名**」フィールドはグレー表示され、編集できません。 **タスク名** フィールドにポインタを合わせると、選択したすべてのタスクのリストが表示されます。
   >
   >
   >![&#x200B; タスク名の表示 &#x200B;](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. **宛先プロジェクトを選択** フィールドに、タスクの移動先のプロジェクトの名前を入力します。 同じプロジェクト内でタスクを移動する場合は、現在のプロジェクトの名前を入力します。

   >[!TIP]
   >
   >* プロジェクト名では大文字と小文字が区別されます。
   >* プロジェクトを検索するには、参照番号を入力するか、プロジェクトの ID を入力します。 これは、同じ名前のプロジェクトを区別するのに役立ちます。
   >* リストには 100 個のプロジェクトのみが表示されます。

1. （条件付き）プロジェクトへのアクセス権がない場合は、「**アクセスをリクエスト**」をクリックします。
1. （条件付き）宛先プロジェクトのいずれかのタスクにタスクを追加するアクセス権がある場合は、アクセス権を要求せずにタスクを宛先プロジェクトに移動し続けます。

   ![&#x200B; アクセスを要求しないタスクの移動 &#x200B;](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Workfront管理者がこれらのプロジェクトにタスクを追加できないときに、選択したプロジェクトが承認保留中、完了、または停止の場合にも、同様のメッセージが表示されます。 詳しくは、[システム全体のプロジェクト環境の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. （オプション）「**オプション**」セクションで、次の表に示す項目の選択を解除して、移動されたタスクから削除します。 デフォルトでは、すべてのオプションが選択されています。

   >[!IMPORTANT]
   >
   >**オプション** リストの項目の選択を解除すると、データが失われます。 既存のタスクの情報は削除され、復元できません。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべて選択</td> 
      <td>タスクを新しい場所に移動する際にタスクからすべての情報を削除するには、このオプションの選択を解除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">制約</td> 
      <td> <p>タスク制約は、プロジェクトのスケジュールモードの設定に応じて、「できるだけ早く」または「できるだけ遅く」に設定されます。</p> <p> 選択すると、タスクの現在の制約がタスクと共に転送されます。 </p> 
      <p>注意：日付固有の制約を持つタスクを別のプロジェクトに移動またはコピーする場合で、そのタスクの制約の日付が新規プロジェクトの日付より前にある場合は、タスクの制約が「できるだけ早く」または「できるだけ遅く」に変更されるか、プロジェクトの予定開始日または予定完了日が調整されます。

   次に、日付固有の制約の例を示します。
   <ul>
      <li> 開始日</li>
      <li> 指定日に終了</li>
      <li> 指定日以降に開始</li>
      <li> 指定日までに開始</li>
      </ul>

   詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">タスク制約の概要</a>を参照してください。</p> </td>
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
      <td>タスクのステータスは「新規」に設定されます。 それ以外の場合は、既存のタスクのステータスが保持されます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">財務情報</td> 
      <td>タスクの財務情報が削除され、Workfront ではタスクの「コストタイプ」を「コストなし」に、「収益タイプ」を「請求不可」に更新します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">すべての先行タスク</td> 
      <td> <p>選択すると、タスクを別のプロジェクトに移動する際に、依存関係がプロジェクト間の先行タスクになります。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td> <p>タスクに添付されたドキュメントは、移動したタスクには転送されません。 これには、バージョン、プルーフ、およびリンクされたドキュメントが含まれます。</p> <p>これには、ドキュメントの承認は含まれません。 タスクを移動する際に、ドキュメント承認を移動することはできません。</p> 
      <p>注意：ドキュメントをタスクと共に移動しないことを選択した場合、ドキュメントは削除され、30 日間ごみ箱に入れられます。 管理者はそれらのドキュメントを復元でき、移動先のタスクで復元されます。 </p>

   <p>タスクを移動した後に削除すると、復元されたドキュメントは、ドキュメントを復元した管理者のユーザーページのドキュメントエリアに配置されます。</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知</td> 
      <td>タスクのリマインダーは、移動先のタスクには転送されません。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>タスクに記録された費用は、移動先のタスクには転送されません。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">権限</td> 
      <td> <p>Workfront は、タスクの共有リストに表示されているすべてのエンティティの名前を削除します。 </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. （オプション）「**親を選択**」セクションで、移動されたタスクの親になる宛先プロジェクトのタスクを選択します。

   >[!TIP]
   >
   >リスト内の複数のタスクを移動するように選択すると、選択したすべてのタスクが、選択した親の子になります。

   次のいずれかの操作を行って、親を選択します。

   * タスクリストのプロジェクト計画で親の 1 つを選択します。
   * 検索アイコン ![検索アイコン](assets/search-icon.png) をクリックし、名前で親タスクを検索します。

   タスクがリストに表示されます。

   ![検索機能によるタスク移動時の親タスクの選択](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

   >[!NOTE]
   >
   >親タスクを選択しない場合、タスクはサブタスクではなくメインタスクとして移動され、宛先プロジェクトのタスクリストの最後に配置されます。

1. **タスクを移動** をクリックします。 タスクは、親タスクのサブタスクまたはプロジェクトの最後のタスクとして、指定されたプロジェクトに移動します。
