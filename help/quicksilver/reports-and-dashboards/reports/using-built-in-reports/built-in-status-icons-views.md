---
product-area: reporting
navigation-topic: using-built-in-reports
title: ビューのビルトインステータスアイコン
description: ビューのビルトインステータスアイコン
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 2%

---

# ビューのビルトインステータスアイコン

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

組み込みの [ ステータスアイコン ] フィールドをビューの列として追加し、オブジェクトの主要ポイントをより詳細に表示することができます。 ステータスアイコンを使用すると、次の条件が存在する場合に一目で確認できます。

* オブジェクトにドキュメントが添付されています
* オブジェクトが承認プロセスに関連付けられています
* オブジェクトには、追加のメモが関連付けられています
* 費用は請求可能または償還可能です
* タスクがクリティカルパス上にあります
* ユーザーが会社、チームに属している、または別のタイムゾーンにいる

[ ステータスアイコン ] フィールドのインジケータのほとんどは、実際のオブジェクトまたはオブジェクトの領域へのクイックリンクです。

アイコンで表される項目がオブジェクトにない場合、見つからない項目を表すアイコンが、完全なイメージではなく、[ ステータスアイコン ] 列にアウトラインとして表示されます。\
![task_status_icons.png](assets/task-status-icons.png)\
詳しくは、 [ステータスアイコンとフラグの概要](#overview-of-status-icons-and-flags) 」の節を参照してください。\
一部の見解では、 **ステータスアイコン** フィールド名 **フラグ** または **アイコンを表示**.\
「ステータスアイコン」フィールドに含まれるアイコンの外観をカスタマイズすることはできません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートに列を追加します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>既存のビューに対する権限の管理</p> <p>レポートに列を追加する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ビューにステータスアイコンフィールドを追加する

一部の組み込みビューおよびレポートには、既に「ステータスアイコン」フィールドが含まれています。

すべてのビューに「ステータスアイコン」フィールドを追加することはできません。

最初から作成したカスタムビューに「ステータスアイコン」フィールドを追加するには、次の手順を実行します。

1. 次のオブジェクトのリストに移動します。

   * タスク
   * 問題
   * プロジェクト
   * テンプレート タスク
   * テンプレート
   * 費用
   * ドキュメント
   * ユーザー\
      これらのオブジェクトのみが **ステータスアイコン** フィールドが使用可能です。\
      オブジェクトリストの詳細については、 [Adobe Workfrontのリストの概要](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. クリック **列を追加**.
1. 内 **この列に表示** ボックスに、次のいずれかのフィールド名を入力し、リストに表示されたら選択します。

   * *状態アイコン*
   * *フラグ*
   * *アイコンを表示*（ドキュメントビューのみ）

   組み込みアイコンは、次の名前の下に表示されます。\
   テンプレートビューには、 **ステータスアイコン** そして **フラグ** フィールド。 この場合、2 つの列に同じアイコンが表示されます。\
   ドキュメントビューには、 **アイコンを表示** フィールドに入力します。

1. クリック **ビューを保存**.
1. （オプション）ビューの新しい名前を指定し、 **ビューを保存**.\
   これにより、 **ステータスアイコン** 列をビューに追加します。
1. （オプション）アイコンの上にマウスポインターを置くと、そのアイコンが何を表すかを把握できます。
1. （オプション）アイコンをクリックして、そのアイコンで表されるオブジェクトの領域に移動します。\
   すべてのアイコンがオブジェクトへのリンクであるわけではありません。\
   各アイコンの属性の完全なリストについては、 [ステータスアイコンとフラグの概要](#overview-of-status-icons-and-flags) 」セクションに入力します。

## ステータスアイコンとフラグの概要 {#overview-of-status-icons-and-flags}

次の表に、Workfrontで使用可能なすべてのステータスアイコン、関連付け可能なオブジェクトのタイプ、およびそれらをクリックしたときの動作を示します。

次のアイコンの一部をクリックしてこれらのオブジェクトにアクセスするには、少なくともオブジェクトの表示権限が必要です。

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
   <td>プロジェクトの条件が、ターゲット上（緑）、トラブル中（赤）、または危険下（黄）であることを示します。<br>プロジェクト条件について詳しくは、 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">プロジェクト条件と条件タイプの概要</a>.</td> 
   <td>プロジェクト</td> 
   <td>をクリックして、プロジェクトのタスクリストを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>オブジェクトが [ 更新 ] タブにメモ（更新）を持っていることを示します。</td> 
   <td> <p>プロジェクト<br>タスク<br>問題<br>テンプレート<br>テンプレートタスク</p> </td> 
   <td> <p>をクリックして、オブジェクトの「更新」タブを開きます。 </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">または <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>オブジェクトにドキュメントが添付されていることを示します。 </td> 
   <td> プロジェクト<br>タスク<br>問題<br>テンプレート<br>テンプレートタスク </td> 
   <td>をクリックして、オブジェクトの「ドキュメント」タブを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">または <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>プロジェクトまたはタスクに未解決の問題があることを示します。</td> 
   <td> プロジェクト<br>タスク </td> 
   <td>をクリックして、オブジェクトを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> または <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>オブジェクトに承認があることを示します。</td> 
   <td> プロジェクト<br>タスク<br>問題<br>テンプレート<br>テンプレートタスク </td> 
   <td>をクリックして、オブジェクトを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>このアイコンを表示するには、ビューに費用アイコン列を追加します。 これは、プロジェクトまたはタスクに関連する費用が含まれていることを示します。</p> </td> 
   <td> <p>プロジェクト</p> <p>タスク</p> </td> 
   <td>プロジェクトまたはタスクの「費用」タブをクリックして開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>タスクの進捗状況ステータスが次のいずれかであることを示します。</p> 
    <ul> 
     <li>オンタイム（緑の四角形）</li> 
     <li>遅延（赤い円）</li> 
     <li>リスク（青いひし形）</li> 
     <li>背後（黄色の三角形）</li> 
    </ul> <p>タスクの進捗状況ステータスについて詳しくは、 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">タスクの進捗状況ステータスの概要</a>.</p> </td> 
   <td>タスク</td> 
   <td>をクリックして、タスクを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> または <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>タスクが現在クリティカルパス上にあることを示します。 <br>プロジェクトのクリティカルパスに関するタスクの詳細については、 <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">プロジェクトの概要の重要なパス</a>.</td> 
   <td>タスク</td> 
   <td>をクリックして、タスクを開きます。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>タスクがマイルストーンに関連付けられていることを示します。 システム管理者は、お使いの環境でダイヤモンドの色をカスタマイズできます。<br>マイルストーンについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">マイルストーンパスを作成</a>.</td> 
   <td>タスク</td> 
   <td>をクリックして、タスクを開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>イシューのソースオブジェクトへのリンク。 イシューのソースオブジェクトは、イシューが記録されたオブジェクトです。 タスクまたはプロジェクトは、タスクのソースオブジェクトにすることができます。 </td> 
   <td>問題</td> 
   <td>クリックして、イシューのソースオブジェクト（タスクまたはプロジェクト）を開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>問題を最終的に解決する解決オブジェクトがあることを示します。 この場合、問題を完了することはできません。 オブジェクトの解決が完了すると完了します。 <br>オブジェクトの解決については、 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</td> 
   <td>問題</td> 
   <td>問題の解決オブジェクトをクリックして開きます。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>ドキュメントを表示します。</td> 
   <td>ドキュメント</td> 
   <td>をクリックして、ドキュメントをダウンロードします。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>ドキュメントをダウンロードします。</td> 
   <td>ドキュメント</td> 
   <td>をクリックして、ドキュメントをダウンロードします。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>ドキュメントのタイプを示します。</td> 
   <td>ドキュメント</td> 
   <td>をクリックして、ドキュメントをダウンロードします。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belons_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>ユーザーが会社に関連付けられていることを示します。 </td> 
   <td>ユーザー</td> 
   <td>使用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>ユーザーがチームに関連付けられていることを示します。</td> 
   <td>ユーザー</td> 
   <td>「 」をクリックして、ユーザープロファイルを開きます。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>ユーザーの「配分」タブへのショートカット。 </td> 
   <td>ユーザー</td> 
   <td>をクリックして、ユーザーの「配分」タブを開き、ユーザーに割り当てられている作業項目について学習します。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>ユーザーがシステムのタイムゾーンとは異なるタイムゾーンにいることを示します。</td> 
   <td>ユーザー</td> 
   <td>使用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_expense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>費用が請求可能であることを示します。<br>費用について詳しくは、 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理 </a>.</td> 
   <td>費用</td> 
   <td>使用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="expense_resurvable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> 費用が償還可能であることを示します。<br>費用について詳しくは、 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理 </a>.</td> 
   <td>費用</td> 
   <td>使用不可</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="respurted_expense_icon.png" style="width: 44;height: 43;"></td> 
   <td> 費用が償還済みであることを示します。<br>費用について詳しくは、 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理 </a>.</td> 
   <td>費用</td> 
   <td>使用不可</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
