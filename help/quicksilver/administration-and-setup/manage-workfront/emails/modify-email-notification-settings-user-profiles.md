---
user-type: administrator
product-area: system-administration
keywords: 変更,メール,通知,設定,一括,一括編集,設定,複数,ユーザー
navigation-topic: emails-administration
title: 複数のユーザーの電子メール通知設定を変更する
description: この記事では、Workfrontまたはグループ管理者が他のユーザーの電子メール通知を更新する方法について説明します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 82%

---

# 複数のユーザーの電子メール通知設定を変更する

<!-- Audited: 12/2023 -->

Adobe Workfront 管理者、または他のユーザーの設定を編集できるプランナーのアクセスレベルを持つユーザーは、一度に複数のユーザーの通知設定を設定できます。ユーザーがイベント発生時に通知を受信するか、1 通の日次ダイジェストメールで受信するかを指定することも含まれます。詳しくは、[Adobe Workfront の通知](../../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。ユーザーの編集に必要なアクセスレベルについて詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

また、自分のプロファイルを含め、ユーザーに対するメール通知を一度に 1 人ずつ設定することもできます。詳しくは、 [独自の電子メール通知を変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>新規プラン：標準 </p>
 <p>または</p> 
<p>現在のプラン：プラン </p> 
</td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 複数のユーザーの電子メール通知設定を変更する

通知設定を一括で設定する場合、選択したユーザーに共通した設定のみを変更できます。

通知設定を変更すると、**編集済み**&#x200B;ラベルがその通知設定に対して表示され、通知設定が変更されたことがわかります。

複数のユーザーの電子メール通知設定を変更するには：

{{step-1-to-users}}

1. ユーザーを選択し、「**編集**」をクリックします。
1. 表示される&#x200B;**ユーザーを編集**&#x200B;ボックスで、「**通知**」をクリックします。

1. カテゴリを展開して、そのカテゴリに関連する通知設定を表示します。

   1 人以上のユーザーを選択し、そのユーザーの通知が他の選択したユーザーの通知と一致しない場合、その通知のカテゴリのチェックボックスには、チェックマークの代わりに水平線 ![](assets/straight-line-instead-of-checkmark.jpg) が表示されます。


1. ユーザーが日次または即時に受信する通知をクリックするか、または受信を停止する通知をクリアします。

   >[!NOTE]
   >
   >   **コミュニケーション**&#x200B;のカテゴリでは、個々の通知を選択して即時配信のみを行うことができます。日次ダイジェストで配信される通知をすべて選択する必要があります。


1. 日次ダイジェストとして送信する通知を選択した場合は、ダイジェストを配信する時刻を、**この時間を過ぎると日次ダイジェストを送信**&#x200B;メニューの「**通知**」セクションの上部で選択します。

   ![](assets/daily-digest-time.png)

   日次ダイジェストには、選択した時間の 24 時間前に通知の条件を満たすイベントが含まれます。ユーザーは、通知タイプごとに 1 通の日次ダイジェストメールを受け取ります。

   日次ダイジェストは、システムで配信用にキューに入れられているメールの数に応じて、選択した時間の後に到着する場合があります。一覧に表示される時刻は、ブラウザー設定で指定されたローカル時間です。
