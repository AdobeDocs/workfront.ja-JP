---
title: リマインダー通知の設定
description: リマインダー通知の設定
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 3d4ba0396c5a59b1109ec70a6e85b77d0d093bf5
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 2%

---

# リマインダー通知の設定

<!--hidden content for the tab redesign in August 2023-->

リマインダー通知では、指定した条件に基づいて受信者に E メールを送信します。 リマインダー通知へのリマインダー通知のアクセスレベルと管理アクセス権を持つAdobe Workfront管理者またはユーザーは、プロジェクト、タスク、タスク、タイムシートなどの作業項目にリマインダー通知を手動で関連付けることができます。

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プランナー以上（リマインダー通知への管理アクセス権を持つ）</p> <p>プランのユーザー管理アクセス権の付与については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## リマインダーの電子メールをカスタマイズ

カスタムの電子メールの件名と本文を含むカスタム電子メールで、リマインダー通知をカスタマイズできます。 E メール本文には、カスタムHTMLを含めることができます。

または、リマインダー通知に含まれるデフォルトの電子メールを使用できます。 デフォルトの E メールでは、リマインダーの通知名を E メールの件名として使用し、通知をトリガーしたイベントを含む E メール本文のオブジェクト名を使用します。

リマインダーの電子メールをカスタマイズする場合は、電子メールテンプレートを作成して、リマインダー通知に添付する必要があります。

E メールテンプレートの作成方法について詳しくは、 [電子メールテンプレートの設定](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## リマインダー通知の作成

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **電子メール** > **通知** > **リマインダー通知**.

   <!--hidden for the tab redesign for August 2023:
   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)
   -->
1. クリック **新しいリマインダー通知**.

