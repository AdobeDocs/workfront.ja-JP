---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: メールコ  [!DNL Adobe Workfront]  テンツを使用したGoogle Workspaceでのタスクの作成
description: 外部メール（Adobe  [!DNL Workfront] によって生成されたものではない）を Workfront タスクに変換できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 76%

---

# [!DNL Google Workspace] でメールコンテンツを使用して [!DNL Adobe Workfront] タスクを作成する

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
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能については、{Gmail モジュール [&#x200B; および &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)2}Google カレンダーモジュール [&#x200B; を参照してください。](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)

外部メール（[!DNL Adobe Workfront] によって生成されたものではない）を [!DNL Workfront] タスクに変換できます。

外部メールを既存のタスクの更新に変換することもできます。詳しくは、[&#x200B; メールコンテンツを使用した  [!DNL Adobe Workfront]  項目の更新  [!DNL Google Workspace]  を参照してください &#x200B;](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)。

[!DNL Google Workspace] を使用して [!DNL Workfront] から送信される通知メールを操作する方法については、[&#x200B; からの管理  [!DNL Adobe Workfront]  通知の詳細  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md) を参照してください。

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

[!DNL Google Workspace] で [!DNL Workfront] タスクを作成する前に、以下の動作を実行する必要があります。

* [!DNL Workfront for Google Workspace] をインストール\
   手順については、[&#x200B; [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md) のインストールを参照してください。

## [!DNL Google Workspace] でメールコンテンツを使用して [!DNL Adobe Workfront] タスクを作成する

1. Google Workspaceの [!UICONTROL Workfront] パネルが表示されない場合は、ページの右端にあるア [!DNL Workfront] オンサイドバーの ![&#x200B; アイコン &#x200B;](assets/wf-lion-icon.png)3&rbrace;Workfront アイコン &rbrace; をクリックします。[!DNL Google Workspace]
1. メールメッセージを [!DNL Google Workspace] で開いたまま、[!DNL Workfront for Google Workspace] でメールを新しい [!DNL Workfront] タスクに変換するオプションをクリックします。

1. 「**[!UICONTROL 新規作成]**」オプションを選択して、タスクをプロジェクトの一部にするか、プロジェクトから独立した個人タスクにするかを指定します。
1. タスクを親プロジェクトに関連付ける場合は、**[!UICONTROL プロジェクト名]**&#x200B;をクリックし、タスクを作成するプロジェクトの名前を入力し、下の一覧に表示されたら、そのプロジェクトの名前をクリックします。
1. 次の変更を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Task name]</td> 
      <td>このテキストの任意の部分（メールの件名から取得）を編集します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>このテキストの任意の部分（メールの本文から取得）を編集します。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Assign To]</td> 
      <td>「<strong>[!UICONTROL Assign To]</strong>」をクリックし、「<strong>[!UICONTROL Assign this to] </strong>」オプションが表示されたらクリックします。ユーザーの名前を入力し始め、下のリストに表示されたらクリックします。追加する各ユーザーに対してこの手順を繰り返し、「<strong>[!UICONTROL Save]</strong>」をクリックします。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Planned Duration]</td> 
      <td> <p>「<strong>[!UICONTROL Planned duration]</strong>」をクリックし、タスクにかかる日数を入力します。 </p> <p>メモ：このオプションは、組織に対して様々な方法で設定できます。例えば、組織の場合、日数ではなく時間数を入力する必要が生じる場合があります。詳しくは、[!DNL Workfront] 管理者を参照してください。設定されたデフォルト以外の期間を指定する場合は、分、時間、日、週、または月を表すために、数値の後に <strong>m</strong>、<strong>h</strong>、<strong>d</strong>、<strong>w</strong>、または <strong>mo</strong> を入力します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>ドロップダウン矢印をクリックし、タスクの優先度をクリックします。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>（メールに少なくとも 1 つの添付ファイルが含まれている場合にのみ使用できます）。 メール内の添付ファイルをタスクの [!UICONTROL ドキュメント &#x200B;] 領域に保存するには、このオプションをクリックします。 </p> <p>添付ファイルを保存しない場合は、名前の右にある X をクリックします。 </p> <p>メールに [!DNL Google Drive] でのドキュメントへのリンクが含まれる場合は、作成中のタスクの [!UICONTROL Overview] タブに保存されます。 </p> <p>重要：これを機能させるには、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合を設定</a>の記事の<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">ドキュメントを管理するために統合を構成</a>の節で説明されているように、[!DNL Workfront] 管理者は [!DNL Google Drive] が [!DNL Workfront] でドキュメントを操作できるように承認する必要があります。</p> <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>元のメールをメール（EML）ファイルとしてタスクの <span>[!UICONTROL Documents] エリア</span>に保存するには、このオプションをクリックします。ここから、ファイルをダブルクリックして、メールアプリケーションでメールを開くことができます。</p> <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL タスクを作成]**」をクリックします。

   新しいタスクの「**[!UICONTROL 詳細]**」タブが [!DNL Workfront for Google Workspace] パネルに表示されます。「**[!UICONTROL アップデート]**」をクリックすると、受信トレイから離れることなく、すぐに共同編集者とのコミュニケーションを開始できます。

   「**[!UICONTROL 詳細]**」タブの下部で、「**[!UICONTROL Workfront で表示[!DNL Workfront]]**」をクリックして、Workfront の新しいタスクに移動することもできます。

   ブラウザーを更新すると、[!DNL Workfront for Google Workspace] パネルの下部に、メールがタスクに変換されたことを通知する、リンク付きのメッセージが表示されます。

   リンクをクリックすると、[!DNL Workfront for Google Workspace] パネル内の作成したタスクの詳細ビューに移動できます。

   これらの手順を繰り返して、同じメールを複数のタスクに変換できます。ブラウザーを更新したり、別のタイミングでメールに戻ったりすると、メール用に作成したすべてのリンクが、[!UICONTROL Google WorkspaceのWorkfront] パネルの下部に表示されます。

1. （オプション）[!DNL Workfront for Google Workspace] パネルでのタスクの作業を続行するには、次のいずれかの操作を行います。

   * 「**[!UICONTROL アップデート]**」タブにアップデートを追加するには、「**[!UICONTROL 新しい更新を開始]**」をクリックし、目的のアップデートを入力します。

   * 「**[!UICONTROL アップデート]**」タブのアップデートに返信するには、「**[!UICONTROL 返信]**」をクリックして返信を入力します。

     上記の両方のアクションについて、コメントに関して特定のユーザーに通知できます。「**[!UICONTROL 通知]**」をクリックし、ユーザーの名前を入力し始めて、ドロップダウンリストに表示されたら名前をクリックします。通知する他のユーザーに対してこのプロセスを繰り返し、「**[!UICONTROL 投稿]**」をクリックします。

   * 「**[!UICONTROL ドキュメント]**」タブをクリックして、タスクと共に保存されたドキュメントを表示します。

これらの手順を繰り返して、同じメールを複数のタスクに変換できます。ブラウザーを更新したり、別の時点でメールに戻ったりすると、メールに対して作成したすべてのリンクが [!DNL Workfront for Google Workspace] パネルの下部に表示されます。
