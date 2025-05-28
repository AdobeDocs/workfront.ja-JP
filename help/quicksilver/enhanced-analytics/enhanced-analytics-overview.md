---
title: 拡張分析の概要
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 拡張分析は、事前に構築されたビジュアライゼーションを備えた Adobe Workfront の強力なツールで、プロジェクトデータを調べ、計画と完了でトレンドを特定できます。このプロジェクトに関するインサイトは、現在の作業を管理するのに役立ち、将来の作業に合わせてより正確に計画できるようになります。
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 96%

---

# 拡張分析の概要

>[!IMPORTANT]
>
>Enhanced Analytics は、5 月 27 日（PT）にWorkfrontから削除されました。 Workfront Data Connect は新しい代替ソリューションであり、現在使用している Enhanced Analytics のビジュアライゼーションをレプリケートするために使用できます。 <br> 詳しくは、[Enhanced Analytics の廃止 ](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) ガイドを参照してください。


拡張分析は、事前に構築されたビジュアライゼーションを備えた Adobe Workfront の強力なツールで、プロジェクトデータを調べ、計画と完了でトレンドを特定できます。このプロジェクトに関するインサイトは、現在の作業を管理するのに役立ち、将来の作業に合わせてより正確に計画できるようになります。

拡張分析により、以下を特定しやすくなりました。

* プロジェクトの計画方法
* 作業をプロジェクトに追加するタイミング
* 様々なプロジェクトで完了する作業の量
* ホームチームがスケジュールされている時間または日数と比較して、プロジェクトの完了に必要な時間または日数
* プロジェクト中に特定のアクションを実行する頻度
* プロジェクトの進行状況と、プロジェクト内の個々のタスク

![Analytics](assets/nwe-full-screen-analytics-350x222.png)

