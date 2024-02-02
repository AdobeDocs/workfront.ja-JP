---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 既存のイテレーションにストーリーを追加
description: イテレーションにストーリーを追加する方法は様々です。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: ht
source-wordcount: '673'
ht-degree: 100%

---

# 既存のイテレーションにストーリーを追加

次のいずれかの方法で、イテレーションにストーリーを追加できます。

* イテレーションが作成された後のバックログから追加（詳しくは、[アジャイルバックログの管理](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)の[バックログからイテレーションまたは[!UICONTROL かんばん]ボードにストーリーを移動](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog)の節を参照）

* 個々のタスクまたはイシューの[!UICONTROL 詳細]ページから追加
* タスクまたはイシューのリストから追加
* レポートから追加
* ダッシュボードから追加

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ストーリーが存在するプロジェクトへの[!UICONTROL Manage]アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

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

個々のスクラムチームが、デフォルトではイテレーション日付よりも、プロジェクト日付を使用するように設定できます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事で[作業アイテムをイテレーションに追加する際に日付を適用する方法の設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)の節を参照してください。

## 既存のイテレーションにストーリーを追加

タスクやイシューから直接イテレーションにストーリーを追加するには、次の手順に従います。

>[!IMPORTANT]
>
>タスクがイテレーションに移動した後は、「[!UICONTROL 期間タイプ]」や「[!UICONTROL タスクの制約]」を更新できません。タスクのタイムラインをイテレーションのタイムラインと一致させるために、「[!UICONTROL 期間タイプ]」は[!UICONTROL シンプル]に設定され、「[!UICONTROL タスクの制約]」は[!UICONTROL 固定日付]に設定されます。

### タスクまたはイシューのタブから追加

プロジェクトへの管理アクセス権を持っている場合は、任意のイテレーションに任意のタスクまたはイシューを追加できます。タスクまたはイシューをイテレーションに移動する際は、次の点に注意してください。

* 複数のチームを追加する場合、タスクまたはイシューは 1 つのチームのイテレーションにのみ表示されます。これは、以下の手順 3 で選択するイテレーションです。
* タスクまたはイシューがアジャイルチームに割り当てられ、別のチームのイテレーションに移動しても、チームの割り当ては変更されません。
* タスクまたはイシューがチームに割り当てられていない場合、そのイテレーションを所有するチームにタスクまたはイシューが割り当てられます。
* 親タスクをイテレーションに追加することはできません。子タスクを追加する場合、親タスクはスイムレーンとしてスクラムボードに表示されます。

1. イテレーションに追加するタスクまたはイシューが含まれるプロジェクト、レポートまたはダッシュボードに移動します。
1. 1 つ以上のタスクまたはイシューを選択します。
1. **[!UICONTROL その他]**![](assets/more-icon.png)／**[!UICONTROL 反復に追加]**&#x200B;をクリックします。\
   非アジャイルチームに割り当てられたタスクやイシューを割り当てることはできません。

1. **[!UICONTROL ストーリーを追加]**&#x200B;ボックスに、イテレーションの名前を入力します。

   >[!NOTE]
   >
   >ストーリーを既存のイテレーションから新しいイテレーションに移動できます。

1. タスクを追加する場合は、「**[!UICONTROL ストーリーを追加]**」をクリックします。\
   または\
   イシューを追加する場合は、「**[!UICONTROL イシューを追加]**」をクリックします。
