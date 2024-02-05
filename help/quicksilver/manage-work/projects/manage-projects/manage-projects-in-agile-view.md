---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: アジャイルビューでのプロジェクトの管理
description: 通常アジャイルプラクティスに伴う管理上の課題（チームバックログの管理やイテレーションの作成など）に煩わされずに、プロジェクトでアジャイル機能を活用できます。
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 88%

---

# アジャイルビューでのプロジェクトの管理

通常アジャイルプラクティスに伴う管理上の課題（チームバックログの管理やイテレーションの作成など）に煩わされずに、プロジェクトでアジャイル機能を活用できます。

チームバックログを使用し、バックログにあるタスクからのイテレーションの作成を許可するアジャイル環境で作業する場合は、[アジャイル環境での作業](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md)の手順に従います。

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
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在：レビュー以上</p> 
   <p>新規：寄稿者以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベルの設定</td> 
   <td> <p>次のエリアへの編集アクセス権：</p> 
    <ul> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>レポート、ダッシュボード、カレンダー</p> </li> 
     <li> <p>フィルター、ビュー、グループ化</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの表示権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。 アクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## アジャイルプロジェクトについて

>[!NOTE]
>
>この節は、従来のアジャイルビューにのみ当てはまり、プロジェクトのボードビューには当てはまりません。

