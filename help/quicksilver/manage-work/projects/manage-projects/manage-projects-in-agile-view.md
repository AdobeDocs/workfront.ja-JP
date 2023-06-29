---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: アジャイルビューでのプロジェクト管理
description: 必要なプラン、ライセンスの種類、およびAdobe Workfront Plan Team、Pro、Business、または Enterprise Workfront License Type Review、Work、または Plan Permissions （アクセスモデルでの確認、作業、またはプラン権限）レポート、ダッシュボード、カレンダーの編集
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 11e239bd47a007adbec1770dafc7f7a5d97eb57e
workflow-type: tm+mt
source-wordcount: '1432'
ht-degree: 0%

---

# アジャイルビューでのプロジェクト管理

{{highlighted-preview}}

<!--
Required plans, license types, and access

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront Plan</a> </p> </td> 
   <td> <p>Team, Pro, Business, or Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront License Type</p> </td> 
   <td> <p>Review, Work, or Plan </p> </td> 
  </tr> 
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
 </tbody> 
</table>
-->

一般的にアジャイルプラクティスに伴う管理上の課題（チームバックログの管理や反復の作成など）がなくても、プロジェクトにアジャイル機能を活用できます。

チームバックログを使用し、バックログ上のタスクから反復を作成できるアジャイル環境で作業する場合は、 [機敏な環境での作業](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の領域へのアクセスを編集します。</p> 
    <ul> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>レポート、ダッシュボード、カレンダー</p> </li> 
     <li> <p>フィルター、表示、グループ化</p> </li> 
    </ul> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限を表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## アジャイルプロジェクトについて

>[!NOTE]
>
><span class="preview">この節は、レガシーのアジャイルビューにのみ適用され、プロジェクトのボードビューには適用されません。</span>

* [プロジェクトのアジャイル機能](#agile-functionality-in-a-project)
* [プロジェクトでアジャイルビューを使用する場合と反復で使用する場合の違い](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### プロジェクトのアジャイル機能 {#agile-functionality-in-a-project}

アジャイルビューでプロジェクトを管理する場合は、次のアジャイル機能を使用できます。

* 完了状態\
  完了ステータスについて詳しくは、 [反復完了ステータスの概要](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* ストーリーボード\
  ストーリーボードについて詳しくは、 [スクラムボード](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) 」セクションに入力します。

プロジェクトでアジャイルビューを使用する場合と、純粋にアジャイルな環境で（バックログと反復を使用して）作業する場合では、いくつかの違いがあります。 詳しくは、 [プロジェクトでアジャイルビューを使用する場合と反復で使用する場合の違い](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) 」を参照してください。

### プロジェクトでアジャイルビューを使用する場合と反復で使用する場合の違い {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [タスクとサブタスクは、ストーリーボード上の様々な表示ルールに従います](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [バックログと繰り返しは使用されません](#backlogs-and-iterations-are-not-used)
* [タスクの順序はアジャイルビューで維持され、順序を変更できません](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [タスクは計画時間でのみ測定されます](#tasks-are-measured-only-in-planned-hours)
* [アジャイルチームは使用されていません](#the-agile-team-is-not-used)
* [プロジェクトの各ユーザーは、異なるアジャイルビューでプロジェクトを表示できます](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### タスクとサブタスクは、ストーリーボード上の様々な表示ルールに従います {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 親タスクもサブタスクも持たないタスクは、常にストーリーボード上に単一ストーリーカードとして表示されます。\
  たとえば、これらのタスクは、プロジェクトの一覧表示で次のように表示されます。

  ![アジャイルプロジェクトリスト — 親タスクまたはサブタスクのないタスク](assets/agile-project-single-list-nwe.png) これらのタスクは、プロジェクトのアジャイルビューでは次のように表示されます。

  ![プロジェクトのアジャイルビュー — 親タスクまたはサブタスクのないタスク](assets/agile-project-singlecard-nwe.png)

* サブタスクを持つ親タスクは、常に **ストーリー** ストーリーボードの列。 サブタスクは、親タスクのスイムレーンに表示されます。\
  たとえば、これらのタスクは、プロジェクトの一覧表示で次のように表示されます。

  ![俊敏なプロジェクトリスト — 親とサブタスクを含むタスク](assets/agile-project-parent-list-nwe.png)\
  これらのタスクは、プロジェクトのアジャイルビューでは次のように表示されます。

  ![アジャイルプロジェクトビュー — 親とサブタスクを含むタスク](assets/agile-project-parent-nwe.png)

* 第 2 レベルのサブタスク（サブタスクのサブタスク）は、直近の親タスクの上にぶら下がったグレーのカードとして表示されます。
* 第 3 レベルのサブタスク（サブタスクのサブタスクのサブタスク）は、ストーリーボードには表示されません。

#### バックログと繰り返しは使用されません {#backlogs-and-iterations-are-not-used}

アジャイルビューでプロジェクトを表示する場合、次のアジャイルコンポーネントは使用されません。

* **バックログ：** プロジェクト内のタスクはストーリーとして自動的に表示されるので、バックログは使用されません。
* **反復：** 作業が完了する日付を定義する反復を作成するのではなく、プロジェクトタイムラインで現在指定されている日が稼働日になります。

#### タスクの順序はアジャイルビューで維持され、順序を変更できません {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

プロジェクトをアジャイルストーリーボードで表示するとき、プロジェクト内でのタスクの表示順序が維持されます。

プロジェクトをアジャイルビューで表示する場合、プロジェクト内のタスクを並べ替えることはできません。 タスクの順序を変更すると、依存関係を持つ他のタスクに影響を与える可能性があるので、タスクの順序を変更するには、標準ビューでプロジェクトを表示する必要があります。

#### タスクは計画時間でのみ測定されます {#tasks-are-measured-only-in-planned-hours}

プロジェクト上のタスクは、常に計画時間数で測定されます。

反復では、タスク（ストーリー）を時間単位またはポイント単位で測定できます。

#### アジャイルチームは使用されていません {#the-agile-team-is-not-used}

アジャイルチームは、割り当てられた反復作業を完了するので、アジャイルビューでプロジェクトを表示する場合は、アジャイルチームは使用されません。

代わりに、プロジェクト上のユーザーは基本的に、そのプロジェクトの俊敏なチームになります。

#### プロジェクトの各ユーザーは、異なるアジャイルビューでプロジェクトを表示できます {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

俊敏な反復とは異なり、プロジェクトのユーザーは俊敏なビューを自分でカスタマイズできますが、他のユーザーは俊敏なビューを別の方法で使用できます。

アジャイル反復では、アジャイルストーリーボードで利用可能な情報（利用可能なステータス列など）は、チームレベルで決定されます。

アジャイルビューのカスタマイズ方法について詳しくは、 [アジャイルビューの作成またはカスタマイズ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## アジャイルビューでのプロジェクトの表示

1. アジャイルビューで表示するプロジェクトに移動します。
1. 次をクリック： **アジャイル** アイコン ![アジャイルアイコン](assets/agile-icon-nwe.png).

   <span class="preview">または</span>

   <span class="preview">次をクリック： **ボード** アイコン ![ボードアイコン](assets/board-icon-for-agile-view.png).</span>

   デフォルトのアジャイルビューにプロジェクトが表示されます。

   <span class="preview">プレビュー環境では、ボードビューがデフォルトで表示されます。</span>

   ![プロジェクトのボードビュー](assets/project-agile-board-view.png)

   （レガシーアジャイルビューのみ）以前にカスタムアジャイルビューでプロジェクトを表示した場合、デフォルトのアジャイルビューではなく、そのビューでプロジェクトが表示されます。

1. <span class="preview">（オプション）「 **設定** をクリックして、列とカードのオプションを設定します。</span>

   <span class="preview">詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) および [カードに表示するフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). プロジェクトのボードビューでは、列ポリシーを定義できません。</span>

1. <span class="preview">（オプション）「 **レガシーアジャイルを使用** を使用して、ボードビューの代わりにレガシーアジャイルビューを使用します。</span>

1. （オプション — レガシーアジャイルビューのみ）カスタムアジャイルビューを作成した場合、または別のユーザーがカスタムアジャイルビューを作成して共有した場合、デフォルトのアジャイルビューの代わりに表示できます。

   次をクリック： **表示** ドロップダウンメニューから、表示するカスタムアジャイルビューをクリックします。

   カスタムアジャイルビューは、次に **アジャイル** アイコン

   新しいアジャイルビューの作成方法について詳しくは、 [アジャイルビューの作成とカスタマイズ](#create-and-customize-agile-views).

   プロジェクトがカスタムアジャイルビューに表示されます。

1. （条件付き — レガシーアジャイルビューのみ）プロジェクト内のタスクで「新規」、「処理中」、「完了」（アジャイルビューのデフォルトステータス）以外のステータスを使用している場合、それらのステータスのタスクをアジャイルビューに追加する必要があります。

   タスクのステータスが「アジャイルストーリー」ボードに表示されない場合、タスク自体は「アジャイルストーリー」ボードに表示されません（ただし、タスクの「完了率」は、親タスクの「完了率」と、プロジェクト全体の「完了率」に影響します）。

   アジャイルビューにステータスを追加するには、記事の「アジャイルビューの作成またはカスタマイズ」の節に従って、新しいアジャイルビューを作成するか、既存のアジャイルビューをカスタマイズします [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. （オプション）リスト表示に戻るには、 **リスト** アイコン\
   ![リストアイコン](assets/list-icon.png)

## アジャイルビューの作成とカスタマイズ {#create-and-customize-agile-views}

>[!NOTE]
>
><span class="preview">この節は、レガシーのアジャイルビューにのみ適用され、プロジェクトのボードビューには適用されません。</span>

Workfrontの標準ビューと同様に、既存のアジャイルビューをカスタマイズしたり、新しいアジャイルビューをゼロから作成したりできます。 標準ビューとは異なり、既存のアジャイルビューに基づいて新しいアジャイルビューを作成することはできません。

アジャイルビューの作成とカスタマイズについて詳しくは、この記事の「アジャイルビューの作成またはカスタマイズ」の節を参照してください [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 既存のアジャイルビューの共有

>[!NOTE]
>
><span class="preview">この節は、レガシーのアジャイルビューにのみ適用され、プロジェクトのボードビューには適用されません。</span>

アジャイルビューの共有方法について詳しくは、 [フィルター、表示またはグループ化の共有](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## 既存のアジャイルビューの削除

>[!NOTE]
>
><span class="preview">この節は、レガシーのアジャイルビューにのみ適用され、プロジェクトのボードビューには適用されません。</span>

ビューの削除方法について詳しくは、この記事の「ビューの削除」の節を参照してください [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
