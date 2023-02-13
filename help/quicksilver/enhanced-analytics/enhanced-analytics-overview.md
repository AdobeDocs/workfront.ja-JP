---
title: 分析の強化の概要
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 拡張分析は、事前に構築されたビジュアライゼーションを備えたAdobe Workfrontの強力なツールで、プロジェクトデータを調べ、計画と完了を通じてトレンドを特定できます。 このプロジェクトのインサイトは、現在の作業を管理するのに役立ち、将来の作業に合わせてより正確に計画できます。
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# 分析の強化の概要

拡張分析は、事前に構築されたビジュアライゼーションを備えたAdobe Workfrontの強力なツールで、プロジェクトデータを調べ、計画と完了を通じてトレンドを特定できます。 このプロジェクトのインサイトは、現在の作業を管理するのに役立ち、将来の作業に合わせてより正確に計画できます。

Analytics の機能強化により、以下を特定しやすくなりました。

* プロジェクトの計画方法
* 作業がプロジェクトに追加されたとき
* 異なるプロジェクトで完了する作業の量
* ホームチームがスケジュールされる時間または日数と比較して、プロジェクトの完了に必要な時間または日数
* プロジェクト中に特定のアクションを実行する頻度
* プロジェクトの進行状況と、プロジェクト内の個々のタスク

![](assets/nwe-full-screen-analytics-350x222.png)

