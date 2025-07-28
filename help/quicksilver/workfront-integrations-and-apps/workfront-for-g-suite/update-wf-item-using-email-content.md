---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: メールコンテンツを使用したGoogle Workspaceからのア  [!DNL Adobe Workfront]  テムの更新
description: Adobe Workfront 以外のメールに含まれている情報を使用して、既存のプロジェクト、タスクまたはイシューを更新できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 68%

---

# メールコンテンツを使用した [!DNL Google Workspace] からの [!DNL Adobe Workfront] アイテムの更新

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Google Workspaceの次のWorkfront機能は、**2026 年 2 月 28 日** 以降は使用できなくなります。
>
>* Workfront内からのGoogle Workspace機能へのアクセス
>
>* Gmail またはWorkfrontのカレンダーサイトパネルからのGoogle タスクの表示と管理
>
>Google Workspaceを使用した組織の統合のニーズに対しては、Workfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能については、{Gmail モジュール [ および ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)2}Google カレンダーモジュール [ を参照してください。](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)

[!DNL Adobe Workfront] 以外のメールに含まれている情報を使用して、既存のプロジェクト、タスクまたはイシューを更新できます。

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

[!DNL Google Workspace] からのメールコンテンツを使用して [!DNL Workfront] アイテムを更新するには、まず以下を行う必要があります。

* [!DNL Workfront for Google Workspace] のインストール\
   手順については、[インストール [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)を参照してください。

## [!DNL Google Workspace] からのメールコンテンツを使用して [!DNL Workfront] アイテムを更新

1. Google Workspaceの [!UICONTROL Workfront] パネルが表示されない場合は、ページの右端にある ![ アドオンサイドバーのWorkfront アイコン ](assets/wf-lion-icon.png)2&rbrace;Workfront アイコン）をクリックします。[!DNL Google Workspace]
1. メールメッセージを [!DNL Google Workspace] で開いた状態で、[!DNL Google Workspace] パネルの「**[!UICONTROL 新しい更新として投稿]**」をクリックします。
1. 「**[!UICONTROL タイプ]**」でドロップダウン矢印をクリックし、続いて更新を追加するオブジェクトのタイプをクリックします。
1. 「**[!UICONTROL 検索]**」オプションをクリックし、更新を追加するオブジェクトの名前を入力していき、目的のアイテムが下のリストに表示されたら選択します。

   このオプションは、手順 3 で選択した内容によって異なります。「**[!UICONTROL プロジェクトを検索]**」、「**[!UICONTROL タスクを検索]**」、「**[!UICONTROL イシューを検索]**」のいずれかです。

   >[!NOTE]
   >
   >タスクの名前を入力する際、アドホックな個人タスクは下に表示される名前のリストから除外されます。

1. 以下のオプションを任意に変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Update]</td> 
      <td>メールの件名行と本文テキストから取得したこのテキストの任意の部分を編集します。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td><p>（メールに少なくとも 1 つの添付ファイルが含まれている場合にのみ使用できます）。 タスクまたは問題の [!UICONTROL ドキュメント &#x200B;] タブに添付ファイルを保存するには、このオプションをクリックします。 </p><p>添付ファイルを保存しない場合は、名前の右にある X をクリックします。 </p><p>メールに [!DNL Google Drive] 内のドキュメントへのリンクが含まれている場合、そのリンクは作成中のタスクやイシューの「[!UICONTROL Overview]」タブに保存されます。 </p><p>重要：<span style="color: #ff1493;"><span style="color: #000000;">これが機能するには、</span></span>[!DNL Workfront] 管理者<span style="color: #ff1493;"><span style="color: #000000;">が [!DNL Google Drive] と [!DNL Workfront]</span></span> の連携を承認する必要があります</p>
      <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">通知</td> 
      <td>「<strong>[!UICONTROL Notify]</strong>」をクリックし、表示される「<strong>[!UICONTROL Search for a user or team]</strong>」オプションして、ユーザーまたはチームの名前を入力していき、目的の名前が下のリストに表示されたらクリックします。追加するユーザーおよびチームごとにこの手順を繰り返したあと、「<strong>[!UICONTROL Save]</strong>」をクリックします。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 更新]**」をクリックします。

   ブラウザーを更新すると、[!DNL Workfront for Google Workspace] パネルの下部にリンクが付いたメッセージが表示されて、メールが更新に変換されたことが確認されます。

   このリンクをクリックすると、手順 4 で指定したオブジェクトの、[!DNL Workfront] の「[!UICONTROL 更新]」タブに移動します。

   これらの手順を繰り返して、同じメールを更新、タスク、問題に変換できます（[ メールコンテンツを使用したAdobe Workfront イシューの作成  [!DNL Google Workspace]  を参照） ](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md) ブラウザーを更新したり、別のタイミングでメールに戻ったりすると、メール用に作成したすべてのリンクが、[!UICONTROL Google WorkspaceのWorkfront] パネルの下部に表示されます。

1. （オプション）以下のいずれかを行って、[!DNL Workfront] アドオンパネルで更新の操作を続けます。

   * 「**[!UICONTROL 更新]**」タブに別の更新を追加するには、「**[!UICONTROL 新しい更新を開始]**」をクリックして情報を入力します。

   * 「**[!UICONTROL 更新]**」タブの更新に返信するには、「**[!UICONTROL 返信]**」をクリックして返信を入力します。

     上記の両方のオプションについて、手順 5 と同様に、「**[!UICONTROL 通知]**」をクリックして返信の受信者を指定することができます。準備が整ったら、「**[!UICONTROL 投稿]**」をクリックして、更新を追加するか、返信します。

   * 「**[!UICONTROL 詳細]**」タブをクリックして、新しいプロジェクト、タスクまたはイシューの詳細を表示します。
