---
content-type: overview
product-area: projects
navigation-topic: manage-projects
title: プロジェクトの概要領域で情報を管理します。
description: プロジェクトの概要領域で情報を管理します。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6113bc62-18f2-4558-bc2f-986b1e7d1a83
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 4%

---

# プロジェクトの概要領域で情報を管理します。

<!--
<p>(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

「プロジェクトの詳細」セクションの「概要」領域にアクセスして、プロジェクトの情報を表示または編集できます。 この領域で表示または編集できるフィールドは限られています。 プロジェクトのすべての情報を編集する方法については、を参照してください。 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセス権以上の表示 </p>

<p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>プロジェクトへのアクセスを表示して、プロジェクトに関する限定的な情報を表示します</p> 
   <p>プロジェクトへのアクセスを管理して、プロジェクトに関する情報を編集します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 「概要」セクションへのアクセス

1. 「概要」セクションを表示するプロジェクトに移動します。
1. クリック **プロジェクトの詳細** をクリックします。
1. The **概要** セクションは、プロジェクトの詳細の一部として最初に表示され、デフォルトで展開される必要があります。

   または

   次をクリック： **編集** アイコン ![](assets/edit-icon.png) 「詳細」セクションの右上隅で、 **概要**. 「概要」領域が開き、編集できます。

   >[!NOTE]
   >
   >Workfrontの管理者がレイアウトテンプレートを設定した方法によっては、「概要」セクションが最初に表示されない場合があります。表示されない場合は折りたたまれます。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. （条件付き）プロジェクト上で更新する必要があるが、このセクションに表示されない特定のフィールドがある場合、 **その他のメニュー** ![](assets/more-icon.png) プロジェクト名の横に表示され、 **編集** をクリックして、さらにプロジェクトフィールドを表示します。

   プロジェクトの編集の詳細については、「 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 以下のテーブルで、「 **概要** 」セクションに入力します。\
   編集可能なフィールドを編集するには、そのフィールドをクリックするか、 **+追加** をクリックして、空のフィールドに情報を追加します。

   >[!NOTE]
   >
   >Workfrontの管理者がレイアウトテンプレートを設定した方法によっては、すべてのフィールドが表示されない場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader"><b>フィールド</b></td> 
      <td><b>説明</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader">説明</td> 
      <td>このプロジェクトの目的を説明します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>このフィールドに URL を挿入します。 Workfront URL などの URL を指定できます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先度</td> 
      <td>プロジェクトの指定された優先度または重要度として機能します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td> <p>プロジェクトのステータス。 </p> <p>ヒント：すべてのタスクと問題が完了していない限り、プロジェクトを完了することはできません。 プロジェクトの [ 完了モード ] が [ 自動 ] に設定されている場合は、手動でプロジェクトを完了することはできません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">条件タイプ</td> 
      <td>管理者がプロジェクトの条件を設定するか、Workfrontが設定するかを決定します。 プロジェクト条件の詳細については、「 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">プロジェクト条件と条件タイプの概要</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">スケジュール モード</td> 
      <td>プロジェクトのスケジュール方法を設定します。 例えば、プロジェクトが「開始日」からスケジュールされているか、「完了日」からスケジュールされているかなどです。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定開始日時</td> 
      <td> プロジェクトを開始する予定の日時。 これは、プロジェクトが開始日からスケジュールされる際に、プロジェクトマネージャが手動で設定します。 Workfrontは、プロジェクトのタスクの期間に基づいて、プロジェクトが完了日からスケジュールされる際に、この日付を自動的に設定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">計画完了日時</td> 
      <td> プロジェクトの完了が計画されている場合。 これは、プロジェクトが完了日からスケジュールされる際に、プロジェクトマネージャが手動で設定します。 Workfrontは、プロジェクトのタスクの期間に基づいて、プロジェクトが開始日からスケジュールされる日付を自動的に設定します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ポートフォリオ</td> 
      <td>プロジェクトに関連付けられたポートフォリオ。 ポートフォリオをプロジェクトに追加する前に、ポートフォリオを作成する必要があります。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プログラム</td> 
      <td>プロジェクトのポートフォリオに関連付けられたプログラム。 プログラムをプロジェクトに追加する前に、プログラムを作成する必要があります。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループ</td> 
      <td> <p>プロジェクトに関連付けられたグループ。</p> <p>適切なグループを選択していることを確認するには、グループにカーソルを移動して、情報アイコンをクリックします。 <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
      別のグループを指定しない限り、デフォルトでは、次のグループの 1 つがプロジェクトの作成時に自動的にプロジェクトに関連付けられます。
        <ul> 
         <li> <p><span>プロジェクトを「プロジェクト」領域から作成すると、プロジェクト作成者の「ホームグループ」がプロジェクトに関連付けられます。</span> </p> </li> 
         <li> <p><span>設定領域のグループのメインページからプロジェクトを作成すると、そのグループは自動的にプロジェクトに関連付けられます。</span> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">会社</td> 
      <td>プロジェクトに関連付けられた会社。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクト所有者 </td> 
      <td>これはプロジェクトの所有者です。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクトスポンサー</td> 
      <td> <p>これがプロジェクトの主な関係者です。 これは通常、エグゼクティブがプロジェクトを監視し、チャンピオンにするか、または予算上の責任を負う人です。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リソース管理者</td> 
      <td> <p>これは、プロジェクトでユーザーリソースを管理できるユーザーです。 </p> <p>リソースマネージャの詳細については、「 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">プロジェクトまたはテンプレートに対するリソースマネージャの指定 </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >「プロジェクト所有者」、「プロジェクトスポンサー」、「リソースマネージャー」の各フィールドを更新する際には、アバター、ユーザーのプライマリの役割、または電子メールアドレスに注意して、同じ名前のユーザーを区別します。
   >
   >ユーザーを追加したときに表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。
   > 
   >ユーザーがユーザーの電子メールを表示するには、アクセスレベルで [ 連絡先情報の表示 ] 設定を有効にしておく必要があります。 詳しくは、 [ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. 「概要」セクションの次のフィールドを確認します。 次のフィールドは編集できません。

   | フィールド | 説明 |
   |---|---|
   | 参照番号 | これは自動生成されたフィールドで、プロジェクトごとに常に一意の値を持ちます。 |
   | 見込み開始日 | これは、完了した作業と残りの作業に基づいて、作業を開始する「リアルタイム」の日付です。 |
   | 見込み完了日 | 完了したタスクの進捗状況と、[ 新規 ] または [ 進行中 ] のステータスのタスクの進捗状況の更新に基づいて、プロジェクトが完了する「リアルタイム」の日付です。 |
   | 予定時間数 | プロジェクトで予定されている時間。 この時間は、各タスクの計画時間の合計です。 |
   | 実際の時間数 | プロジェクトにログオンした時間。 これらの時間は、プロジェクト、タスク、またはプロジェクトの問題に関するログに記録された時間の合計です。 |
   | 予定期間 | タスクの最も早い計画開始日から、プロジェクトのタスクの最も遅い計画完了日までの期間に基づいて、プロジェクトが期間を設定します。 |
   | 実際の期間 | タスクの最も早い実績開始日から、プロジェクトの最も遅い実績完了日までの期間に基づいて、プロジェクトが実際に実行する期間を示します。 |
   | エントリ日 | プロジェクトが作成された日時。 |
   | 入力者 | プロジェクトを作成したユーザーの名前。 |
   | 最終更新日 | プロジェクトが最後に更新された日時。 |
   | 最終更新者 | プロジェクトを最後に更新したユーザーの名前。 |
   | テンプレート |   |


1. 会社がAdobe Workfront Scenario Planner の追加ライセンスを購入し、プロジェクトにリンクされたイニシアチブから公開された情報がある場合は、「シナリオプランナー」領域で次のイニシアチブ情報を確認します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>フィールド</b></td> 
      <td><b>説明</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader"><span>イニシアチブ期間</span> </td> 
      <td><span>プロジェクトがイニシアチブにリンクされている場合の、対応するイニシアチブの期間。 このフィールドは編集できません。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>最終公開日</span> </td> 
      <td><span>対応するイニシアチブからプロジェクトが最後に公開された日付。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>イニシアティブ開始日</span> </td> 
      <td><span>プロジェクトがイニシアチブにリンクされるイニシアチブの開始月の最初の日。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>イニシアティブ終了日</span> </td> 
      <td><span>プロジェクトがイニシアチブにリンクされるイニシアチブの終了月の最終日。 </span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>FTE と時間におけるイニシアチブ・ジョブの役割</span> </td> 
      <td> <p>関連するジョブの役割とイニシアチブの時間割り当てに関する情報。 これには以下が含まれます。</p> 
       <ul> 
        <li>ジョブの役割名</li> 
        <li>FTE の数</li> 
        <li> <p>すべての FTE の時間数</p> <p>時間または工数を使用して、計画またはイニシアチブに必要な役割の量を見積もることができます。 </p> <p>詳しくは、 <a href="../../../scenario-planner/create-and-edit-plans.md" class="MCXref xref">シナリオプランナーでのプランの作成と編集</a>. </p> </li> 
       </ul> <p>ヒント： <span>イニシアチブ内の月ごとにジョブの役割の数が異なる場合、このフィールドには、イニシアチブに必要な役割の最大数が表示されます。 例えば、1 月に 1 名のコンサルタントが、2 月に 2 名のコンサルタントが必要な場合、この列にはすべての月に対して、2FTE に 2 時間と、対応する 2FTE に時間が表示されます。</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   プロジェクトとイニシアチブとのリンクについて詳しくは、 [シナリオプランナーでイニシアチブを公開して、プロジェクトを更新または作成します](../../../scenario-planner/publish-scenarios-update-projects.md).

1. 「**変更を保存**」をクリックします。
