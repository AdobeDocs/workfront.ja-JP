---
navigation-topic: notifications
title: アプリ内通知の表示と管理
description: アプリ内通知では、お知らせ通知と作業項目通知の 2 種類の情報を常に確認できます。Web アプリケーションとモバイルアプリケーションの両方から利用できます」
author: Lisa
feature: Get Started with Workfront
exl-id: 4c5da114-33cc-422b-84f4-67bc7fcd67c6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: ht
source-wordcount: '938'
ht-degree: 100%

---

# アプリ内通知の表示と管理

アプリ内通知では、お知らせ通知と作業アイテム通知の 2 種類の情報について常に知らせます。Web アプリケーションとモバイルアプリケーションの両方から使用できます。

受け取る作業アイテムとお知らせの通知のリストについては、[アプリ内通知の概要](../../workfront-basics/using-notifications/in-app-notifications-overview.md)を参照してください。

>[!NOTE]
>
>* 作業アクティビティのアプリ内通知は、[!DNL Workfront] のメール通知に結び付けられません。詳しくは、[[!DNL Adobe Workfront]  の通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。
>* アプリ内通知はカスタマイズできません。
>



## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

保有するプランまたはライセンスタイプを確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 通知の表示

[!DNL Workfront] の右上隅にある番号付きアイコンは、まだ確認していない通知の数を表示します。

>[!NOTE]
>
>Web アプリケーションとモバイルアプリケーションの両方から、すべてのアプリ内通知を表示できます。これらの通知の一部のみが、モバイルアプリケーションでプッシュ通知として送信されます。モバイルアプリでの通知について詳しくは、iOS 用の ](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)[[!DNL Adobe Workfront]  または Android 用の [[!DNL Adobe Workfront] ](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) を参照してください。

1. [!DNL Workfront] の右上隅で番号付きアイコン ![](assets/notifications-icon-jewel.jpg) をクリックし、通知のリストを開きます。

   最新の未読の通知が番号付きアイコンの下に表示され、一番上に最新の未読の通知が表示されます。

   ![最近の未読の通知](assets/qs-notifications-350x330.png)

   スクロール可能なリストには、最大 80 件の通知が表示されます。さらに多くの情報を見るには、リストの一番下にある「**[!UICONTROL すべての通知]**」をクリックすると、最大 100 件の通知が表示されます。通知は、30 日後に自動的に削除されます。

   各通知の下部に、[!UICONTROL 通知タイプ]と対応する識別アイコンが表示されます。これらは、明記された [!DNL Workfront] の項目に何が起こったかを特定するのに役立ち、アクション項目がある場合は、警告が表示されます。

   * お知らせの通知は、[!UICONTROL お知らせ]アイコン ![](assets/announcement.png) によって表示されます。

   * その他すべての通知は、関連付けられている作業アイテムのタイプを提案するアイコンによって表示されます。

     ![通知アイコン](assets/ntfcntype&icon-350x330.png)
青いドットの右側のアイコンには、次のいずれかが表示されます。

   * 情報（通常は、作業中の [!DNL Workfront] のオブジェクトの更新）を入力した人物のプロファイル写真。
   * 通知がシステムのお知らせの場合、[!DNL Workfront] ロゴ。


1. （オプション）通知を受け取った日付を表示する場合は、通知の右上隅にある日または時間のインジケーターの上にポインタを合わせます。

   ![](assets/hoveroverdate-350x437.png)

1. 表示する通知をクリックします。

   * クリックした通知が作業アイテムに関するものである場合は、関連する [!DNL Workfront] オブジェクトが開き、「**[!UICONTROL 更新]**」タブ上にメッセージ全体が表示されます。**[!UICONTROL 新しい更新エリアを開始]**&#x200B;または&#x200B;**[!UICONTROL 返信を入力]**&#x200B;できます。

     ![](assets/object-opens-click-work-ntfctn-qs-350x183.png)

   * クリックする通知がお知らせ用の場合、![](assets/announcement.png)**[!UICONTROL お知らせ]**&#x200B;ページが表示され、すべてのお知らせが表示されます。クリックしたお知らせが左側で選択され、メッセージが右側に表示されます。

     ![](assets/announcements-page-qs-350x210.png)

1. （オプション）通知メッセージに含まれている添付ファイルをダウンロードするか、すべての添付ファイルを ZIP ファイルとしてダウンロードします。

   ![](assets/download-attachments-350x106.png)

## 通知の確認

通知を表示した後で、通知を確認して、[!UICONTROL 通知]リストから取り除き、後で返信するように残します。

[!UICONTROL 通知]ページで、現在の通知とクリアされた通知を表示できます。クリアした通知を[!UICONTROL 通知]リストに戻すこともできます。

* [通知の確認](#acknowledge-notifications)
* [確認済みの通知を表示](#view-acknowledged-notifications)

### 通知の確認

番号付きアイコンをクリックして通知リストを開いても、すべての通知を読み取ったことを自動的には認識しません。

通知を確認し、通知リストからクリアするには、次の手順に従います。

1. [!DNL Workfront] の右上隅にある番号付きアイコン ![](assets/notifications-icon-jewel.jpg) をクリックして、通知リストを開きます。
1. 次のいずれかの操作を行います。

   * 通知の左上隅にある青い点をクリックします。
   * 通知が（お知らせではなく）作業アイテムに対する通知の場合は、通知をクリックすると、そのアイテムに移動します。
   * お知らせの通知の場合は、通知をクリックすると、**[!UICONTROL お知らせ]**&#x200B;ページが開きます。
   * 通知リストの右下隅にある「**[!UICONTROL すべての通知]**」をクリックして、**[!UICONTROL 通知]**&#x200B;ページを表示したあと、Workfront の右上にある「**[!UICONTROL すべてを既読とマーク]**」をクリックします。

### 確認済みの通知を表示

既に確認した通知を表示するには、次の手順に従います。

1. [!DNL Workfront] の右上隅にある番号付きアイコン ![](assets/notifications-icon-jewel.jpg) をクリックして、通知リストを開きます。
1. 通知リストの右下隅にある「**[!UICONTROL すべての通知]**」をクリックします。
1. 表示された&#x200B;**[!UICONTROL 通知]**&#x200B;ページで、下にスクロールして過去の通知を表示します。
1. （オプション）確認済み通知を通知リストに戻すには、通知の横にある青い円をクリックします。

## お知らせ通知の削除

作業アイテムの通知は削除できません。[!DNL Workfront] では、30 日後にすべての通知（既読か未読かにかかわらず）を削除します。

ただし、お知らせの通知は削除できます。また、削除後 30 日以内であれば、削除したお知らせにアクセスすることもできます。[!DNL Workfront] では、お知らせは自動的には削除されません。

* [お知らせを削除](#delete-an-announcement)
* [最近削除したお知らせにアクセスし復元](#access-and-restore-an-announcement-you-deleted-recently)

### お知らせを削除

1. [!DNL Workfront] の右上隅にある番号付きアイコン ![](assets/notifications-icon-jewel.jpg) をクリックして、通知リストを開きます。
1. 「**[!UICONTROL お知らせ]**」または「**[!UICONTROL お知らせの表示]**」をクリックします。

1. 表示される&#x200B;**[!DNL Announcements]**&#x200B;ページで、削除するお知らせを左側のリストでクリックしたあと、「**[!UICONTROL 削除]**」をクリックします。

### 最近削除したお知らせにアクセスし復元

過去 30 日以内に削除した通知にアクセスできます。

1. [!DNL Workfront] の右上隅にある番号付きアイコン ![](assets/notifications-icon-jewel.jpg) をクリックして、通知リストを開きます。
1. 「**[!UICONTROL お知らせ]**」または「**[!UICONTROL お知らせの表示]**」をクリックします。

1. 表示された&#x200B;**[!UICONTROL お知らせ]**&#x200B;ページで、「**[!UICONTROL 削除済み]**」をクリックします。

1. 表示するメッセージをクリックします。
1. (オプション）お知らせを復元する場合は、お知らせの本文の右上にある「」**[!UICONTROL 受信トレイに移動]**&#x200B;をクリックします。
