---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: 承認プロセスの編集
description: Adobe Workfront管理者、または承認プロセスへの管理者アクセス権を持っている場合、システム内のすべての承認プロセスを表示および編集できます。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 5%

---

# 承認プロセスの編集

Adobe Workfront管理者、または承認プロセスへの管理者アクセス権を持っている場合、システム内のすべての承認プロセスを表示および編集できます。

グループ管理者は、管理対象のグループに関連付けられた承認プロセスを表示および編集できます。

承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* 既に使用中のグローバル承認プロセスを編集すると、変更は、既に関連付けられているシステム全体のすべてのオブジェクトに影響を与えます。
>* オブジェクトで既に開始している承認プロセスの現在のステージに新しい承認者を追加すると、そのオブジェクトのプロセスがリセットされ、承認者が再開する必要があります。
>
>  ただし、オブジェクトで既に開始している承認プロセスで次の変更を加えた場合、そのプロセスは中断せずに続行されます。
>
>* 現在のステージの後にステージを追加
>* 現在のステージの前に承認者を追加


## アクセス要件

以下が必要です。

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
   <td> <p>システム管理者以外の場合は、承認プロセスへの管理者アクセス</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 既存の承認プロセスの編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).
1. （条件付き）システムレベルの承認プロセスを編集する場合、 **プロセス** > **承認** をクリックします。

   または

   グループレベルの承認プロセスを編集する場合は、次の手順を実行します。

   1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).
   1. グループ承認プロセスを一覧表示または管理するグループの名前をクリックします。
   1. 左側のパネルで、 **承認**. クリックが必要になる場合があります **さらに表示** 1 つ目は

1. 次をクリック： **プロジェクト承認**, **タスク承認**&#x200B;または **問題の承認** タブに表示されます。

1. 編集する承認プロセスを選択し、「 **編集** をクリックします。 「承認プロセスの編集」ボックスが表示されます。

   ![](assets/edit-approval-process-global-area-new.png)

