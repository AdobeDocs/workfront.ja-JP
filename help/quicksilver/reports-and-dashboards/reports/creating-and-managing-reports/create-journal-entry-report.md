---
title: 更新エリアに関するレポート
description: ジャーナルエントリレポートには、これまで Adobe Workfront API を介してのみ利用可能であった、プロジェクト、タスク、イシューなどのオブジェクトの更新エリアからのシステム更新が表示されます。これは特定のユースケースを対象とした高度なレポートですが、よりわかりやすい形式により、Workfront 内のプロジェクトアクティビティやシステム更新に関するレポートを簡単に作成できるようになります。
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 94c2930d155f38a56fe36e5a09bd29f27d1593f0
workflow-type: tm+mt
source-wordcount: '2765'
ht-degree: 89%

---

# 更新エリアに関するレポート

ジャーナルエントリレポートには、これまで Adobe Workfront API を介してのみ利用可能であった、プロジェクト、タスク、イシューなどのオブジェクトの更新エリアからのシステム更新が表示されます。これは特定のユースケースを対象とした高度なレポートですが、よりわかりやすい形式により、Workfront 内のプロジェクトアクティビティやシステム更新に関するレポートを簡単に作成できるようになります。

>[!TIP]
>
>ジャーナルエントリレポートには、オブジェクトの更新エリアからのシステム更新のみが含まれます。更新エリアに残されたコメントに関するレポートを作成するには、「メモ」レポートを使用する必要があります。\
>メモレポートについて詳しくは、[メモレポートでのすべての更新の表示](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md)を参照してください。

ジャーナルエントリレポートには、次の情報が表示されます。

* ステータスの変更が発生した回数
* タスクまたはイシューがいつ削除されたか
* 重要なカスタムフィールドの値が、プロジェクトのライフサイクルの過程でどのように変化したか
* プロジェクトのライフサイクルの過程で変更された重要な日付
* プロジェクトの所有者が変更されたかどうか

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>新規：標準 </p><p>または </p><p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに表示するジャーナルエントリを含んだオブジェクトの表示権限</p> <p>レポートの管理権限は、レポートの作成後に取得されます</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

この記事で説明している操作を実行する前に、次の点を確認する必要があります。

* レポートの対象となるフィールドはすべて Workfront で追跡されていること。追跡されている更新エリアのデータのみをレポートできます。

  Workfront で追跡するフィールドの追加方法については、[システム更新の設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)を参照してください。

* レポートの対象となるすべてのカスタムフィールドで「**更新フィードにフィールド変更を表示**」の設定が有効になっていること。

  カスタムフィールドに対してこの設定を有効にする方法については、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#).

## ジャーナルエントリレポートの概要

ジャーナルエントリレポートは、システム更新をクエリするので、かなりの数の結果を返す可能性があります。そのため、レポートを作成する際は、プロジェクト、プログラム、ポートフォリオ、グループなどの特定のオブジェクトに絞り込むことをお勧めします。

Workfront の様々なオブジェクトタイプについて詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)を参照してください。

>[!NOTE]
>
>ジャーナルエントリレポートは非常にたくさんのデータを返すので、書き出しとスケジュール済みレポートの配信はサポートされていません。

このレポートのデフォルトビューには、次の列が含まれています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>フィールド</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>フィールド名</strong> </td> 
   <td> <p><span style="font-weight: normal;">影響を受けるフィールドの名前。レポートの設定方法に応じて、「ステータス」、「所有者 ID」、「タスク名」、「予定完了日」などのフィールドがこの列に含まれます。</span> </p> <p><span style="font-weight: normal;"></span><strong>DE</strong>:<span style="font-weight: normal;"> がこの列に表示される場合は、一覧表示されているフィールドがカスタムフィールドであることを示します。</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>変更の種類</strong> </td> 
   <td> <p>影響を受けるフィールドに加えられた変更のタイプ。設定したフィルタールールと、ユーザーが実行したアクションに応じて、このフィールドに次のように表示されます。</p> 
    <ul> 
     <li> <p>追加</p> </li> 
     <li> <p>監査</p> </li> 
     <li> <p>削除</p> </li> 
     <li> <p>ダイジェスト</p> </li> 
     <li> <p>編集</p> </li> 
     <li> <p>復元</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>トップ ObjCode</strong> </td> 
   <td> <p>階層内の最上位の親オブジェクト。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>範囲</strong> </td> 
   <td> <p>変更されたオブジェクトのタイプ。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>エントリ日</strong> </td> 
   <td> <p>フィールドが変更された日付。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>編集者名</strong> </td> 
   <td> <p>フィールドを変更したユーザー。</p> </td> 
  </tr> 
 </tbody> 
