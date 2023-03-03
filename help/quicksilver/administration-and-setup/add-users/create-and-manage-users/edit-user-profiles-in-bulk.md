---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザープロファイルの一括編集
description: Adobe Workfront管理者は、ユーザーアカウントを一括で編集できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '2363'
ht-degree: 0%

---

# ユーザープロファイルの一括編集

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdmin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、Adobe Admin Consoleを通じてこの操作を実行する必要があります。
>
>Adobe Admin Consoleでユーザーのプロファイルを編集する手順については、この記事の「ユーザーの詳細を編集する」の節を参照してください [ユーザーの一括アップロード](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) または、Adobe Admin Console管理者に問い合わせてください。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

ユーザーアカウントは一括で編集できます。 ユーザーを一括編集する場合、特に選択したフィールドのみが更新され、選択したすべてのユーザーに同じ情報が反映されます。 選択を解除したままにしたその他のフィールドは、ユーザーごとに異なる場合でも、個々のユーザーに対して同じ状態に保たれます。

>[!NOTE]
>
>* ユーザーのプロファイルの「個人情報」セクションは一括編集できません。この情報はユーザーごとに一意である必要があるからです。
>* データの正確性と最適なパフォーマンスを確保するために、一括編集では一度に 2,000 人以下のユーザーを選択することをお勧めします。
>


## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

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
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> </li> 
     <li> <p><b>ユーザー</b> 設定を <b>編集</b> アクセス、 <b>作成</b> そして少なくとも 2 つのうち 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>この 2 つのオプションのうち、ユーザー <b>管理者（グループユーザー）</b> が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>詳しくは、 <b>ユーザー</b> アクセスレベルでの設定については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## ユーザーアカウントの一括編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png).

1. 複数のユーザーを選択して、編集アイコンをクリックします。 ![](assets/edit-icon.png).