1. 表示されるボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス名</td> 
      <td>承認プロセスのわかりやすい名前を入力します。 オブジェクトに承認プロセスを適用すると、この名前が表示されます ( <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">新規または既存の承認プロセスと作業の関連付け</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>承認プロセスの説明を入力します。 これは、 <b>承認</b> セクション <b>設定</b> 承認プロセス名の横の領域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>他のユーザーが作成するプロジェクト、タスクおよびイシューに承認プロセスを添付できるようにする場合は、このオプションを有効のままにします。 </p> <p>このオプションは、デフォルトで有効になっています。</p> <p>ヒント：承認プロセスを非アクティブとしてマークすると、組織で承認プロセスを使用する必要がなくなり、使用履歴情報を保持したい場合に役立ちます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">この承認の利用者 </td> 
      <td> <p>特定のグループにのみ属するプロジェクト、タスク、タスク、タスクおよびテンプレートに対して承認プロセスを使用できるようにするには、グループの名前を入力し、表示されたら名前を選択します。</p> 
       <ul> 
        <li>システム管理者、または承認プロセスへの管理者アクセス権を持っている場合は、名前を入力すると、システム内の任意のグループが表示されます。 <b>すべてのグループ</b> はデフォルトで選択されています。 </li> 
        <li>承認プロセスへの管理者アクセス権を持たないグループ管理者は、その名前を入力する際に、管理対象のグループに承認プロセスを割り当てることができます。 この <b>すべてのグループ</b> オプションは使用できません。</li> 
       </ul> <p>このオプションは、単一使用の承認プロセスには使用できません。</p> <p><b>警告</b>:グループ固有の承認プロセスを変更すると、既に作業項目に関連付けられている既存の承認プロセスが変更される場合があります。 これらの変更点について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が、割り当てられた承認プロセスに及ぼす影響</a>.</p> <p>グループのページからグループの承認プロセスを一覧表示および管理する方法については、 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">グループレベルの承認プロセス</a>. </p> <p>承認プロセスへの管理者アクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 次のオプションを使用して、承認プロセスのパスを設定します。

   パスとは、承認プロセスで実行する必要がある操作を指定する場所です。 パスにステージを作成して、承認作業の実行者と順序を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">ステータスが次のように設定された場合、承認プロセスを開始</p> </td> 
      <td> <p>作業項目の承認プロセスをトリガーにするステータスを選択します。 誰かが作業項目をこのステータスに更新すると、承認プロセスが開始されます。 </p> <p>複数の承認プロセスパスに対して同じステータスを選択することはできません。</p> <p>使用可能なステータスは、「 」オプションで選択した内容に基づきます <b>この承認は、</b> （上記の表で説明）:</p> 
      <ul> 
      <li> If <b>すべてのグループ</b> を選択した場合、システム全体でロックされたステータスのみを使用できます。 <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>特定のグループを選択した場合、そのグループで使用可能なステータスのみが使用可能になります</p> </li> 
      </ul> <p>承認プロセスとステータスの連携について詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">承認プロセスがステータスに依存する方法</a> 記事内 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージ名</td> 
      <td>（オプション）パスの最初のステージを表す名前を入力します。 ステージ名を指定しない場合、デフォルトの名前はです。 <b>ステージ 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認者</td> 
      <td> <p>このステージの承認者として指定するユーザー、チームまたはジョブの役割の名前を入力し始め、ドロップダウンリストに表示されたら名前をクリックします。 追加できるのは、アクティブなユーザー、ジョブの役割、チームのみです。 </p>

   <p><b>ヒント</b>:</p>

   <p>ユーザーを承認者として追加する場合は、アバター、ユーザーのプライマリの役割、または電子メールアドレスに注目して、同じ名前のユーザーを区別します。 ユーザーを追加したときに表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。</p>

   <p><b>メモ</b>:

   承認者としてユーザー、チーム、または役割を追加しても、その承認に関連付けられたオブジェクトに対する権限は自動的には付与されません。 承認ステップがトリガーされると、オブジェクトに対する権限を受け取ります。 そうしない場合、承認を決定する前に、オブジェクトをオブジェクトと共有する必要があります。 </p>
   <p>また、個人の役割を指定することで、個人を承認者に指定することもできます。 例えば、プロジェクト所有者、プロジェクトスポンサー、Portfolio所有者、プログラム所有者、または管理者を承認者として割り当てることができます。 これらのオプションは、入力を始めると自動的に表示されます。</p> 
      <p><b>重要</b>:  
      <ul> 
      <li> プロジェクトスポンサーに承認を割り当て、誰もプロジェクトのスポンサーとして指定されていない場合、承認はプロジェクト所有者に再割り当てされます。 プロジェクトの所有者が指定されていない場合、承認はWorkfront管理者に割り当てられます。 </li> 
      <li> ロールとオプションに承認を割り当てる場合 <b>承認者がプロジェクトチームに属している必要はありません</b> は無効ですが、承認時の役割に一致するプロジェクトチームの役割はありません。承認はプロジェクト所有者に再割り当てされます。 承認設定について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">グローバル承認設定の指定</a>.
      </li> 
      <li>プロジェクト所有者に承認を割り当てて、誰もプロジェクトの所有者に指定されていない場合、「セットアップ」領域の「顧客情報」セクションで示されたように、承認はメインのWorkfront管理者に再割り当てされます。 詳しくは、 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">システムの基本情報を設定する</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>ジョブの役割を承認者として割り当てると、そのジョブの役割に関連付けられ、プロジェクトチームにも属するすべてのユーザーが承認を決定できます。 </p> 
      <p>チームを承認者として割り当てると、そのチーム内のすべてのユーザーが承認を決定できます。 </p> 
      <p>プロジェクトチームの詳細については、 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>. 作業の承認について詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">作業の承認 </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">1 件の決定のみ必要です。</td> 
      <td>（ステージに複数の承認者を追加した場合にのみ表示されます）このステージで、ステージ上のいずれかの承認者が作業項目を承認または拒否できる場合は、このオプションを選択します。 このアクションを実行すると、作業項目がステージから移動します。  
      <p>このオプションを選択しない場合、識別されたすべての承認者は、項目がステージから離れる前に（任意の順序で）ステージを承認または拒否する必要があります。 承認者のいずれかがステージを拒否した場合、プロセスは中断し、必要な変更を加えるためにやり直します。 その後、承認者はステージを再び承認または拒否できます。</p> 
      <p>チームが承認者として指定されると、チームの任意のメンバーがステージを許可または却下できます。</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">ステージを追加</p> </td> 
      <td>（オプション）上記の 3 行で説明したオプションを使用して、パスに別のステージを追加します。 パスには、必要な数のステージを追加できます。</td> 
     </tr>
     <tr> 
      <td role="rowheader"> 承認が却下された場合の処理を選択</td> 
      <td> <p>パスの任意のステージで作業項目が拒否された場合に実行するアクションを選択します。</p> 
      <ul> <li><strong>イシューの作成</strong>:（プロジェクトとタスクの承認プロセスに対してのみ使用可能）承認プロセスが実行されているプロジェクトまたはタスクにイシューが作成されます。 タスクに割り当てられたデフォルトのリソース、またはプロジェクトの所有者がイシューに割り当てられます。 デフォルトでは、作成されるイシューの名前は次のようになります。 <strong>承認却下（プロジェクト名またはタスク名）</strong>. 却下が発生した承認プロセスに応じて、タスクまたはプロジェクトの下に入力される却下の問題です。</li> 
      <li> <p><strong>ステータスをに設定</strong>:次のいずれかを選択します。</p> 
      <ul> <li><strong>前のステータス</strong>:却下されたプロジェクト、タスクまたはイシューは、承認プロセスを有効化したステータスの前のステータスに戻ります。</li> 
      <li> <p><strong>リスト内のその他のステータス</strong>:却下されたオブジェクトは、「保留中」など、選択したステータスに移動します。 Workfrontシステムに追加したデフォルトのステータスまたはカスタムのステータスの 1 つを選択できます。</p> <p>承認パスの却下ステータスとして、承認プロセスに関連付けられたステータスを選択すると、却下されたオブジェクトは選択したステータスに移動し、「承認待ち」としてマークされます。</p>
      <p>例えば、却下ステータスに「保留中」を選択し、「保留中」ステータスが承認プロセスに関連付けられている場合、却下されたオブジェクトは承認が必要な「保留中 — 承認待ち」のステータスになります。</p>    <p>システム全体の承認プロセスでは、システム全体のステータスのみを使用できます。</p> <p>グループ固有の承認プロセスの場合、すべてのグループステータスを使用できます。 これには、グループ管理者が特にグループ用に作成したカスタムステータスや、システム全体のステータスが含まれます。 </p> <p>承認プロセスとステータスの連携について詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">承認プロセスがステータスに依存する方法</a> 記事内 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「 **パスを追加** 承認プロセスに別のパスを追加するには、前の手順のオプションのリストを参照します。

   新しいパスは、別のステータスに関連付ける必要があります。 パストリガー。項目が更新され、このステータスが表示されます。 同じステータスに対して 2 つのパスを指定することはできません。

1. 「**保存**」をクリックします。
1. （オプション）次のいずれかの操作をおこないます。

   * 承認プロセスを、システム全体の特定のプロジェクト、タスクまたは問題に関連付けます。詳しくは、 [新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Workfront以外で、承認プロセスがプロジェクト、タスクまたはイシューに関連付けられることをユーザーに通知します。詳しくは、 [新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * この承認プロセスが却下され、項目が別のステータスを取る場合にトリガーされる別の承認プロセスを作成します。 これにより、承認プロセスを相互にリンクすることができます。
