---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: タイムゾーンをまたいでの作業
description: 次の方法を理解すると役立ちます。 [!DNL Adobe Workfront] は、タイムゾーンを使用して以下の計算を行います — EDIT ME.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 0%

---

# タイムゾーンをまたいでの作業

次の方法を理解すると役立ちます。 [!DNL Adobe Workfront] では、タイムゾーンを使用して次の計算をおこないます。

* オブジェクトの時間フィールド
* その他の回数 [!DNL Workfront] 自動Workfront E メールなどの領域

## のタイムゾーン [!DNL Workfront]

に表示される回数 [!DNL Workfront] は、組織のタイムゾーン設定に基づいています [!DNL Workfront] インスタンスとユーザープロファイルの両方に存在します。 これら 2 つのタイムゾーンが異なる場合、で使用する様々な領域や機能に時間の相違が生じる可能性があります。 [!DNL Workfront].

>[!NOTE]
>
><div class="preview">オブジェクトに関連付けられたカスタムフォームでは、計算されたカスタムフィールドの日付と時刻のステートメントは、組織のインスタンスとユーザープロファイルに設定されたタイムゾーン設定ではなく、協定世界時 (UTC) で計算および保存されます。 カスタムフォームの計算は、各ユーザーの個々のタイムゾーンに基づいて生成され、表示されます。</div>




