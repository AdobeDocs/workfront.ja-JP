---
user-type: administrator
product-area: system-administration
keywords: 変更，電子メール，通知，設定，一括，一括編集，設定，複数，ユーザー
navigation-topic: emails-administration
title: ユーザーのプロファイルの電子メール通知設定を変更する
description: この記事では、Workfrontまたはグループ管理者が他のユーザーの電子メール通知を更新する方法について説明します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 658f97cd-0500-421d-9c89-26041ca59655
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# ユーザーのプロファイルの電子メール通知設定を変更する

Adobe Workfront管理者、または Planner のアクセスレベルで他のユーザーの設定を編集できる場合、一度に複数のユーザーの通知設定を構成できます。 これには、ユーザーがイベントとして通知を受け取るか、1 日のダイジェスト電子メールで通知を受け取るかを指定することが含まれます。詳しくは、 [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md). ユーザーの編集に必要なアクセスレベルについて詳しくは、 [ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

一括通知設定を構成する場合、選択したユーザーに共通する設定のみを変更できます。

>[!NOTE]
>
>また、自分のプロファイルを含め、一度に 1 人のユーザーに対する電子メール通知を設定することもできます。 詳しくは、 [独自の電子メール通知を変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプランまたはライセンスの種類を確認するには、Workfront管理者に問い合わせてください。

## 複数のユーザーの電子メール通知設定を一括で変更する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー** ![](assets/users-icon-in-main-menu.png). ユーザーを選択し、「 **編集**.
1. Adobe Analytics の **担当者の編集** 表示されるボックスで、 **通知**.

1. カテゴリを展開して、そのカテゴリに関連する通知設定を表示します。

   1 人以上のユーザーが選択し、そのユーザーの通知が他の選択したユーザーの通知と一致しない場合、その通知のカテゴリチェックボックスには水平線が表示されます ![](assets/straight-line-instead-of-checkmark.jpg) チェックマークの代わりに使用します。

1. ユーザーが毎日または即座に受信する通知をクリックするか、受信を停止する通知をクリアします。

   の **通信** 」カテゴリでは、個々の通知を選択して即時配信のみを行うことができます。 1 日のダイジェストで配信される通知をすべて選択する必要があります。

   通知設定を変更すると、ラベル **編集済み** はその通知設定に対して表示され、その通知設定が変更されたことを知らせます。

1. 日別のダイジェストとして送信する通知を選択した場合は、ダイジェストを配信する時刻を **通知** セクション内 **1 日のダイジェストの電子メール送信後** メニュー。

   配信時間を選択すると、 **1 日のダイジェストの電子メール送信後** ボックスに、配信の時刻が編集されたことを示すオレンジ色の枠が表示されます。

   1 日のダイジェストには、選択した時間の 24 時間前に通知の条件を満たすイベントが含まれます。 ユーザーは、通知タイプごとに 1 日に 1 通のダイジェスト電子メールを受け取ります。

   毎日のダイジェストは、選択した時間の後に、システムで配信用にキューに入れられている電子メールの数に応じて、到着する場合があります。 一覧に表示される時刻は、ブラウザー設定で指定されたローカル時間です。
