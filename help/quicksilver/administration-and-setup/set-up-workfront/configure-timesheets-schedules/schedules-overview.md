---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: ユーザー、スケジュール
navigation-topic: configure-timesheets-and-schedules
title: スケジュールの概要
description: スケジュールを使用して、週の作業時間を定義できます。ユーザーやプロジェクトに、スケジュールを関連付けることができます。これにより、 [!DNL Adobe Workfront]  がタイムラインとユーザーの空き時間を計算します。手順については、スケジュールを作成を参照してください。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 87%

---

# スケジュールの概要

<!-- Audited: 1/2024 -->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

スケジュールを使用して週の作業時間を定義し、スケジュールをユーザーまたはプロジェクトに関連付けることができます。これにより、[!DNL Adobe Workfront] がタイムラインとユーザーの空き時間を計算できるようになります。手順については、[スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

Workfront でスケジュールを操作する際は、次の点に注意してください。

* [!DNL Workfront] 管理者は、組織の稼働時間をスケジュールで特定します。

  同様に、グループ管理者は、管理するグループによって管理されているスケジュールの稼働時間を特定できます。グループ管理者について詳しくは、[グループ管理者](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)を参照してください。

  例えば、月曜日から金曜日まで、午前 8 時から午後 5 時まで、昼食に 1 時間の休憩があるようにスケジュールを定義できます。

* [!DNL Workfront] はスケジュールを使用して、稼働日の開始と終了を決定します。

  これは、ユーザーが通常の営業時間外に [!DNL Workfront] で作業したり、作業を完了したりすることを妨げるものではありません。通常、夕方に予定されている作業に集中するために、新しいスケジュールやスケジュールの例外を作成する必要はありません。

  同様に、組織では稼働日の出勤時間を柔軟に設定できます。ある従業員が午前 8 時に出勤し、別の従業員が午前 9 時に出勤する場合があります。グループに類似または同一のスケジュールがある場合、各グループに一意のスケジュールを作成する必要はありません。ただし、グループのスケジュールが大幅に異なる場合は、ユーザーを一意のスケジュールに関連付ける必要があります。従業員は、割り当てが午後 5 時に完了する予定かどうかを把握します。これは、作業に就く時間に関係なく、営業日の終わりまでに作業を行う必要があることを意味します。

* 組織に関連付けられたタイムゾーンごとに個別のスケジュールを作成することをお勧めします。

  異なるタイムゾーンで作業するユーザーに対して、作業が適切にスケジュールされるように、各スケジュールに特定のタイムゾーンを割り当てることができます。

* [!DNL Workfront] のデフォルトのスケジュールは、ユーザーやプロジェクトがスケジュールに関連付けられていない場合に、タイムラインの計算で使用されます。

  デフォルトのスケジュールは [!DNL Workfront] システムに付属しており、作成した新しいスケジュールに置き換えない限り削除できません。

* タイムラインの計算に加えて、[!DNL Workfront] はスケジュールを使用してユーザーの可用性を計算します。

  >[!IMPORTANT]
  >
  >[!DNL Workfront] は、ユーザーまたはプロジェクトのスケジュールを使用して、リソースプランナーでのリソースの可用性を決定します。どのスケジュールが使用されるかは、[!DNL Workfront] 管理者が[!UICONTROL リソースの空き時間計算に次を使用]設定で選択した内容によって異なります。リソース管理の設定について詳しくは、[リソース管理環境設定を設計](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

## スケジュールの階層

タスクがスケジュールに関連付けられているユーザーに割り当てられ、2 番目のスケジュールに関連付けられているプロジェクトに常駐している場合、タイムラインの計算に適用される可能性のあるスケジュールが少なくとも 2 つあります。

>[!IMPORTANT]
>
>[!DNL Workfront] は、[!UICONTROL リソースの空き時間計算に次を使用]設定が、[!UICONTROL 設定]の[!UICONTROL リソース管理]エリアの[!UICONTROL ユーザーのスケジュール]に設定されている場合にのみ、ユーザーのスケジュールを使用します。[!UICONTROL リソースの空き時間計算に次を使用]設定がリソース管理に使用されるスケジュールにどのように影響するかについて詳しくは、[リソース管理環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

複数のスケジュールが存在する場合に、システムでスケジュールが使用される順序は次のとおりです。


* 1 人のユーザーをタスクに割り当てると、使用する環境に応じて、次のようなシナリオが発生します。

   * 実稼動環境では、[!DNL Workfront] はユーザーのスケジュールを使用してタスクのタイムラインを計算します。 これには、ユーザーの個人的な時間も含まれます。プロジェクトのスケジュールは無視されます。

     個人スケジュールについて詳しくは、[個人休暇の設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)を参照してください。

   * <span class="preview"> プレビュー環境では、[!DNL Workfront] の [!UICONTROL  設定 ] の [!UICONTROL  プロジェクト環境設定 ] 領域で定義された次のいずれかのスケジュールを使用します。</span>

      * <span class="preview"> タスク </span> に割り当てられたユーザーのスケジュール
      * <span class="preview"> プロジェクトに関連付けられたスケジュール。</span>

* 複数のユーザーが 1 つのタスクに割り当てられ、タスクの期間中に異なるスケジュールを持つ場合、[!DNL Workfront] は、[!UICONTROL 設定]の[!UICONTROL プロジェクト環境設定]エリアで定義されている次のスケジュールのいずれかを使用します。

   * プライマリ担当者に指定されたユーザーのスケジュール
   * プロジェクトに関連付けられたスケジュール。

     プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

* タスクに割り当てられているユーザーにスケジュールがない場合、またはタスクが担当業務やチームにのみ割り当てられていたり、あるいは割り当てられていない場合、[!DNL Workfront] は、タイムラインの計算にプロジェクトスケジュールを使用します。
* タスクに割り当てられているユーザーにスケジュールがない場合、またはタスクが担当業務やチームにのみ割り当てられていたり、あるいは割り当てられていない場合、およびプロジェクトにスケジュールがない場合、[!DNL Workfront] は、タイムライン計算のデフォルトスケジュールとして指定されているシステム内のスケジュールを使用します。

  ![](assets/default-schedule.png)

## タイムゾーンをまたいだ [!DNL Workfront] での共同作業

ユーザーが [!DNL Workfront] でタイムゾーンをまたいで共同作業できるようにスケジュールを使用する方法について詳しくは、[タイムゾーンをまたいだ作業](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)を参照してください。
