---
product-area: reporting
navigation-topic: using-built-in-reports
title: ビュー内のビルトインステータスアイコン
description: 組み込みの「状態アイコン」フィールドをビューの列として追加し、オブジェクトの主要ポイントをより明確に表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: ht
source-wordcount: '1322'
ht-degree: 100%

---

# ビュー内のビルトインステータスアイコン

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

組み込みの「状態アイコン」フィールドをビューの列として追加し、オブジェクトの主要ポイントをより明確に表示できます。状態アイコンを使用すると、次の条件が存在する場合に一目で確認できます。

* オブジェクトにドキュメントが添付されている
* オブジェクトが承認プロセスに関連付けられている
* オブジェクトに追加のメモが関連付けられている
* 費用は請求可能または払い戻し可能
* タスクがクリティカルパス上にある
* ユーザーが会社またはチームに属しているか、別のタイムゾーンにいる

次の点に注意してください。

* 「状態アイコン」フィールドのインジケーターのほとんどは、実際のオブジェクトまたはそれらが表すオブジェクトのエリアへのクイックリンクです。

* アイコンで表されるアイテムがオブジェクトにない場合は、見つからないアイテムを表すアイコンが、色付きの画像ではなく淡色表示で「状態アイコン」列に表示されます。

  ![task_status_icons.png](assets/task-status-icons.png)

  詳しくは、この記事の[状態アイコンとフラグの概要](#overview-of-status-icons-and-flags)を参照してください。

* 一部のビューでは、「**状態アイコン**」フィールドの名前が「**フラグ**」または「**アイコンの表示**」になっています。\
  「状態アイコン」フィールドに含まれるアイコンのルックアンドフィールをカスタマイズすることはできません。

* 「状態アイコン」フィールドでは、アイコン数を編集できません。

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
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートに列を追加</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>既存のビューに対する権限を管理</p> <p>レポートに列を追加する権限を管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## ビューにステータスアイコンフィールドを追加

一部のビルトインビューおよびビルトインレポートには、既にステータスアイコンフィールドが含まれています。

すべてのビューにステータスアイコンフィールドを追加することはできません。

最初から作成したカスタムビューにステータスアイコンフィールドを追加するには、次の手順を実行します。

1. 次のいずれかのオブジェクトのリストに移動します。

   * タスク
   * イシュー
   * プロジェクト
   * テンプレートタスク
   * テンプレート
   * 費用
   * ドキュメント
   * ユーザー\
     **ステータスアイコン**&#x200B;フィールドが使用できるのは、これらのオブジェクトのみです。\
     オブジェクトリストについて詳しくは、[Adobe Workfront のリストの概要](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)を参照してください。

1. **ビュー**&#x200B;ドロップダウンメニューから、「**新規ビュー**」を選択します。

1. 「**列を追加**」をクリックします。
1. 「**この列に表示**」ボックスに、次のいずれかのフィールド名を入力し、リストに表示されたら選択します。

   * *ステータスアイコン*
   * *フラグ*
   * *表示アイコン*（ドキュメントビューのみ）。

   ビルトインのアイコンは、これらのいずれかの名前の下に表示されます。\
   テンプレートビューには、「**ステータスアイコン**」フィールドと「**フラグ**」フィールドの両方が含まれます。この場合、2 つの列に同じアイコンが表示されます。\
   ドキュメントビューには、「**表示アイコン**」フィールドが含まれます。

1. 「**ビューを保存**」をクリックします。
1. （オプション）ビューの新しい名前を指定し、「**ビューを保存**」をクリックします。\
   これにより、「**ステータスアイコン**」列がビューに追加されます。
1. （オプション）アイコンの上にポインタを合わせると、そのアイコンが何を表すかがわかります。
1. （オプション）アイコンをクリックして、そのアイコンが表すオブジェクトのエリアに移動します。\
   一部のアイコンには、オブジェクトへのリンクがありません。\
   各アイコンの属性の完全なリストについては、[ステータスアイコンとフラグの概要](#overview-of-status-icons-and-flags)の節を参照してください。

## ステータスアイコンとフラグの概要 {#overview-of-status-icons-and-flags}

次の表に、Workfront で使用可能なすべてのステータスアイコン、関連付け可能なオブジェクトのタイプ、およびそのアイコンをクリックしたときの動作を示します。

以下のアイコンのいくつかをクリックしてそのオブジェクトにアクセスするには、少なくともそのオブジェクトを表示する権限が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>ステータスアイコンまたはフラグ</strong> </th> 
   <th><strong>説明</strong> </th> 
   <th><strong>オブジェクト</strong> </th> 
   <th>クリック時</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">または <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_troble.png" style="width: 29;height: 26;"> または <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> または <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>プロジェクト状況が、目標どおり（緑）、トラブル発生中（赤）、またはリスクあり（黄）であることを示します。<br>プロジェクト状況について詳しくは、<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">プロジェクト状況と状況タイプの概要</a>を参照してください。</td> 
   <td>プロジェクト</td> 
   <td>クリックして、プロジェクトのタスクリストを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>オブジェクトの「更新」タブにメモ（更新）があることを示します。</td> 
   <td> <p>プロジェクト<br>タスク<br>イシュー<br>テンプレート<br>テンプレートタスク</p> </td> 
   <td> <p>クリックして、オブジェクトの「更新」タブを開きます。 </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">または <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>オブジェクトにドキュメントが添付されていることを示します。 </td> 
   <td> プロジェクト<br>タスク<br>イシュー<br>テンプレート<br>テンプレートタスク </td> 
   <td>クリックして、オブジェクトの「ドキュメント」タブを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">または <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>プロジェクトまたはタスクに未解決の問題があることを示します。</td> 
   <td> プロジェクト<br>タスク </td> 
   <td>クリックしてオブジェクトを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> または <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>オブジェクトに承認があることを示します。</td> 
   <td> プロジェクト<br>タスク<br>イシュー<br>テンプレート<br>テンプレートタスク </td> 
   <td>クリックしてオブジェクトを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>このアイコンを表示するには、ビューに費用アイコン列を追加します。これは、プロジェクトまたはタスクに関連する費用が含まれていることを示します。</p> </td> 
   <td> <p>プロジェクト</p> <p>タスク</p> </td> 
   <td>プロジェクトまたはタスクの「費用」タブをクリックして開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>タスクの進捗ステータスが次のいずれかであることを示します。</p> 
    <ul> 
     <li>目標通り（緑の正方形）</li> 
     <li>遅延（赤い円）</li> 
     <li>リスクあり（青いひし形）</li> 
     <li>遅れ（黄色の三角形）</li> 
    </ul> <p>タスクの進捗ステータスについて詳しくは、<a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">タスクの進捗ステータスの概要</a>を参照してください。</p> </td> 
   <td>タスク</td> 
   <td>クリックしてタスクを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> または <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>タスクが現在クリティカルパス上にあることを示します。<br>プロジェクトのクリティカルパスにあるタスクの詳細については、<a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">プロジェクトのクリティカルパスの概要</a>を参照してください。</td> 
   <td>タスク</td> 
   <td>クリックしてタスクを開きます。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>タスクがマイルストーンに関連付けられていることを示します。システム管理者は、環境でダイヤモンドのカラーをカスタマイズできます。<br>マイルストーンについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">マイルストーンパスの作成</a>を参照してください。</td> 
   <td>タスク</td> 
   <td>クリックしてタスクを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>イシューのソースオブジェクトへのリンク。イシューのソースオブジェクトは、イシューが記録されたオブジェクトです。タスクまたはプロジェクトは、タスクのソースオブジェクトにすることができます。 </td> 
   <td>イシュー</td> 
   <td>クリックして、イシューのソースオブジェクト（タスクまたはプロジェクト）を開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>イシューを最終的に解決する解決オブジェクトがあることを示します。この場合、イシューを完了することはできません。解決オブジェクトが完了すると、完了します。<br>解決オブジェクトについては、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決オブジェクトと解決可能オブジェクトの概要</a>を参照してください。</td> 
   <td>イシュー</td> 
   <td>イシューの解決オブジェクトをクリックして開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>ドキュメントを表示します。</td> 
   <td>ドキュメント</td> 
   <td>クリックしてドキュメントをダウンロードします。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>ドキュメントをダウンロードします。</td> 
   <td>ドキュメント</td> 
   <td>クリックしてドキュメントをダウンロードします。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>ドキュメントのタイプを示します。</td> 
   <td>ドキュメント</td> 
   <td>クリックしてドキュメントをダウンロードします。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belons_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>ユーザーが会社に関連付けられていることを示します。 </td> 
   <td>ユーザー</td> 
   <td>利用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>ユーザーがチームに関連付けられていることを示します。</td> 
   <td>ユーザー</td> 
   <td>クリックして、ユーザープロファイルを開きます。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>ユーザーの「配分」タブへのショートカット。 </td> 
   <td>ユーザー</td> 
   <td>クリックして、ユーザーの「配分」タブを開き、ユーザーに割り当てられている作業アイテムについて学びます。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>ユーザーがシステムのタイムゾーンとは異なるタイムゾーンにいることを示します。</td> 
   <td>ユーザー</td> 
   <td>利用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_expense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>費用が請求可能であることを示します。<br>費用について詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理 </a>を参照してください。</td> 
   <td>費用</td> 
   <td>利用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="expense_resurbable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> 費用が償還可能であることを示します。<br>費用について詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理</a>を参照してください。</td> 
   <td>費用</td> 
   <td>利用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="respurted_expense_icon.png" style="width: 44;height: 43;"></td> 
   <td> 費用が払い戻されたことを示します。<br>費用について詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理</a>を参照してください。</td> 
   <td>費用</td> 
   <td>利用不可</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