1. 内 **ユーザーを編集** 表示されるボックスで、次のいずれかのオプションを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">環境設定</td> 
      <td> 
       <ul> 
        <li><b>タイムゾーン：</b> ユーザーのタイムゾーン。</li> 
        <li><b>ロケール</b>:ユーザーの優先ロケール。 これは、Workfrontから送信される E メールの数値および日付の形式に影響します。</li> 
        <li><b>更新ステータスの完了率を表示</b>:すべてのユーザーのタスクの更新ストリーム内に完了率のバーを表示する場合は、このオプションを選択します。</li> 
        <li><b>自分に割り当てた作業を [ 作業 ] タブに送信する</b>:ユーザーが自分に割り当てたすべてのものを、ユーザーの [ 作業 ] タブに直接表示する場合は、このオプションを選択します。 デフォルトでは、ユーザーに割り当てられたすべての項目が「作業リクエスト」タブにリストされます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>新しいユーザーに対して有効にする電子メール通知を選択します。<p>インスタント通知と、毎日のダイジェスト通知を選択できます。 選択したすべてのユーザーに対して、毎日のダイジェスト通知が同じ時間後にすべて配信されます。 詳しくは、 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">システムの全員に対するイベント通知を設定する</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクセス</td> 
      <td> 
       <ul> 
        <li><b>アクティブ：</b> このフィールドを選択して、ユーザーがアクティブかどうかを示します。 アクティブなユーザーはWorkfrontのライセンスを使用しています。 このフィールドを選択解除すると、ユーザーがアクティベート解除されます。</li> 
        <li> 
        <p><b>アクセスレベル：</b> これらのユーザーに割り当てるアクセスレベルを選択します。 選択したすべてのユーザーのアクセスレベルは同じになります。
        </p> 
        <p>ユーザーにアクセスレベルを割り当てる際に、自分のアクセスレベルと等しいかそれ以下のレベルを割り当てることができます。 （たとえば、アクセス・レベルが「プランナ」の場合は、管理者アクセス・レベルを割り当てることはできません）。 </p>
        <p>ただし、Workfront管理者が自分でも有効になっていないアクセスレベルに対する権限を自分で有効にしている場合は、自分より低いアクセスレベルを割り当てることはできません ( <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>) をクリックします。</p> 
        <p>アクセスレベルの詳細については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfrontへのアクセスの設定</a>.</p> 
         </li> 
        <li> 
        <p><b>レイアウトテンプレート</b>:ユーザー用のレイアウトテンプレートを選択します。 ユーザーに割り当てられたレイアウトテンプレートは、ホームグループ、ホームチーム、または主要な職務の役割に割り当てられたレイアウトテンプレートよりも優先されます。 レイアウトテンプレートの割り当て優先度の詳細については、 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>.</p> 
        <p><b>注意</b>:このフィールドで使用できるレイアウトテンプレートのリストは、アクセス権によって異なります。
          <ul>
           <li>Workfront管理者は、すべてのシステムレベルおよびグループレベルのレイアウトテンプレートを表示できます。</li>
           <li>グループ管理者は、システムレベルのレイアウトテンプレートと、管理するグループに関連付けられたレイアウトテンプレートを表示できます。</li>
           <li><p>Planner ライセンスを持ち、ユーザーを編集するアクセス権を持つユーザーは、システムレベルのレイアウトテンプレートのみを表示できます。 </p>
           <p>グループレベルのレイアウトテンプレートについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織</td> 
      <td> 
       <ul> 
        <li><b>会社</b>:ユーザーの会社。 ユーザーは、1 つの会社にのみ関連付けることができます。 会社をユーザーに関連付ける前に、会社を作成する必要があります。 アクティブな会社のみがリストに表示されます。 会社の作成に関する詳細は、「会社の理解と管理」を参照してください。</li> 
        <li><b>ホームチーム</b>:ユーザーのホームチームを指定します。 ホームチームは 1 つだけです。 </li> 
        <li><b>その他のチーム</b>:ユーザーは複数のチームに属することができます。 </li> 
        <li> <p><b>ホームグループ：</b> 適切なグループを選択して、ユーザーをホームグループに割り当てます。 これにより、ユーザーはグループと共有されているオブジェクトにアクセスできます。</p> <p><b>注意</b>:これは必須フィールドです。 ユーザをホームグループに関連付けることはできません。</p> <p>グループは次の状況でのみユーザーに割り当てることができます。</p> 
         <ul> 
          <li>Workfront管理者です。</li> 
          <li>あなたはそのグループの管理者です。</li> 
          <li>グループは公開されています。</li> 
         </ul> </li> 
        <li> <p><b>その他のグループ</b>:ユーザーは複数のグループに属することができます。 グループは、次の状況でのみユーザーに割り当てることができます。</p> 
         <ul> 
          <li>Workfront管理者です。</li> 
          <li>あなたはそのグループの管理者です。</li> 
          <li> <p>グループは公開されています。 </p> 
          <p>パブリックグループについて詳しくは、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">グループの作成</a>.</p> 
          <p>グループについて詳しくは、 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>.</p> 
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
       <b>作業時間</b>:ユーザーが実際の作業に使用できるフルタイム相当 (FTE) 時間の割合を表します（オーバーヘッドは含まれません）。 [ 作業時間 ] には 1 までの 10 進数を指定する必要があります。0 は指定できません。 例えば、実際の作業時間の 20%の可用性は 0.2 となります。

   フィールドのデフォルト値は 1 で、ユーザーが FTE 全体を実際のプロジェクト関連の作業に費やすことを示します。

   この数値を使用して、プロジェクト関連の実際の作業に対するユーザーの可用性が計算されます。

   Workfrontでスケジュールを作成する方法について詳しくは、 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>.

   スケジュールの例外とタイムオフも、ユーザーの容量に影響を与える可能性があります。

   Workfrontは、セットアップ領域のリソース管理環境設定に基づいて、ユーザーの可用性を計算します。 詳しくは、 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>.

   <b>ヒント</b>

   [ 作業時間 ] の値を 1 に設定して、プロジェクト関連の作業でユーザーがフルタイムの同等の作業全体で使用できるようにします。
   </li>

   <li><b>無効化をスケジュール</b>:一定期間後にユーザーの非アクティブ化をスケジュールする場合は、このチェックボックスをオンにします。</li> 
       <li><b>予定されている非アクティブ化日</b>:ユーザーが非アクティブ化された日付。 非アクティブ化のためのユーザーのスケジュール設定について詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">ユーザーのアクティベーション解除をスケジュール</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーを非アクティブ化または再アクティブ化する</a>.</li> 
       <li> <p><b>プライマリの役割</b>:これは、Workfrontでユーザーが持つ主な役割です。 ユーザーが割り当てられているタスクとタスクも、デフォルトでこのジョブの役割に割り当てられます。 リソース管理には、ジョブの役割が不可欠です。 ジョブの役割について詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">ジョブの役割の作成と管理</a></p> <p>このフィールドは、管理者ユーザーアクセス権を持つプランライセンスを持っている場合、またはWorkfront管理者である場合にのみ更新できます。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
       <li>（条件付き） <b>プライマリの役割</b>、 <b>FTE の可用性の割合</b> フィールドが表示されます。 このジョブの役割に割り当てるユーザーのスケジュールの時間の割合を指定します。 [プライマリロールの FTE 可用性の割合 ] のデフォルト値は 100%です。</li> 
       <li> <p><b>その他の役割</b>:Workfrontでは複数のジョブの役割を持つことができます。 リソース管理には、ジョブの役割が不可欠です。 ユーザーが実行できるジョブの役割の数に制限はありません。 ただし、リソース管理が複雑すぎる場合があるので、1 人のユーザーを多数のジョブの役割に割り当てすぎないようにすることをお勧めします。</p> <p>ジョブの役割について詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">ジョブの役割の作成と管理</a>.</p> <p>このフィールドは、管理者ユーザーアクセス権を持つプランライセンスを持っている場合、またはWorkfront管理者である場合にのみ更新できます。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
       <li> <p>（条件付き）1 つまたは複数の <b>その他の役割</b>、 <b>FTE の可用性の割合</b> 各役割に対して表示されるフィールド 各ジョブの役割に割り当てるユーザーのスケジュールの時間の割合を指定します。 その他のロールの FTE 可用性の割合のデフォルト値は 0%です。</p> <p><b>メモ</b>:  
       <ul> 
       <li>「その他のロール」に 0%の FTE 可用性がある場合は、ユーザーがこれらのロールのタスクに割り当てられていない限り、リソース・プランナには表示されません。</li> 
       <li> <p>すべてのロールの FTE 可用性の全パーセンテージの合計は 100%にする必要があります。 FTE 可用性の各割合は、リソース・プランナの各ユーザーのロールの使用可能時間を計算します。 各役割の使用可能時間は、ユーザーの使用可能時間によって異なります。</p> <p>ユーザーの使用可能な時間は、Workfront管理者がリソース管理環境設定で FTE を計算する際に選択した方法に応じて、Workfrontが計算します。</p> <p>ユーザーの可用性の計算の詳細については、 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソース・プランナのユーザーとロールの時間と工数の計算の概要</a>.</p> <p>リソース管理環境設定の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理環境設定の指定</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>スケジュール</b>:スケジュールをユーザーに関連付けます。 ユーザーのスケジュールは、ユーザーが割り当てられているタスクのタイムラインを計算します。</p> <p>Workfront管理者またはグループ管理者は、スケジュールを作成してから、ユーザーに関連付ける必要があります。</p> <p>選択したユーザーに割り当てるシステムレベルまたはグループスケジュールを選択します。</p> <p>システムレベルおよびグループスケジュールの詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールの作成</a>.</p> <p><b>重要</b>:Workfrontは、[ 次の使用方法でリソースの可用性を計算する ] 設定が [ ユーザーのスケジュール ] に設定されている場合にのみ、ユーザーのスケジュールを使用します。 [ 次を使用してリソースの可用性を計算する ] 設定が、リソース管理に使用するスケジュールに与える影響の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理環境設定の指定</a>.</p> </li> 
       <li> <p><b>タイムシートプロファイル</b>:タイムシートプロファイルをユーザーに関連付けます。 これにより、ユーザーに対してタイムシートが自動的に生成されます。</p> 
       <p><b>メモ</b>:  
       <ul> 
       <li>このフィールドで使用可能なタイムシートプロファイルの一覧は、アクセス権によって異なります。
       <ul>
       <li>Workfrontの管理者は、すべてのシステムレベルおよびグループレベルのタイムシートプロファイルを確認できます。</li>
       <li><p>グループ管理者は、システムレベルのタイムシートプロファイルと、管理するグループに関連付けられたプロファイルを確認できます。</p></li>
       <li><p>プランナーのライセンスを持ち、ユーザーを編集するアクセス権を持つユーザーは、システムレベルのタイムシートプロファイルのみを表示できます。</p></li>
       </ul></li> 
       <li>グループ管理者の場合、編集中のすべてのユーザは、管理しているグループのメンバである必要があります。</li> 
       </ul> </p> </li> 
       <li><b>デフォルトの時間タイプ</b>:ユーザーのデフォルトの時間タイプを選択します。 これは、ユーザーが時刻をログに記録する際にデフォルトで使用される時間タイプです。</li> 
       <li> <p><b>利用可能な時間タイプ</b>:ユーザーが使用できる時間タイプを選択します。 これらの時間タイプは、Workfrontのどこでもユーザーが時間をログに記録できる場所に表示されます。 ユーザーは、プロジェクトレベルおよびユーザーレベルで有効になっている時間タイプのみを表示できます。</p> 
       <p>ユーザーが使用できる時間のタイプについて詳しくは、 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">タイムシートの時間の種類と可用性を定義する</a>.</p> 
       </li> 
       <li> <b>FTE</b>:これは、ユーザーと同等のフルタイムです。 Workfrontは、この数値を使用して、システム・レベルの「生産資源管理プリファレンス」が「デフォルト・スケジュール」に設定されている場合にのみ、デフォルト・スケジュールに基づいてユーザーの可用性を計算します。

   <p>FTE は、ユーザーが仕事に費やす時間を示します。 これには、オーバーヘッドや、プロジェクト作業に費やされた時間が含まれます。 例えば、ミーティングやトレーニングに費やした時間も FTE に含まれます。</p>

   FTE は 1 までの 10 進数で、0 にはできません。 例えば、FTE 値が 0.5 で、Workfrontのデフォルトのスケジュールが 40 時間の場合、ユーザーは週に 20 時間使用できます。

   フィールドのデフォルトは 1 です。

   スケジュールの例外、タイムオフ、および作業時間の値は、ユーザーの可用性に影響を与える場合があります。

   Workfrontは、セットアップ領域のリソース管理環境設定に基づいて、ユーザーの可用性を計算します。

   システム・レベルの「生産資源管理プリファレンス」が「ユーザーのスケジュール」に設定されている場合、ここで指定した値は無視され、ユーザーはスケジュールで指定された内容に従って使用可能と見なされます。

   詳しくは、 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>.

   Workfrontでスケジュールを作成する方法について詳しくは、 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>.
   </li> 
       <li> <p><b>リソースプール</b>:ユーザーをリソースプールに関連付けます。</p> <p><b>注意</b>:このフィールドには、選択したすべてのユーザーに共通するリソースプールのみが表示されます。 選択したユーザーに共有リソースプールがない場合、このフィールドは空になります。 このフィールドが空の場合、ここで指定したリソースプールは、個々のリソースプールを上書きします。</p> 
       <p>リソースプールの詳細については、 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> リソースプールの概要 </a>.</p> </li> 
       <li><b>時間あたりのコスト</b>:ユーザーの 1 時間あたりのコストの量。 </li> 
       <li><b>1 時間あたりの請求</b>:ユーザーの 1 時間あたりの請求額。</li> 
       <li><b>カスタムForms</b>:既存のユーザーカスタムフォームをユーザーに関連付けます。 カスタムフォームをユーザーに関連付ける前に、カスタムフォームを作成する必要があります。 リストには、アクティブなカスタムフォームのみが表示されます。 カスタムフォームの作成について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>.</li> 
       <li><b>コメント</b>:提供されたフィールドにコメントを入力します。 選択したすべてのユーザーに、アプリ内通知と、コメントが記載された電子メール通知が送信されます。 コメントは、ユーザーのプロファイルの「更新」タブに表示されます。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション） **カスタムForms** セクションで、 **カスタム式の再計算** オプションを使用して、選択したユーザーに添付されるカスタムフォーム内のすべての計算済みカスタムフィールドを最新の状態に保ちます。

1. クリック **変更を保存**.
