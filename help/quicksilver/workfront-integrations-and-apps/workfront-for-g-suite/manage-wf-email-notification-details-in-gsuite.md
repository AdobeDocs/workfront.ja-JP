---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: 管理 [!DNL Adobe Workfront] G Suite からの通知の詳細
description: G Suite で、通知メールAdobeを開くとき [!DNL Workfront] が送信された場合は、関連する作業項目の詳細を表示し、インボックスから離れることなく返信できます。 リクエストの承認などアクションが使用可能な場合は、Workfront for G Suite から直接これらのアクションを実行できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: d5ca31d8-3667-4405-a523-3dc248a94746
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 管理 [!DNL Adobe Workfront] 通知の詳細 [!DNL G Suite]

>[!NOTE]
>
>ここに [既知の問題](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 現在のバージョンの [!DNL Workfront for G Suite] 期待どおりに動作しない。 新しいバージョンで作業中で、このバージョンはにリリースされると予想されています [!DNL Google Marketplace] 近い将来に

In [!DNL G Suite]（通知電子メールを開いたとき） [!DNL Adobe Workfront] が送信された場合、関連する作業項目の詳細を表示し、 [!UICONTROL インボックス]. リクエストの承認などアクションが使用可能な場合は、 [!DNL Workfront for G Suite].

>[!NOTE]
>
> [!DNL Workfront for G Suite] は、受け取ることのできるほとんどすべてのタイプの電子メール通知をサポートします [!DNL Workfront] （約 120 種類）。 [!UICONTROL 日別ダイジェスト] から送信された電子メール [!DNL Workfront] 次に表示されない [!DNL Workfront for G Suite]. 詳しくは、 [!DNL Workfront] 電子メール通知のタイプについては、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
  </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

通知の詳細を次の場所から管理する前に： [!DNL G Suite]を

* インストール [!DNL Workfront for G suite]\
   手順については、 [インストール [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## 管理 [!DNL Adobe Workfront] 通知の詳細 [!DNL G Suite]

1. この [!DNL Workfront for G Suite] パネルが表示されない場合は、 [!DNL Workfront] アイコン ![](assets/wf-lion-icon.png) 内 [!DNL G Suite] ページの右端にあるアドオンサイドバー。
1. In [!DNL G Suite]、を開きます。 [!DNL Workfront] 通知メール。
1. クリック **[!UICONTROL すべての更新を表示]** （パネルの上部付近に表示される場合）。
1. クリック **[!UICONTROL 詳細]**.
1. 使用可能なオプションをクリックします。

   表示されるオプションは、開いた電子メール通知のタイプに関連しています。 例えば、タスクの承認を求める電子メール通知の場合、 **[!UICONTROL 承認]** および **[!UICONTROL 拒否]** 次のようなオプションの代わりに使用します。 **[!UICONTROL 作業]** または **[!UICONTROL 完了]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>電子メール通知のタイプ</th> 
      <th>アクション</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>タスクまたは問題</td> 
      <td><strong>[!UICONTROL 承認 ]</strong> それは <strong>[!UICONTROL 却下 ]</strong> それは <strong>[!UICONTROL 付与 ]</strong> アクセス可能 <strong>[!UICONTROL 無視 ]</strong> アクセスを要求する <strong>[!UICONTROL の操作 ]</strong>または、「 」オプションをクリックして、 <strong>[!UICONTROL 完了 ]</strong> その</td> 
     </tr> 
     <tr> 
      <td>プロジェクト</td> 
      <td><strong>[!UICONTROL 承認 ]</strong> それは <strong>[!UICONTROL 却下 ]</strong> それは <strong>[!UICONTROL 付与 ]</strong> アクセスするか、 <strong>[!UICONTROL 無視 ]</strong> アクセスの要請</td> 
     </tr> 
     <tr> 
      <td>ドキュメント</td> 
      <td><strong>[!UICONTROL 承認 ]</strong> それは <strong>[!UICONTROL 却下 ]</strong> それは <strong>[!UICONTROL 付与 ]</strong> アクセスするか、 <strong>[!UICONTROL 無視 ]</strong> アクセスの要請</td> 
     </tr> 
     <tr> 
      <td>更新 </td> 
      <td> <p>項目の更新のリスト全体の任意の部分を表示して、必要なコンテキストを取得する <strong>[!UICONTROL Post]</strong> 新しい更新または <strong>[!UICONTROL 返信 ]</strong>. 次をクリックできます。 <strong>[!UICONTROL 通知 ]</strong> 返信に関して特定のユーザーに警告する場合。 </p> <p>詳しくは、 <a href="../../workfront-integrations-and-apps/workfront-for-g-suite/reply-to-wf-update-notification-from-gsuite.md" class="MCXref xref">返信先： [!DNL Adobe Workfront] 通知を更新 [!DNL G Suite]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>承認リクエスト</td> 
      <td><strong>[!UICONTROL 承認 ]</strong> または <strong>[!UICONTROL 却下 ]</strong> （他のオプションをクリックして、心を変えることができます）、ダウンロード、所有者の表示、または参照番号の表示を行うことができます</td> 
     </tr> 
     <tr> 
      <td>プロジェクトのステータスの変更</td> 
      <td> カスタムフォームを含め、プロジェクトに関する現在の情報をすべて表示します。 </td> 
     </tr> 
    </tbody> 
   </table>
