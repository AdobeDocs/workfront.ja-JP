---
title: カスタムアクセスレベルの作成と変更
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、カスタムアクセスレベルを作成し、ユーザーに付与できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: f84611ef1c6ba1e5b2ec55375c4eb222bcf1cf5e
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 94%

---

# カスタムアクセスレベルの作成と変更

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Adobe Workfront 管理者は、カスタムアクセスレベルを作成し、ユーザーに付与できます。アクセスレベルを設定する場合は、ユーザーがオブジェクトを共有する際に付与するオブジェクト権限と連携する方法を理解することが重要です。アクセス・レベルの詳細は、次を参照してください。

* [新規アクセスレベルの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>ユーザーを設定した後で参照できるように、組み込みのアクセスレベルを変更しないことを強くお勧めします。アクセスレベルをカスタマイズするには、デフォルトのアクセスレベルをコピーし、そのコピーを変更します。これは、システム管理者と外部ユーザーを除くすべてのアクセスレベルで実行できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td>新規：標準
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## カスタムアクセスレベルの作成または編集

{{step-1-to-setup}}

1. 左側のパネルで「**アクセスレベル**」をクリックします。
1. コピーしてカスタマイズするアクセスレベルを選択し、「**コピー**」をクリックします。

   または

   （以前にコピーした）既存のアクセスレベルを編集する場合は、その名前をクリックします。

1. 表示されるボックスで、次のいずれかの操作を行って、カスタムアクセスレベルの設定を開始します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>アクセスレベルの名前を入力します。 </p> <p>アクセスレベルをコピーして新しいアクセスレベルを作成した場合、デフォルトの名前は「アクセスレベル名（コピー）」になります。ここでの「アクセスレベル名」とは、コピーしたアクセスレベルを指します。</p> <p><strong>ヒント</strong>：コピーの名前に、元のアクセスレベルの名前を含めることをお勧めします。例えば、ACME 社では、標準アクセスレベルのコピーを「ACME 標準」という名前にできます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明 </td> 
      <td>アクセスレベルの説明を入力します。このアクセスレベルを持つユーザーがアクセスできる内容をここにリストすると便利です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ライセンスタイプ</td> 
      <td>ここで選択したライセンスが、作成または編集するアクセスレベルのタイプに最も近く、関連しているライセンスであることを確認します。選択したライセンスによって、アクセスレベルで使用できる設定が決まります。詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新しいライセンスの概要</a>または<a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">ライセンスの概要</a>を参照してください。</td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）**ライセンスタイプ**&#x200B;ボックスで「**標準**」または「**プラン**」が選択されている場合は、「**次の管理アクセスを許可**」セクションまでスクロールし、このアクセスレベルを持つユーザーに対する管理アクセス許可を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td>システム全体および特定のグループで使用する承認プロセスを作成および管理します。<p>このアクセス権がない場合、ユーザーは自分が管理するアクセス権を持つ項目に対してのみ、アドホックの承認プロセスを作成できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">会社</td> 
      <td>Workfront で新しい会社を追加し、既存の会社を編集します。<br><p>このアクセス権がない場合、ユーザーは既存の会社のみを表示できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>グループ内のすべてのカスタムフォームを作成し、管理します。 <br><p>このアクセス権がない場合、ユーザーは、投稿や管理のアクセス権を持つオブジェクトに対してのみ既存のフォームを添付できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">為替レート</td> 
      <td> Workfront に新しい通貨を追加します。 <p>このアクセス権がない場合、ユーザーは作成したプロジェクトにのみ既存の通貨を追加できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>Workfront のオブジェクトに関するすべての費用を表示します。<p>このアクセス権がない場合、ユーザーは次の項目のみを表示できます。</p>
       <ul>
        <li>管理するプロジェクト、タスクまたはイシューに関する費用</li>
        <li>自身の費用</li>
        <li>部下の費用</li>
       </ul><p><b>メモ</b>：ユーザーは新しい費用タイプを作成できません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">担当業務</td> 
      <td> このアクセス権を持つユーザーは、次の操作を実行できます。 
       <ul> 
        <li>既存の担当業務を表示および編集</li> 
        <li>新規担当業務を追加</li> 
        <li>役割請求率と役割コスト率を編集</li> 
       </ul> 
       <p>担当業務への管理アクセスを持つ標準またはプランナーユーザーが利用できる財務データへのアクセスに関する重要な情報について詳しくは、<a href="#standard-or-planner-users-with-administrative-access-to-job-roles">担当業務への管理アクセスを持つ標準またはプランナーユーザー</a>を参照してください。</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">マイグループのマイルストーン</td> 
      <td>「設定」のマイルストーンパスメニューで、システム内のすべてのマイルストーンパスを表示します。ユーザーは、自分のグループに属するマイルストーンパスを編集または削除することもできます。ユーザーは、自分のグループに割り当てられていないマイルストーンパスを管理（編集または削除）することはできません。<p>このアクセス権がない場合、ユーザーは既存のマイルストーンパスを表示し、管理するアクセス権を持つプロジェクトに適用することのみ可能です。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知</td> 
      <td>Workfront でリマインダー通知を作成および管理します。<p>このアクセス権がない場合、ユーザーは通知の受信と表示が制限されます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートと時間</td> 
      <td> グループ管理者は、管理するグループとサブグループ内のユーザーに、タイムシートプロファイルを割り当てることができます。 <p>このオプションを有効にしないと、グループ管理者は、タイムシートプロファイルを作成することはできても、管理するグループおよびサブグループ内の他のユーザーにタイムシートプロファイルを割り当てることはできません。</p> <p>標準ライセンスやプランライセンスを持つ他のすべてのユーザーは、Workfront ですべての時間数とタイムシートを表示できます。</p> <p>このオプションを有効にしないと、ユーザーは次の項目に対して、時間のみが表示できます。</p> 
       <ul> 
        <li>管理するプロジェクト、タスクまたはイシュー</li> 
        <li>自分のタイムシート</li> 
        <li>自分に報告するユーザーのタイムシート</li> 
        <li>承認するタイムシート</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**追加の制限事項を設定**」をクリックし、次にアクセスレベルに対して次のいずれかの制限を設定します。

   >[!IMPORTANT]
   >
   >ベンダー（組織に属さないユーザー）などの外部ユーザーに対しては、タスク、プロジェクト、アップデート、通知、その他の会社、チーム、グループへのアクセスを制限することをお勧めします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">タスクまたはイシューに割り当てられている場合に、プロジェクト全体へのアクセス権限を与えない</td> 
      <td> プロジェクトの権限で許可されている場合でも、タスクやイシューに割り当てられたユーザーが、親プロジェクトへの権限も取得できないようにします。<p>プロジェクトの権限の設定について詳しくは、<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトの編集</a>の記事の <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> の節を参照してください。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">プロジェクト、タスク、イシューなどからドキュメントへのアクセス権限を継承しない</td> 
      <td>親オブジェクトに設定された権限を、ドキュメントが継承しないようにします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーが含まれている会話の更新のみを表示する</td> 
      <td> ユーザーが自分の名前またはチームの名前が含まれるコメントのみを表示できるようにします。 <p> <p><b>メモ</b>：これにより、ユーザーが Workfront で項目を登録できなくなります。項目の購読について詳しくは、 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Adobe Workfrontの項目を購読</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">絶対にユーザーによるコメントの削除を許可しない </td> 
      <td> ユーザーが項目に対して付けたコメントを削除できないようにします。  <p><b>メモ</b>：誰も他のユーザーのコメントを削除できません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーが所属する会社、グループおよびチームのみを表示する</td> 
      <td>ユーザーが、所属する会社、グループおよびチームとのみ項目を表示、共有できるようにします。<p><strong>注意</strong>：要求者ライセンスを持つユーザーは、このオプションが選択されている場合でも、その要求者が属さない会社を表示できません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定時間数または実際の時間数の表示を許可しない</td> 
      <td>ユーザーがアクセス権を持つ作業項目の予定時間数と実際の時間数を、ユーザーが表示できないようにします。ただし、ユーザー自身が記録した実際の時間数や、ユーザーの直属の部下が記録した時間数を表示することはできます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">絶対にユーザーによるお知らせの削除を許可しない</td> 
      <td>ユーザーがお知らせセンターの通知を削除できないようにします。詳しくは、<a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">通知の送信</a>を参照してください</td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付きおよびオプション）Workfront システムが複数の会社に属するユーザーに対して設定されている場合は、「**他の会社のユーザーに表示するユーザーの限定**」のセクションで、所属する会社に基づいて他のユーザーに対する表示を制限します。

   ユーザーに対して、自分の会社のユーザーや、プライマリ会社として指定した会社のユーザーのみを表示するように制限できます。通常、プライマリ会社は、ほとんどのユーザーが作業するWorkfrontアカウントを表します。 プライマリ会社について詳しくは、[会社の作成および編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。

   >[!NOTE]
   >
   >2 人のユーザーが 2 つの異なる会社に属していても、両方のユーザーがプライマリ会社のユーザーを表示できる場合、プライマリ会社に関連付けられた更新エリアが表示されます。

1. （オプション）作業中のアクセスレベルで他のオブジェクトや他のエリアのアクセス権を設定するには、[Adobe Workfront へのアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)にある記事のうちの 1 つ（[タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)、[財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)など）に従って、作業を続けます。
1. 「**保存**」をクリックします。

   アクセスレベルを作成したら、そのアクセスレベルをユーザーに割り当てることができます（システム管理者のアクセスレベルでない場合）。

   詳しくは、[ユーザープロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

   アドビ管理者がユーザーにシステム管理者のアクセスレベルを割り当てる方法について詳しくは、[ユーザーへの完全な管理アクセスの付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)を参照してください。

## 担当業務への管理アクセス権を持つ標準ユーザーまたはプランナーユーザー {#planner-users}

標準ユーザーまたはプランナーユーザーに担当業務への管理アクセス権を付与すると、そのユーザーに対して「役割請求率と役割コスト率を編集」の設定が自動的に有効になります。

後にそのユーザーの担当業務への管理アクセス権を無効にした場合、「役割請求率と役割コスト率を編集」設定が有効なままなので、担当業務は依然としてそのユーザーに対して表示されます。

これが発生し、担当業務を表示するためのユーザーのアクセス権を削除する必要がある場合は、ユーザーの「役割請求率と役割コスト率を編集」権限設定を無効にする必要があります。手順について詳しくは、[財務データへのアクセス権の付与](grant-access-financial.md)を参照してください。
