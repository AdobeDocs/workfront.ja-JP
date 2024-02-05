---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: タイムゾーンをまたいでの作業
description: ' [!DNL Adobe Workfront]  では、タイムゾーンを使用して、オブジェクトの時間フィールドやメールなどの他のエリアの時間を計算する方法を理解すると役立ちます。'
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 97%

---

# タイムゾーンをまたいでの作業

[!DNL Adobe Workfront] では、タイムゾーンを使用して次の計算を行う方法を理解すると役立ちます。

* オブジェクトの時間フィールド
* Workfront の自動メールなど、他の [!DNL Workfront] 領域での時間

## [!DNL Workfront] のタイムゾーン

[!DNL Workfront] に表示される時間は、組織の [!DNL Workfront] インスタンスとユーザープロフィールのタイムゾーン設定に基づいています。これら 2 つのタイムゾーンが異なる場合、[!DNL Workfront] で使用する様々な領域や機能に時間の相違が生じる可能性があります。

>[!NOTE]
>
>オブジェクトに添付されたカスタムフォームでは、計算されたカスタムフィールドの日付と時刻のステートメントは、組織のインスタンスとユーザープロファイルに設定されたタイムゾーン設定ではなく、協定世界時（UTC）で計算および保存されます。カスタムフォームの計算は、各ユーザーの個々のタイムゾーンに基づいて生成され、表示されます。

