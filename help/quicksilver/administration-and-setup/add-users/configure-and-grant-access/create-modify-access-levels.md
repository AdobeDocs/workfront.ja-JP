---
title: カスタムアクセスレベルの作成と変更
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Adobe Workfront管理者は、カスタムアクセスレベルを作成し、ユーザーに適用できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: f84611ef1c6ba1e5b2ec55375c4eb222bcf1cf5e
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 6%

---

# カスタムアクセスレベルの作成と変更

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Adobe Workfront管理者は、カスタムアクセスレベルを作成し、ユーザーに適用できます。 アクセスレベルを使用する場合は、ユーザーがオブジェクトを共有する際に付与するオブジェクト権限と連携する方法を理解することが重要です。 アクセス・レベルの詳細は、次を参照してください。

* [新しいアクセスレベルの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>ユーザーを設定した後で参照できるように、組み込みのアクセスレベルを変更しないことを強くお勧めします。 アクセスレベルをカスタマイズするには、デフォルトのアクセスレベルをコピーし、コピーを変更します。 これは、システム管理者と外部ユーザーを除くすべてのアクセスレベルで実行できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>新規：標準
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## カスタムアクセスレベルの作成または編集

{{step-1-to-setup}}

1. クリック **アクセスレベル** をクリックします。
1. コピーしてカスタマイズするアクセスレベルを選択し、 **コピー**.

   または

   （以前にコピーした）既存のアクセスレベルを編集する場合は、その名前をクリックします。

1. 表示されるボックスで、次のいずれかの操作を行って、カスタムアクセスレベルの設定を開始します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td> <p>アクセスレベルの名前を入力します。 </p> <p>アクセスレベルをコピーして新しいアクセスレベルを作成した場合、デフォルトの名前は「アクセスレベル名（コピー）」です。ここで、「アクセスレベル名」はコピーしたアクセスレベルです。</p> <p><strong>ヒント</strong>：コピーの名前に、元のアクセスレベル名を含めることをお勧めします。 例えば、ACME の会社では、標準アクセスレベルのコピーを ACME Standard という名前にできます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明 </td> 
      <td>アクセスレベルの説明を入力します。 このアクセスレベルを持つユーザーがアクセスできる内容をここにリストすると役立ちます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ライセンスの種類</td> 
      <td>ここで選択したライセンスが、作成または編集するアクセスレベルの種類に最も密接に関連しているライセンスであることを確認します。 選択したライセンスによって、アクセスレベルで使用できる設定が決まります。 詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">新しいライセンスの概要</a> または <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">ライセンスの概要</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き） **標準** または **プラン** が **ライセンスの種類** ボックス、セクションまでスクロール **次の管理アクセスを許可：** をクリックし、このアクセスレベルを持つユーザーに対する管理アクセス権限を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td>システム全体および特定のグループで使用する承認プロセスを作成および管理します。<p>このアクセス権がない場合、ユーザーは管理するアクセス権を持つ品目に対してアドホック承認プロセスのみを作成できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">会社</td> 
      <td>Workfrontで新しい会社を追加し、既存の会社を編集します。<br><p>このアクセス権がない場合、ユーザーは既存の会社のみを表示できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td>グループ内のすべてのカスタムフォームを作成し、管理します。 <br><p>このアクセス権がない場合、ユーザーは、投稿や管理のアクセス権を持つオブジェクトに対してのみ既存のフォームを添付できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">為替レート</td> 
      <td> Workfrontに新しい通貨を追加します。 <p>このアクセス権がない場合、ユーザーは作成したプロジェクトにのみ既存の通貨を追加できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>Workfrontのオブジェクトに関するすべての費用を表示します。<p>このアクセス権がない場合、ユーザーは次の項目のみを表示できます。</p>
       <ul>
        <li>管理するプロジェクト、タスクまたは問題に関する費用</li>
        <li>自費</li>
        <li>部下の費用</li>
       </ul><p><b>注意</b>：ユーザーは新しい費用タイプを作成できません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">担当業務</td> 
      <td> このアクセス権を持つユーザーは、次の操作を実行できます。 
       <ul> 
        <li>既存のジョブの役割の表示と編集</li> 
        <li>新しいジョブの役割を追加</li> 
        <li>ロールの請求とコスト率を編集します</li> 
       </ul> 
       <p>ジョブ・ロールへの管理アクセス権を持つ標準またはプランナ・ユーザーが使用できる財務データへのアクセスに関する重要な情報は、次を参照してください： <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">ジョブ・ロールへの管理アクセス権を持つ標準ユーザーまたはプランナ・ユーザー</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">マイ グループのマイルストーン</td> 
      <td>[ セットアップ ] の [ マイルストーンのパス ] メニューで、システム内のすべてのマイルストーンのパスを表示します。 ユーザーは、任意のグループに属するマイルストーンパスを編集または削除することもできます。 ユーザーは、自分のグループに割り当てられていないマイルストーンパスを管理（編集または削除）できません。<p>このアクセス権がない場合、ユーザーは既存のマイルストーンパスを表示し、アクセス権を持つ管理プロジェクトに適用することができます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダ通知</td> 
      <td>Workfrontでリマインダー通知を作成および管理します。<p>このアクセス権がない場合、ユーザーは通知の受信と表示に制限されます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートと時間</td> 
      <td> グループ管理者は、管理するグループとサブグループ内のユーザーにタイムシートプロファイルを割り当てることができます。 <p>このオプションを有効にしないと、グループ管理者は管理するグループとサブグループ内の他のユーザーにタイムシートプロファイルを割り当てることができませんが、作成はできます。</p> <p>Standard または Plan のライセンスを持つ他のすべてのユーザーは、Workfrontですべての時間とタイムシートを表示できます。</p> <p>このオプションを有効にしないと、ユーザーは次の日にのみ時間を表示できます。</p> 
       <ul> 
        <li>管理するプロジェクト、タスクまたは問題</li> 
        <li>自分のタイムシート</li> 
        <li>自分に報告する人のタイムシート</li> 
        <li>承認したタイムシート</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **追加の制限の設定**&#x200B;次に、アクセスレベルに対して次のいずれかの制限を設定します。

   >[!IMPORTANT]
   >
   >ベンダー（組織に属さないすべてのユーザー）などの外部ユーザーの場合、タスク、プロジェクト、更新、お知らせ、その他の会社、チーム、グループへのアクセスを制限することをお勧めします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">タスクまたは問題に割り当てられた場合に、プロジェクト全体へのアクセス権限を与えない</td> 
      <td> タスクまたはタスクに割り当てられたユーザーが親プロジェクトに対する権限を取得できないようにします。親プロジェクトに対する権限を取得できるようにする権限がプロジェクト権限で許可されている場合も同様です。<p>プロジェクトに対する権限の設定について詳しくは、「 <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> 記事内 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトを編集</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">プロジェクト、タスク、問題などからドキュメントへのアクセス権限を継承しない...</td> 
      <td>ドキュメントが親オブジェクトに設定された権限を継承しないようにします。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーが含まれている会話の更新のみを表示する</td> 
      <td> ユーザーは、自分の名前やチーム名が含まれているコメントのみを表示できます。 <p> <p><b>注意</b>：ユーザーがWorkfrontの項目を購読できなくなります。 項目の購読について詳しくは、 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Adobe Workfrontの項目を購読</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">絶対にユーザーによるコメントの削除を許可しない </td> 
      <td> ユーザーが項目に対して行ったコメントを削除できないようにします。  <p><b>注意</b>：他のユーザーのコメントを削除できません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーが所属する会社、グループおよびチームのみを表示する</td> 
      <td>ユーザーが所属する会社、グループ、チームに対してのみ、項目の表示と共有を許可します。<p><strong>注意</strong>：要求者ライセンスを持つユーザーは、このオプションが選択されている場合でも、その要求者が属さない会社を表示できません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定時間数または実際の時間数の表示を許可しない</td> 
      <td>ユーザーがアクセス権を持つ作業項目の計画時間と実際の時間を表示できないようにします。 ただし、実際のログ時間、またはレポートを受ける人がログに記録した時間を確認できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">絶対にユーザーによるお知らせの削除を許可しない</td> 
      <td>お知らせセンターでのお知らせの削除を禁止します。 詳しくは、 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">お知らせの送信</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付きおよびオプション）Workfrontシステムが複数の会社に属するユーザーに対して設定されている場合、「 」セクションで属する会社に基づいて他のユーザーに対する表示を制限します **他の会社の担当者は、次のユーザーのみを表示する必要があります：**.

   ユーザーに対して、自分の会社のユーザーや、主要な会社として指定した会社のユーザーのみを表示するように制限できます。 通常、プライマリ会社は、ほとんどのユーザーが作業するWorkfrontアカウントを表します。 主な会社について詳しくは、 [会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >2 人のユーザーが異なる 2 つの会社に属しているが、両方のユーザーが主な会社のユーザーを表示できる場合、主な会社に関連付けられた「更新」領域を表示できます。

1. （オプション）作業中のアクセスレベルの他のオブジェクトや領域のアクセス設定を構成するには、 [Adobe Workfrontへのアクセスの設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)、例： [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) および [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 「**保存**」をクリックします。

   アクセスレベルを作成した後は、そのアクセスレベルをユーザーに割り当てることができます（システム管理者のアクセスレベル以外）。

   詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   システム管理者がAdobeにシステム管理者のアクセスレベルを割り当てる方法については、 [ユーザーに完全な管理アクセス権を付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## ジョブ・ロールへの管理アクセス権を持つ標準ユーザーまたはプランナ・ユーザー {#planner-users}

標準またはプランナのユーザー管理アクセス権をジョブ・ロールに付与すると、「ロールの請求と原価率の編集」設定が自動的にユーザーに対して有効になります。

後で、ユーザーのジョブロールへの管理アクセスを無効にしても、「ロールの請求とコスト率の編集」設定が有効なままなので、ジョブロールは引き続きユーザーに表示されます。

これが発生し、ジョブの役割を表示するためにユーザーのアクセス権を削除する必要がある場合は、ユーザーの役割の請求とコスト率の編集権限設定を無効にする必要があります。 手順については、 [財務データへのアクセス権の付与](grant-access-financial.md).
