---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新セクションの概要
description: オブジェクトの「更新」セクションには、オブジェクトに対してユーザーが行ったコメント、またはオブジェクトの変更をトラックするシステム更新が表示されます。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 158af1f48fba264b98108b5f0a573b7904eb875e
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 72%

---


# 「更新」セクションの概要

<!-- Audited: 1/2024 -->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

オブジェクトの「更新」セクションには、オブジェクトに対してユーザーが行ったコメント、またはオブジェクトの変更をトラックするシステム更新が表示されます。

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process.
-->

## 「更新」セクションの概要

オブジェクトの「更新」セクションには、システムの更新と、ユーザーが過去 90 日以内に行った最新の更新のうち最大 200 件が表示されます。

![「更新」セクション](assets/updates-tab-with-unified-experience-for-issues-all-tab.png)

<!--Info for April 11: Add the following right under the screen shot above:-->

次のオブジェクトには、コメントを追加したりシステムの更新を確認したりできる「更新」セクションがあります。

* プロジェクト
* タスク
* イシュー
* プログラム
* ポートフォリオ
* テンプレート
* テンプレートタスク
* ユーザー
* タイムシート
* チーム
* Goals
* イテレーション

次のオブジェクトには、コメントを追加したり、システムの更新を確認できる領域があります。

* ボード上のカード
* Workfront Planning のレコード

<!--info for April 11: remove all the information below, all the way down to the following section: -->

<!--
Depending on what objects you access the commenting experience for, you might find the following experience for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

  * Project
  * Task (this includes Stories)
  * Issue
  * Document

    >[!TIP]
    >
    >Use the New commenting option to display the new commenting experience (when you enable it) or the legacy commenting experience (when you disable it). The new commenting experience is the default. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

  * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations

    There is no option to enable the new commenting experience for iterations. For more information, see [Manage iteration comments](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md). 
-->

<!--Info for April 11: reword the section title below to: Overview of the Updates section; and remove the preview tags-->

### セクション タブの更新：概要

![「更新」セクション](assets/updates-tab-after-unified-experience-for-tasks-all-tab.png)

「更新」セクションの次のタブに情報が表示されます。

* **コメント**：ユーザーが行ったコメントと、そのコメントに対する返信を表示します。「コメント」タブを使用して、新しいコメントを追加したり、既存のコメントに返信したりします。オブジェクトの更新については、[ 作業の更新 ](../updating-work-items-and-viewing-updates/update-work.md) を参照してください。
* **システムアクティビティ**：システムの更新を表示します。これは、オブジェクト上の特定のイベントを記録するためにWorkfrontが作成する情報メッセージです。 例えば、ステータス、名前またはカスタムフィールドの変更は、システム更新で取り込むことができます。Workfront またはグループ管理者は、オブジェクトのシステム更新を有効にすることができます。従来のコメント機能でシステムアクティビティレコードに対して行われた返信は、読み取り専用として「システムアクティビティ」タブに入力されます。 詳しくは、[システム更新の設定](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)を参照してください。
* **すべて (読み取り専用)**：ユーザーコメントとシステムアクティビティコメントの両方を 1 か所に表示します。これは表示専用のタブです。「すべて」タブでは、コメントに返信したり、既存のコメントに他のユーザーをタグ付けしたりすることはできません。特定のコメントに返信するには、「すべて」タブから「コメント」タブへのリンクを使用します。オブジェクトの更新については、[ 作業の更新 ](../updating-work-items-and-viewing-updates/update-work.md) を参照してください。

  >[!NOTE]
  >
  >「コメント」タブと「システムアクティビティ」タブがリアルタイムで更新されます。 最新の更新を表示するには、[ すべて ] タブを更新する必要があります。

### 異なるオブジェクトの更新領域の類似点と相違点

異なるオブジェクトのコメントや更新の表示方法には違いがあります。

* 次のオブジェクトは、「更新」セクションの 3 つのタブすべてで同様のエクスペリエンスを持っています。

   * プロジェクト
   * タスク
   * イシュー
   * プログラム
   * ポートフォリオ
   * ユーザー
   * タイムシート

* 次のオブジェクトには「システムアクティビティ」タブや「すべて」タブがなく、「コメント」タブのエクスペリエンスがその他のすべてのオブジェクトと一致します。

   * チーム
   * テンプレート
   * テンプレートタスク

* 次のオブジェクトには「システムアクティビティ」タブや「すべて」タブがなく、「コメント」タブのエクスペリエンスが他のすべてのオブジェクトとは異なります。

   * イテレーション
   * ボード エリアのアドホックカード

     カードの更新について詳しくは、[ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)を参照してください。

* 次のオブジェクトには「システムアクティビティ」タブがあり、「すべて」タブはありません。

   * ボード領域の接続されたカード

     詳しくは、[ ボードでのコネクテッドカードの使用 ](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) を参照してください。

* 次のオブジェクトには、「システム」アクティビティタブに代わる「履歴」タブがあります。

   * Workfront Planning のレコード

     詳しくは、[ 履歴セクションの概要 ](/help/quicksilver/planning/records/history-section-overview.md) を参照してください。

* 次のオブジェクトには「すべて」のタブがなく、「コメント」タブのエクスペリエンスはほとんどのオブジェクトと一致します。

   * Goals

     目標の更新について詳しくは、[目標のコメントの管理](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md)を参照してください。