* [組織の  [!DNL Workfront]  インスタンス](#your-organization-s-workfront-instance)
* [ユーザープロファイル](#your-user-profile)

### 組織の [!DNL Workfront] インスタンス {#your-organization-s-workfront-instance}

組織の [!DNL Workfront] インスタンスのタイムゾーンは、通常、本社の場所に設定されます。これにより、次のことが決定されます。

* [!DNL Workfront] が生成したメールに表示される時間
* 新しく追加されたユーザーのタイムゾーン（[!DNL Workfront] 管理者が、ユーザーの勤務先の場所に基づいたタイムゾーンを設定する前）

  この 2 つの例について詳しくは、[システムの基本情報の設定](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。

* 上書きされたプロジェクトの請求レートの開始または終了。詳しくは、[プロジェクトレベルで担当業務の請求レートを上書き](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)を参照してください。

### ユーザープロファイル {#your-user-profile}

ユーザープロファイルのタイムゾーンは、勤務先の場所に設定する必要があります。これにより、次のことが決定されます。

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 作業対象のオブジェクトの時間（開始時間や終了時間など）

  複数のタイムゾーンのユーザーが 1 つのオブジェクトに割り当てられている場合、[!DNL Workfront] は、各ユーザープロファイルで設定されているタイムゾーンを使用して、関係するすべてのユーザーのオブジェクト時間を変換します。

  **例：**&#x200B;勤務先の東部標準時（EST）ゾーンでは、午後 4 時に開始するタスクを設定し、太平洋標準時（PST）ゾーンで勤務しているユーザーに割り当てます。これらのユーザーの場合、開始時間は午後 1 時と表示されます。午後 4 時と表示されている場合、3 時間遅れて作業を開始することになります。

  オブジェクト作成者が割り当て先のタイムゾーンの違いに気づかず、オブジェクトの時間を設定する際に必要な調整を行わない場合や、担当者がその違いに気づかない場合は、全員がオブジェクトで共同作業を行う間のタイミングを正しく把握するのが難しくなります。

  **例：**&#x200B;タスクの一部のユーザーが PST ゾーンで勤務していることを忘れて、1 日のタスクを EST の午前 9 時に開始するように設定するとします。これらのユーザーの場合、開始時刻は午前 6 時になります。ユーザーが作業を開始するのは 9:00（あなたのタイムゾーンでは正午）なので、タスクの開始と終了が 3 時間遅れます。

ユーザープロファイルでのタイムゾーンの設定について詳しくは、[個人設定を行う](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)を参照してください。

[!DNL Workfront] 管理者（または、ユーザーへの[!UICONTROL 編集]アクセス権を持つユーザー）がユーザープロファイルのタイムゾーンを設定する方法については、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ユーザーが複数のタイムゾーンをまたいで簡単に作業する方法

複数のタイムゾーンのユーザーがより簡単に作業できるようにするには、次の方法があります。

* [スケジュールを使用](#use-schedules)
* [カスタムフォームでの計算時間フィールドの使用](#use-calculated-time-fields-in-a-custom-form)
* [カスタムフォームで日付フィールドの代わりにテキストフィールドを使用](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### スケジュールを使用 {#use-schedules}

[!DNL Workfront] 管理者は、組織内のタイムゾーンごとに別々のスケジュールを作成し、すべてのユーザーがどこにいても作業が適切にスケジュールされるようにします。管理者がスケジュールを作成したら、特定のプロジェクトやユーザーに関連付けることができます。

* **[!UICONTROL プロジェクト]**：プロジェクト作成者は、個々のプロジェクトのスケジュールを選択できます。この結果、割り当て先のタイムゾーンに設定された作業時間に基づいて、プロジェクト内のタスクのスケジュールが決定されます。
* **[!UICONTROL ユーザー]**：[!DNL Workfront] 管理者（または、ユーザーへの[!UICONTROL 編集]アクセス権を持つユーザー）は、ユーザープロファイルで個々のユーザーのスケジュールを選択できます。

  このスケジュールは、プロジェクトスケジュールとは異なる場合があります。例えば、誰かがプロジェクト内にタスクを作成し、まだ誰にも割り当てていない場合、そのタスクはプロジェクトスケジュールを使用します。ユーザーがタスクに割り当てられると、そのタスクはそのユーザーのスケジュールを使用します。

  複数のユーザーがタスクに割り当てられている場合、システム全体のプロジェクト環境設定で設定した、次のいずれかが使用されます。

   * タスクのプライマリ所有者のスケジュールのタイムゾーン
   * プロジェクトのスケジュールのタイムゾーン。

  これにより、タスクの日付が変更される場合があります。

  **例：** EST ユーザーは、EST の正午である PST の午前 9:00 に開始するようにスケジュールされた 1 日限りのタスクに割り当てられます。EST ユーザーは、その日の残り作業時間が 2 時間に過ぎないので、タスク完了日は次の作業日まで約 6 時間延長されます。

  [!UICONTROL 設定]の[!UICONTROL プロジェクト環境設定]エリアについては、[システム全体のプロジェクト環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

  プロジェクトまたはユーザーにスケジュールを割り当てる手順については、[スケジュールを作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

  スケジュールで設定されたタイムゾーンが[!UICONTROL ワークロードバランサー]での[!UICONTROL 予定時間数]の配分に与える影響については、[[!UICONTROL ワークロードバランサー]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)でのユーザー割り当ての管理を参照してください。


### カスタムフォームでの計算時間フィールドの使用 {#use-calculated-time-fields-in-a-custom-form}

カスタムフォームで一連の計算カスタムフィールドを使用して、複数の都市の時刻を表示する空港時計の列のように、組織のユーザーの現在時刻を表示できます。ユーザーが作業するタイムゾーンごとにフィールドを作成し、それぞれのタイムゾーンの時刻を各フィールドで計算できます。

詳しくは、 [計算データをカスタムフォームに追加する](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)を追加し、セクションを [日付と時刻の計算されたカスタムフィールド](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 記事内 [計算データ式の概要](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### カスタムフォームで日付フィールドの代わりにテキストフィールドを使用 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

設定した時刻がタイムゾーンの異なるユーザー向けに [!DNL Workfront] によってオブジェクト内で変換されないようにする場合は、オブジェクトに添付するカスタムフォームで、日付フィールドではなくテキストフィールドを使用します。これにより、入力した時刻が、プロジェクトのすべてのメンバーに対して表示されます。

この場合、開発者のタイムゾーンとの時差を計算して作業の開始日時と終了日時を判断できるようにすることをフォームのユーザーに注意することをお勧めします。これは、カスタムフォームに入力する説明文や、そのフィールドのツールヒントに含めることもできます。詳しくは、[カスタムフォームへのカスタムフィールドの追加](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)を参照してください。
