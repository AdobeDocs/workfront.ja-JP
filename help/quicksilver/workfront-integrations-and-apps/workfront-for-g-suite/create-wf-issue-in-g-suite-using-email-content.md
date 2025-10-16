---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: メールコンテンツ  [!DNL Adobe Workfront]  使用したGoogle Workspaceでのイシューの作成
description: 外部メール（ [!DNL Adobe Workfront)]  以外で生成）を  [!DNL Workfront]  イシューに変換できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 67%

---

# [!DNL Google Workspace] でメールコンテンツを使用して [!DNL Adobe Workfront] イシューを作成する

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
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 &#x200B;](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能については、{Gmail モジュール [&#x200B; および &#x200B;](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)2}Google カレンダーモジュール [&#x200B; を参照してください。](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)

外部メール（[!DNL Adobe Workfront] 以外で生成）を [!DNL Workfront] イシューに変換できます。

また、外部メールを既存のイシューのアップデートに変換することもできます。詳しくは、[&#x200B; メールコンテンツを使用した  [!DNL Adobe Workfront]  項目の更新  [!DNL Google Workspace]  を参照してください &#x200B;](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)。

[!DNL Google Workspace] を使用して [!DNL Workfront] から送信される通知メールを操作する方法については、[&#x200B; からの管理  [!DNL Adobe Workfront]  通知の詳細  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p><p>ワークまたはそれ以上</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!DNL Google Workspace] からイシューを作成する前に、次を実行する必要があります。

* [!DNL Workfront for Google Workspace] のインストール\
   手順については、[&#x200B; [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md) のインストールを参照してください。

## メールコンテンツを使用して [!DNL Google Workspace] で [!DNL Adobe Workfront] イシューを作成する

1. Google Workspaceの [!UICONTROL Workfront] パネルが表示されない場合は、ページの右端にあるア [!DNL Workfront] オンサイドバーの ![&#x200B; アイコン &#x200B;](assets/wf-lion-icon.png)3&rbrace;Workfront アイコン &rbrace; をクリックします。[!DNL Google Workspace]
1. メールメッセージを [!DNL Google Workspace] で開いたまま、[!DNL Workfront for Google Workspace] でメールを新しい [!DNL Workfront] イシューに変換するオプションをクリックします。

   ![&#x200B; メールを変換 &#x200B;](assets/convert-email-task-issue-update.png)

1. イシューを親プロジェクトに関連付ける場合は、**[!UICONTROL プロジェクト名]**&#x200B;をクリックし、イシューを作成するプロジェクトの名前を入力し、下の一覧に表示されたら、そのプロジェクトの名前をクリックします。
1. 次の変更を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Issue Name]</td> 
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
      <td role="rowheader">[!UICONTROL Priority]</td> 
      <td>ドロップダウン矢印をクリックし、イシューの優先度をクリックします。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email attachments]</td> 
      <td> <p>（メールに少なくとも 1 つの添付ファイルが含まれている場合にのみ使用できます）。 このオプションをクリックして、メールの添付ファイルをイシューの [!UICONTROL ドキュメント &#x200B;] 領域に保存します。 </p> <p>添付ファイルを保存しない場合は、名前の右にある X をクリックします。 </p> <p>メールに [!DNL Google Drive] でのドキュメントへのリンクが含まれる場合は、作成中のイシューの [!UICONTROL Overview] タブに保存されます。 </p> <p>重要：これを機能させるには、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の構成</a>の記事の<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">ドキュメントを管理するための統合の構成</a>の節で説明されているように、[!DNL Workfront] 管理者は [!DNL Google Drive] が [!DNL Workfront] でドキュメントを操作できるように承認する必要があります。</p> <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">メールファイルを含める</td> 
      <td> <p>元のメールをメール（EML）（メール）ファイルとしてイシューの<span>[!UICONTROL Documents]領域</span>に保存するには、このオプションをクリックします。ここから、ファイルをダブルクリックして、メールアプリケーションでメールを開くことができます。</p> <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL イシューを作成]**&#x200B;をクリックします。

   新しいイシューの「**[!UICONTROL 詳細]**」タブが [!DNL Workfront for Google Workspace] パネルに表示されます。「**[!UICONTROL アップデート]**」をクリックすると、受信ボックスから離れることなく、すぐに共同編集者とのコミュニケーションを開始できます。

   「**[!UICONTROL 詳細]**」タブの下部で「**[!UICONTROL Workfront で表示]**」をクリックして、Workfront で新しいイシューに移動することもできます。

   ブラウザーを更新すると、[!UICONTROL Google WorkspaceのWorkfront] パネルの下部に、メールが問題に変換されたことを示すリンクが表示されます。

   リンクをクリックすると、[!DNL Workfront for Google Workspace] パネル内の作成したイシューの詳細ビューに移動できます。

   これらの手順を繰り返して、同じメールを複数のイシューに変換できます。ブラウザーを更新したり、別のタイミングでメールに戻ったりすると、メール用に作成したすべてのリンクが、[!UICONTROL Google WorkspaceのWorkfront] パネルの下部に表示されます。

1. （オプション）[!DNL Workfront for Google Workspace] パネルで次のいずれかの操作を行って、イシューでの作業を続行します。

   * 「**[!UICONTROL アップデート]**」タブに更新を追加するには、「**[!UICONTROL 新しい更新を開始]**」をクリックして更新を入力します。

   * 「**[!UICONTROL アップデート]**」タブのアップデートに返信するには、「**[!UICONTROL 返信]**」をクリックして返信を入力します。

     上記の両方のアクションについて、コメントに関して特定のユーザーに通知できます。「**[!UICONTROL 通知]**」をクリックし、ユーザーの名前を入力し始めて、ドロップダウンリストに表示されたら名前をクリックします。通知する他のユーザーに対してこのプロセスを繰り返し、「**[!UICONTROL 投稿]**」をクリックします。

   * 「**[!UICONTROL ドキュメント]**」タブをクリックして、イシュー付きで保存されたドキュメントを表示します。
