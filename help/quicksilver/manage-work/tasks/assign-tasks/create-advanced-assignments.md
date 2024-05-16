---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 高度な割り当てを作成
description: 高度な割り当てを使用して、タスクまたはイシューの割り当てを管理できます。
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 97%

---

# 高度な割り当てを作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、を参照してください。 [2024 年第 3 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

高度な割り当てを使用して、タスクまたはイシューの割り当てを管理できます。

高度な割り当てを行う際に、割り当て情報を次のように調整できます。

* タスクまたはイシューにユーザーを割り当て（高度な割り当て以外で実行可能）。
* 各担当者に配分される時間数を調整および再配分。
* タスクまたはイシューの所有者またはプライマリ担当者に指定するユーザーを決定。
* タスクまたはイシューで作業する際に各ユーザーが果たす役割を指定。
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>ユーザーを作業に割り当てる場合、ユーザーのスケジュールに応じた空き時間は、タスクやイシューの予定日と見込日に影響します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

## 高度な割り当てを行える Adobe Workfront の領域

この記事では、タスクまたはイシューのヘッダーで高度な割り当てにアクセスする方法について説明します。

Workfront の次の領域でも、高度な割り当てをおこなうことができます。

* リストとレポート（割り当てフィールドがビューに表示されている場合）。
* タスクの編集時の「割り当て」セクション。

。（詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください）
* 割り当て領域のタスクまたはイシューのヘッダー。
* ワークロードバランサー内（詳しくは、[ワークロードバランサーを使用した手動による作業の割り当て](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)を参照してください）

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびイシューに対する編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクまたはイシューに対する、参加以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 高度な割り当てを行う

1. タスクまたはイシューを割り当てるプロジェクトに移動します。
1. 左側のパネルで「**タスク**」または「**イシュー**」をクリックし、リスト内のタスクまたはイシューの名前をクリックします。

   >[!TIP]
   >
   >複数の担当者が割り当てられている場合は、タスクまたはイシューのリストで直接、高度な割り当てを行うことができます。タスクまたはイシューと同じ行の&#x200B;**割り当て**&#x200B;フィールド内をクリックし、**ユーザーアイコン**&#x200B;をクリックして、高度な割り当てウィンドウを開きます。高度な割り当ての作成を続行するには、手順 5 に進んでください。\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. タスクまたはイシューのヘッダーにある&#x200B;**割り当て**&#x200B;フィールドの「**割り当て先**」をクリックします。

   または

   タスクまたはイシューが既に割り当てられている場合は、割り当ての名前をクリックします。

1. 「**詳細**」をクリックします。

   実稼動環境のサンプル画像：
   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">プレビュー環境のサンプル画像：</span>
   ![「詳細」をクリックします](assets/assignments-box-in-task-header.png)

1. **ユーザー、役割、チームを検索**&#x200B;フィールドに、ユーザー、役割、またはチームの名前を入力し、ドロップダウンリストに表示された名前をクリックします。

   >[!NOTE]
   >
   >ユーザーの名前に特殊文字が含まれている場合は、その特殊文字を検索フィールドに含める必要があります。

1. （オプション）引き続き&#x200B;**ユーザー、役割、チームを検索**&#x200B;ボックスに担当者を追加して、タスクまたはイシューに複数のリソースを追加します。

   >[!TIP]
   >
   >* 複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
   >
   >
   >* ユーザー割り当てを追加する際には、アバター、ユーザーの主要な役割やメールアドレスに注意して、同じ名前のユーザーを区別してください。
   >ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
   >ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。
   >
   >
   >* 非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
   >   
   >   * 作業アイテムをアクティブなリソースに再割り当てする。
   >   * 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. 「**担当者**」列で、ユーザーごとに次の情報を指定します。


   * **所有者**：担当者をタスクまたはイシューの所有者としてマークする場合は、担当者の名前にポインタを合わせ、所有者フィールドの「**プライマリにする**」をクリックします。緑のチェックボックスは、指定したユーザーがタスクまたはイシューのプライマリ連絡先であることを示します。Adobe Workfront は、タスクやイシューに最初に割り当てたユーザーや担当業務を、所有者またはプライマリ割り当てとしてマークします。チームは、タスクやイシューのプライマリ所有者に指定できません。

     >[!IMPORTANT]
     >
     >Workfront 管理者またはグループ管理者がプロジェクトの環境設定をどのように指定したかに応じて、複数のユーザーがタスクに割り当てられている場合、Workfront はタスク所有者のスケジュールを使用してタスクのタイムラインを計算する場合があります。複数のタスクの担当者について詳しくは、[タスクの割り当て](../../../manage-work/tasks/assign-tasks/assign-tasks.md)の記事の「複数のユーザーをタスクに割り当て」の節を参照してください。

   * **配分**：タスクの期間タイプが「シンプル」の場合は、各ユーザーや担当業務にタスクを割り当てる時間数を指定します。各ユーザーに割り当てられたすべての時間の合計は、「配分」列の下部にある&#x200B;**予定時間数**&#x200B;フィールドの数値と等しくなります。それ以外のすべての期間タイプでは、タスクやイシューの解決に担当者が費やす時間の割合（または配分）を指定します。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * タスクの割り当ての配分を手動で変更すると、タスクの予定時間数がそれに応じて更新される場合があります。詳しくは、[予定時間数の概要](../../../manage-work/tasks/task-information/planned-hours.md)の記事の「ユーザーの配分を管理する際のタスクの予定時間数を更新」の節を参照してください。
     >   * イシューに対する割り当ての配分を手動で変更することはできません。
     >   * タスクに割り当てられたチームの配分を手動で変更することはできません。
     >   
     >

   * **割り当て先の役割：**&#x200B;この割り当てを実行する際にユーザーが使用する役割を選択します。デフォルトでは、ユーザーの主要役割が表示されます。「割り当て先の役割」ボックスをクリックして、別の役割を選択します。最初にタスクやイシューを役割に割り当て、次にその役割を実行できるユーザーを 2 番目の割り当てとして追加すると、ユーザー候補のリストは、タスクやイシューに既に割り当てられている役割を実行できるユーザーに絞り込まれます。

     実稼動環境のサンプル画像：
     ![](assets/advanced-assignments-box-select-a-role-350x243.png)

     <span class="preview">プレビュー環境のサンプル画像：</span>
     ![割り当て先の役割](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **期間タイプ**：これは、タスクでのみ使用できます。期間タイプの名前をクリックし、ドロップダウンメニューから期間タイプを選択します。期間タイプについては、[タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

   * **期間：**&#x200B;タスクに対する管理権限がある場合は、タスクのこのフィールドを更新できます。

     詳しくは、[タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。割り当て情報を一括編集すると、ユーザー、時間数、配分およびタスク所有者を割り当てるための同様のダイアログボックスが表示されます。

   * **予定時間数**：期間タイプが「予定割り当て時間」または「シンプル」の場合は、予定時間数の数値を更新します。その結果、それぞれのリソースの配分率または時間数が均等に配分されます。Workfront では、期間タイプが「予定作業」または「残存作業時間の優先」の場合は、予定時間数を計算します。詳しくは、[タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

     実稼動環境のサンプル画像：
     ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

     <div class="preview">

     プレビュー環境のサンプル画像：
     ![高度な割り当て](assets/advanced-assignments-duration-type-allocations.png)

     </div>

1. 「**保存**」をクリックします。
