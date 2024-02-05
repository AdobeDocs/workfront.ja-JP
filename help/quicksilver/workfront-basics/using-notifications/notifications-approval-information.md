---
content-type: reference
navigation-topic: notifications
title: 通知：承認情報
description: 以下の通知は、自分が関係する作業アイテムで承認アクティビティが発生したことを知らせるものです。受信する通知の設定について詳しくは、「独自の電子メール通知を変更する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 95%

---

# 通知：承認情報

以下の通知は、自分が関係する作業アイテムで承認アクティビティが発生したことを知らせるものです。受信する通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

[イベント通知](../../workfront-basics/using-notifications/event-notifications.md)も参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>含まれるフィールド </p> <p> *日次ダイジェストフィールドのみ</p> </th> 
   <th>デフォルトステータス</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>委任されたイシューの承認リクエストが完了しました</strong> </p> <p>別のユーザーに委任したイシューの承認が、そのユーザーによって承認または却下されました。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Issue Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt;</em></p> <p>日刊ダイジェスト通知の件名：<em> [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> <p>イシュー名<br>プロジェクト名<br>イシュー参照番号<br>代理でイシューを承認または却下したユーザー名<br>承認決定<br>イシューステータス<br>承認申請者名<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*委任されたイシューの承認の総数<br>*イシュー名<br>*承認者名<br>*日刊ダイジェストの日付<br><br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>委任されたプロジェクトの承認リクエストが完了しました</strong> </p> <p>別のユーザーに委任したプロジェクトの承認が、そのユーザーによって承認または却下されました。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Project Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt;</em></p> <p><em>日刊ダイジェスト通知の件名は次のとおりです：[!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em> </p> </td> 
   <td> プロジェクト名<br>[!UICONTROL Portfolio Name]<br>[!UICONTROL Project Reference Number]<br>代理でプロジェクトを承認または却下したユーザー名<br>[!UICONTROL Approval Decision]<br>[!UICONTROL Project Status]<br>承認申請者名<br><strong>[!UICONTROL See More Details]</strong> ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*承認者名<br>[!UICONTROL *Date of the daily digest]<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>委任されたタスクの承認リクエストが完了しました</strong> </p> <p>別のユーザーに委任したタスクの承認が、そのユーザーによって承認または却下されました。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Task Approval/ Rejection Made on Your Behalf by] &lt;User Name&gt;</em></p> <p>日刊ダイジェスト通知の件名は次のとおりです：<em> [!UICONTROL Digest of Approval Information] &lt;Date of daily digest&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>代理でタスクを承認または却下したユーザー名<br>承認の決定<br>タスクステータス<br>承認申請者名<br><strong>詳細を見る</strong>ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*委任されたタスクの承認の合計数<br>*タスク名<br>*承認者名<br>*日刊ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメント承認リクエストがキャンセルされました</strong> </p> <p>ドキュメントのドキュメント承認者は、ドキュメント承認リクエストがキャンセルされると、メール通知を受け取ります。</p> <p>インスタント通知メールの件名：<em>&lt;User Name&gt; [!UICONTROL canceled the document approval request]</em></p> <p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </p> </td> 
   <td> 承認リクエストをキャンセルしたユーザー名<br>[!UICONTROL Document Name] </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私は承認者として委任されました</strong> </p> <p>誰かに承認を委任されると、メール通知が届きます。 </p> <p>インスタント通知メールの件名：<em>[!UICONTROL Delegated] &lt;Object Type&gt; [!UICONTROL Approval - Please Review] &lt;Object Name&gt;</em></p> <p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL Parent Object Name]<br>[!UICONTROL Object Reference Number]<br>承認用にオブジェクトを送信したユーザー名<br>オブジェクトを承認する代理ユーザー名<br>オブジェクトステータス<br>承認申請日時<br>オブジェクトの優先度<br>承認ステップ名<br>オブジェクトの [!UICONTROL Planned Completion Date]<br><strong>[!UICONTROL Make Approval Decision]</strong> ボタン</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のタイムシートが承認されました</strong> </p> <p>自分のタイムシートが承認されると、メール通知が届きます。</p> <p>インスタント通知メールの件名：<em>[!UICONTROL Timesheet Approved]：&lt;Timesheet Start Date&gt; - &lt;Timesheet End Date&gt;</em></p> <p> <p>メモ：この通知を日刊ダイジェストメールに設定することはできません。</p> </p> </td> 
   <td> タイムシートを承認したユーザー名<br>タイムシートが承認された日時<br>タイムシートのステータス（[!UICONTROL Approved]）<br>タイムシートの開始日と終了日<br>タイムシートに記録された合計時間数<br>タイムシートに記録された超過時間数 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
 </tbody> 
</table>