拡張分析を使用して現在の作業を管理し、将来の作業を計画する方法について詳しくは、[拡張分析の学習パス](https://experienceleague.adobe.com/ja/docs/workfront-learn/tutorials-workfront/home)を参照してください。

## 前提条件

拡張分析領域にアクセスするには、以下が必要です。

* ビジネスプランまたはエンタープライズプランを有している。

  詳しくは、[Workfront プラン](https://business.adobe.com/products/workfront/pricing.html)を参照してください。

* Workfront 管理者に、拡張分析をレイアウトテンプレートに追加してもらいます。

  詳しくは、[拡張分析：レイアウトテンプレートに分析を追加](https://experienceleague.adobe.com/ja/docs/workfront/using/home)を参照してください。

プロジェクトおよびタスクの情報を表示するには、以下が必要です。

* アクセスレベルのプロジェクトおよびタスク領域に対する表示権限を持っている。

  Workfront 管理者がユーザーのアクセスレベルを変更する方法については、[カスタムアクセスレベルの作成または変更](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* 特定のタスクやプロジェクトの表示権限を持っている。

  追加のアクセス権のリクエストについて詳しくは、[オブジェクトへの利用申請](../workfront-basics/grant-and-request-access-to-objects/request-access.md)を参照してください。

## 拡張分析のベストプラクティス

プロジェクトに最適なデータを取得するには、正確な予定時間数と期間日数を含むテンプレートを使用します。また、ユーザーが以下のフィールドをできるだけ正確に入力し、更新する必要があります。

>[!NOTE]
>
>次に示すフィールドの一部は、ユーザーが入力した情報に基づいて Workfront が実行する計算です。これらのフィールドを手動で更新することはできません。

* 予定時間数

  これは、入力する最も重要なフィールドです。

  >[!NOTE]
  >
  >チームが予定時間数を使用していない場合でも、プロジェクト期間に基づいて一部のデータを表示できます。\
  >詳しくは、この記事の[期間ビュー](#duration-view)の節を参照してください。

* プロジェクト名

  名前は、プロジェクトを説明する名前にする必要があります。

* プロジェクト状況
* プロジェクトのステータス
* プロジェクトの予定開始日
* 予定完了日
* プロジェクトの実際の開始日
* プロジェクトの実際の完了日
* プロジェクト期間（時間）
* プロジェクトの実際の時間数
* タスクステータス（これには、タスクに「完了済み」のマークを付けることが含まれます。）
* タスク名
* タスク完了率
* タスクの予定開始日
* タスクの予定完了日

>[!IMPORTANT]
>
>タスクやプロジェクトに加えた変更が拡張分析に反映されるまでに、最大 24 時間かかる場合があります。

## 期間ビュー {#duration-view}

デフォルトでは、バーンダウンとプロジェクトツリーマップのビジュアライゼーションは、予定時間数に基づいています。チームが予定時間数を使用しない場合は、プロジェクト期間に基づいたこれらのビジュアライゼーションを確認できます。

拡張分析では、プロジェクトの期間は以下の数式で計算されます。

* 予定時間枠：

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* 稼働日数：

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >**1 日あたりの標準的な時間数**&#x200B;のデフォルトの数は 8 時間です。Adobe Workfront 管理者は、**設定**／**プロジェクト環境設定**／**プロジェクト**／**タイムライン**&#x200B;と進んで、**1 日あたりの標準的な時間数**&#x200B;の設定をアップデートすることができます。\
  >詳しくは、[システム全体のプロジェクト環境設定を指定](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

予定期間について詳しくは、[プロジェクト期間の概要](../manage-work/projects/planning-a-project/project-duration.md)を参照してください。

## キーボードショートカット

キーボードの以下のキーを使用して、拡張分析エリアで特定のアクションを移動または完了できます。

| キー | アクション |
|---|---|
| **タブ** | ページ上のそれぞれの要素に移動します。また、ページに表示されないそれぞれのビジュアライゼーションに関する情報を含むテーブルにも移動します |
| **入力** | カレンダーウィジェットを開き、既存のフィルターを削除し、「フィルターを追加」オプションを開き、フィルターの値を選択または選択解除し、作成したフィルターを適用し、各ビジュアライゼーションの「書き出し」オプションを開き、さらにバーンダウン、作業中のタスク、プロジェクトツリーマップのビジュアライゼーションのドロップダウンメニューを開きます。 |
| **矢印キー** | フィルターの追加の場合は「フィルター」オプションで、ビジュアライゼーションの場合はすべてのドロップダウンメニューのオプションで、カレンダーウィジェットの日付に移動します。 |
| **スペースバー** | カレンダーウィジェットで日付を選択し、フィルターを追加する場合はフィルタータイプを選択し、各ビジュアライゼーションのドロップダウンメニューから「書き出し」オプションを選択し、さらにバーンダウン、作業中のタスク、プロジェクトツリーマップのビジュアライゼーションのドロップダウンメニューからオプションを選択 |

{style="table-layout:auto"}

スクリーン読み上げソフトウェアまたはプラグインを使用している場合、スクリーンリーダーは画面上の情報を音読し、上記のキーを使用して実行する操作を説明します。

## 拡張分析のビューおよび機能

拡張分析内の特定の機能や、詳細なインサイトを得るために実行できるアクション、このデータから学習できる内容に関する詳細情報は、以下の記事を参照してください。

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
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">拡張分析にフィルターを適用</a> </td> 
   <td> <p>カスタムフィルター、プロジェクトフィールドフィルターやチームフィルターを適用して、特定の条件に適合するプロジェクトのみを表示できます。フィルターを追加すると、それに応じてプロジェクトの数がアップデートされます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">拡張分析 KPI について</a> </td> 
   <td> <p>特定の期間内のすべてのプロジェクトの主要パフォーマンス指標（KPI）は、画面の上部に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">拡張機能での進行計画ビジュアライゼーションの表示</a> </p> </td> 
   <td> <p><b>進行計画</b>ビジュアライゼーションは、プロジェクトのライフサイクル中に状況が変化したことを示します。ビジュアライゼーションを操作すると、特定の日付に関する詳細が表示されます。プロジェクトを選択すると、「作業中のタスク」および「バーンダウン」ビジュアライゼーションが開きます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">拡張分析でバーンダウンビジュアライゼーションを表示</a> </td> 
   <td> <p><b>バーンダウン</b>ビジュアライゼーションは、プロジェクトに費やした実際の時間数と比較した、プロジェクトの予定速度を示します。ビジュアライゼーションを操作すると、特定の日付のプロジェクトの状態に関する詳細が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">拡張分析での「作業中のタスク」ビジュアライゼーションの表示</a> </td> 
   <td> <p><b>実行中のタスク</b>ビジュアライゼーションは、プロジェクト内の各タスクのステータスを示します。ビジュアライゼーションを操作すると、タスクをすばやく簡単に変更できます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">拡張分析でプロジェクトアクティビティのビジュアライゼーションを表示</a> </td> 
   <td> <p><b>プロジェクトアクティビティ</b>ビジュアライゼーションには、プロジェクトに割り当てられたユーザーが Workfront にログインした時、そのプロジェクトのタスクのステータスを変更した時、そのプロジェクトのタスクを完了し時のヒートマップが表示されます。ビジュアライゼーションを操作すると、各ユーザーに関するこれらの詳細を表示できます。また、これらのアクションの特定の日付や、各アクションが完了した回数を確認することもできます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">拡張分析でプロジェクトツリーマップビジュアライゼーションを表示</a> </td> 
   <td> <p><b>プロジェクトツリーマップ</b>ビジュアライゼーションは、他のプロジェクトと比較して、一部のプロジェクトにどれだけの時間が費やされたかを示します。ビジュアライゼーションを操作すると、プロジェクトの状態、プロジェクトの予定完了日、プロジェクトの実際の完了日に関する詳細が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">拡張分析でチームごとのアクティビティのビジュアライゼーションを表示</a> </td> 
   <td> <p><b>チームごとのアクティビティ</b>ビジュアライゼーションには、ホームチームのユーザーが Workfront にログインし、タスクのステータスを変更し、タスクを完了したときのヒートマップが表示されます。ビジュアライゼーションを操作すると、個々のユーザーに関するこれらの詳細を表示できます。また、これらのアクションの特定の日付や、各アクションが完了した回数を確認することもできます。</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>