* [組織の [!DNL Workfront] インスタンス](#your-organization-s-workfront-instance)
* [ユーザープロファイル](#your-user-profile)

### 組織の [!DNL Workfront] インスタンス {#your-organization-s-workfront-instance}

組織のタイムゾーン [!DNL Workfront] インスタンスは通常、メインオフィスの場所に設定されます。 これにより、次のことが決まります。

* が生成した E メールに表示される時間 [!DNL Workfront]
* 新しく追加されたユーザーのタイムゾーン ( [!DNL Workfront] 管理者が、作業場所に基づいて異なるタイムゾーンを設定します。

   この 2 つの例について詳しくは、 [システムの基本情報を設定する](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 上書きされたプロジェクトの請求率の開始または終了。 詳しくは、 [プロジェクト・レベルでの役割請求率の上書き](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### ユーザープロファイル {#your-user-profile}

ユーザープロファイルのタイムゾーンは、勤務先の場所に対して設定する必要があります。 これにより、次のことが決まります。

* 送信時刻が表示されます [!DNL Workfront] 電子メールメッセージ
* 作業対象のオブジェクトの時間（開始時間や終了時間など）

   複数のタイムゾーンのユーザーが 1 つのオブジェクトに割り当てられている場合、 [!DNL Workfront] は、各ユーザープロファイルで設定されたタイムゾーンを使用して、関係するすべてのユーザーのオブジェクト時間を変換します。

   **例：** 勤務先の東部標準時 (EST) ゾーンで、午後 4 時に開始するタスクを設定し、太平洋標準時 (PST) ゾーンで勤務するユーザーに割り当てます。 これらのユーザーの場合、開始時間は午後 1 時と表示されます。 午後 4 時に表示する場合、3 時間遅れて作業を開始します。

   オブジェクト作成者が割り当て先のタイムゾーンの違いをメモせず、オブジェクトの時間を設定する際に必要な調整を行う場合や、割り当て先が違いをメモしない場合は、誰もがオブジェクトで共同作業する間にタイミングを正しく取得するのが難しくなります。

   **例：** 1 日のタスクを、PST ゾーンでの作業を忘れて、EST の午前 9 時に開始するように設定します。 これらのユーザーの場合、開始時刻は午前 6 時です。 ユーザーが作業を開始するのは 9:00（正午の時間）までないので、タスクは開始され、3 時間遅れて完了します。

ユーザープロファイルでのタイムゾーンの設定については、 [設定を行う](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

を [!DNL Workfront] 管理者 ( または、 [!UICONTROL 編集] ユーザーへのアクセス ) は、ユーザープロファイルでタイムゾーンを設定できます。詳しくは、 [ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## ユーザーが複数のタイムゾーンをまたいで作業しやすくする方法

複数のタイムゾーンでユーザーがより簡単に作業できるようにするには、次の方法があります。

* [スケジュールを使用](#use-schedules)
* [カスタムフォームで計算時間フィールドを使用する](#use-calculated-time-fields-in-a-custom-form)
* [カスタムフォームで日付フィールドの代わりにテキストフィールドを使用する](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### スケジュールを使用 {#use-schedules}

[!DNL Workfront] 管理者は、組織内のタイムゾーンごとに別々のスケジュールを作成し、すべてのユーザーがどこにいても作業が適切にスケジュールされるようにします。 管理者がスケジュールを作成したら、特定のプロジェクトおよびユーザーに関連付けることができます。

* **[!UICONTROL プロジェクト]**:プロジェクト作成者は、個々のプロジェクトのスケジュールを選択できます。 割り当て先のタイムゾーンに設定された作業時間に基づいて、プロジェクト内のタスクのスケジュールを決定します。
* **[!UICONTROL ユーザー]**:A [!DNL Workfront] 管理者 ( または、 [!UICONTROL 編集] ユーザーへのアクセス ) は、ユーザーのプロファイル内の個々のユーザーのスケジュールを選択できます。

   このスケジュールは、プロジェクトスケジュールとは異なる場合があります。 例えば、誰かがプロジェクト内にタスクを作成し、まだ誰も割り当てていない場合、そのタスクはプロジェクトスケジュールを使用します。 ユーザーがタスクに割り当てられると、そのタスクはそのユーザーのスケジュールを使用します。

   複数のユーザーがタスクに割り当てられている場合、システム全体のプロジェクトプリファレンスで設定した次のいずれかが使用されます。

   * タスクのプライマリ所有者のスケジュールのタイムゾーン
   * プロジェクトのスケジュールのタイムゾーン。

   これにより、タスクの日付が変更される場合があります。

   **例：** EST ユーザーは、EST の正午である PST の午前 9 時に開始するようにスケジュールされた 1 日のタスクに割り当てられます。 EST ユーザーは 1 日の残り作業時間が 2 時間しかないので、タスク完了日は次の作業日まで約 6 時間延長されます。

   詳しくは、 [!UICONTROL プロジェクト環境設定] ～の面積 [!UICONTROL 設定]を参照してください。 [システム全体のプロジェクト環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   プロジェクトまたはユーザーにスケジュールを割り当てる手順については、 [スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   スケジュールで設定されたタイムゾーンがの配布に与える影響について詳しくは、 [!UICONTROL 予定時間] 内 [!UICONTROL スケジュール] ツールと [!DNL Workload Balancer]を参照してください。

   * [ユーザー割り当てを [!UICONTROL スケジュール] 領域](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md)
   * [ユーザー割り当てを [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)



### カスタムフォームで計算時間フィールドを使用する {#use-calculated-time-fields-in-a-custom-form}

カスタムフォームで一連の計算済みカスタムフィールドを使用して、複数の都市で時刻を表示する空港時計の列など、組織のユーザーの現在時刻を表示できます。 ユーザーが作業する各タイムゾーンに対してフィールドを作成し、それぞれのタイムゾーンの時間を計算できます。

詳しくは、 [計算データをカスタムフォームに追加する](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)を追加し、セクションに [日付と時刻の計算されたカスタムフィールド](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 記事内 [計算データ式](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### カスタムフォームで日付フィールドの代わりにテキストフィールドを使用する {#use-text-fields-instead-of-date-fields-in-a-custom-form}

もしあなたが望まないなら [!DNL Workfront] 異なるタイムゾーンのユーザー向けにオブジェクトのに設定した時間を変換するには、日付フィールドではなく、オブジェクトに添付するカスタムフォームのテキストフィールドを使用します。 これにより、時間は、プロジェクトの全員に対して入力した時間を表示します。

この場合、ユーザーにタイムゾーンとユーザーの時間差を計算して、いつ作業を開始し、終了するかを指定するようにフォームのユーザーに促すことをお勧めします。 これは、カスタムフォームの入力手順や、そのフィールドのツールヒントに含めることができます。 詳しくは、 [カスタムフォームにカスタムフィールドを追加する](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
