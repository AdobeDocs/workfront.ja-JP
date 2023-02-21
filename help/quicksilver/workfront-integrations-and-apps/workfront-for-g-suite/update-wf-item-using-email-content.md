---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: の更新 [!DNL Adobe Workfront] メールコンテンツを使用する G スイートの項目
description: Adobe Workfront以外の E メールからの情報に関する既存のプロジェクト、タスクまたはイシューを更新できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# の更新 [!DNL Adobe Workfront] 項目： [!DNL G Suite] e メールコンテンツの使用

>[!NOTE]
>
>ここに [既知の問題](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 現在のバージョンの [!DNL Workfront for G Suite] 期待どおりに動作しない。 新しいバージョンで作業中で、このバージョンはにリリースされると予想されています [!DNL Google Marketplace] 近い将来に

既存のプロジェクト、タスクまたはイシューを、以外の[!DNL Adobe Workfront] 電子メール。

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

事前に [!DNL Workfront] メールコンテンツを使用する項目 [!DNL G Suite]を

* インストール [!DNL Workfront for G suite]\
   手順については、 [インストール [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## の更新 [!DNL Workfront] メールコンテンツを使用する項目 [!DNL G Suite]

1. この [!UICONTROL Workfront for G Suite] パネルが表示されない場合は、「Workfront」アイコン ![](assets/wf-lion-icon.png) 内 [!DNL G Suite] ページの右端にあるアドオンサイドバー。
1. 電子メールメッセージをで開きます。 [!DNL G Suite]をクリックし、 **[!UICONTROL 新しい更新として投稿]** 内 [!DNL G Suite] パネル。
1. の下 **[!UICONTROL タイプ]**」をクリックし、ドロップダウン矢印をクリックして、更新を追加するオブジェクトのタイプをクリックします。
1. 次をクリック： **[!UICONTROL を検索]** 「 」オプションで、更新を追加するオブジェクトの名前の入力を開始し、下のリストに表示されたら項目を選択します。

   このオプションは、手順 3 で選択した内容に応じて異なります。 そうかもしれません **[!UICONTROL プロジェクトの検索]**, **[!UICONTROL タスクの検索]**&#x200B;または **[!UICONTROL 問題を検索]**.

   >[!NOTE]
   >
   >タスクの名前を入力すると、アドホックな個人タスクは下に表示される名前のリストから除外されます。

1. 次のオプションの変更を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 更新 ]</td> 
      <td>E メールの件名行と本文から取得した、このテキストの任意の部分を編集します。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 電子メールの添付ファイルを含める ]</td> 
      <td><p>（E メールに少なくとも 1 つの添付ファイルが含まれている場合にのみ使用できます）。 タスクまたはイシューの「[!UICONTROL ドキュメント ]」タブに添付ファイルを保存するには、このオプションをクリックします。 </p><p>添付ファイルを保存しない場合は、名前の右にある X をクリックします。 </p><p>電子メールにドキュメントへのリンクが含まれる場合は、 [!DNL Google Drive]リンクは、作成中のタスクまたは問題の「[!UICONTROL 概要 ]」タブに保存されます。 </p><p>重要： <span style="color: #ff1493;"><span style="color: #000000;">これを機能させるには、</span></span>[!DNL Workfront] administrator<span style="color: #ff1493;"><span style="color: #000000;"> 許可する [!DNL Google Drive] 働く [!DNL Workfront]</span></span></p>
      <p>このオプションを有効にした場合、タスク、問題、更新に変換する他のメールに対しても有効なままになります。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知 </td> 
      <td>クリック <strong>[!UICONTROL 通知 ]</strong>、 <strong>[!UICONTROL ユーザーまたはチームの検索 ]</strong> オプションが表示されたら、ユーザーまたはチームの名前を入力し、下のリストに表示されたらクリックします。 追加する各ユーザーとチームに対してこの手順を繰り返し、 <strong>[!UICONTROL 保存 ]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 更新]**.

   ブラウザーを更新すると、 [!DNL Workfront for G Suite] 電子メールを更新に変換したことを確認するパネルが表示されます。

   リンクをクリックすると、 [!UICONTROL 更新] タブ [!DNL Workfront] 手順 4 で指定したオブジェクトの

   これらの手順を繰り返して、同じ電子メールを更新、タスクおよびタスクに変換できます ( [E メールコンテンツを使用して、[!DNL G Suite] でAdobe Workfrontイシューを作成する](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)) をクリックします。 ブラウザーを更新したり、別の時点で電子メールに戻ったりすると、電子メールに対して作成したすべてのリンクが [!UICONTROL Workfront for G Suite] パネル。

1. （オプション）更新を引き続き [!DNL Workfront] 次のいずれかの操作を行って、アドオンパネルを追加します。

   * 別の更新を **[!UICONTROL 更新]** タブ、クリック **[!UICONTROL 新しい更新を開始]** 情報を入力します。

   * の更新に返信するには **[!UICONTROL 更新]** タブ、クリック **[!UICONTROL 返信]** 返信を入力します。

      上記のオプションの両方で、 **[!UICONTROL 通知]** をクリックして、手順 5 に従って返信の受信者を指定します。 準備が整ったら、「 **[!UICONTROL 投稿]** をクリックして、更新または返信を追加します。

   * 次をクリック： **[!UICONTROL 詳細]** タブをクリックして、新しいプロジェクト、タスク、またはタスクの詳細を表示します。
