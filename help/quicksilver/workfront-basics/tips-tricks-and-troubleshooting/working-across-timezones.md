---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: タイムゾーンをまたいでの作業
description: ' [!DNL Adobe Workfront]  では、タイムゾーンを使用して、オブジェクトの時間フィールドやメールなどの他のエリアの時間を計算する方法を理解すると役立ちます。'
feature: Get Started with Workfront
author: Becky
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 70%

---

# タイムゾーンをまたいでの作業

<!-- Audited: 2/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

[!DNL Adobe Workfront] では、タイムゾーンを使用して次の計算を行う方法を理解すると役立ちます。

* オブジェクトの時間フィールド
* Workfront の自動メールなど、他の [!DNL Workfront] 領域での時間

>[!WARNING]
>
>提供されているリストに正確なタイムゾーンが見つからない場合は、自身に最も近いタイムゾーンを見つけ、インスタンスに合わせて更新します。
>
>また、同様のタイムゾーンであっても、自身のタイムゾーンと完全には一致しない可能性があることも考慮してください。
>
>例えば、一部の国や地域では夏時間が適用され、お客様の国では適用されていない可能性があります。必要に応じ、これらの変更に従ってシステムのタイムゾーンを調整する必要がある場合があります。


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

ユーザーのプロファイルの「タイムゾーン」フィールドは、送信メールメッセージに表示される時間を制御します。

タイムゾーンは、PTO カレンダーレポートに表示される内容にも影響します。

ユーザープロファイルでのタイムゾーンの設定について詳しくは、[個人設定を行う](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)を参照してください。

[!DNL Workfront] 管理者（または、ユーザーへの[!UICONTROL 編集]アクセス権を持つユーザー）がユーザープロファイルのタイムゾーンを設定する方法については、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

### ブラウザーのタイムゾーン

勤務先の場所用に、ブラウザーのタイムゾーンを設定する必要があります。 これにより、次のことが決定されます。

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 開始時間や終了時間など、作業対象のオブジェクトの時間。

  複数のタイムゾーンのユーザーが 1 つのオブジェクトに割り当てられている場合、[!DNL Workfront] は、各ユーザーのブラウザーで設定されたタイムゾーンを使用して、関係するすべてのユーザーのオブジェクト時間を変換します。

  **例**
作業を行う東部標準時（EST） ゾーンで、午後 4 時に開始するようにタスクを設定し、太平洋標準時（PST） ゾーンで作業するユーザーにそのタスクを割り当てます :00 これらのユーザーの場合、開始時刻は午後 1:00 と表示されます。 仮に午後 4 時と表示した場合 :00、3 時間遅れて作業を開始することになります。

  オブジェクトの作成者が担当者のタイムゾーンの違いを知らず、オブジェクトの時間を設定する際に必要な調整を行わない場合、または担当者がその違いを知らない場合、全員がオブジェクトで共同作業をしている間にタイミングを正しく把握するのは難しい可能性があります。

  **例**

  タスクの一部のユーザーが PST ゾーンで作業することを忘れて、EST の午前 9:00 に開始するように 1 日タスクを設定します。 彼らのために、開始時刻 6:00 午前。 彼らは彼らの時間（あなたの時間の正午）に 9:00 までそれを作業し始めないので、タスクが始まり、3 時間遅れて完了します。

タイムゾーンの設定は、ブラウザー間で異なります。 詳しくは、各ブラウザーのドキュメントまたはヘルプ情報を参照してください。

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

  複数のユーザーが 1 つのタスクに割り当てられている場合、システムは、システム全体またはグループ全体のプロジェクト環境設定で設定されているように、次のいずれかを使用します。

   * タスクのプライマリ所有者のスケジュールのタイムゾーン
   * プロジェクトのスケジュールのタイムゾーン。

  1 人のユーザーがタスクに割り当てられている場合、システムは、システム全体またはグループ全体のプロジェクト環境設定で設定されているように、次のいずれかを使用します。

   * タスクの担当者のスケジュールのタイムゾーン
   * プロジェクトのスケジュールのタイムゾーン。

  これにより、タスクの日付が変更される場合があります。

>[!BEGINSHADEBOX]

**例：**
EST ユーザーは、午前 9:00 （PST）（EST の正午）に開始されるようにスケジュールされた 1 日のタスクに割り当てられます。 EST ユーザーは、その日の残り作業時間が 2 時間に過ぎないので、タスク完了日は次の作業日まで約 6 時間延長されます。


>[!ENDSHADEBOX]

[!UICONTROL 設定]の[!UICONTROL プロジェクト環境設定]エリアについては、[システム全体のプロジェクト環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

プロジェクトまたはユーザーにスケジュールを割り当てる手順については、[スケジュールを作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

スケジュールで設定されたタイムゾーンが[!UICONTROL ワークロードバランサー]での[!UICONTROL 予定時間数]の配分に与える影響については、[[!UICONTROL ワークロードバランサー]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)でのユーザー割り当ての管理を参照してください。


### カスタムフォームでの計算時間フィールドの使用 {#use-calculated-time-fields-in-a-custom-form}

カスタムフォームで一連の計算カスタムフィールドを使用して、複数の都市の時刻を表示する空港時計の列のように、組織のユーザーの現在時刻を表示できます。ユーザーが作業するタイムゾーンごとにフィールドを作成し、それぞれのタイムゾーンの時刻を各フィールドで計算できます。

詳しくは、[&#x200B; フォームへの計算フィールドの追加 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) および [&#x200B; 計算データ式の概要 &#x200B;](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) の記事 [&#x200B; 日付と時刻の計算カスタムフィールド &#x200B;](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md) を参照してください。

### カスタムフォームで日付フィールドの代わりにテキストフィールドを使用 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

設定した時刻がタイムゾーンの異なるユーザー向けに [!DNL Workfront] によってオブジェクト内で変換されないようにする場合は、オブジェクトに添付するカスタムフォームで、日付フィールドではなくテキストフィールドを使用します。これにより、入力した時刻が、プロジェクトのすべてのメンバーに対して表示されます。

この場合、開発者のタイムゾーンとの時差を計算して作業の開始日時と終了日時を判断できるようにすることをフォームのユーザーに注意することをお勧めします。これは、カスタムフォームに入力する説明文や、そのフィールドのツールヒントに含めることもできます。詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。
