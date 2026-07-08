---
content-type: reference
navigation-topic: notifications
title: 通知：Goals
description: 通知：Goals
author: Courtney, Alina
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6kIc-y3DRa7mDVX14gA5jDbIzZveHH1MNIghGpQP7hc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 4bce43b6edd473f55b323e1d878b6e131213e179
workflow-type: tm+mt
source-wordcount: 425
ht-degree: 85%

---

# 通知：Goals

プロファイルから、[!DNL Adobe Workfront Goals] で発生したイベントのメール通知を有効にすることができます。 ユーザーが[!UICONTROL プラン]ライセンスを使用して、他のユーザーに対して有効にすることもできます。 詳しくは、[[!DNL Adobe Workfront]  の通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## アクセス要件

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td>
   <p>コントリビューター以上</p>
    <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>その他の製品</strong></td> 
   <td>[!DNL Workfront Goals] <p>[!DNL Workfront Goals] について詳しくは、<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!DNL Goals] に対する[!UICONTROL View]以上のアクセス権</p></td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* [!DNL Goals]通知を更新するユーザーには、[!UICONTROL  メインメニュー]の[!DNL Goals]領域を含むレイアウトテンプレートが必要です。


## [!UICONTROL  ユーザープロファイル ]エリアにある [!DNL Goals] の通知

次のテーブルに表示される通知は、[!DNL Workfront Goals] で発生しているイベントに関する警告です。例えば、目標、結果、アクティビティを割り当てているユーザーや、所有する目標、結果、アクティビティを更新しているユーザーなどです。 受信する通知の設定について詳しくは、[自身のメール通知の変更](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)を参照してください。

![通知の環境設定](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>* [!DNL Goals] のインスタント通知は、デフォルトでは無効になっています。 毎日の通知を有効または無効にすることはできません。また、このカテゴリのイベントに関する日々のダイジェストメールを受信することもできません。 [!DNL Goals] カテゴリのインスタント通知を個別に有効または無効にできます。
>* アクセスレベルで目標にアクセスできなくても、目標の更新に関する電子メールを受け取ることができますが、割り当てられた目標に対して目標、結果、アクティビティまたはコメントが割り当てられています。

[イベント通知](../../workfront-basics/using-notifications/event-notifications.md)も参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>通知</strong></td> 
   <td> <p><strong>含まれるフィールド</strong> </p> <p><strong>*インスタント通知のみ</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>誰かに成果 / アクティブを割り当てられました</strong></td> 
   <td> <p>結果またはアクティビティを割り当てたユーザーの名前</p> <p>結果またはアクティビティの目標の期間</p> <p>結果またはアクティビティの名前</p> <p>[!UICONTROL Goal Details] パネルを開く <strong>[!UICONTROL Open in web app]</strong> ボタン</p> <p><strong>[!UICONTROL Change Notifications Settings]</strong> ボタンで通知を管理できます。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>誰かが自分の個人用目標を新しく作成しました</strong> </td> 
   <td> <p>目標を割り当てたユーザーの名前</p> <p>目標の期間</p> <p>目標の名前</p> <p>[!UICONTROL Goal Details] パネルを開く <strong>[!UICONTROL Open in web app]</strong> ボタン</p> <p><strong>[!UICONTROL Change Notifications Settings]</strong> ボタンで通知を管理できます。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>誰かが自分の目標にコメントを残しました</strong></td> 
   <td> <p>コメントを残したユーザーの名前</p> <p>目標の期間 </p> <p>目標の名前</p> <p>コメントのテキスト</p> <p>[!UICONTROL Goal Details] パネルを開く <strong>[!UICONTROL Open in web app]</strong> ボタン</p> <p>通知を管理できる <strong>[!UICONTROL Change Notifications Settings]</strong> ボタン。</p> </td> 
  </tr> 
  <tr> 
  </tbody> 
</table>

<!--
these were removed at some point: 

   <td><strong>Someone liked my comment on a Goal</strong></td> 
   <td> <p>The name of the person who liked the comment</p> <p>The Period of the goal </p> <p>The name of the goal</p> <p>The text of the comment </p> <p>The <strong>[!UICONTROL Open in web app]</strong> button which opens the [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> button which allows you to manage your notifications.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Someone liked an update on my Goal</strong></td> 
   <td> <p>You receive an email when someone likes a comment you made on a goal or when you update the progress of your results or activities on the goal. </p> <p>The name of the person who liked the update</p> <p>The Period of the goal </p> <p>The name of the goal</p> <p>The <strong>[!UICONTROL Open in web app]</strong> button which opens the [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> button which allows you to manage your notifications.</p> </td> 
  </tr> 
 -->

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
