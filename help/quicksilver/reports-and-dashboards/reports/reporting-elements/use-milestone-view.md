---
product-area: reporting
navigation-topic: reporting-elements
title: マイルストーンビューの使用
description: マイルストーン ビューは、プロジェクト リストまたはレポートに適用できます。 マイルストーン ビューを使用して、表示しているプロジェクト内のタスクに関連付けられているすべてのマイルストーンを表示できます。
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 66%

---

# マイルストーンビューの使用

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

マイルストーン ビューは、プロジェクト リストまたはレポートに適用できます。 マイルストーン ビューを使用して、表示しているプロジェクト内のタスクに関連付けられているすべてのマイルストーンを表示できます。

マイルストーン ビューを使用するには、まず次の要素が存在している必要があります。

* マイルストーンパスが設定されます。 詳しくは、[ マイルストーンパスの作成 ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) を参照してください。
* 必要なマイルストーンパスをプロジェクトに追加する。 詳しくは、[プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。
* マイルストーンはタスクに関連付けられます。 詳しくは、[マイルストーンとタスクの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)を参照してください。

マイルストーン ビューは、プロジェクトリストまたはプロジェクトレポートを表示するときに使用できます。 次の節では、マイルストーンビューの表示方法と使用方法について説明します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>ワークまたはそれ以上</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を表示またはそれ以上の権限に設定する</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>マイルストーンビューをレポートに適用するための、プロジェクトレポートに対する表示権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## マイルストーンビューへの切り替え {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. 「**ビュー**」ドロップダウンメニューをクリックして、「**マイルストーン**」をクリックします。

   リストやレポートがマイルストーンビューで表示されます。

   マイルストーンビューについて詳しくは、この記事の[マイルストーンビューの概要](#milestone-view-overview)の節を参照してください。

## マイルストーンビューの概要 {#milestone-view-overview}

マイルストーンビューは、プロジェクトリストやプロジェクトレポートで使用できます。表示しているプロジェクト内のタスクに関連付けられているすべてのマイルストーンをすばやく表示できます。


>[!NOTE]
>
>以下のエリアでは、マイルストーンビューを使用できません。
>
>* タイムシート（プロジェクト追加時のプロジェクトリスト内）。

マイルストーンビューに切り替える方法については、この記事の[マイルストーンビューへの切り替え](#switch-to-the-milestone-view)の節を参照してください。

<!--add new screen shot for preview or prod release-->

![マイルストーンビューのプロジェクト](assets/project-with-milestone-view-with-complete.png)

### マイルストーンビューのセクション

マイルストーンビューをプロジェクトのリストに適用すると、プロジェクトは以下のセクションに表示されます。

* マイルストーンパスに関連付けられているプロジェクトが最初に表示され、それぞれのマイルストーンパス名の下にリストアップされます。

  Workfront は、最初のセクションのプロジェクトを以下の基準に従って、次の順序で並べ替えます。

   1. マイルストーンパス ID。マイルストーンパス ID は、マイルストーンパスレポートで確認できます。

   2. マイルストーンビューを選択する前に、以前にプロジェクトリストに適用されたビューのプロジェクトリストの最初の並べ替えフィールドとして選択されていたフィールド。

* 次にマイルストーンパスに関連付けられていないプロジェクトが、「未割り当て」セクションに表示されます。Workfront は、マイルストーンビューを選択する前に、以前にプロジェクトリストに適用されたビューのプロジェクトリストの最初の並べ替えフィールドとして選択されていたフィールドを基に、「未割り当て」セクションのプロジェクトを並べ替えます。

### マイルストーンビューのプロジェクト情報

マイルストーンビューでプロジェクトリストやプロジェクトレポートを表示すると、次の情報を確認できます。

* **予定日または見込み日：**&#x200B;マイルストーンビューに予定日と見込み日のどちらを表示するかを指定します。\
  日付は、プロジェクトの開始日と完了日、およびマイルストーン パスの各マイルストーン タスクの完了日に表示されます。

  見込日を表示している場合は、日付を編集できません。 見込日はWorkfrontによって計算され、手動で変更することはできません。

  予定日付を表示しており、さらにプロジェクトに対する管理アクセス権を持っている場合は、マイルストーン ビューから直接、次の日付を編集できます。

   * **プロジェクト開始日：** プロジェクトが開始日からスケジュールされている場合、プロジェクトの計画開始日を手動で変更すると、計画完了日が計算されます。
   * **プロジェクト完了日：** プロジェクトが計画完了日からスケジュールされている場合、プロジェクトの計画完了日を手動で変更すると、計画開始日が計算されます。
   * **タスクの完了日：** タスクの完了予定日は、マイルストーン ビューから直接手動で更新できます。

* **完了率：**&#x200B;各タスクとプロジェクトの完了率を表示します。

  この記事の、[マイルストーンビューに表示される情報を設定する](#configure-what-information-displays-in-the-milestone-view)の節で説明されているように、完了率が表示されないようにすることができます。

  完了率は、[マイルストーンビューでタスクの完了率を調整する](#adjust-percent-complete-for-tasks-in-the-milestone-view)の節で説明されているように、完了率が表示されないようにすることができます。

* **タスクの進捗ステータスアイコン：** マイルストーンビューでは、各プロジェクトおよびタスクの横にステータス アイコンが表示されます。<!--get new screen shots or hide them for preview or prod - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  <!--A progress status icon in the shape of a colored circle displays next to each project and task in the Milestone view. The possible statuses and circle colors are: 
   * On Time - green
   * Behind - yellow
   * At Risk - blue
   * Late - red-->


   * 予定通り\
     ![ オンタイムアイコン ](assets/gantt-ontime.png)

   * 遅れ\
     ![ 背後のアイコン ](assets/gantt-behind.png)

   * リスクあり\
     ![ 危険アイコン ](assets/gantt-atrisk.png)

   * 遅延\
     ![ 遅延アイコン ](assets/gantt-late.png)

  これらのステータスアイコンは、[マイルストーンビューに表示する情報を設定する](#configure-what-information-displays-in-the-milestone-view)の節で説明されているように、表示されないようにすることができます。

  各ステータスタイプについて詳しくは、[タスクの進捗ステータスの概要](../../../manage-work/tasks/task-information/task-progress-status.md)を参照してください。

* **完了したタスクのステータスの色合い**：タスクが「完了」とマークされた後、マイルストーンビューでタスクの背景に色が付き、タスクが時間通りに完了したか、遅れて完了したかを示します。

   * **タスク列の赤い背景色**：進捗ステータスが&#x200B;**遅延**&#x200B;の場合、タスクの背景は赤色で表示されます。

   * **タスク列の緑の背景色**：進捗ステータスが&#x200B;**オンタイム**&#x200B;の場合、タスクの背景は緑色で表示されます。

* **プロジェクトの開始列と完了列のプロジェクトステータスの背景色**：

   * **プロジェクトの開始列**：「実際の開始日」が入力されている場合にのみ、プロジェクトの開始列の背景が、赤色または緑色になります。

      * **プロジェクトの開始列の赤い背景色**：プロジェクトの進捗ステータスが&#x200B;**遅延**&#x200B;の場合、プロジェクトの開始列の背景は赤色で表示されます。

      * **プロジェクトの開始の列の緑の色合い**：プロジェクトの進捗ステータスが&#x200B;**オンタイム**&#x200B;の場合、プロジェクトの開始の列の背景は緑色で表示されます。

     >[!TIP]
     >
     >プロジェクトの実際の開始日を表示するには、プロジェクトの詳細ページに移動する必要があります。

   * **プロジェクトの完了列**：プロジェクトの完了列の背景は、実際の完了日が入力されている場合にのみ、赤色または緑色で表示されます。

      * **プロジェクトの完了列の赤い背景色**：プロジェクトの進捗ステータスが&#x200B;**遅延**&#x200B;の場合、プロジェクトの完了列の背景は赤色で表示されます。

      * **プロジェクトの完了列の緑の背景色**：プロジェクトの進捗ステータスが&#x200B;**オンタイム**&#x200B;の場合、プロジェクトの完了列の背景は緑色で表示されます。

     >[!TIP]
     >
     >プロジェクトの実際の完了日を表示するには、プロジェクト詳細ページに移動する必要があります。

   * タスクの進捗ステータスが「危険あり」または「遅れ」の場合、開始日と完了日の列の背景色は変わりません。

  <!--add new screen shot for preview or prod release-->

  ![マイルストーンビューの背景色](assets/milestone-view-with-shading.png)

* **プロジェクト名**：プロジェクト名が、プロジェクトへのリンクと共に表示されます。
* **プロジェクト条件アイコン**：プロジェクト名の横に、プロジェクトの条件を示すアイコンが表示されます。

  <!--
   <div class="preview">
   A condition icon in the shape of a colored circle displays next to each project in the Milestone view. The possible project conditions and circle colors are: 
   * On Target - green
   * At Risk - yellow
   * In Trouble - red
   </div>
   -->

  プロジェクトの状況は、次のいずれかになる可能性があります。

   * 目標どおり
   * リスクあり
   * トラブル発生中

## マイルストーンビューに表示する情報を設定する {#configure-what-information-displays-in-the-milestone-view}

マイルストーンビューに次の要素を表示するかどうかを設定できます。

* 進行ステータスのアイコン
* プロジェクトとタスクの完了率

デフォルトでは、プロジェクトとタスクの進捗ステータスアイコンと完了率が表示されます。

これらのオプションに対して行った変更は、自分にのみ適用され、他のユーザーは影響を受けません。変更内容は、次回Workfrontにログインしても保持されます。

プロジェクトのステータスアイコンとプロジェクトの完了率を表示するかどうかを設定するには、次の手順に従います。

{{step1-to-projects}}

1. 「**表示**」ドロップダウンメニューをクリックして、「**マイルストーン**」をクリックします。
   <!--No longer available: If you are viewing a list of projects inside a Portfolio or a Program, select the **Milestone** subtab.  -->

1. <!--In the Production environment,--> マイルストーンビューの右上隅にある「**オプション**」をクリックします。

   <!--<div class="preview">In the Preview environment, select from the options in the next step, from the upper-right corner of the Milestone view.</div>-->

   <!--at Prod release, replace this screen shot and adjust the Production/ Preview text above-->

   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. 次のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">進捗ステータス</td> 
      <td> <p>各プロジェクトとタスクの横に進捗ステータスアイコンを表示するには、このオプションを選択します。</p> <p>このオプションは、デフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了率</td> 
      <td> <p>各プロジェクトとタスクの横に完了率を表示するには、このオプションを選択します。</p> <p>このオプションは、デフォルトで有効になっています。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## マイルストーンビューでタスクの完了率を調整する {#adjust-percent-complete-for-tasks-in-the-milestone-view}

マイルストーンビューで、タスクの完了率を調整できます。親タスク（サブタスクを含むタスク）またはプロジェクトの完了率を調整することはできません。

マイルストーンビューでタスクの完了率を調整するには、次の手順を実行します。

{{step1-to-projects}}

1. 「**表示**」ドロップダウンメニューをクリックして、「**マイルストーン**」をクリックします。

1. （条件付き）完了率がマイルストーン ビューに現在表示されていない場合は、この記事の [ マイルストーン ビューに表示する情報の設定 ](#configure-what-information-displays-in-the-milestone-view) の節の説明に従って、タスクおよびプロジェクトの完了率を表示できるようにします。

1. <!--In the Production environment,--> タスクの下にある「完了率」をクリックし、新しい割合を指定して、Enter キーを押します。

   <!--<div class="preview">In the Preview environment, move the Percent Complete slide to the new percent complete to update it. </div>-->
