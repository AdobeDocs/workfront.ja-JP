---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: G Suite でメールコンテンツを使用して  [!DNL Adobe Workfront]  タスクを作成する
description: 外部メール（Adobe  [!DNL Workfront] によって生成されたものではない）を Workfront タスクに変換できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: ht
source-wordcount: '930'
ht-degree: 100%

---

# [!DNL G Suite] でメールコンテンツを使用して [!DNL Adobe Workfront] タスクを作成する

>[!NOTE]
>
>Google 用の Adobe Workfront プラグインの最新バージョンは、2023年6月26日にリリースされました。

外部メール（[!DNL Adobe Workfront] によって生成されたものではない）を [!DNL Workfront] タスクに変換できます。

外部メールを既存のタスクの更新に変換することもできます。詳しくは、[メールコンテンツを使用して [!DNL G Suite] から  [!DNL Adobe Workfront]  アイテムを更新](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md)を参照してください。

[!DNL G Suite] を使用して [!DNL Workfront] から送信された通知メールを操作する方法について詳しくは、[ [!DNL G Suite] から  [!DNL Adobe Workfront]  通知の詳細を管理](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md)を参照してください。

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

[!DNL G Suite] で [!DNL Workfront] タスクを作成する前に、次を実行する必要があります。

* [!DNL Workfront for G suite] をインストール\
   手順については、[ [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md) のインストールを参照してください。

## [!DNL G Suite] でメールコンテンツを使用して [!DNL Adobe Workfront] タスクを作成する

1. [!UICONTROL Workfront for G Suite] パネルが表示されない場合は、ページの右端にある [!DNL G Suite] アドオンサイドバーで [!DNL Workfront] アイコン![](assets/wf-lion-icon.png)をクリックしてください。
1. メールメッセージを [!DNL G Suite] で開いたまま、[!DNL Workfront for G Suite] でメールを新しい [!DNL Workfront] タスクに変換するオプションをクリックします。

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
      <td>「<strong>[!UICONTROL Assign To]</strong>」をクリックし、「<strong>[!UICONTROL Assign this to]</strong>」オプションが表示されたらクリックします。ユーザーの名前を入力し始め、下のリストに表示されたらクリックします。追加する各ユーザーに対してこの手順を繰り返し、「<strong>[!UICONTROL Save]</strong>」をクリックします。</td> 
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
      <td> <p>（メールに 1 つ以上の添付ファイルが含まれている場合にのみ使用できます。）メール内の添付ファイルをタスクの [!UICONTROL Documents] エリアに保存するには、このオプションをクリックします。 </p> <p>添付ファイルを保存しない場合は、名前の右にある X をクリックします。 </p> <p>メールに [!DNL Google Drive] でのドキュメントへのリンクが含まれる場合は、作成中のタスクの [!UICONTROL Overview] タブに保存されます。 </p> <p>重要：これを機能させるには、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合を設定</a>の記事の<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">ドキュメントを管理するために統合を構成</a>の節で説明されているように、[!DNL Workfront] 管理者は [!DNL Google Drive] が [!DNL Workfront] でドキュメントを操作できるように承認する必要があります。</p> <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Include email file]</td> 
      <td> <p>元のメールをメール（EML）ファイルとしてタスクの <span>[!UICONTROL Documents] エリア</span>に保存するには、このオプションをクリックします。ここから、ファイルをダブルクリックして、メールアプリケーションでメールを開くことができます。</p> <p>このオプションを有効にした場合、タスク、イシュー、更新に変換する他のメールに対しても有効なままになります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL タスクを作成]**」をクリックします。

   新しいタスクの「**[!UICONTROL 詳細]**」タブが [!DNL Workfront for G Suite] パネルに表示されます。「**[!UICONTROL アップデート]**」をクリックすると、受信トレイから離れることなく、すぐに共同編集者とのコミュニケーションを開始できます。

   「**[!UICONTROL 詳細]**」タブの下部で、「**[!UICONTROL Workfront で表示[!DNL Workfront]]**」をクリックして、Workfront の新しいタスクに移動することもできます。

   ブラウザーを更新すると、[!DNL Workfront for G Suite] パネルの下部に、メールがタスクに変換されたことを通知する、リンク付きのメッセージが表示されます。

   リンクをクリックすると、[!DNL Workfront for G Suite] パネル内の作成したタスクの詳細ビューに移動できます。

   これらの手順を繰り返して、同じメールを複数のタスクに変換できます。ブラウザーを更新したり、別の時点でメールに戻ったりすると、メールに対して作成したすべてのリンクが [!UICONTROL G Suite 用 Workfront] パネルの下部に表示されます。

1. （オプション）[!DNL Workfront for G Suite] パネルでのタスクの作業を続行するには、次のいずれかの操作を行います。

   * 「**[!UICONTROL アップデート]**」タブにアップデートを追加するには、「**[!UICONTROL 新しい更新を開始]**」をクリックし、目的のアップデートを入力します。

   * 「**[!UICONTROL アップデート]**」タブのアップデートに返信するには、「**[!UICONTROL 返信]**」をクリックして返信を入力します。

     上記の両方のアクションについて、コメントに関して特定のユーザーに通知できます。「**[!UICONTROL 通知]**」をクリックし、ユーザーの名前を一部入力し、名前がドロップダウンリストに表示されたらクリックします。通知する他のユーザーに対してこのプロセスを繰り返し、「**[!UICONTROL 投稿]**」をクリックします。

   * 「**[!UICONTROL ドキュメント]**」タブをクリックして、タスクと共に保存されたドキュメントを表示します。

これらの手順を繰り返して、同じメールを複数のタスクに変換できます。ブラウザーを更新したり、別の時点でメールに戻ったりすると、メールに対して作成したすべてのリンクが [!DNL Workfront for G Suite] パネルの下部に表示されます。