</table>

このレポートの情報を整理するには、プロジェクトと呼ばれる組み込みのグループを使用します。 プロジェクトのグループ化では、プロジェクト名がプライマリ、エントリ日がセカンダリにグループ化されます。この既存のグループ化は、レポートの作成時に適用することも、レポートの表示時に適用することもできます。

レポートの表示、フィルター、グループを設定する方法については、次の関連する節を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [ステータスの変更の発生状況を確認する](#see-what-status-changes-occurred)
* [タスクまたはイシューが削除された日時を確認する](#see-when-a-task-or-issue-was-deleted)
* [プロジェクトのライフサイクルの過程でカスタムフィールドがどのように変化したかを確認する](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [予定完了日がプロジェクトのライフサイクルの過程でどのように変更されたかを確認する](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [プロジェクトの所有者が変更されたかどうかを確認する](#see-if-the-owner-of-a-project-changed)

## ステータスの変更の発生状況を確認する {#see-what-status-changes-occurred}

次の項目を表示するジャーナルエントリレポートを設定できます。

* プロジェクト、タスク、またはイシューに対して行われたステータスの変更の数

* 変更前のステータス
* ステータスを変更したユーザー
* ステータスの変更が発生した日時

プロジェクトの正常性を確認する場合は、プロジェクトの「**条件**」フィールドを使用して、これと同じ情報を表示するようにレポートを設定することもできます。

この情報は、監査に役立ち、お客様とお客様の組織がどの程度計画を立てているかを説明するために使用できます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>条件の変更間の日数の差を比較する場合は、拡張分析を使用できます。\
>拡張分析について詳しくは、[拡張分析の概要](../../../enhanced-analytics/enhanced-analytics-overview.md)を参照してください。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅で、「 **レポート**.
1. 「**新規レポート**」をクリックしてから、「**ジャーナルエントリ**」を選択します。

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder が読み込まれます。

1. 「**列（表示）**」タブで、以下の列を追加します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">フィールド名</p> </td> 
      <td> <p>影響を受けるフィールドの名前。この場合、<strong>ステータス</strong>がこの列に表示される必要があります。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">変更タイプ</p> </td> 
      <td> <p>影響を受けるフィールドに加えられた変更のタイプ（例：<strong>追加</strong>、<strong>削除</strong>、<strong>編集</strong>）。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">編集者名</p> </td> 
      <td> <p>ステータスを更新したユーザーの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">エントリ日</p> </td> 
      <td> <p>ステータスが変更された日付。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">古いテキスト値</p> </td> 
      <td> <p>前のステータスのキー。デフォルトのプロジェクトステータスのステータスキーは次のとおりです。</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>：現在</p> </li> 
        <li> <p><strong>DED</strong>：無効</p> </li> 
        <li> <p><strong>ONH</strong>：保留中</p> </li> 
        <li> <p><strong>PLN</strong>：計画</p> </li> 
        <li> <p><strong>CPL</strong>：完了</p> </li> 
        <li> <p><strong>REQ</strong>：リクエスト済み</p> </li> 
        <li> <p><strong>APR</strong>：承認済み</p> </li> 
        <li> <p><strong>REJ</strong>：却下</p> </li> 
        <li> <p><strong>IDA</strong>：アイデア</p> </li> 
       </ul> <p>組織がカスタムステータスを設定している場合、この列に他のステータスキーが表示されることがあります。ステータスキーに関連するカスタムステータスについては、Workfront の管理者またはグループ管理者に問い合わせてください。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新規テキスト値</p> </td> 
      <td> <p>更新されたステータスのキー。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">上位 ObjCode</p> </td> 
      <td> <p>ステータスが変更されたフィールドの最上位の親オブジェクト。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">範囲</p> </td> 
      <td> <p>ステータスが変更されたオブジェクトのタイプ。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">イシュー名<br>（オプション）</p> </td> 
      <td> <p>ステータスが変更されたイシューの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">タスク名<br>（オプション）</p> </td> 
      <td> <p>ステータスが変更されたタスクの名前。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   列の追加について詳しくは、[Adobe Workfront の概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

1. Adobe Analytics の「**フィルター**」タブで、「**フィルタールールを追加**」をクリックし、フィルタールール「**フィールド名**／**次と等しい**／**ステータス**」追加します。

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >条件の変更に関するレポートを作成する場合は、代わりにフィルタールール「**フィールド名**／**次と等しい**／**条件**」を追加できます。

   フィルターの追加について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （オプション）レポートの焦点を絞り、読み込み時間を短縮するには、プロンプトを追加します。

   または

   特定のプロジェクト、タスクまたはイシューを含めるための追加のフィルタールールを作成します。

   >[!IMPORTANT]
   >
   >修飾子&#x200B;**次を含む**&#x200B;を使用するフィルタールールを作成すると、実際に読み込み時間が増加することがあります。そのため、特定のプロジェクトまたは上位のオブジェクト ID を対象にフィルタリングできる場合、**が次に等しい**&#x200B;などの異なる修飾子を使用することをお勧めします。

   プロンプトを追加する方法については、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

1. 「**グループ化**」タブで、「**既存のグループ化を適用**」をクリックし、「**プロジェクト**」を選択します。

   グループ化の追加について詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   新しいレポートが読み込まれます。

## タスクやイシューが削除された日時を表示 {#see-when-a-task-or-issue-was-deleted}

次の項目を表示するジャーナルエントリレポートを設定できます。

* 削除されたタスクまやイシュー
* タスクやイシューを削除したユーザー

タスクやイシューがいつ削除されたかを確認するには、以下のように行います。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅で、「 **レポート**.
1. 「**新規レポート**」をクリックしてから、「**ジャーナルエントリ**」を選択します。

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder が読み込まれます。

1. 「**列（表示）**」タブで、以下の列を追加します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">範囲</p> </td> 
      <td> <p>削除されたオブジェクトのタイプ。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">変更タイプ</p> </td> 
      <td> <p>発生した変更のタイプ。<strong>削除</strong>変更がこの列に表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">エントリ日</p> </td> 
      <td> <p>タスクやイシューが削除された日付。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">編集者名</p> </td> 
      <td> <p>タスクやイシューを削除したユーザーの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">プロジェクト名</p> </td> 
      <td> <p>タスクやイシューが削除されたプロジェクトの名前。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   列の追加について詳しくは、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

1. Adobe Analytics の **フィルター** タブ、クリック **フィルタールールを追加**&#x200B;次のフィルターを追加します。

   * **変更の種類**／**が次に等しい**／**削除**
   * **プロジェクト ID**／**が次に等しい**／**`<project>`**

     <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->

   フィルターの追加について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （オプション）レポートの焦点を絞り、読み込み時間を短縮するには、プロンプトを追加します。

   または

   特定のプロジェクト、タスクまたはイシューを含めるための追加のフィルタールールを作成します。

   >[!IMPORTANT]
   >
   >修飾子&#x200B;**次を含む**&#x200B;を使用するフィルタールールを作成すると、実際に読み込み時間が増加することがあります。そのため、特定のプロジェクトまたは上位のオブジェクト ID を対象にフィルタリングできる場合、**が次に等しい**&#x200B;などの異なる修飾子を使用することをお勧めします。

   プロンプトを追加する方法については、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

1. （オプション）「**グループ化**」タブで、「**既存のグループ化を適用する**」をクリックしたあと、「**プロジェクト**」を選択します。

   グループ化の追加について詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   新しいレポートが読み込まれます。

## プロジェクトのライフサイクルの過程でカスタムフィールドがどのように変化したかを確認 {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

プロジェクトの過程での重要なフィールドの変更を追跡できます。それには、追跡するジャーナルエントリを次のように設定します。

* 特定のカスタムフィールドが追加、更新または編集されたかどうか
* これらの変更がいつ発生したか
* 誰が変更を加えたか

プロジェクトのライフサイクルの過程でカスタムフィールドがどのように変化したかを確認するには、次の手順に従います。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅で、「 **レポート**.
1. 「**新規レポート**」をクリックしてから、「**ジャーナルエントリ**」を選択します。

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder が読み込まれます。

1. 「**列（表示）**」タブで、以下の列を追加します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">フィールド名</p> </td> 
      <td> <p>影響を受けるカスタムフィールドの名前。</p> <p><span style="font-weight: normal;"></span><strong>DE</strong>:<span style="font-weight: normal;"> がこの列に表示される場合は、一覧表示されているフィールドがカスタムフィールドであることを示します。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">変更タイプ</p> </td> 
      <td> <p>影響を受けるフィールドに加えられた変更のタイプ（例：<strong>追加</strong>、<strong>削除</strong>、<strong>編集</strong>）。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">編集者名</p> </td> 
      <td> <p>カスタムフィールドを更新したユーザーの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">エントリ日</p> </td> 
      <td> <p>カスタムフィールドの値が変更された日付。</p> <p>このフィールドは降順で並べ替える必要があります。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">古い数値</p> </td> 
      <td> <p>カスタムフィールドの前の数値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新規数値</p> </td> 
      <td> <p>カスタムフィールドの現在の数値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">古い日付値</p> </td> 
      <td> <p>カスタムフィールドの前の日付値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新規日付値</p> </td> 
      <td> <p>カスタムフィールドの現在の日付値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">古いテキスト値</p> </td> 
      <td> <p>カスタムフィールドの前のテキスト値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新規テキスト値</p> </td> 
      <td> <p>カスタムフィールド内の現在のテキスト値。</p> <p>カスタムフィールドが typeahead フィールドの場合、「<strong>新しいテキスト値</strong>」列にはオブジェクト ID が表示されます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   列の追加について詳しくは、[Adobe Workfront の概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

1. Adobe Analytics の **フィルター** タブ、クリック **フィルタールールを追加**&#x200B;次のフィルターを追加します。

   * **ジャーナルエントリフィールド名**／**次を含む**／**DE**

     >[!TIP]
     >
     >このレポートを特定のカスタムフィールドに限定するには、フィルタールール「**ジャーナルエントリフィールド名**／**次と等しい**／**`<custom field>`**」を追加します。

   * **プロジェクト ID**／**次と等しい**／**`<project>`**

     ![](assets/qs-custom-form-changes-filter-350x92.png)

   フィルターの追加について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （オプション）レポートの焦点を絞り、読み込み時間を短縮するには、プロンプトを追加します。

   または

   特定のプロジェクト、タスクまたはイシューを含めるための追加のフィルタールールを作成します。

   >[!IMPORTANT]
   >
   >修飾子&#x200B;**次を含む**&#x200B;を使用するフィルタールールを作成すると、実際に読み込み時間が増加することがあります。そのため、特定のプロジェクトまたは上位のオブジェクト ID を対象にフィルタリングできる場合、**が次に等しい**&#x200B;などの異なる修飾子を使用することをお勧めします。

   プロンプトを追加する方法については、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

1. 「**グループ化**」タブで、「**既存のグループ化を適用**」をクリックし、「**プロジェクト**」を選択します。

   グループ化の追加について詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   新しいレポートが読み込まれます。

## 予定完了日がプロジェクトのライフサイクルの過程でどのように変更されたかを確認する {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

ジャーナルエントリレポートを設定して、プロジェクトの存続エントリ予定完了日が変更される頻度を表示できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅で、「 **レポート**.
1. 「**新規レポート**」をクリックしてから、「**ジャーナルエントリ**」を選択します。

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder が読み込まれます。

1. 「**列（表示）**」タブで、以下の列を追加します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">フィールド名</p> </td> 
      <td> <p>影響を受けるフィールドの名前。</p> <p><span style="font-weight: normal;">この列に「</span> <strong>DE</strong>:<span style="font-weight: normal;">」と表示されている場合は、リストに表示されているフィールドがカスタムフィールドであることを示します。</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">変更タイプ</p> </td> 
      <td>影響を受けるフィールドに加えられた変更のタイプ（例：<strong>追加</strong>、<strong>削除</strong>、<strong>編集</strong>）。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">編集者名</p> </td> 
      <td> <p>プロジェクトの計画完了日を更新したユーザーの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">エントリ日</p> </td> 
      <td> <p>プロジェクトの予定完了日が変更された日付。</p> <p>このフィールドは降順で並べ替える必要があります。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">上位 ObjCode</p> </td> 
      <td> <p>「予定完了日」が変更されたフィールドの最も高い親オブジェクト。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">範囲</p> </td> 
      <td> <p>予定完了日が変更されたオブジェクト。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">古い日付値</p> </td> 
      <td> <p>予定完了日の前の値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">新規日付値</p> </td> 
      <td> <p>予定完了日の現在の値。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">プロジェクト名</p> <p>（オプション）</p> </td> 
      <td> <p>予定完了日が変更されたプロジェクトの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">タスク名</p> <p>（オプション）</p> </td> 
      <td> <p>予定完了日が変更されたプロジェクト内のタスクの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">イシュー名</p> <p>（オプション）</p> </td> 
      <td>予定完了日が変更されたプロジェクト内のイシューの名前。</td> 
     </tr> 
    </tbody> 
   </table>

   列の追加の詳細情報については、「[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)」を参照してください。

1. 「**フィルター**」タブで、「**フィルタールールを追加**」をクリックし、以下を追加します。

   * **フィールド名**／**次と等しい**／**日付**
   * **プロジェクト ID**／**次と等しい**／**`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   フィルターの追加について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （オプション）レポートの焦点を絞り、読み込み時間を短縮するには、プロンプトを追加します。

   または

   特定のプロジェクト、タスクまたはイシューを含めるための追加のフィルタールールを作成します。

   >[!IMPORTANT]
   >
   >修飾子&#x200B;**次を含む**&#x200B;を使用するフィルタールールを作成すると、実際に読み込み時間が増加することがあります。そのため、特定のプロジェクトまたは上位のオブジェクト ID を対象にフィルタリングできる場合、**が次に等しい**&#x200B;などの異なる修飾子を使用することをお勧めします。

   プロンプトを追加する方法については、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

1. 「**グループ化**」タブで、「**既存のグループ化を適用**」をクリックし、「**プロジェクト**」を選択します。

   グループ化の追加について詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   新しいレポートが読み込まれます。

## プロジェクトの所有者が変更されたかどうかを確認する {#see-if-the-owner-of-a-project-changed}

ジャーナルエントリレポートを設定して、プロジェクトの存続期間中にプロジェクト所有者（またはプロジェクトマネージャー）が何回変更されたかを表示できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅で、「 **レポート**.
1. 「**新規レポート**」をクリックしてから、「**ジャーナルエントリ**」を選択します。

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder が読み込まれます。

1. 「**列（表示）**」タブで、以下の列を追加します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>列</th> 
      <th>説明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">フィールド名</p> </td> 
      <td>影響を受けるフィールドの名前。<strong>ownerID</strong> がこの列に表示されます。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">変更タイプ</p> </td> 
      <td> <p>影響を受けるフィールドに加えられた変更のタイプ（例：<strong>追加</strong>、<strong>削除</strong>、<strong>編集</strong>）。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">上位 ObjCode</p> </td> 
      <td> <p>プロジェクト所有者が更新したプロジェクトの最上位の親オブジェクト。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">エントリ日</p> </td> 
      <td>プロジェクト所有者が変更された日付。<br>このフィールドは降順で並べ替える必要があります。</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">編集者名</p> </td> 
      <td> <p>プロジェクト所有者を更新したユーザーの名前。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">追加情報 1</p> </td> 
      <td> <p>プロジェクトの現在のプロジェクト所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">追加情報 2</p> </td> 
      <td> <p>プロジェクトの前のプロジェクト所有者。</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">プロジェクト名</p> </td> 
      <td> <p>「プロジェクト所有者」フィールドが更新されたプロジェクト。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   列の追加について詳しくは、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

1. 「**フィルター**」タブで、「**フィルタールールを追加**」をクリックし、以下を追加します。

   * **フィールド名**／**次と等しい**／**ownerID**
   * **プロジェクト ID**／**次と等しい**／**`<project name>`**

     ![](assets/qs-owner-changes-filter-350x94.png)

   フィルターの追加について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （オプション）レポートの焦点を絞り、読み込み時間を短縮するには、プロンプトを追加します。

   または

   特定のプロジェクト、タスクまたはイシューを含めるための追加のフィルタールールを作成します。

   >[!IMPORTANT]
   >
   >修飾子&#x200B;**次を含む**&#x200B;を使用するフィルタールールを作成すると、実際に読み込み時間が増加することがあります。そのため、特定のプロジェクトまたは上位のオブジェクト ID を対象にフィルタリングできる場合、**が次に等しい**&#x200B;などの異なる修飾子を使用することをお勧めします。

   プロンプトを追加する方法については、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

1. （オプション）「**グループ化**」タブで、「**既存のグループ化を適用する**」をクリックしたあと、「**プロジェクト**」を選択します。

   グループ化の追加について詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   新しいレポートが読み込まれます。
