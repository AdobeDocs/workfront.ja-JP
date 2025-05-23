---
content-type: reference
navigation-topic: notifications
title: 通知：Goals
description: 通知：Goals
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: 585a65c497211c84cffafeeaa5016218fd66acd2
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 92%

---

# 通知：Goals

プロファイルから、[!DNL Adobe Workfront Goals] で発生したイベントのメール通知を有効にすることができます。ユーザーが[!UICONTROL プラン]ライセンスを使用して、他のユーザーに対して有効にすることもできます。詳しくは、[[!DNL Adobe Workfront]  の通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## アクセス要件

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>製品</strong></td> 
   <td>[!DNL Workfront Goals] <p>[!DNL Workfront Goals] について詳しくは、<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!DNL Goals] に対する[!UICONTROL View]以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront]管理者によってアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

+++

## 前提条件

* [!DNL Goals] 通知を更新するユーザーには、[!UICONTROL &#x200B; メインメニュー &#x200B;] の [!DNL Goals] 領域を含むレイアウトテンプレートが必要です。


## [!UICONTROL &#x200B; ユーザープロファイル &#x200B;]エリアにある [!DNL Goals] の通知

次のテーブルに表示される通知は、[!DNL Workfront Goals] で発生しているイベントに関する警告です。例えば、目標、結果、アクティビティを割り当てているユーザーや、所有する目標、結果、アクティビティを更新しているユーザーなどです。受信する通知の設定について詳しくは、[自身のメール通知の変更](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)を参照してください。

![ 通知環境設定 ](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>[!DNL Goals] のインスタント通知は、デフォルトでは無効になっています。毎日の通知を有効または無効にすることはできません。また、このカテゴリのイベントに関する日々のダイジェストメールを受信することもできません。[!DNL Goals] カテゴリのインスタント通知を個別に有効または無効にできます。

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

<!--these were removed at some point: 

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
