---
content-type: reference
navigation-topic: notifications
title: '通知：承認情報'
description: 以下の通知は、関係する作業項目での承認アクティビティの発生に関する警告です。 受信する通知の設定については、「独自のイベント通知をアクティブ化または非アクティブ化する」を参照してください。
author: Lisa
feature: Get Started with Workfront
exl-id: e152913e-de7e-405f-af63-827a9b91e2ae
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 6%

---

# 通知：承認情報

以下の通知は、関係する作業項目での承認アクティビティの発生に関する警告です。 受信する通知の設定については、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

関連トピック [イベント通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>含まれるフィールド </p> <p> *日別のダイジェストフィールドのみ</p> </th> 
   <th>デフォルトのステータス</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>問題の代理承認要求が完了しました</strong> </p> <p>別のユーザーに委任した問題の承認が、そのユーザーによって承認または却下されました。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 自分に代わって行われた問題の承認/拒否 ] &lt;user name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 承認情報のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名<br>プロジェクト名<br>問題の参照番号<br>代理で問題を承認または却下したユーザーの名前<br>承認の決定<br>問題ステータス<br>承認をリクエストしたユーザーの名前<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*委任された問題の承認の合計数<br>*問題名<br>*承認者名<br>*日別ダイジェストの日付<br><br></p> </td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>プロジェクトの代理承認要求が完了しました</strong> </p> <p>別のユーザーに委任したプロジェクト承認が、そのユーザーによって承認または却下されました。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 自分に代わっておこなわれたプロジェクトの承認/拒否 ] &lt;user name=""&gt;</em></p> <p><em>日次ダイジェスト通知の件名は次のとおりです。[!UICONTROL 承認情報のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em> </p> </td> 
   <td> プロジェクト名<br>[!UICONTROLPortfolio名 ]<br>[!UICONTROL プロジェクト参照番号 ]<br>代理でプロジェクトを承認または却下したユーザーの名前<br>[!UICONTROL 承認の決定 ]<br>[!UICONTROL プロジェクトのステータス ]<br>承認をリクエストしたユーザーの名前<br><strong>[!UICONTROL 詳細を表示 ]</strong> ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*承認者名<br>[!UICONTROL *1 日のダイジェストの日付 ]<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>タスクの代理承認要求が完了しました</strong> </p> <p>別のユーザーに委任したタスクの承認が、そのユーザーによって承認または却下されました。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 自分に代わっておこなわれたタスクの承認/拒否 ] &lt;user name=""&gt;</em></p> <p>日次ダイジェスト通知の件名は次のとおりです。<em> [!UICONTROL 承認情報のダイジェスト ] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> タスク名<br>プロジェクト名<br>タスク参照番号<br>代理でタスクを承認または却下したユーザーの名前<br>承認の決定<br>タスクステータス<br>承認をリクエストしたユーザーの名前<br><strong>詳細を表示</strong> ボタン<br>*プロジェクト参照番号<br>*プロジェクト名<br>*委任されたタスク承認の合計数<br>*タスク名<br>*承認者名<br>*日別ダイジェストの日付<br></td> 
   <td><strong>日次</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>ドキュメント承認要求がキャンセルされた</strong> </p> <p>ドキュメントのドキュメント承認者は、ドキュメント承認リクエストがキャンセルされると、電子メール通知を受け取ります。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>&lt;user name=""&gt; [!UICONTROL がドキュメント承認リクエストをキャンセルしました ]</em></p> <p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </p> </td> 
   <td> 承認リクエストをキャンセルしたユーザーの名前<br>[!UICONTROL ドキュメント名 ] </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>私は承認者の役割を委任されました</strong> </p> <p>誰かがあなたに承認を委任した場合は、電子メール通知が送信されます。 </p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL 委任 ] &lt;object type=""&gt; [!UICONTROL 承認 — 確認してください ] &lt;object name=""&gt;</em></p> <p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </p> </td> 
   <td> <p>[!UICONTROL Object Name]<br>[!UICONTROL 親オブジェクト名 ]<br>[!UICONTROL オブジェクト参照番号 ]<br>承認用にオブジェクトを送信したユーザーの名前<br>オブジェクトを承認するユーザーの名前<br>オブジェクトステータス<br>承認がリクエストされた日時<br>オブジェクトの優先度<br>承認ステップ名<br>オブジェクトの [!UICONTROL 計画完了日 ]<br><strong>[!UICONTROL 承認を決定 ]</strong> ボタン</p> </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>自分のタイムシートが承認された</strong> </p> <p>タイムシートが承認されると、電子メール通知が送信されます。</p> <p>即時通知 E メールの件名は次のとおりです。 <em>[!UICONTROL タイムシート承認済み ]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> <p>注意：この通知は、毎日のダイジェスト電子メールには設定できません。</p> </p> </td> 
   <td> タイムシートを承認したユーザーの名前<br>タイムシートが承認された日時<br>タイムシートのステータス（[!UICONTROL 承認済み ]）<br>タイムシートの開始日と終了日<br>タイムシートに記録された合計時間数<br>タイムシートに記録された残業時間 </td> 
   <td><strong>今すぐ</strong> </td> 
  </tr> 
 </tbody> 
</table>
