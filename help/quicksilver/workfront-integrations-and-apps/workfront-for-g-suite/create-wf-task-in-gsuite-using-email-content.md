---
product-area: workfront-integrations;projects
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: の作成 [!DNL Adobe Workfront] メールコンテンツを使用する G Suite のタスク
description: 外部 E メールを変換できます (Adobeで生成されません ) [!DNL Workfront]) をWorkfrontタスクに追加します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# の作成 [!DNL Adobe Workfront] タスク [!DNL G Suite] e メールコンテンツの使用

>[!NOTE]
>
>ここに [既知の問題](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) 現在のバージョンの [!DNL Workfront for G Suite] 期待どおりに動作しない。 新しいバージョンで作業中で、このバージョンはにリリースされると予想されています [!DNL Google Marketplace] 近い将来に

外部 E メールを ( [!DNL Adobe Workfront]) から [!DNL Workfront] タスク。

外部電子メールを既存のタスクの更新に変換することもできます。 詳しくは、 [の更新 [!DNL Adobe Workfront] 電子メールコンテンツを使用して [!DNL G Suite] から取得した項目](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

の使用に関する情報 [!DNL G Suite] 送信した通知メールを処理する [!DNL Workfront]を参照してください。 [管理 [!DNL Adobe Workfront] [!DNL G Suite] からの通知の詳細](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

事前に [!DNL Workfront] タスク [!DNL G Suite]を

* インストール [!DNL Workfront for G suite]\
   手順については、 [インストール [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## の作成 [!DNL Adobe Workfront] タスク [!DNL G Suite] e メールコンテンツの使用

1. この [!UICONTROL Workfront for G Suite] パネルが表示されない場合は、 [!DNL Workfront] アイコン ![](assets/wf-lion-icon.png) 内 [!DNL G Suite] ページの右端にあるアドオンサイドバー。
1. 電子メールメッセージをで開きます。 [!DNL G Suite]、「 [!DNL Workfront for G Suite] 電子メールを新しい [!DNL Workfront] タスク。

1. を選択します。 **[!UICONTROL 新規作成]** タスクをプロジェクトに含めるか、プロジェクトから独立した個人用タスクにするかを指定するオプションです。
1. タスクを親プロジェクトに添付する場合は、 **[!UICONTROL プロジェクト名]**&#x200B;タスクを実行するプロジェクトの名前を入力し、下の一覧に表示されたら、プロジェクト名をクリックします。
1. 次の変更を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL タスク名 ]</td> 
      <td>E メールの件名から取得した、このテキストの任意の部分を編集します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>このテキストの任意の部分（E メールの本文から取得）を編集します。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 割り当て先 ]</td> 
      <td>クリック <strong>[!UICONTROL 割り当て先 ]</strong>、 <strong>[!UICONTROL これをに割り当て ]</strong> オプションが表示されたら、人物の名前を入力し始め、下のリストに表示されたらクリックします。 追加する各担当者に対してこの手順を繰り返し、 <strong>[!UICONTROL 保存 ]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 予定期間 ]</td> 
      <td> <p>クリック <strong>[!UICONTROL 予定期間 ]</strong>に設定し、タスクにかかる日数を入力します。 </p> <p>注意：このオプションは、様々な方法で組織に対して設定できます。 例えば、組織の場合、日数ではなく時間数を入力する必要が生じる場合があります。 詳しくは、 [!DNL Workfront] 管理者。 設定されたデフォルト以外の期間を指定する場合は、「 <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>または <strong>mo</strong> 分、時間、日、週、月を示す数値の後。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 優先度 ]</td> 
      <td>ドロップダウン矢印をクリックし、タスクの優先度をクリックします。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 電子メールの添付ファイルを含める ]</td> 
      <td> <p>（E メールに少なくとも 1 つの添付ファイルが含まれている場合にのみ使用できます）。 電子メール内の添付ファイルをタスクの [!UICONTROL ドキュメント ] 領域に保存するには、このオプションをクリックします。 </p> <p>添付ファイルを保存しない場合は、名前の右にある X をクリックします。 </p> <p>電子メールにドキュメントへのリンクが含まれる場合は、 [!DNL Google Drive]と入力すると、作成中のタスクの「[!UICONTROL 概要 ]」タブに保存されます。 </p> <p>重要：これを機能させるには、 [!DNL Workfront] 管理者が認証する必要があります [!DNL Google Drive] で文書を扱う [!DNL Workfront]（を参照） <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">ドキュメントを管理するための統合の設定</a> 記事内 <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の設定</a>.</p> <p>このオプションを有効にした場合、タスク、問題、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 電子メールファイルを含める ]</td> 
      <td> <p>元の E メールを E メール (EML) ファイルとして保存するには、このオプションをクリックします <span>を [!UICONTROL ドキュメント ] 領域に追加します。</span> タスクの ここから、ファイルをダブルクリックして、メールアプリケーションで E メールを開くことができます。</p> <p>このオプションを有効にした場合、タスク、問題、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL タスクを作成]**.

   この **[!UICONTROL 詳細]** 新しいタスクのタブが [!DNL Workfront for G Suite] パネル。 次をクリックできます。 **[!UICONTROL 更新]** また、共同作業者とすぐにコミュニケーションを取り始めることができます。

   の下部に **[!UICONTROL 詳細]** 」タブで、 **[!UICONTROL 表示場所[!DNL Workfront]]** Workfrontの新しいタスクに移動する

   ブラウザーを更新すると、 [!DNL Workfront for G Suite] 電子メールをタスクに変換したことを確認するパネルが表示されます。

   リンクをクリックして、 [!DNL Workfront for G Suite] パネル（作成したタスク用）

   これらの手順を繰り返して、同じ E メールを複数のタスクに変換できます。 ブラウザーを更新したり、別の時点で電子メールに戻ったりすると、電子メールに対して作成したすべてのリンクが [!UICONTROL Workfront for G Suite] パネル。

1. （オプション） [!DNL Workfront for G Suite] パネルで次のいずれかの操作をおこないます。

   * 更新を **[!UICONTROL 更新]** タブ、クリック **[!UICONTROL 新しい更新を開始]** 更新を入力します。

   * の更新に返信するには **[!UICONTROL 更新]** タブ、クリック **[!UICONTROL 返信]** 返信を入力します。

      上記の両方のアクションについて、コメントに関して特定のユーザーに通知できます。 クリック **[!UICONTROL 通知]**&#x200B;をクリックし、ユーザーの名前を入力し始めて、ドロップダウンリストに表示されたら名前をクリックします。 通知する他のユーザーに対してこのプロセスを繰り返し、 **[!UICONTROL 投稿]**.

   * 次をクリック： **[!UICONTROL ドキュメント]** タブをクリックすると、タスクと共に保存されたドキュメントが表示されます。

これらの手順を繰り返して、同じ E メールを複数のタスクに変換できます。 ブラウザーを更新したり、別の時点で電子メールに戻ったりすると、電子メールに対して作成したすべてのリンクが [!DNL Workfront for G Suite] パネル。
