---
product-area: workfront-integrations
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: G Suite から  [!DNL Adobe Workfront]  通知の詳細の管理
description: G Suite で、Adobe  [!DNL Workfront]  が送信した通知メールを開く際に、関連する作業項目の詳細を表示し、インボックスから離れることなく返信できます。リクエストの承認などアクションが使用可能な場合は、Workfront for G Suite から直接これらのアクションを実行できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 97%

---

# [!DNL G Suite] からの [!DNL Adobe Workfront] 通知の詳細の管理

>[!NOTE]
>
>Google 用の Adobe Workfront プラグインの最新バージョンは、2023年6月26日にリリースされました。

[!DNL G Suite] で、[!DNL Adobe Workfront] が送信した通知メールを開く際に、関連する作業項目の詳細を表示し、[!UICONTROL インボックス]から離れることなく返信できます。リクエストの承認などアクションが使用可能な場合は、[!DNL Workfront for G Suite] から直接これらのアクションを実行できます。

>[!NOTE]
>
> [!DNL Workfront for G Suite] は、[!DNL Workfront] から受信できるほとんどすべてのタイプのメール通知をサポートします（約 120 種類）。[!DNL Workfront] から送信される[!UICONTROL 日次ダイジェスト]が [!DNL Workfront for G Suite] に表示されません。詳しくは、 [!DNL Workfront] 電子メール通知のタイプについては、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL G Suite] から通知の詳細を管理する前に、次の操作を実行する必要があります。

* [!DNL Workfront for G suite] をインストール\
   手順について詳しくは、[インストール [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)を参照してください。

## [!DNL G Suite] から [!DNL Adobe Workfront] 通知の詳細の管理

1. [!DNL Workfront for G Suite] パネルが表示されない場合は、ページの右端にある [!DNL G Suite] アドオンサイドバーの [!DNL Workfront] アイコン ![](assets/wf-lion-icon.png) をクリックします。
1. [!DNL G Suite] で [!DNL Workfront] 通知メールを開きます。
1. パネルの上部付近に表示される場合、「**[!UICONTROL すべての更新を表示]**」をクリックします。
1. 「**[!UICONTROL 詳細]**」をクリックします。
1. 使用可能なオプションをクリックします。

   表示されるオプションは、開いたメール通知のタイプに関連しています。例えば、タスクの承認を求めるメール通知の場合、「**[!UICONTROL 作業中]**」オプションまたは「**[!UICONTROL 完了]**」のオプションの代わりに、「**[!UICONTROL 承認]**」および「**[!UICONTROL 拒否]**」が表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>メール通知のタイプ</th> 
      <th>アクション</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>タスクまたはイシュー</td> 
      <td><strong>[!UICONTROL Approve]</strong> する、<strong>[!UICONTROL Reject]</strong> する、アクセスを <strong>[!UICONTROL Grant]</strong> する、アクセスのリクエストを <strong>[!UICONTROL Ignore]</strong> する、<strong>[!UICONTROL Work on it]</strong> または <strong>[!UICONTROL Done]</strong> であることを示すオプションをクリックする</td> 
     </tr> 
     <tr> 
      <td>プロジェクト</td> 
      <td><strong>[!UICONTROL Approve]</strong> する、<strong>[!UICONTROL Reject]</strong> する、アクセスを <strong>[!UICONTROL Grant]</strong> するまたは アクセスのリクエストを <strong>[!UICONTROL Ignore]</strong> する</td> 
     </tr> 
     <tr> 
      <td>ドキュメント</td> 
      <td><strong>[!UICONTROL Approve]</strong> する、<strong>[!UICONTROL Reject]</strong> する、アクセスを <strong>[!UICONTROL Grant]</strong> する、アクセスのリクエストを <strong>[!UICONTROL Ignore]</strong> する</td> 
     </tr> 
     <tr> 
      <td>アップデート </td> 
      <td> <p>新しい更新を <strong>[!UICONTROL Post]</strong> または <strong>[!UICONTROL Reply]</strong> することが必要なコンテキストを把握できるように、項目の更新のリスト全体の任意の部分を表示します。<strong>[!UICONTROL Notify]</strong> をクリックして、返信に関して特定のユーザーに警告を送信できます。 </p> <p>詳しくは、<a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">[!DNL G Suite]</a> から [!DNL Adobe Workfront] 更新通知への返信を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td>承認リクエスト</td> 
      <td><strong>[!UICONTROL Approve]</strong> するかまたは <strong>[!UICONTROL Reject]</strong> する（他のオプションをクリックして変更可能）、ダウンロードする、所有者を表示するまたは参照番号を表示する</td> 
     </tr> 
     <tr> 
      <td>プロジェクトのステータスの変更</td> 
      <td> カスタムフォームを含め、プロジェクトに関する現在の情報をすべて表示します。 </td> 
     </tr> 
    </tbody> 
   </table>