<!-- info for April 11: hide the entire section below: -->

<!--
### Overview of the legacy Updates section 

![](assets/updates-tab-before-unified-experience-for-tasks.png)

The legacy Updates section shows the following information:

* **User updates**: Comments made by users and replies to those comments. 
* **System updates**: Informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your objects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

The following objects don't record system updates:

* Team
* Template
* Template Task
* Iterations
-->

## 上位のオブジェクトにも表示される更新

特定のオブジェクトに対するコメント、返信まはたシステム更新は、上位のオブジェクトの「更新」セクションにも表示されます。

例えば、タスクを更新すると、その更新はタスクの「更新」セクションと、そのタスクを含んだプロジェクトの「更新」セクションに表示されます。

コメントが上位のオブジェクトにも表示されるオブジェクトを次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>元の更新が追加されたオブジェクト</strong> </th> 
   <th> <p><strong>元の更新も表示される上位のオブジェクト</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>イシュー</td> 
   <td>プロジェクト</td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>プロジェクト</td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>プログラム、ポートフォリオ</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ドキュメント </td> 
   <td>ドキュメントが添付されるオブジェクト、プロジェクト </td> 
  </tr> 
 </tr> 
  <tr data-mc-conditions=""> 
   <td>プルーフ </td> 
   <td>ドキュメント </td> 
  </tr>

<tr> 
   <td>プログラム</td> 
   <td>ポートフォリオ</td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>チーム</td> 
  </tr> 
  <tr> 
   <td>タイムシート</td> 
   <td><p>ユーザー、チーム</p>
   <p><b>メモ</b></p>
   <p>タイムシートのコメントは、コメントを作成したユーザーの「更新」セクションおよびホームチームの「更新」セクションに表示されます。</p>
   </td> 
  </tr> 
  <tr> 
   <td>テンプレートタスク</td> 
   <td>テンプレート</td> 
  </tr> 
  <tr> 
   <td>ストーリー</td> 
   <td>イテレーション、チーム</td> 
  </tr> 
  <tr> 
   <td>イテレーション</td> 
   <td>チーム</td> 
  </tr>

<tr> 
   <td>結果</td> 
   <td>目標</td> 
  </tr> 
  <tr> 
   <td>アクティビティ</td> 
   <td>目標</td> 
  </tr> 
 </tbody> 
</table>

<!--info for April 11: hide the note below-->

<!--
>[!NOTE]
>
>Replies added to system updates do not roll up to the parent object. Only direct replies on a child object and replies added to existing updates roll up to parent objects.
>
>For information about the object hierarchy in Adobe Workfront, see [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> It is not possible to reply to system updates in the new commenting experience. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
-->


## 「更新」セクションの概要

チームの「更新」セクションでは、他のユーザーに代わって更新を入力する場合の制限事項がいくつかあります。

### ユーザーおよびチームの制限

ユーザーとチームの更新を表示する際は、次の点を考慮してください。

* チームの「更新」セクションで新しいコメントを追加できません。

* チームの「更新」セクションには、次のオブジェクトに入力された更新が入力されます。

   * ユーザー
   * ストーリー
   * タイムシート
   * イテレーション

* チームで表示する更新に返信を追加できます。返信は、チームの「更新」セクションとそのチームが属するオブジェクトの「更新」セクションにも表示されます。

* ユーザーおよびチームの「更新」セクションでは、過去 90 日間に入力された更新を表示できます。

  ユーザーまたはチームに対して行われたすべての更新を 90 日の制限を超えて確認する場合は、メモに関するレポートを作成できます。ユーザーまたはチームが行った更新をすべて表示する時間フィルターをレポートに含めないでください。詳しくは、[カスタムレポートの作成](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

### 別のユーザーの代わりにコメントを入力する際の制限

Adobe Workfront 管理者とグループ管理者は、他のユーザーとしてログインし、Workfront でコメントの入力などのアクションを実行できます。

詳しくは、[別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)を参照してください。

別のユーザーとしてログインし、コメントを追加する際は、次の点を考慮してください。

* 別のユーザーに代わって行われたコメントは、コメントに示されます。

* グループ管理者は、別のユーザーの代わりにコメントを作成できますが、そのコメントは削除できません。別のユーザーに代わって作成したコメントを削除できるのは、Adobe Workfront 管理者のみです。

* Workfront 管理者またはグループ管理者は、ユーザーとしてログアウトし、自分自身として再度ログインした場合にのみ、別のユーザーに代わって追加したコメントを編集できます。別のユーザーに代わってコメントを削除できません。

## ジャーナルエントリレポートを使用した作業アイテムのシステム更新の表示

ジャーナルエントリレポートには、プロジェクト、タスク、イシューの更新エリアからシステムの更新が表示されます。

このレポートでは、次の情報を確認できます。

* ステータスの変更が発生した回数
* タスクまたはイシューがいつ削除されたか
* 重要なカスタムフィールドの値が、プロジェクトの過程でどのように変化したか
* プロジェクトの過程で変わった重要な日付
* プロジェクトの過程で優先度が変更されたかどうか
* プロジェクトの所有者が変更されたかどうか

詳細については、[ 仕訳レポートを使用した更新領域のレポート ](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md) を参照してください。
