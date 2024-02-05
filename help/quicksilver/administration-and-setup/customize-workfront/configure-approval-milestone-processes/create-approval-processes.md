---
title: 作業項目の承認プロセスの作成
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: ユーザーが作業アイテム（プロジェクト、タスク、イシュー、テンプレート、テンプレートタスク）、ドキュメント、プルーフに添付できる承認プロセスを作成できます。承認プロセスを実行すると、オブジェクトに指定された担当者が、システム内のオブジェクトが進行する前に、特定の変更を確認するようになります。
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '2163'
ht-degree: 95%

---

# 作業項目の承認プロセスの作成

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

ユーザーが作業アイテム（プロジェクト、タスク、イシュー、テンプレート、テンプレートタスク）、ドキュメント、プルーフに添付できる承認プロセスを作成できます。承認プロセスを実行すると、オブジェクトに指定された担当者が、システム内のオブジェクトが進行する前に、特定の変更を確認するようになります。

この記事では、作業アイテム（プロジェクト、タスク、イシュー、テンプレート、テンプレートタスク）のシステムレベルまたはグループレベルのグローバル承認プロセスを作成する方法について説明します。

ドキュメントまたはプルーフに関連する承認について詳しくは、次の記事を参照してください。

* [ドキュメント承認のリクエスト](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [自動ワークフローの概要](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>また、ユーザーは、管理権限を持つプロジェクト、タスク、イシュー、テンプレート、テンプレートタスクに対して、1 回限りの承認プロセスを作成することもできます。
>
>この記事では、「グローバル承認プロセス」という用語を使用して、1 回限りの承認プロセスと区別します。グローバル承認プロセスは繰り返し使用できます。
>
>グループレベルでは、グローバル承認プロセスは、そのグループに属する作業アイテムとステータスに制限されます。
>
>1 回限りの承認プロセスについて詳しくは、[承認プロセスの概要](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)および[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>新規プラン：標準 </p>
 <p>または</p> 
<p>現在のプラン：プラン </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront 管理者である場合や、承認プロセスに対する管理者アクセス権を持っている場合は、システムレベルの承認プロセスを作成することも、特定のグループに対してグループレベルの承認プロセスを作成することもできます。</p> 
   <p>グループ管理者である場合は、管理するグループに対してグループレベルの承認プロセスを作成できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 作業アイテムのシステムレベルまたはグループレベルのグローバル承認プロセスを作成する

{{step-1-to-setup}}

1. （条件付き）システムレベルの承認プロセスを作成する場合、左パネルで&#x200B;**プロセス**／**承認**&#x200B;をクリックします。

   または

   グループレベルの承認プロセスを作成する場合は、**グループ** ![](assets/groups-icon.png) をクリックし、グループの名前をクリックしてから「**承認**」をクリックします。

   <!--hidden for the new tab redesign - August 2023: 
   ![](assets/approvals-area-in-setup-processes.png)
   -->

1. 次のいずれかを選択します。 **プロジェクト承認**, **タスクの承認**&#x200B;または **問題の承認** タブをクリックします。

1. 「**新規承認プロセス**」をクリックします。
1. 表示されるボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス名</td> 
      <td><p>承認プロセスにわかりやすい名前を入力します。ユーザーがオブジェクトに承認プロセスを適用すると、この名前が表示されます（<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">新規または既存の承認プロセスと作業の関連付け</a>参照）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td><p>承認プロセスの説明を入力します。これは、<b>設定</b>エリアの<b>承認</b>セクションの承認プロセス名の横に表示されます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>他のユーザーが作成するプロジェクト、タスクおよびイシューに承認プロセスを添付できるようにする場合は、このオプションを有効のままにします。 </p> <p>このオプションは、デフォルトで有効になっています。</p> <p> ヒント：承認プロセスを非アクティブとしてマークすると、組織で承認プロセスを使用する必要がなくなったが使用履歴情報を保持したい場合に役立ちます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">この承認の利用者 </td> 
      <td> <p>特定のグループにのみ属するプロジェクト、タスク、イシュー、テンプレートに対して承認プロセスを使用できるようにするには、グループの名前を入力し始め、表示されたら選択します。</p> 
       <ul> 
       <li>システム管理者、または承認プロセスへの管理者アクセス権を持っている場合は、名前を入力すると、システム内のすべてのグループが表示されます。<b>すべてのグループ</b> はデフォルトで選択されています。 </li> 
       <li>承認プロセスへの管理者アクセス権を持たないグループ管理者は、その名前を入力する際に、管理対象のグループに承認プロセスを割り当てることができます。「<b>すべてのグループ</b>」オプションは利用できません。</li> 
       </ul> 
       <p>このオプションは、1 回限りの承認プロセスには使用できません。</p> 
       <p><b>警告</b>：グループ固有の承認プロセスを変更すると、既に作業アイテムに関連付けられている既存の承認プロセスが変更される場合があります。これらの変更点について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">グループと承認プロセスの変更が割り当てられた承認プロセスに及ぼす影響</a>を参照してください。</p> 
       <p>グループのページからグループの承認プロセスを一覧表示および管理する方法について詳しくは、<a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">グループレベルの承認プロセス</a>を参照してください。 </p> 
       <p>承認プロセスへの管理者アクセス権について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 次のオプションを使用して、承認プロセスのパスを設定します。

   パスとは、承認プロセスで実行する必要がある操作を指定する場所です。パスにステージを作成して、承認作業の実行者と順序を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">ステータスが次のように設定された場合、承認プロセスを開始</p> </td> 
      <td> <p>作業アイテムの承認プロセスをトリガーにするステータスを選択します。誰かが作業アイテムをこのステータスに更新すると、承認プロセスが開始します。 </p> <p>複数の承認プロセスパスに対して同じステータスを選択することはできません。</p> <p>使用可能なステータスは、「<b>」オプションで選択した内容に基づきます。この承認は、</b> によってしようされることができます（上記の表で説明）。</p> 
       <ul> 
       <li> <b>すべてのグループ</b>が選択されている場合、システム全体のステータスのみを使用できます。
       <li> <p>特定のグループを選択した場合、そのグループが使用できるステータスのみが使用可能になります</p> </li> 
       </ul> <p>承認プロセスとステータスの連携について詳しくは、<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>記事の<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">承認プロセスがステータスに依存する仕組み</a>の節を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステージ名</td> 
      <td>（オプション）パスの最初のステージを表す名前を入力します。ステージ名を指定しない場合、デフォルトの名前は<b>ステージ 1</b> です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認者</td> 
      <td> <p>このステージの承認者として指定するユーザー、チームまたは担当業務の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。アクティブなユーザー、<span>担当業務</span>およびチームのみを追加できます。 </p>

   <p><b>ヒント</b>：</p>

   <p>ユーザーを承認者として追加する場合は、同じ名前のユーザーを区別するために、アバター、ユーザーのプライマリの役割、またはメールアドレスに注意してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。</p>
      <p>ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、<a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">ユーザーにアクセス権を付与</a>を参照してください。 </p>

   <p><b>メモ</b>：

   承認者としてユーザー、チームまたは役割を追加しても、その承認に関連付けられたオブジェクトに対する権限は自動的には付与されません。承認ステップがトリガーされると、オブジェクトに対する権限が付与されます。そうでない場合は、承認を決定する前に、オブジェクトをユーザー、チームまたは役割と共有する必要があります。 </p> <p>また、個人の役割を指定することで、個人を承認者に指定することもできます。例えば、プロジェクト所有者、プロジェクトスポンサー、ポートフォリオ所有者、プログラム所有者、または管理者を承認者として割り当てることができます。これらのオプションは、入力を始めると自動的に表示されます。</p>

   <p><b>重要</b>：  
       <ul> 
       <li> <p>プロジェクトスポンサーに承認を割り当て、誰もプロジェクトのスポンサーとして指定されていない場合、承認はプロジェクト所有者に再割り当てされます。プロジェクトの所有者として誰も指定されていない場合、承認は Workfront 管理者に割り当てられます。 </p> </li> 
      </ul> 
       <ul> 
       <li> <p>承認を役割に割り当て、「<b>承認者がプロジェクトチームに所属している必要はない（役割を含む承認プロセスの場合）</b>」が無効になっているが、承認時に一致する役割がプロジェクトチームに存在しない場合、承認はプロジェクト所有者に再割り当てされます。承認設定について詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">グローバル承認設定を指定</a>を参照してください。</p> </li> 
       </ul> 
       <ul> 
       <li> <p>プロジェクト所有者に承認を割り当て、誰もプロジェクトの所有者として指定されていない場合、設定エリアの「顧客情報」セクションで示されているように、承認はメインの Workfront 管理者に再割り当てされます。詳しくは、<a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">システムの基本情報を設定</a>を参照してください。  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>このプロセスを繰り返して、複数の承認者をステージに追加できます。1 つのステージには、ユーザー、チーム、および承認者としての担当業務の組み合わせを含めることができます。ステージに追加できる承認者の数に制限はありません。</p> <p><b>重要</b>：  <p>担当業務を承認者として割り当てると、その担当業務に関連付けられ、プロジェクトチームにも属するすべてのユーザーが承認を決定できます。 </p> <p>チームを承認者として割り当てると、そのチーム内のすべてのユーザーが承認を決定できます。 </p> <p>プロジェクトチームについて詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>を参照してください。作業の承認について詳しくは、<a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">作業の承認</a>を参照してください。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つの決定のみが必要です <br> <br>（ステージに複数の承認者を追加した場合にのみ表示されます） </td> 
      <td> <p>ステージ上の任意の承認者が、このステージで作業項目を承認または拒否できる場合は、このオプションを選択します。 このアクションによって、作業項目のステージからの移動が許可されます。 </p> <p>このオプションを選択しない場合、項目がステージから移動する前に、指定されたすべての承認者が（任意の順序で）ステージを承認または拒否する必要があります。承認者のいずれか 1 人がステージを却下した場合、プロセスは中断し、必要な変更を行うためにやり直します。その後、承認者はステージを再び承認または却下できます。</p> <p>チームが承認者として指定されると、チームのメンバーは誰でもステージを許可または却下できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">ステージを追加</p> </td> 
      <td><p>（オプション）上記の 3 つの行で説明したオプションを使用して、パスに別のステージを追加します。パスには、必要な数のステージを追加できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認が却下されたときのアクションを選択します</p> </td> 
      <td> <p>パスの任意のステージで作業項目が却下された場合に実行するアクションを選択します。</p> 
       <ul> 
       <li><b>イシューを作成</b>：（プロジェクトおよびタスクの承認プロセスでのみ使用可能）承認プロセスが実行されているプロジェクトまたはタスクにイシューが作成されます。タスクに割り当てられたデフォルトのリソース、またはプロジェクトの所有者がイシューに割り当てられます。デフォルトでは、作成されるイシューの名前は「<b>承認却下（&lt;プロジェクトまたはタスク名&gt;）</b>」となります。却下が発生した承認プロセスに応じて、タスクまたはプロジェクトの下に入力される拒否イシューです。</li> 
       <li> <p><b>ステータスを次の値に設定</b>：次のいずれかを選択します。</p> 
       <ul> 
       <li><b>前のステータス</b>：却下されたプロジェクト、タスクまたはイシューは、承認プロセスを有効化するステータスの前のステータスに戻ります。</li> 
       <li><p><b>リスト内のその他のステータス</b>：却下されたオブジェクトは、「保留中」など、選択したステータスに移動します。Workfront システムに追加したデフォルトのステータスまたはカスタムステータスの 1 つを選択できます。</p>
       <p>承認プロセスに関連付けられたステータスを却下ステータスとして選択すると、却下されたオブジェクトは選択したステータスに移動し、「承認保留中」としてマークされます。</p> 
       <p> 例えば、「保留中」を却下ステータスとして選択し、「保留中」のステータスが承認プロセスと関連付けられている場合、却下されたオブジェクトは「保留中 - 承認保留中」ステータスに配置され、承認が必要となります。</p>

   </tr> 
    </tbody> 
   </table>

1. （オプション）「**パスを追加**」をクリックして、前の手順のオプションのリストを参照し、承認プロセスに別のパスを追加します。

   新しいパスは、別のステータスに関連付ける必要があります。このパスは、項目が更新されてこのステータスを表示するときにトリガーされます。同じステータスに対して 2 つのパスを指定することはできません。

1. 「**保存**」をクリックします。
1. 承認プロセスが作成されたら、次のいずれかを続行します。

   * 承認プロセスを、システム全体の特定のプロジェクト、タスクまたはイシューに関連付けます。詳くは、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。
   * Workfront 以外では、承認プロセスとプロジェクト、タスクまたはイシューに関連付けられることをユーザーに通知します。詳しくは、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。
   * この承認プロセスが却下され、項目が別のステータスになった場合、トリガーされる別の承認プロセスを作成します。これにより、承認プロセスを相互にリンクすることができます。

承認プロセスの編集について詳しくは、[承認プロセスの編集](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)を参照してください。

## 作業アイテムへの承認プロセスの関連付け

作業項目（プロジェクト、タスク、またはタスク）の承認プロセスを作成する場合は、次の手順を実行します。

1. 最初に承認プロセスを作成
1. 作業項目の作成
1. 承認プロセスと作業項目の関連付け

承認プロセスと作業アイテムの関連付けの手順について詳しくは、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。

>[!NOTE]
>
>プロジェクト、タスクまたはイシューの管理権限がある Workfront ユーザーは、作成先のオブジェクトでのみ使用する、1 回限りの承認プロセスを作成できます。詳しくは、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。

## 単一の作業アイテムに対するグローバル承認プロセスの変更をユーザーに許可

デフォルトでは、プロジェクト、タスクおよびイシューに対する権限を管理するユーザーは、1 回限りの承認プロセスを作成できます。プロジェクト、タスクおよびイシューに 1 回限りの承認プロセスを追加する方法について詳しくは、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)の記事の [1 回限りの承認プロセスをプロジェクト、タスク、イシュー、テンプレートまたはテンプレートのタスクに関連付ける](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process)の節を参照してください。

また、作業アイテムに関連付けられたグローバル承認プロセスの設定を変更することもできます。これらの変更は、システムレベルの承認プロセスに関連するプロジェクト、タスクまたはイシューにのみ影響します。詳しくは、[新規または既存の承認プロセスと作業の関連付け](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)の記事の[特定のオブジェクトで使用するグローバル承認プロセスを変更](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process)の節を参照してください。
