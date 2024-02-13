---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザープロファイルの一括編集
description: Adobe Workfront 管理者は、ユーザーアカウントを一括で編集できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '2285'
ht-degree: 98%

---

# ユーザープロファイルの一括編集

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

ユーザーアカウントは一括で編集できます。ユーザーを一括編集する場合、特に選択したフィールドのみが更新され、選択したすべてのユーザーに同じ情報が反映されます。選択を解除したままにしたその他のフィールドは、ユーザーごとに異なる場合でも、個々のユーザーに対して同じ状態に保たれます。

>[!NOTE]
>
>* ユーザーのプロファイルの「個人情報」セクションは一括編集できません。この情報はユーザーごとに一意である必要があるからです。
>* データの正確性と最適なパフォーマンスを確保するために、一括編集では一度に 2,000 人以下のユーザーを選択することをお勧めします。
>

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

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
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。 </p> </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>この 2 つのオプションのうち、ユーザー<b>管理者（グループユーザー）</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>アクセスレベルの<b>ユーザー</b>設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーアカウントを一括編集する

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**ユーザー** ![](assets/users-icon-in-main-menu.png) をクリックします。

1. 複数のユーザーを選択して、編集アイコン ![](assets/edit-icon.png) をクリックします。

1. 表示される「**ユーザーの編集**」ボックスで、次のオプションのいずれかを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">環境設定</td> 
      <td> 
       <ul> 
        <li><b>タイムゾーン：</b>ユーザーのタイムゾーン。</li> 
        <li><b>ロケール</b>：ユーザーの優先ロケール。これは、Workfront から送信されるメールの数値や日付の形式に影響します。</li> 
        <li><b>更新ステータスの完了率を表示</b>：従来のコメント付けエクスペリエンスを使用する場合に、すべてのユーザーのタスクの更新領域内に完了率のバーを表示するには、このオプションを選択します。 詳しくは、 <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">新しいコメントエクスペリエンス</a>.</li> 
        <li><b>自分に割り当てた作業を「作業中」タブに送信</b>：ユーザーが自分に割り当てたすべてのものを、ユーザーの「作業中」タブに直接表示する場合は、このオプションを選択します。デフォルトでは、ユーザーに割り当てられたすべての項目が「作業リクエスト」タブに一覧表示されます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>新しいユーザーに対して有効にするメール通知を選択します。<p>Workfront 管理者は、システムレベルおよびグループレベルのすべてのレイアウトテンプレートを表示できます。すべての日次ダイジェスト通知は、選択したすべてのユーザーに同じ時間の後に配信されます。詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">システムの全員に対するイベント通知の設定</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクセス</td> 
      <td> 
       <ul> 
        <li><b>アクティブ：</b> このフィールドを選択して、ユーザーがアクティブかどうかを示します。アクティブなユーザーは Workfront のライセンスを使用しています。このフィールドを選択解除すると、ユーザーが非アクティブ化します。</li> 
        <li> 
        <p><b>アクセスレベル：</b>これらのユーザーに割り当てるアクセスレベルを選択します。選択したすべてのユーザーのアクセスレベルは同じになります。
        </p> 
        <p>ユーザーにアクセスレベルを割り当てる際に、自分のアクセスレベルと等しいかそれ以下のレベルを割り当てることができます。（例えば、アクセスレベルがプランナーの場合は、管理者のアクセスレベルを割り当てることはできません。） </p>
        <p>ただし、Workfront 管理者が権限を有効にしたアクセスレベルが、自分のアクセスレベルで有効になっていない場合（<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>で説明されている微調整の設定）は、自分より低いアクセスレベルを割り当てることはできません。</p> 
        <p>アクセスレベルについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront へのアクセスを設定</a>を参照してください。</p> 
         </li> 
        <li> 
        <p><b>レイアウトテンプレート</b>：ユーザー用のレイアウトテンプレートを選択します。ユーザーに割り当てられたレイアウトテンプレートは、ホームグループ、ホームチームまたはプライマリ担当業務に割り当てられたレイアウトテンプレートよりも優先されます。レイアウトテンプレートの割り当て優先度について詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>を参照してください。</p> 
        <p><b>メモ</b>：このフィールドで使用できるレイアウトテンプレートのリストは、アクセス権によって異なります。
          <ul>
           <li>Workfront 管理者は、システムレベルおよびグループレベルのすべてのレイアウトテンプレートを表示できます。</li>
           <li>グループ管理者は、システムレベルのレイアウトテンプレートと、管理するグループに関連付けられたレイアウトテンプレートを表示できます。</li>
           <li><p>プランナーライセンスを持ち、ユーザーを編集するアクセス権を持つユーザーは、システムレベルのレイアウトテンプレートのみを表示できます。 </p>
           <p>グループレベルのレイアウトテンプレートについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>を参照してください。</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織</td> 
      <td> 
       <ul> 
        <li><b>会社</b>：ユーザーの会社。ユーザーは、1 つの会社にのみ関連付けることができます。会社をユーザーに関連付ける前に、会社を作成する必要があります。アクティブな会社のみがリストに表示されます。会社の作成について詳しくは、「会社の理解と管理」を参照してください。</li> 
        <li><b>ホームチーム</b>：ユーザーのホームチームを指定します。ホームチームは 1 つのみです。 </li> 
        <li><b>その他のチーム</b>：ユーザーは複数のチームに属することができます。 </li> 
        <li> <p><b>ホームグループ：</b>適切なグループを選択して、ユーザーのホームグループとして割り当てます。これにより、ユーザーはグループと共有されているオブジェクトにアクセスできます。</p> <p><b>メモ</b>：これは必須フィールドです。ホームグループに関連付けられていないユーザーを持つことはできません。</p> <p>グループは、次の状況でのみユーザーに割り当てることができます。</p> 
         <ul> 
          <li>Workfront 管理者が割り当てる場合。</li> 
          <li>そのグループの管理者が割り当てる場合。</li> 
          <li>グループがパブリックである場合。</li> 
         </ul> </li> 
        <li> <p><b>その他のグループ</b>：ユーザーは複数のグループに属することができます。グループは、次の状況でのみユーザーに割り当てることができます。</p> 
         <ul> 
          <li>Workfront 管理者が割り当てる場合。</li> 
          <li>そのグループの管理者が割り当てる場合。</li> 
          <li> <p>グループがパブリックである場合。 </p> 
          <p>パブリックグループについて詳しくは、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">グループの作成</a>を参照してください。</p> 
          <p>グループについて詳しくは、<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>を参照してください。</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リソース計画</td> 
      <td> 
       <ul>

   <li>
       <b>作業時間</b>：ユーザーが実際の作業に使用できる（オーバーヘッドを含まない）フルタイム相当の（FTE）時間の割合を表します。「作業時間」は、1 までの小数で指定する必要があります。0 は指定できません。例えば、実際の作業可能時間が 20%の場合は 0.2 になります。

   フィールドのデフォルト値は 1 で、これはユーザーが FTE 時間全体を実際のプロジェクト関連の作業に費やすことを示します。

   この数値を使用して、プロジェクト関連の実際の作業に対するユーザーの作業可能時間が計算されます。

   Workfront でスケジュールを作成する方法について詳しくは、<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>を参照してください。

   スケジュールの例外と休暇も、ユーザーのキャパシティに影響を与える可能性があります。

   Workfront では、設定エリアのリソース管理環境設定に応じて、ユーザーの空き時間を計算します。詳しくは、<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>を参照してください。

   <b>説明</b>

   「作業時間」の値を 1 に設定すると、プロジェクト関連の作業でユーザーがフルタイム相当の時間をすべて使用できることを示します。
   </li>

   <li><b>アクティブ化解除をスケジュール</b>：一定期間後にユーザーのアクティブ化解除をスケジュールする場合は、このチェックボックスをオンにします。</li> 
       <li><b>スケジュール済みアクティブ化解除日</b>：この日を過ぎると、ユーザーのアクティブ化は解除されます。ユーザーのアクティブ化解除のスケジュールについて詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーを非アクティブ化または再アクティブ化する</a>の<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">ユーザーの非アクティブ化をスケジュール</a>を参照してください。</li> 
       <li> <p><b>主要役割</b>：Workfront でのユーザーのプライマリ担当業務。ユーザーが割り当てられているタスクとイシューは、デフォルトでこの担当業務にも割り当てられます。リソース管理には、担当業務が不可欠です。担当業務について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> <p>このフィールドは、管理者ユーザーアクセス権があるプランライセンスのユーザー、または Workfront 管理者のみが更新できます。管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
       <li>（条件付き）「<b>主要役割</b>」を選択すると、「<b>FTE の可用性の割合</b>」フィールドが表示されます。この担当業務に割り当てるユーザーのスケジュールの時間の割合を指定します。主要役割における FTEの可用性の割合のデフォルト値は 100%です。</li> 
       <li> <p><b>その他の役割</b>：ユーザーは Workfront で複数の担当業務を持つことができます。リソース管理には、担当業務が不可欠です。ユーザーが実行できる担当業務の数に制限はありません。ただし、リソース管理が複雑になりすぎる可能性があるため、1 人のユーザーにあまり多くの担当業務を割り当てないことをお勧めします。</p> <p>担当業務について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> <p>このフィールドは、管理者ユーザーアクセス権があるプランライセンスのユーザー、または Workfront 管理者のみが更新できます。管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
       <li> <p>（条件付き）1 つ以上の「<b>その他の役割</b>」を選択すると、各役割で「<b>FTE の可用性の割合</b>」フィールドが表示されます。それぞれの担当業務に割り当てるユーザーのスケジュールの時間の割合を指定します。その他の役割における FTE の可用性の割合のデフォルト値は 0%です。</p> <p><b>メモ</b>:  
       <ul> 
       <li>その他の役割の FTE 可用性が 0%の場合、ユーザーがこれらのロールのタスクに割り当てられていない限り、リソースプランナーには表示されません。</li> 
       <li> <p>すべての役割における FTE の可用性の全割合の合計は 100%にする必要があります。FTE の可用性の各割合では、リソースプランナーの各ユーザーの役割における空き時間が計算されます。ユーザーごとの各役割の空き時間は、それぞれのユーザーの空き時間に左右されます。</p> <p>ユーザーの空き時間は、Workfront 管理者がリソース管理環境設定で FTE を計算する際に選択した方法に応じて、Workfront によって計算されます。</p> <p>ユーザーの空き時間の計算の詳細については、<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナーのユーザーと役割に対する時間と FTE の計算の概要</a>を参照してください。</p> <p>リソース管理環の境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理の環境設定の指定</a>を参照してください。</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>スケジュール</b>：スケジュールをユーザーに関連付けます。ユーザーのスケジュールによって、割り当てられているタスクのタイムラインが計算されます。</p> <p>Workfront 管理者またはグループ管理者は、スケジュールを作成してからユーザーに関連付ける必要があります。</p> <p>選択したユーザーに割り当てるシステムレベルまたはグループスケジュールを選択します。</p> <p>システムレベルおよびグループスケジュールの詳細については、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールの作成</a>を参照してください。</p> <p><b>重要</b>：Workfront でユーザーのスケジュールが使用されるのは、「リソースの空き時間計算に次を使用:」設定が「ユーザーのスケジュール」に設定されている場合のみです。「リソースの空き時間計算に次を使用:」設定が、リソース管理に使用されるスケジュールに与える影響の詳細については、「<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理環境設定の指定</a>」を参照してください。</p> </li> 
       <li> <p><b>タイムシートプロファイル</b>：タイムシートプロファイルはユーザーに関連付けます。これにより、ユーザーに対してタイムシートが自動的に生成されるようになります。</p> 
       <p><b>メモ</b>:  
       <ul> 
       <li>このフィールドで使用できるタイムシートプロファイルは、アクセス権によって異なります。
       <ul>
       <li>Workfront 管理者は、すべてのシステムレベルおよびグループレベルのタイムシートプロファイルを確認できます。</li>
       <li><p>グループ管理者は、システムレベルのタイムシートプロファイルと、自分が管理するグループに関連付けられたタイムシートプロファイルを確認できます。</p></li>
       <li><p>プランナーのライセンスでユーザーを編集する権限を持つユーザーは、システムレベルのタイムシートプロファイルのみを表示できます。</p></li>
       </ul></li> 
       <li>グループ管理者の場合、編集するすべてのユーザーは、自分が管理しているグループのメンバーである必要があります。</li> 
       </ul> </p> </li> 
       <li><b>デフォルトの時間タイプ</b>：ユーザーのデフォルトの時間タイプを選択します。これは、ユーザーが時間をログに記録する際にデフォルトで使用される時間タイプです。</li> 
       <li> <p><b>利用可能な時間タイプ</b>：ユーザーが使用できる時間タイプを選択します。これらの時間タイプは、Workfront でユーザーが時間をログに記録できる場所に表示されます。ユーザーは、プロジェクトレベルおよびユーザーレベルで有効になっている時間タイプのみを表示できます。</p> 
       <p>ユーザーが使用できる時間タイプについて詳しくは、<a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">タイムシートの時間タイプと空き時間の定義</a>を参照してください。</p> 
       </li> 
       <li> <b>FTE</b>：これは、フルタイムでのユーザーと同じです。Workfront ではこの数値を使用して、システムレベルの「リソース管理環境設定」が「規定のスケジュール」に設定されている場合にのみ、規定のスケジュールに基づいてユーザーの空き時間が計算されます。

   <p>FTE は、ユーザーが作業に費やせる時間を示します。これには、オーバーヘッドや、プロジェクト作業に費やされた時間が含まれます。例えば、ミーティングやトレーニングに費やした時間も FTE に含まれます。</p>

   FTE は 1 以下の小数にする必要があり、0 にはできません。例えば、FTE 値が 0.5 で、Workfront のデフォルトのスケジュールが 40 時間の場合、そのユーザーは週に 20 時間空いています。

   このフィールドのデフォルトは 1 です。

   スケジュールの例外、休暇および作業時間の値は、ユーザーの空き時間に影響を与える場合があります。

   Workfront では、設定エリアのリソース管理環境設定に応じて、ユーザーの空き時間を計算します。

   システムレベルのリソース管理環境設定がユーザーのスケジュールに設定されている場合、ここで指定した値は無視され、ユーザーはスケジュールで指定された内容に従って空いていると見なされます。

   詳しくは、<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理の環境設定</a>を参照してください。

   Workfront でのスケジュールの作成について詳しくは、<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールを作成</a>を参照してください。
   </li> 
       <li> <p><b>リソースプール</b>：ユーザーをリソースプールに関連付けます。</p> <p><b>メモ</b>：選択したすべてのユーザーに共通のリソースプールのみがこのフィールドに表示されます。選択したユーザーに共有のリソースプールがない場合、このフィールドは空になります。このフィールドが空の場合、ここで指定したリソースプールは、個々のリソースプールを上書きします。</p> 
       <p>リソースプールについて詳しくは、<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">リソースプールの概要</a>を参照してください。</p> </li> 
       <li><b>1 時間当たりのコスト</b>：ユーザーの 1 時間当たりのコストの額です。 </li> 
       <li><b>1 時間当たりの請求</b>：ユーザーの 1 時間当たりの請求額です。</li> 
       <li><b>カスタムフォーム</b>：既存のユーザーカスタムフォームをユーザーに関連付けます。カスタムフォームをユーザーに関連付けるには、カスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。カスタムフォームの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームを作成または編集</a>を参照してください。</li> 
       <li><b>コメント</b>：提供されたフィールドにコメントを入力します。選択したすべてのユーザーに、アプリ内通知と、コメントが記載されたメール通知が送信されます。コメントは、ユーザーのプロファイルの「アップデート」タブに表示されます。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「**カスタムフォーム**」セクションで、「**カスタム式を再計算**」オプションを選択して、選択したユーザーに添付されるカスタムフォーム内のすべての計算済みカスタムフィールドを最新の状態に保ちます。

1. 「**変更を保存**」をクリックします。
