---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 既存の反復へのストーリーの追加
description: イテレーションにストーリーを追加する方法は様々です。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 86%

---

# 既存のイテレーションにストーリーを追加

次のいずれかの方法で、イテレーションにストーリーを追加できます。

* イテレーションが作成された後のバックログから追加（詳しくは、[アジャイルバックログの管理](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)の[バックログからイテレーションまたは[!UICONTROL かんばん]ボードにストーリーを移動](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board)の節を参照）

* 個々のタスクまたはイシューの[!UICONTROL 詳細]ページから追加
* タスクまたはイシューのリストから追加
* レポートから追加
* ダッシュボードから追加

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p> 
   または
   <p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>ストーリーが存在するプロジェクトへの[!UICONTROL Manage]アクセス権 </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ストーリーの追加がタスクの日付に与える影響について

デフォルトでは、既存のタスクをイテレーションに追加すると、タスクの[!UICONTROL 予定開始日]および[!UICONTROL 予定完了日]が次のように設定されます。

### タスクの[!UICONTROL 予定開始日]

* タスクでは、以下の場合にイテレーションの開始日を使用します。

   * プロジェクトに[!UICONTROL 予定開始日]が設定されていない。
   * プロジェクトの[!UICONTROL 予定開始日]が、イテレーションの開始日の&#x200B;*前*&#x200B;または&#x200B;*当日*&#x200B;である。

* タスクでは、以下の場合にプロジェクトの[!UICONTROL 予定開始日]を使用します。

   * プロジェクトの[!UICONTROL 予定開始日]が、イテレーションの開始日の&#x200B;*後*&#x200B;である。

### タスクの[!UICONTROL 予定完了日]

* タスクでは、以下の場合にイテレーションの終了日を使用します。

   * プロジェクトに[!UICONTROL 予定完了日]が設定されていない。
   * プロジェクトの[!UICONTROL 予定開始日]がイテレーションの開始日の&#x200B;*前または当日*&#x200B;であるか、プロジェクトの[!UICONTROL 予定完了日]がイテレーションの終了日の&#x200B;*前または当日*&#x200B;である。

* タスクでは、以下の場合にプロジェクトの[!UICONTROL 予定完了日]を使用します。

   * プロジェクトの[!UICONTROL 予定開始日]がイテレーションの開始日の&#x200B;*後*&#x200B;で、プロジェクトの[!UICONTROL 予定完了日]がイテレーションの終了日の&#x200B;*後*&#x200B;である。

個々のスクラムチームが、デフォルトではイテレーション日付よりも、プロジェクト日付を使用するように設定できます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事で[作業アイテムをイテレーションに追加する際に日付を適用する方法の設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)の節を参照してください。

## 既存のイテレーションにストーリーを追加

プロジェクトへの管理アクセス権を持っている場合は、任意のイテレーションに任意のタスクまたはイシューを追加できます。タスクまたはイシューをイテレーションに移動する際は、次の点に注意してください。

* 複数のチームを追加する場合、タスクまたはイシューは 1 つのチームのイテレーションにのみ表示されます。これは、以下の手順 3 で選択するイテレーションです。
* タスクまたはイシューがアジャイルチームに割り当てられ、別のチームのイテレーションに移動しても、チームの割り当ては変更されません。
* タスクまたはイシューがチームに割り当てられていない場合、そのイテレーションを所有するチームにタスクまたはイシューが割り当てられます。
* 親タスクをイテレーションに追加することはできません。子タスクを追加する場合、親タスクはスイムレーンとしてスクラムボードに表示されます。

>[!IMPORTANT]
>
>タスクがイテレーションに移動した後は、「[!UICONTROL 期間タイプ]」や「[!UICONTROL タスクの制約]」を更新できません。タスクのタイムラインをイテレーションのタイムラインと一致させるために、「[!UICONTROL 期間タイプ]」は[!UICONTROL シンプル]に設定され、「[!UICONTROL タスクの制約]」は[!UICONTROL 固定日付]に設定されます。

1. 反復に追加するタスクまたは問題を開きます。
または
反復に追加するタスクまたは問題を含むプロジェクト、レポート、またはダッシュボードに移動します。 次に、1 つ以上のタスクまたは問題を選択します。

1. **[!UICONTROL 詳細]**![](assets/more-icon.png)/**[!UICONTROL イテレーションに追加]** をクリックします。
非アジャイルチームに割り当てられたタスクやイシューを割り当てることはできません。

1. 「**[!UICONTROL 追加先]**」ボックスにイテレーションの名前の入力を開始し、リストに表示されたら選択します。

   >[!NOTE]
   >
   >ストーリーを既存のイテレーションから新しいイテレーションに移動できます。

1. 「**[!UICONTROL 追加]**」をクリックします。
