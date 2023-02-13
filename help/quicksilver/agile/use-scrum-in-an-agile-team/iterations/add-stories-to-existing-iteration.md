---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 既存の反復にストーリーを追加する
description: 繰り返しにストーリーを追加する方法は様々です。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 既存の反復にストーリーを追加する

次のいずれかの方法で、ストーリーを繰り返しに追加できます。

* 反復が作成された後のバックログから、 [バックログからイテレーションにストーリーを移動するか、 [!UICONTROL かんばん] ボード](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) セクション [アジャイルバックログの管理](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* 次の [!UICONTROL 詳細] 個々のタスクまたは問題のページ
* タスクまたはタスクリストから
* レポートから
* ダッシュボードから

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>[!UICONTROL ストーリーが存在するプロジェクトへの [!UICONTROL 管理 ] アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ストーリーを追加するとタスクの日付に与える影響を理解する

デフォルトでは、既存のタスクをイテレーションに追加すると、タスクの [!UICONTROL 計画開始日] および [!UICONTROL 計画完了日] は次のように設定されます。

### タスク [!UICONTROL 計画開始日]

* タスクは、以下の場合に反復の開始日を使用します。

   * プロジェクトには [!UICONTROL 計画開始日] 設定します。
   * プロジェクトの [!UICONTROL 計画開始日] が *前* または *オン* 反復の開始日。

* タスクは、プロジェクトの [!UICONTROL 計画開始日] 条件：

   * プロジェクトの [!UICONTROL 計画開始日] が *後* 反復の開始日。

### タスク [!UICONTROL 計画完了日]

* タスクは、以下の場合に反復の終了日を使用します。

   * プロジェクトには [!UICONTROL 計画完了日] 設定します。
   * プロジェクトの [!UICONTROL 計画開始日] が *次の日以前* イテレーションの開始日またはプロジェクトの [!UICONTROL 計画完了日] が *次の日以前* 反復の終了日。

* タスクは、プロジェクトの [!UICONTROL 計画完了日] 条件：

   * プロジェクトの [!UICONTROL 計画開始日] が *後* イテレーションの開始日とプロジェクトの [!UICONTROL 計画完了日] が *後* 反復の終了日。

個々のスクラムチームが、繰り返し日付ではなく、デフォルトでプロジェクト日付を使用するように設定できます。 詳しくは、 [作業項目を反復処理に追加する際の日付の適用方法を設定する](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 記事内 [スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## 既存の反復にストーリーを追加

タスクやイシューから直接イテレーションにストーリーを追加するには、次の手順に従います。

>[!IMPORTANT]
>
>タスクが反復に移行した後は、 [!UICONTROL 期間のタイプ] または [!UICONTROL タスク制約]. [!UICONTROL 期間のタイプ] が [!UICONTROL シンプル] および [!UICONTROL タスク制約] が [!UICONTROL 固定日付] タスクタイムラインをその反復のタイムラインと一致させるため。

### タスクまたは問題タブから

プロジェクトへの「管理」アクセス権を持っている場合は、任意のイテレーションに任意のタスクやイシューを追加できます。 タスクまたはイシューをイテレーションに移動する際は、次の点に注意してください。

* 複数のチームを追加する場合、タスクまたはイシューは 1 つのチームのイテレーションにのみ表示されます。 これは、以下の手順 3 で選択する反復です。
* タスクまたは問題がアジャイルチームに割り当てられ、別のチームのイテレーションに移動した場合、チームの割り当ては変更されません。
* タスクまたはイシューがチームに割り当てられていない場合、そのイテレーションを所有するチームにタスクまたはイシューが割り当てられます。
* 親タスクをイテレーションに追加することはできません。 子タスクを追加する場合、親タスクはスイムレーンとしてスクラムボードに表示されます。

1. 反復に追加するタスクまたは問題が含まれるプロジェクト、レポート、またはダッシュボードに移動します。
1. 1 つ以上のタスクまたはタスクを選択します。
1. クリック **[!UICONTROL 詳細]** ![](assets/more-icon.png) > **[!UICONTROL 反復に追加]**.\
   非アジャイルチームに割り当てられたタスクや問題を割り当てることはできません。

1. 内 **[!UICONTROL ストーリーを追加]** ボックスに、反復の名前を入力します。

   >[!NOTE]
   >
   >ストーリーを既存のイテレーションから新しいイテレーションに移動できます。

1. タスクを追加する場合は、 **[!UICONTROL ストーリーを追加]**.\
   または\
   問題を追加する場合は、 **[!UICONTROL 問題の追加]**.