* [プロジェクトでのアジャイル機能](#agile-functionality-in-a-project)
* [アジャイルビューをプロジェクトで使用する場合とイテレーションで使用する場合の違い](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### プロジェクトでのアジャイル機能 {#agile-functionality-in-a-project}

アジャイルビューでプロジェクトを管理する場合、次のアジャイル機能を使用できます。

* 完了状態\
  完了状態について詳しくは、[イテレーション完了状態の概要](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md)を参照してください。

* ストーリーボード\
  ストーリーボードについて詳しくは、[スクラムボード](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md)を参照してください。

プロジェクトでアジャイルビューを使用する場合と、純粋なアジャイル環境（バックログとイテレーションを伴う）で作業する場合とでは、いくつかの違いがあります。詳しくは、この記事の[アジャイルビューをプロジェクトで使用する場合とイテレーションで使用する場合の違い](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)を参照してください。

### アジャイルビューをプロジェクトで使用する場合とイテレーションで使用する場合の違い {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [ストーリーボード上でタスクとサブタスクは異なる表示ルールに従う](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [バックログとイテレーションは使用されない](#backlogs-and-iterations-are-not-used)
* [タスクの順序はアジャイルビューで維持され、並べ替えはできない](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [タスクは予定時間数でのみ測定される](#tasks-are-measured-only-in-planned-hours)
* [アジャイルチームは使用されない](#the-agile-team-is-not-used)
* [プロジェクトはプロジェクトのユーザーごとに異なるアジャイルビューで表示される](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### ストーリーボード上でタスクとサブタスクは異なる表示ルールに従う {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* 親タスクもサブタスクもないタスクは、ストーリーボードに常に 1 つのストーリーカードとして表示されます。\
  例えば、これらのタスクはプロジェクトリストビューでは次のように表示されます。

  ![アジャイルプロジェクトリスト — 親タスクまたはサブタスクのないタスク](assets/agile-project-single-list-nwe.png)

  これらのタスクは、プロジェクトアジャイルビューでは次のように表示されます。

  ![プロジェクトアジャイルビュー - 親タスクやサブタスクのないタスク](assets/agile-project-singlecard-nwe.png)

* サブタスクを持つ親タスクは、常にストーリーボードの&#x200B;**ストーリー**&#x200B;列に表示されます。サブタスクは、親タスクのスイムレーンに表示されます。\
  例えば、これらのタスクはプロジェクトリストビューでは次のように表示されます。

  ![アジャイルプロジェクトリスト - 親タスクとサブタスクを持つタスク](assets/agile-project-parent-list-nwe.png)\
  これらのタスクは、プロジェクトアジャイルビューでは次のように表示されます。

  ![アジャイルプロジェクトビュー - 親タスクとサブタスクを持つタスク](assets/agile-project-parent-nwe.png)

* 第 2 レベルのサブタスク（サブタスクのサブタスク）は、直接の親タスクからぶら下がっている灰色のカードとして表示されます。
* 第 3 レベルのサブタスク（サブタスクのサブタスクのサブタスク）はストーリーボードには表示されません。

#### バックログとイテレーションは使用されない {#backlogs-and-iterations-are-not-used}

アジャイルビューでプロジェクトを表示する場合、次のアジャイルコンポーネントは使用されません。

* **バックログ**：プロジェクトのタスクはすべて自動的にストーリーとして表示されるので、バックログは使用されません。
* **イテレーション**：イテレーションを作成して作業が完了する日付を定義するのではなく、プロジェクトのタイムラインで現在指定されている日が稼働日になります。

#### タスクの順序はアジャイルビューで維持され、並べ替えはできない {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

プロジェクトでのタスクの表示順序は、プロジェクトをアジャイルストーリーボードで表示する際に維持されます。

プロジェクトをアジャイルビューで表示している場合、プロジェクトのタスクの順序を変更することはできません。タスクの順序を変更すると、依存関係がある可能性のある他のタスクに影響を与えるおそれがあるので、タスクの順序を変更するには標準ビューでプロジェクトを表示する必要があります。

#### タスクは予定時間数でのみ測定される {#tasks-are-measured-only-in-planned-hours}

プロジェクトのタスクは常に予定時間数で測定されます。

イテレーションでは、タスク（ストーリー）を時間数またはポイント単位で測定できます。

#### アジャイルチームは使用されない {#the-agile-team-is-not-used}

アジャイルチームは割り当てられたイテレーションで作業を完了するので、アジャイルビューでプロジェクトを表示する場合、アジャイルチームは使用されません。

代わりに、プロジェクトに参加しているすべてのユーザーが、基本的にそのプロジェクトのアジャイルチームになります。

#### プロジェクトはプロジェクトのユーザーごとに異なるアジャイルビューで表示される {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

アジャイルイテレーションとは異なり、プロジェクトのユーザーはアジャイルビューを自分用にカスタマイズできますが、他のユーザーは別のアジャイルビューを使用します。

アジャイルイテレーションでは、アジャイルストーリーボードで得られる情報（使用可能なステータス列など）はチームレベルで決定されます。

アジャイルビューのカスタマイズ方法については、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)の[アジャイルビューの作成またはカスタマイズ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)を参照してください。

## アジャイルビューでのプロジェクトの表示

1. タスクリストまたはイシューリストのアジャイルビューで表示するプロジェクトに移動します。
1. 次をクリック： **ボード表示** アイコン ![ボードアイコン](assets/board-icon-for-agile-view.png).

   プロジェクトのボードビューがデフォルトで表示されます。

   ![プロジェクトのボードビュー](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. （オプション）「**設定**」をクリックして、列とカードのオプションを設定します。

   詳しくは、[ボード列の管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)と[カードに表示されるフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)を参照してください。プロジェクトのボードビューでは列ポリシーを定義できないことに注意してください。

1. （オプション）ボードビューではなく従来のアジャイルビューを使用するには、「**従来のアジャイルを使用**」をクリックします。

1. （オプション - 従来のアジャイルビューのみ）カスタムアジャイルビューを作成してある場合や、別のユーザーが作成したカスタムアジャイルビューを共有している場合は、デフォルトのアジャイルビューの代わりにそれを表示できます。

   **表示**&#x200B;ドロップダウンメニューをクリックし、表示するカスタムアジャイルビューをクリックします。

   そのカスタムアジャイルビューは、次に&#x200B;**アジャイル**&#x200B;アイコンをクリックしたときに使用されます。

   新規アジャイルビューの作成方法については、[アジャイルビューの作成とカスタマイズ](#create-and-customize-agile-views)を参照してください。

   プロジェクトはカスタムアジャイルビューに表示されます。

1. （条件付き - 従来のアジャイルビューのみ）プロジェクトのタスクが「新規」、「進行中」または「完了」（アジャイルビューのデフォルトステータス）以外のステータスを使用している場合、それらのステータスにあるタスクを表示するには、そのステータスをアジャイルビューに追加する必要があります。

   タスクが、アジャイルストーリーボードに表示されないステータスにある場合、タスク自体がアジャイルストーリーボードに表示されません（ただし、これらのタスクの完了率は、親タスクの完了率とプロジェクト全体の完了率に影響します）。

   アジャイルビューにステータスを追加するには、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)の記事の「アジャイルビューの作成またはカスタマイズ」の節で説明されているとおりに、新規アジャイルビューを作成するか、既存のアジャイルビューをカスタマイズします。

1. （オプション）リストビューに戻るには、**リスト**&#x200B;アイコンをクリックします。

## アジャイルビューの作成とカスタマイズ {#create-and-customize-agile-views}

>[!NOTE]
>
>この節は、従来のアジャイルビューにのみ当てはまり、プロジェクトのボードビューには当てはまりません。

Workfront の標準ビューの場合と同様に、既存のアジャイルビューをカスタマイズしたり、新規アジャイルビューを最初から作成したりできます。標準ビューとは異なり、既存のアジャイルビューに基づいて新規アジャイルビューを作成することはできません。

アジャイルビューの作成とカスタマイズについて詳しくは、 [アジャイルビューの作成またはカスタマイズ](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) 記事のセクション [Adobe Workfrontでビューを作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## 既存のアジャイルビューの共有

>[!NOTE]
>
>この節は、従来のアジャイルビューにのみ当てはまり、プロジェクトのボードビューには当てはまりません。

自分で作成したアジャイルビューを共有したり、他のビューを共有するのと同じ方法で権限を持つことができます。また、フィルターやグループ化も可能です。

詳しくは、[フィルター、ビュー、グループ化の共有](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)を参照してください。

## 既存のアジャイルビューの削除

>[!NOTE]
>
>この節は、従来のアジャイルビューにのみ当てはまり、プロジェクトのボードビューには当てはまりません。

他のビューを削除するのと同じ方法で、アジャイルビューを削除したり、フィルターまたはグループ化を実行したりできます。

詳しくは、 [フィルター、ビュー、およびグループを削除する](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
