---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザープロファイルの一括編集
description: Adobe Workfront 管理者は、ユーザーアカウントを一括で編集できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '2587'
ht-degree: 64%

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

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これら 2 つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーアカウントを一括編集する

{{step-1-to-users}}

1. 複数のユーザーを選択し、「**編集**」アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

1. 「**ユーザーを編集**」ボックスで、任意のセクションの情報を変更し、いつでも **保存** をクリックします。

### 環境設定

* **タイムゾーン**: ユーザーのタイムゾーン。

  ユーザーが Workfront でタイムゾーンをまたいで共同作業できるようにスケジュールを使用する方法について詳しくは、[タイムゾーンをまたいだ作業](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)を参照してください。

* **メールのロケール**：ユーザーが希望するメールのロケール。これは、Workfront からこのユーザーに送信されるメール内の数値と日付の形式に影響します。

  >[!NOTE]
  >
  >組織がAdobe統合エクスペリエンスを使用している場合、ユーザーの言語環境設定はAdobe プロファイルに保存され、メールのロケールは使用されません。 これらの環境設定へのアクセスについて詳しくは、[Adobe Workfront統合エクスペリエンス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md) を参照してください。

### 通知

ユーザーに対して有効にする必要があるメール通知を選択します。

Workfront 管理者は、システムレベルおよびグループレベルのすべてのレイアウトテンプレートを表示できます。すべての 1 日のダイジェスト通知は、選択したすべてのユーザーに対して同じ時間の後に配信されます。

