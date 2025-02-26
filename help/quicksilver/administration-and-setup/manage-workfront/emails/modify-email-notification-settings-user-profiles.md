---
user-type: administrator
product-area: system-administration
keywords: 変更,メール,通知,設定,一括,一括編集,設定,複数,ユーザー
navigation-topic: emails-administration
title: 複数ユーザーのメール通知設定の変更
description: この記事では、Workfront 管理者またはグループ管理者が他のユーザーのメール通知を更新する方法について説明します。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: e8acdf8f7b3859385237e788dfda34ee62ee11d1
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 86%

---

# 複数ユーザーのメール通知設定の変更

<!-- Audited: 12/2023 -->

Adobe Workfront 管理者、または他のユーザーの設定を編集できるプランナーのアクセスレベルを持つユーザーは、一度に複数のユーザーの通知設定を設定できます。ユーザーがイベント発生時に通知を受信するか、1 通の日次ダイジェストメールで受信するかを指定することも含まれます。詳しくは、[Adobe Workfront の通知](../../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。ユーザーの編集に必要なアクセスレベルについて詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

また、自分のプロファイルを含め、ユーザーに対するメール通知を一度に 1 人ずつ設定することもできます。詳しくは、[自身のメール通知の変更](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>プラン</p></li>
         </ul>
   </td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 複数のユーザーのメール通知設定を変更する

通知設定を一括で設定する場合、選択したユーザーに共通した設定のみを変更できます。

通知設定を変更すると、**編集済み**&#x200B;ラベルがその通知設定に対して表示され、通知設定が変更されたことがわかります。

複数ユーザーのメール通知設定を変更するには：

{{step-1-to-users}}

1. ユーザーを選択し、「**編集**」をクリックします。
1. 表示される&#x200B;**ユーザーを編集**&#x200B;ボックスで、「**通知**」をクリックします。

1. カテゴリを展開して、そのカテゴリに関連する通知設定を表示します。

   少なくとも 1 人のユーザーが選択されていて、その通知が他の選択されたユーザーの通知と一致しない場合、その通知の「カテゴリ」チェックボックスには、チェックマークではなく横線 ![ チェックの代わりに線 ](assets/straight-line-instead-of-checkmark.jpg) が表示されます。


1. ユーザーが日次または即時に受信する通知をクリックするか、または受信を停止する通知をクリアします。

   >[!NOTE]
   >
   >   **コミュニケーション**&#x200B;のカテゴリでは、個々の通知を選択して即時配信のみを行うことができます。日次ダイジェストで配信される通知をすべて選択する必要があります。


1. 日次ダイジェストとして送信する通知を選択した場合は、ダイジェストを配信する時刻を、**この時間を過ぎると日次ダイジェストを送信**&#x200B;メニューの「**通知**」セクションの上部で選択します。

   ![ デイリーダイジェスト時間 ](assets/daily-digest-time.png)

   日次ダイジェストには、選択した時間の 24 時間前に通知の条件を満たすイベントが含まれます。ユーザーは、通知タイプごとに 1 通の日次ダイジェストメールを受け取ります。

   日次ダイジェストは、システムで配信用にキューに入れられているメールの数に応じて、選択した時間の後に到着する場合があります。一覧に表示される時刻は、ブラウザー設定で指定されたローカル時間です。