拡張分析を使用して現在の作業を管理し、将来の作業を計画する方法について詳しくは、 [Analytics 学習パスの強化](https://one.workfront.com/s/enhanced-analytics-program).

## 前提条件

拡張分析領域にアクセスするには、次の操作が必要です。

* ビジネスプランまたはエンタープライズプランを用意している。

   詳しくは、 [Workfrontプラン](https://www.workfront.com/plans).

* Workfront管理者に、Enhanced Analytics をレイアウトテンプレートに追加してもらいます。

   詳しくは、 [Analytics の強化：レイアウトテンプレートへの分析の追加](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

プロジェクトおよびタスクの情報を表示するには、次の操作を行う必要があります。

* アクセスレベルのプロジェクトおよびタスク領域に対する表示権限を持っている。

   Workfront管理者がアクセスレベルを変更する方法について詳しくは、 [カスタムアクセスレベルの作成または変更](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 特定のタスクやプロジェクトの表示権限を持っている。

   追加のアクセス権のリクエストについて詳しくは、 [オブジェクトへのアクセスのリクエスト](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## 拡張分析のベストプラクティス

プロジェクトに最適なデータを取得するには、正確な計画時間と期間の日数を持つテンプレートを使用します。 また、ユーザーが以下のフィールドをできるだけ正確に入力し、更新する必要があります。

>[!NOTE]
>
>次に示すフィールドの一部は、ユーザーが入力した情報に基づいてWorkfrontが実行する計算です。 これらのフィールドは手動で更新できません。

* 予定時間数

   これは、入力する最も重要なフィールドです。

   >[!NOTE]
   >
   >チームが予定時間を使用しない場合でも、プロジェクト期間に基づくデータを表示できます。\
   >詳しくは、 [期間表示](#duration-view) 」を参照してください。

* プロジェクト名

   名前は、プロジェクトの内容を説明する名前にする必要があります。

* プロジェクト状況
* プロジェクト状態
* プロジェクト計画開始日
* 予定完了日
* プロジェクトの実績開始日
* プロジェクトの実績終了日
* プロジェクト期間時間
* プロジェクトの実績時間
* タスクステータス（「完了済」のマークタスクを含む）
* タスク名
* タスク完了率
* タスクの予定開始日
* タスクの予定完了日

>[!IMPORTANT]
>
>タスクやプロジェクトに加えた変更が Enhanced Analytics に反映されるまでに、最大 24 時間かかる場合があります。

## 期間表示 {#duration-view}

デフォルトでは、バーンダウンとプロジェクトツリーマップのビジュアライゼーションは、予定時間に基づいています。 チームが予定時間を使用しない場合は、プロジェクトの期間に基づいて、これらのビジュアライゼーションを表示できます。

Enhanced Analytics では、プロジェクトの期間は次の数式で計算されます。

* 予定時間枠:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* 稼働日数:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8 時間がデフォルトの **1 日あたりの通常の時間**. Adobe Workfront管理者は、 **1 日あたりの通常の時間** 下に置く **設定** > **プロジェクト環境設定** > **プロジェクト** > **タイムライン**.\
   >詳しくは、 [システム全体のプロジェクト環境設定の指定](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

計画期間について詳しくは、 [プロジェクト期間の概要](../manage-work/projects/planning-a-project/project-duration.md).

## キーボードショートカット

キーボードの次のキーを使用して、拡張分析領域で特定のアクションを移動または完了できます。

| キー | アクション |
|---|---|
| **タブ** | ページ上の各要素に移動し、ページに表示されない各ビジュアライゼーションに関する情報を含むテーブルに移動します |
| **入力** | カレンダーウィジェットを開き、既存のフィルターを削除し、フィルター値を追加/選択解除、作成したフィルターの適用、各ビジュアライゼーションの書き出しオプションの開閉、Burndown、Tasks in flight、Project treemap ビジュアライゼーションのドロップダウンメニューの開閉 |
| **矢印キー** | カレンダーウィジェットの日付、フィルターの追加時のフィルターオプション、ビジュアライゼーションのすべてのドロップダウンメニューのオプションに移動します |
| **スペースバー** | カレンダーウィジェットで日付を選択し、フィルターを追加する際にフィルタータイプを選択し、各ビジュアライゼーションのドロップダウンメニューからエクスポートオプションを選択し、バーンダウン、フライト中のタスク、プロジェクトツリーマップビジュアライゼーション |

{style=&quot;table-layout:auto&quot;}

読み上げソフトウェアまたはプラグインを使用している場合、スクリーンリーダーは画面上の情報を読み上げ、上記のキーを使用して実行する操作を説明します。

## 分析のビューと機能の強化

拡張分析内の特定の機能の詳細、詳細なインサイトを得るために実行できるアクション、このデータから学習できる内容について詳しくは、次の記事を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>記事</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">拡張分析でのフィルターの適用</a> </td> 
   <td> <p>カスタムフィルタ、プロジェクトフィールドフィルタ、またはチームフィルタを適用して、特定の条件に適合するプロジェクトのみを表示できます。 フィルターを追加すると、それに応じてプロジェクトの数が更新されます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">拡張分析 KPI の理解</a> </td> 
   <td> <p>特定の期間内のすべてのプロジェクトの主要業績評価指標 (KPI) は、画面の上部に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">Enhanced Analytics でのフライトプランビジュアライゼーションの表示</a> </p> </td> 
   <td> <p>この <b>フライトプラン</b> ビジュアライゼーションは、プロジェクトの存続期間中に条件が変化したことを示します。 ビジュアライゼーションを操作すると、特定の日付に関する詳細が表示されます。 プロジェクトを選択すると、フライトビジュアライゼーションのバーンダウンとタスクが開きます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">拡張分析でのバーンダウンビジュアライゼーションの表示</a> </td> 
   <td> <p>この <b>バーンダウン</b> ビジュアライゼーションは、プロジェクトに費やした実際の時間数と比較した、プロジェクトの計画速度を示します。 ビジュアライゼーションを操作すると、特定の日付のプロジェクトの条件に関する詳細が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">Enhanced Analytics でのフライトビジュアライゼーションでのタスクの表示</a> </td> 
   <td> <p>この <b>進行中のタスク</b> ビジュアライゼーションは、プロジェクト内の各タスクのステータスを表示します。 ビジュアライゼーションを操作すると、タスクをすばやく簡単に変更できます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">拡張分析でのプロジェクトアクティビティのビジュアライゼーションの表示</a> </td> 
   <td> <p>この <b>プロジェクトアクティビティ</b> ビジュアライゼーションには、ユーザーがWorkfrontにログインし、そのプロジェクトのタスクのステータスを変更した日時、そのプロジェクトで完了したタスクのヒートマップが表示されます。 ビジュアライゼーションを操作すると、各ユーザーに関するこれらの詳細を表示できます。 また、これらのアクションの特定の日付や、各アクションが完了した回数を確認することもできます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">拡張分析でのプロジェクトツリーマップビジュアライゼーションの表示</a> </td> 
   <td> <p>この <b>プロジェクトツリーマップ</b> ビジュアライゼーションは、一部のプロジェクトに費やした時間と他のプロジェクトに費やした時間を示します。 ビジュアライゼーションを操作すると、プロジェクトの状態、計画されたプロジェクトの完了、実際のプロジェクトの完了に関する詳細が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">Enhanced Analytics でのチーム別アクティビティのビジュアライゼーションの表示</a> </td> 
   <td> <p>この <b>チーム別アクティビティ</b> ビジュアライゼーションには、ホームチームのユーザーがWorkfrontにログインし、タスクのステータスを変更し、タスクを完了した日時のヒートマップが表示されます。 ビジュアライゼーションを操作すると、個々のユーザーに関するこれらの詳細を表示できます。 また、これらのアクションの特定の日付や、各アクションが完了した回数を確認することもできます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">拡張分析でのリソース容量ビジュアライゼーションの表示</a> </td> 
   <td> <p>この <b>リソース容量</b> ビジュアライゼーションは、どのホームチームがより多くの作業を引き受ける能力を持っているか、およびどのホームチームが完了する以上の作業を割り当てているかを示します。 ビジュアライゼーションを操作すると、完了した作業に関する詳細や、その他の作業に使用できる時間を確認できます。 チームを選択すると、チームの能力ビジュアライゼーションが開きます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">拡張分析でのチーム容量ビジュアライゼーションの表示</a> </td> 
   <td> <p>この <b>チームの能力</b> ビジュアライゼーションは、割り当てられた作業量のうち、ホームチームが完了した作業量の割合を示します。 ビジュアライゼーションを操作すると、特定の日付の予定時間と予定時間、容量の割合、およびホームチームがその日の容量を超えたか、下回ったか、または達成したかを確認できます。</p> </td> 
  </tr> 
 </tbody> 
</table>
