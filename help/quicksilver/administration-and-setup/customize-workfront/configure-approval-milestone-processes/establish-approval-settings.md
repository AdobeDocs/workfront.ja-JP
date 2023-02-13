---
title: グローバル承認設定の指定
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfrontの管理者は、Workfrontでの承認プロセスのグローバル設定を決定できます。 これらの設定は、システム内のすべての作業項目承認プロセスに影響を与えます。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# グローバル承認設定の指定

Adobe Workfrontの管理者は、Workfrontでの承認プロセスのグローバル設定を決定できます。 これらの設定は、システム内のすべての作業項目承認プロセスに影響を与えます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>システム管理者か、承認プロセスへの管理アクセス権を持つプランライセンスが必要です</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## グローバル承認設定の指定

1. Workfront as a Workfront administrator としてログインします。
1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **プロセス** > **承認** .

1. 次をクリック： **設定** アイコン ![](assets/gear-icon-settings.png) の横 **承認** 領域名。

1. 内 **承認設定** 表示されるボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">追加 &lt;number&gt; 承認プロセスに対応する計画完了日までの日数</td> 
      <td> <p>承認が必要なタスクの予定完了日に時間を追加する時間を分、時間、日、週または月数で指定します。 「経過時間」分、時間、日、または週を選択して、システムの作業スケジュールカレンダーで指定された週末、休日、非営業時間を含む時間を追加します。</p> 
      <p>例えば、タスクが金曜日に割り当てられ、期間が 3 日の場合、タスクの完了日は月曜日（土曜日と日曜日が週末の場合）に設定されます。 タスクの期間が 3 日（経過日ではない）の場合、タスクの完了日は水曜日に設定されます。</p>
      <p><b>注意</b>:タスクの承認を得るために余分な時間を追加すると、タスクとプロジェクトのタイムラインに影響します。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">（役割を含む承認プロセスの）承認者がプロジェクトチームに属している必要はありません</td> 
      <td> <p>承認プロセスに役割が含まれている場合に、承認者がプロジェクトチームに属している必要がない場合に、これを選択します。 ジョブの役割に承認の決定を割り当てると、プロジェクト上でその決定に関連付けられた役割を持つユーザーのみが承認を表示します。 この設定を有効にした場合、そのジョブの役割を持つユーザーは、プロジェクトチームに属しているかどうかに関わらず、承認リクエストを受け取ります。 ユーザーのプロジェクトの役割の編集について詳しくは、 <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">プロジェクトチームを管理</a>. </p> 
      <p><b>ヒント</b>:ロールとオプションに承認を割り当てる場合 <b>（役割を含む承認プロセスの）承認者がプロジェクトチームに属している必要はありません</b> は無効ですが、承認時の役割に一致する役割がプロジェクトチームに存在しません。承認はプロジェクト所有者に再割り当てされます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認委任を無効にする</td> 
      <td> <p>システム内のユーザーが別のユーザーに承認を委任する機能を無効にするには、このオプションを選択します。 このオプションを選択すると、承認を委任するオプションがWorkfrontから削除され、既存の承認委任が停止されます。</p> <p>Workfrontでの承認の委任について詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">承認リクエストを委任</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクト、タスクまたは問題が承認待ちステータスの場合にカスタムフォームの編集を許可</td> 
      <td> <p>承認待ちステータスの場合に、ユーザーがプロジェクト、タスクおよび問題のカスタムフォームを編集できるようにするには、このオプションを選択します。 これはデフォルト設定です。</p> 
      <p>このオプションを選択した場合：</p> 
       <ul> 
       <li>現在の承認パスや承認ステップに関係なく、すべての承認者（およびカスタムフォームを編集するアクセス権を持つ他のユーザー）は、オブジェクトが承認待ちの場合に、カスタムフォームに変更を加えることができます。</li> 
       <li>承認プロセス中にカスタムフォームに対して行われた変更は、変更前に行われた承認の決定には影響しません。</li> 
       <li> <p>プロジェクト、タスク、またはイシューに加えた変更は、この設定に関係なく、同じ方法で追跡されます。 </p> <p>例えば、更新ストリームで追跡するカスタムフォームフィールドを追加した場合、フォームに対する変更は、オブジェクト上の更新ストリームで追跡されます。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーに、新しく作成された、承認待ちの要求のリコールを許可する</td> 
      <td> <p>このオプションを選択して、ユーザーが問題を取り消せるか、最初のステータスの承認待ちリクエストにするかを設定します。 リクエストキューを設定することで、問題の最初のステータスまたはリクエストを承認プロセスに関連付けることができます。 </p> 
      <p>リクエストキューについて詳しくは、 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>.</p> 
      <p>次のいずれかの操作を行います。</p> 
       <ul> 
       <li>ユーザーが問題または要求の最初のステータスの承認を取り消す場合に、このオプションを選択します。 この場合、新しい問題やリクエストで「リコール &lt;」ボタンが表示され、承認待ちステータスになることがあります。 問題の再現を選択すると、その問題も削除されるという警告が表示されます。 問題は、再呼び出しを確認した後で削除されます。 </li> 
       <li> <p>ユーザーが問題や最初のステータスが承認待ちのリクエストを呼び出さないようにするには、このオプションの選択を解除します。 新しい問題やリクエストに [ リコール &lt;] ボタンを表示することはできません。また、承認を許可する必要があります。 これはデフォルトのオプションです。</p> 
       <p>承認待ちの項目のレビューについて詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">承認を表示 </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **変更を保存します。**