1. ドロップダウンリストで、リマインダー通知に関連付けるオブジェクトタイプをクリックします。

   たとえば、タイムシートにリマインダー通知を添付する場合は、[ **タイムシート**.

1. Adobe Analytics の **新しいリマインダー通知** 表示されるボックスで、次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">リマインダー通知名</td> 
      <td>リマインダー通知の名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">対象期間</td> 
      <td> <p>日付の前後の時間数、稼働日、日数（カレンダー日数）、週数または月数を指定します <strong>タイミング</strong> フィールドに入力します。</p> <p><b>メモ</b>:  
        <ul> 
         <li> <p>リマインダー通知は、指定した日付の 24 時間後に開始され、すべての条件が満たされたら開始されます。</p> </li> 
         <li> <p>毎晩午前 0 時（米国山岳部標準時）に、プロジェクト、タスクおよび問題のトリガーに関するリマインダー通知が届きます。 その日以降にリマインダー通知を受け取るすべてのオブジェクト。指定したトリガーに対する通知は、その時間の直後に通知されます。</p> </li> 
         <li> <p>タイムシートのリマインダー通知は、指定した時間に、タイムゾーンとタイムシートの終了日、開始日、または最終更新日に基づいて送信されます。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイミング</td> 
      <td> <p>リマインダー通知をスケジュールするトリガーを設定するイベントを選択します。</p> <p>リマインダー通知がプロジェクト、タスクまたは問題を対象としている場合は、使用可能なオプションは「完了日」または「開始日」に関連しています。 リマインダー通知では、プロジェクト、タスクおよび問題の「完了」および「開始」日のタイムスタンプが考慮されます。</p>

   <p>リマインダー通知がタイムシートを対象としている場合は、[ 終了日 ]、[ 開始日 ]、または [ 最終更新日 ] に関連するオプションを使用できます。 タイムシートのリマインダー通知では、タイムシートの [ 終了 ]、[ 開始 ]、[ 最終更新日 ] のタイムスタンプが考慮されます。 タイムシートは開始日（午前 12:00）の午前 0 時に開始し、終了日（午後 11:59）の午前 0 時に終了します。</p>

   <p><b>メモ</b></p>
      <p>タイムシートのリマインダー通知は、24 時間に 1 回のみ配布されます。</p> <p>24 時間以内に複数のリマインダー通知を設定した場合、Workfrontは 1 つの通知電子メールを送信し、その通知に含まれるすべてのリマインダーを送信します。</p>
      <p>例えば、3 つのリマインダー通知をトリガーの 10 時間前、2 時間前、および期日の 1 時間前に設定した場合、同じ日に発生した場合、3 つのリマインダーはすべて同じ通知に組み合わされます。</p> <p>ただし、リマインダー通知を 26 時間前に設定し、別の通知を期限前に 1 時間設定した場合、ユーザーは 2 つの異なる通知を受け取ります。 </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">基準</td> 
      <td> <p>リマインダー通知をスケジュールする条件を選択します。 リマインダーの通知は、条件の選択が満たされない限り、スケジュールされません。</p> <p>手順 4 で選択したオブジェクトタイプに応じて、次の条件オプションを使用できます。</p> 
       <ul> 
        <li><strong>現在のプロジェクトで不完全です：</strong> （タスクおよび問題のリマインダーで使用可能）リマインダー通知は、リマインダー通知が関連付けられているオブジェクトの状態が [ 完了 ] ではなく、プロジェクトの状態が [ 現在 ] の場合にのみ送信されるようにスケジュールされます。</li> 
        <li><strong>現在のプロジェクト内のすべて：</strong>（タスクおよび問題のリマインダーで使用可能）リマインダー通知は、オブジェクトの状態に関係なく、リマインダー通知が関連付けられているプロジェクトの状態が「現在」の場合にのみ、送信されるようにスケジュールされます。</li> 
        <li><strong>不完全なプロジェクト：</strong> （プロジェクトのリマインダーに使用可能）プロジェクトのステータスが [ 完了 ] 以外の場合、リマインダー通知が送信されるようにスケジュールされます。</li> 
        <li><strong>プロジェクトを完了：</strong> （プロジェクトのリマインダーに使用可能）プロジェクトのステータスが「完了」のときに、リマインダー通知が送信されるようにスケジュールされています。</li> 
        <li><strong>タイムシートを開く：</strong> （タイムシートのリマインダーに使用可能）タイムシートの状態が [ 開く ] の場合に、リマインダー通知が送信されるようにスケジュールされます。</li> 
        <li><strong>提出済みタイムシート：</strong> （タイムシートのリマインダーに使用可能）タイムシートの状態が [ 提出済み ] になったときに、リマインダー通知が送信されるようにスケジュールされます。</li> 
        <li><strong>タイムシートを開くか、週に 40 時間未満で開く：</strong> （タイムシートのリマインダーに使用可能）タイムシートの状態が [ 開封 ] の場合、またはタイムシートが 40 時間未満の場合に、リマインダー通知が送信されるようにスケジュールされます。</li> 
        <li><strong>メールテンプレート：</strong> 「 」ドロップダウンで、リマインダーに添付する電子メールテンプレートを選択します。<br>電子メールテンプレートの作成方法について詳しくは、 <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">電子メールテンプレートの設定</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">受信者</td> 
      <td>通知を受け取るユーザーのタイプを選択します。 所有者、承認者、担当者など、様々なオブジェクトの関係者から選択します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
1. 作業項目にリマインダー通知を添付する ( [オブジェクトにリマインダー通知を添付する](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## リマインダー通知を受信

リマインダー通知が添付されている項目で条件が満たされると、リマインダー通知で定義されたユーザーに対して電子メール通知がトリガーされます。

リマインダー通知の受信について詳しくは、 [リマインダーの通知](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) のセクション [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## リマインダー通知配信のテスト

リマインダー通知トリガーは、毎晩午前 0 時、山岳部時間に設定されています。 リマインダー通知の対象となるすべてのオブジェクト。その直後に、指定したトリガーに通知が届きます。

リマインダー通知を手動でトリガーさせるには、まずリマインダーの条件を満たす必要があります。\
例えば、プロジェクトの計画完了日から 1 時間後にリマインダーをトリガーに設定した場合、リマインダーが設定されてから今に至るまでの間にリマインダーの時間が経過している必要があります。 リマインダーが有効化される前に、計画完了日が過ぎたプロジェクトには通知がトリガーされません。

リマインダー通知を手動でトリガーするには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **診断** Workfrontの左下隅に

1. クリック **リマインダー通知の送信** 画面上部に、送信されたことを確認するメッセージが表示されるのを待ちます。

   リマインダーの通知で指定されたユーザーに電子メールが送信されます。