詳しくは、[システムの全員に対するイベント通知の設定](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

### アクセス

* **ユーザーがアクティブ**：ユーザーがアクティブであることを示すには、このオプションを有効にします。 アクティブなユーザーは Workfront のライセンスを使用しています。このフィールドを無効にすると、ユーザーはアクティベート解除され、Workfrontにログインできなくなります。

* **アクセスレベル**：これらのユーザーに割り当てるアクセスレベルを選択します。 選択したすべてのユーザーが同じアクセスレベルになります。

  ユーザーにアクセスレベルを割り当てる場合、独自のアクセスレベル以下のレベルを割り当てることができます。 （例えば、アクセスレベルが「標準」の場合、管理者のアクセスレベルを割り当てることはできません。）

  ただし、Workfront 管理者がデフォルト以外の権限を有効にしたアクセスレベルが、自分のアクセスレベルで有効になっていない場合は、自分のアクセスレベルよりデフォルトで下位のアクセスレベルを割り当てることはできません。

  たとえば、タスクを削除するアクセス権のない標準ライセンスがある場合、Light ライセンスは標準ライセンスより低いものの、削除するアクセス権のある Light ライセンスを割り当てることはできません。 詳しくは、[カスタムアクセスレベルの作成または変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

  アクセスレベルについて詳しくは、[Adobe Workfront へのアクセスの設定](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md)を参照してください。

  >[!NOTE]
  >
  >組織で新しいアクセスモデル（標準／ライト／コントリビューター）を使用している場合、そのユーザーが月の決定制限に達している場合、標準またはライトユーザーをコントリビューターアクセスレベルに再割り当てすることはできません。
  >
  >新しいアクセスモデルについて詳しくは、[新しいアクセスレベルの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)を参照してください。
  >
  >決定制限について詳しくは、[無償ユーザーに対する限定的なドキュメントおよびプルーフの決定の概要](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)を参照してください。

* **レイアウトテンプレート**：ユーザー用のレイアウトテンプレートを選択します。このレイアウトテンプレートは、ホームグループ、ホームチームまたはプライマリロールに割り当てられたレイアウトテンプレートよりも優先されます。 レイアウトテンプレートの割り当て優先度の詳細については、「[ レイアウトテンプレートの作成と管理 ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) を参照してください。

  このフィールドで使用できるテンプレートのリストがアクセス権によってどう異なるかを次のリストで示します。

   * Workfront 管理者は、システムレベルおよびグループレベルのすべてのレイアウトテンプレートを表示できます。
   * グループ管理者は、システムレベルのレイアウトテンプレートと、管理するグループに関連付けられているレイアウトテンプレートを表示できます。
   * 標準またはプランのライセンスを持ち、ユーザーを編集するためのアクセス権を持つユーザーには、システムレベルのレイアウトテンプレートのみが表示されます。

     グループレベルのレイアウトテンプレートの詳細については、[ グループのレイアウトテンプレートの作成と変更 ](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md) を参照してください。

### 組織

* **会社**：ユーザーの会社。ユーザーは、1 つの会社にのみ関連付けることができます。会社をユーザーに関連付ける前に、会社を作成する必要があります。アクティブな会社のみがリストに表示されます。会社の作成について詳しくは、[会社の作成と編集](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。
* **ホームチーム**：ユーザーのホームチームを指定します。ホームチームは 1 つのみです。
* **その他のチーム**：ユーザーは複数のチームに属することができます。
* **現在のホームグループ**：ユーザーを割り当てる適切なグループを選択します。 これにより、ユーザーは、グループと共有されているオブジェクトにアクセスできるようになります。 また、レイアウトテンプレートをホームグループと共有することもできます。

  必須フィールドです。すべてのユーザーは、ホームグループに関連付ける必要があります。選択しない場合、ホームグループがホームグループとして割り当てられます。

  次のいずれかに該当する場合にのみ、ユーザーにグループを割り当てることができます。

   * Workfront 管理者である
   * グループの管理者である
   * グループはパブリックです

* **その他のグループ**：ユーザーは複数のグループに属することができます。ユーザーにグループを割り当てることができるのは、Workfront管理者、グループの管理者、またはグループが公開されている場合のみです。

  >[!IMPORTANT]
  >
  >ユーザーを 100 を超えるグループに追加すると、グループのリストを読み込む Workfront のエリアで、パフォーマンスの問題が発生する場合があります。

  公開グループについて詳しくは、[グループの作成](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)を参照してください。

  グループについて詳しくは、[グループの概要](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md)を参照してください。

### リソース計画

* **作業時間**：オーバーヘッドを含まない、ユーザーが実際の作業に使用できるフルタイム相当（FTE）時間の割合を表します。 「作業時間」は、1 までの小数で指定する必要があります。0 は指定できません。例えば、実際の作業可能時間が 20%の場合は 0.2 になります。

  フィールドのデフォルト値は 1 で、これはユーザーが FTE 時間全体を実際のプロジェクト関連の作業に費やすことを示します。

  この数値を使用して、プロジェクト関連の実際の作業に対するユーザーの作業可能時間が計算されます。

  Workfront でスケジュールを作成する方法について詳しくは、[スケジュールの作成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

  スケジュール例外と休暇も、ユーザーのキャパシティに影響を与える可能性があります。

  Workfront では、設定エリアのリソース管理環境設定に応じて、ユーザーの空き時間を計算します。詳しくは、[リソース管理環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

  >[!TIP]
  >
  >「作業時間」の値を 1 に設定すると、ユーザーがフルタイム当量の時間をプロジェクト関連の作業に使用できることを示します。

* **アクティベート解除日を設定**：これらのユーザーを特定の日付に、特定の時間にアクティベート解除するようにスケジュールする場合は、このボタンをクリックします。
* **アクティベート解除日**: ユーザーがアクティベート解除された日時。 ユーザーを非アクティブ化するスケジュールについて詳しくは、[ ユーザーの非アクティブ化または再アクティブ化 ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) の「[ 非アクティブ化するユーザーのスケジュール ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)」を参照してください。
* **プライマリの役割**：これは、Workfrontでユーザーが果たすことができる主要な担当業務です。 ユーザーが割り当てられているすべてのタスクとイシューも、この担当業務に割り当てられます。 リソース管理には、担当業務が不可欠です。このフィールドを更新できるのは、管理ユーザーアクセス権を持つ標準ライセンスまたはプランライセンスがある場合、またはWorkfront管理者の場合のみです。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、[ユーザーへのアクセス権の付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

  リストには、アクティブな担当業務のみが表示されます。

* （条件付き）「**主要役割**」を選択すると、「**FTE の可用性の割合**」フィールドが表示されます。この担当業務に割り当てるユーザーのスケジュールの時間の割合を指定します。主要役割における FTEの可用性の割合のデフォルト値は 100%です。
* **その他の役割**：ユーザーは Workfront で複数の担当業務を持つことができます。リソース管理には、担当業務が不可欠です。ユーザーが実行できる担当業務の数に制限はありません。ただし、リソース管理が複雑になりすぎる可能性があるため、1 人のユーザーにあまり多くの担当業務を割り当てないことをお勧めします。

  リストには、アクティブな担当業務のみが表示されます。担当業務について詳しくは、[担当業務の作成と管理](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

  このフィールドを更新できるのは、管理ユーザーアクセス権を持つ標準ライセンスまたはプランライセンスがある場合、またはWorkfront管理者の場合のみです。

  管理ユーザーアクセス権を持つユーザーの設定について詳しくは、[ユーザーへのアクセス権の付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

* （条件付き）1 つ以上の「**その他の役割**」を選択すると、各役割で「**FTE の可用性の割合**」フィールドが表示されます。それぞれの担当業務に割り当てるユーザーのスケジュールの時間の割合を指定します。その他の役割における FTE の可用性の割合のデフォルト値は 0%です。

  その他の役割の FTE 可用性が 0%の場合、ユーザーがこれらのロールのタスクに割り当てられていない限り、リソースプランナーには表示されません。

  すべての役割における **FTE の空き時間の割合**&#x200B;の合計を 100％にする必要があります。FTE の可用性の各割合では、リソースプランナーの各ユーザーの役割における空き時間が計算されます。ユーザーごとの各役割の空き時間は、それぞれのユーザーの空き時間に左右されます。

  ユーザーの空き時間は、Workfront 管理者がリソース管理環境設定で FTE を計算する際に選択した方法に応じて、Workfront によって計算されます。

  ユーザーの空き時間の計算について詳しくは、[リソースプランナーのユーザーと役割に対する時間と FTE の計算の概要](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)を参照してください。

  リソース管理の環境設定の指定について詳しくは、[リソース管理の環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

* **スケジュール**：スケジュールをユーザーに関連付けます。ユーザーのスケジュールによって、割り当てられているタスクのタイムラインが計算されます。

  スケジュールをユーザーに関連付けるには、スケジュールを作成する必要があります。 スケジュールの作成について詳しくは、[スケジュールを作成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

  >[!IMPORTANT]
  >
  >Workfrontは、「**次を使用してリソースの空き時間を計算** 設定が **ユーザーのスケジュール** に設定されている場合にのみ、ユーザーのスケジュールを使用します。 この設定がリソース管理に使用されるスケジュールにどのように影響するかについては、[ リソース管理環境設定の構成 ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) を参照してください。

* **タイムシートプロファイル**：タイムシートプロファイルをユーザーに関連付けて、タイムシートが自動的に生成されるようにします。

  このフィールドに入力できるプロファイルのリストは、アクセス権によって異なります。

   * Workfront 管理者は、すべてのシステムレベルおよびすべてのグループレベルのタイムシートプロファイルを表示することができます。
   * グループ管理者は、システムレベルのタイムシートプロファイルと、自分が管理するグループに関連付けられたタイムシートプロファイルを確認できます。
   * 標準またはプラン ライセンスを持ち、ユーザーを編集するアクセス権を持つユーザーには、システムレベルのタイムシートプロファイルのみが表示されます。 グループレベルのタイムシートプロファイルについて詳しくは、[タイムシートプロファイルの作成、編集、割り当て](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

* **デフォルトの時間タイプ**：ユーザーのデフォルトの時間タイプを選択します。これは、ユーザーが時間をログに記録する際にデフォルトで使用される時間タイプです。
* **利用可能な時間タイプ**：ユーザーが使用できる時間タイプを選択します。 これらの時間タイプは、Workfront でユーザーが時間をログに記録できる場所に表示されます。ユーザーは、プロジェクトレベルおよびユーザーレベルで有効になっている時間タイプのみを表示できます。 ユーザーが使用できる時間タイプについて詳しくは、[ 時間タイプと空き時間を定義 ](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) を参照してください。
* **FTE**：これは、のユーザーに相当するフルタイムのリソースです。 Workfrontでは、この数値を使用して、システムレベルの「リソース管理の環境設定」が「デフォルトのスケジュール」に設定されている場合にのみ、デフォルトのスケジュールに基づいたユーザーの空き時間が計算されます。

  FTE は、ユーザーが仕事に費やすことができる時間を示します。 これには、オーバーヘッドや、プロジェクト作業に費やされた時間が含まれます。例えば、ミーティングやトレーニングに費やした時間も FTE に含まれます。

  FTE は 1 以下の小数にする必要があり、0 にはできません。例えば、FTE 値が 0.5 で、Workfrontのデフォルトスケジュールが 40 時間の場合、ユーザーは週に 20 時間利用できます。

  このフィールドのデフォルトは 1 です。

  スケジュール例外、休暇、および作業時間の値は、ユーザーの空き時間に影響を与える可能性があります。

  Workfront では、設定エリアのリソース管理環境設定に応じて、ユーザーの空き時間を計算します。

  システムレベルのリソース管理環境設定がユーザーのスケジュールに設定されている場合、ここで指定した値は無視され、ユーザーはスケジュールで指定された内容に従って空いていると見なされます。

  詳しくは、[リソース管理の環境設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

  Workfront でスケジュールを作成する方法について詳しくは、[スケジュールの作成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

* **リソース プール**: ユーザーをリソース プールに関連付けます。

  >[!NOTE]
  >
  >このフィールドには、選択したすべてのユーザーに共通するリソースプールのみが表示されます。選択したユーザーに共有リソース プールがない場合、このフィールドは空になります。 このフィールドが空の場合、ここで指定したリソースプールは、個々のリソースプールを上書きします。

  リソース プールの詳細については、[ リソース プールとユーザーの関連付け ](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md) を参照してください。

* **コスト率**：ユーザーの 1 時間あたりのコストの量。

  有効日のコスト率については、「**レートを追加**」をクリックします。期間のコスト率の値を入力し、必要に応じて開始日と終了日を割り当てます。コスト率 1 には開始日が設定されず、最後のコスト率には終了日が設定されません。

  一部の日付は自動的に追加されます。例えば、コスト率 1 に終了日がなく、開始日が2023年5月1日のコスト率 2 を追加した場合、ギャップが生じないように、2023年4月30日の終了日がコスト率 1 に追加されます。

* **請求レート**：ユーザーの 1 時間あたりの請求額。

  有効日の請求レートについては、「**レートを追加**」をクリックします。期間の請求レートの値を入力し、必要に応じて開始日と終了日を割り当てます。請求レート 1 には開始日が設定されず、最後の請求レートには終了日が設定されません。

  一部の日付は自動的に追加されます。例えば、請求レート 1 に終了日がなく、開始日が 2023年5月1日の請求レート 2 を追加すると、ギャップが生じないように、請求レート 1 の終了日に 2023年4月30日が追加されます。

### カスタムフォーム

既存のユーザーカスタムフォームをユーザーに関連付けます。 カスタムフォームをユーザーに関連付けるには、カスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。編集するアクセス権がないフィールドは、個々のカスタムフォームには表示されません。

>[!NOTE]
>
>外部検索フィールドやWorkfront ネイティブフィールドなどの高度なカスタムフォーム機能は、ユーザーを編集ダイアログではなく、詳細ページでユーザーレコードを開いた場合にのみ使用できます。 （ユーザーのリストで、ユーザー名をクリックすると詳細が開きます）。

必要に応じて、「**カスタム式を再計算**」オプションを選択して、選択したユーザーに添付されたカスタムフォームの計算カスタムフィールドがすべて最新であることを確認できます。

カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

### コメント

ユーザーに送信するコメントと、ユーザープロファイルの更新エリアに入力します。

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

