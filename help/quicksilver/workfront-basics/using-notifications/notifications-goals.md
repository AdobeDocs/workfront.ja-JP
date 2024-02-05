---
content-type: reference
navigation-topic: notifications
title: 「通知：Goals」
description: 「通知：Goals」
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 97%

---

# 通知：Goals

プロファイルから、[!DNL Adobe Workfront Goals] で発生したイベントのメール通知を有効にすることができます。ユーザーが[!UICONTROL プラン]ライセンスを使用して、他のユーザーに対して有効にすることもできます。詳しくは、[[!DNL Adobe Workfront]  の通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## アクセス要件

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

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

## 前提条件

[!DNL Goals] の通知が更新されるユーザーは、次の条件を満たす必要があります。

* [!UICONTROL メインメニュー]の [!DNL Goals] エリアを含むレイアウトテンプレート
* 新しい [!DNL Adobe Workfront] エクスペリエンスに切り替える。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!UICONTROL  ユーザープロファイル ]エリアにある [!DNL Goals] の通知

次のテーブルに表示される通知は、[!DNL Workfront Goals] で発生しているイベントに関する警告です。例えば、目標、結果、アクティビティを割り当てているユーザーや、所有する目標、結果、アクティビティを更新しているユーザーなどです。受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/goals-notifications-preferences-350x114.png)

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
   <td> <p>コメントを残したユーザーの名前</p> <p>目標の期間 </p> <p>目標の名前</p> <p>コメントのテキスト</p> <p>[!UICONTROL Goal Details] パネルを開く <strong>[!UICONTROL Open in web app]</strong> ボタン</p> <p><strong>[!UICONTROL Change Notifications Settings]</strong> ボタンで通知を管理できます。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>誰かが目標に関する自分のコメントを気に入りました</strong></td> 
   <td> <p>コメントを評価したユーザーの名前</p> <p>目標の期間 </p> <p>目標の名前</p> <p>コメントのテキスト </p> <p>[!UICONTROL Goal Details] パネルを開く <strong>[!UICONTROL Open in web app]</strong> ボタン</p> <p>通知の管理に使用する <strong>[!UICONTROL Change Notifications Settings]</strong> ボタン。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>誰かが自分の目標更新を評価しました</strong></td> 
   <td> <p>目標に対して行ったコメントを誰かが評価したとき、または目標に関する結果やアクティビティの進行状況を更新したときに、メールが送信されます。 </p> <p>更新を評価した人の名前</p> <p>目標の期間 </p> <p>目標の名前</p> <p>[!UICONTROL Goal Details] パネルを開く <strong>[!UICONTROL Open in web app]</strong> ボタン</p> <p>通知を管理できる <strong>[!UICONTROL Change Notifications Settings]</strong> ボタン。</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
