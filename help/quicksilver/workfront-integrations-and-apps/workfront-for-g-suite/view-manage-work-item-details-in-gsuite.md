---
product-area: workfront-integrations;projects
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Google Workspaceからのオブジェク  [!DNL Adobe Workfront]  の詳細の表示と管理
description: Google Workspaceを離れることなく、作業項目の詳細を表示および管理できます。 例えば、Google Workspaceで、タスクの説明を読み取り、親オブジェクトを確認し、ステータスを変更し、完了としてマークするこ  [!DNL Adobe Workfront]  ができます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 0f15b05f-3b4a-4f0b-9d9a-21a0f97de1ea
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 60%

---

# [!DNL Google Workspace] から [!DNL Adobe Workfront] オブジェクトの詳細を表示および管理

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

[!DNL Google Workspace] から離れることなく、作業アイテムの詳細を表示および管理できます。例えば、タスクの説明を読み取り、その親オブジェクトを表示し、そのステータスを変更し、タスクを完了としてマークすることをすべて [!DNL Adobe Workfront for Google Workspace] 内で行うことができます。

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

[!DNL Google Workspace] で作業アイテムの詳細を表示および管理するには、次のことを行う必要があります。

* [!DNL Workfront for Google Workspace] をインストール\
   手順については、[ [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md) をインストールを参照してください。

## [!DNL Google Workspace] で作業アイテムの詳細を表示および管理する

1. Google Workspaceの [!UICONTROL Workfront] パネルが表示されない場合は、ページの右端にあるア [!DNL Workfront] オンサイドバーの ![ アイコン ](assets/wf-lion-icon.png)3&rbrace;Workfront アイコン &rbrace; をクリックします。[!DNL Google Workspace]
1. [!DNL Workfront] からの [!DNL Google Workspace] アクセス [ ホーム  [!DNL Adobe Workfront] [!UICONTROL &#x200B; コンテンツの説明に従って、] 内の  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md) のタスクまたはイシューに移動します。

   タスクまたはイシューを選択すると、「**[!UICONTROL 詳細]**」タブが開きます。「**[!UICONTROL 詳細]**」タブの上のエリアには、親オブジェクトの名前、タスクまたはイシューの名前、[!UICONTROL 期日]（タスクの場合）または[!UICONTROL 優先日]（イシューの場合）が表示されます。


   [!DNL Google Workspace] から離れることなく、このタブで次のような様々なタスクを実行できます。

   * オブジェクトの&#x200B;**[!UICONTROL 説明]**、およびオブジェクトに割り当てられたユーザー、**[!UICONTROL 優先度]**、リクエスター、**[!UICONTROL 予定完了日]**、オブジェクトに添付されたカスタムフィールドやフォームなど、その他の詳細を表示します。

     カスタムフォームには、情報が追加されたフィールドのみが表示されます。

   * **[!UICONTROL 親プロジェクト]**&#x200B;エリアをクリックして、親オブジェクトの詳細を表示します。

     >[!TIP]
     >
     >これは、同じ名前のタスクやイシューがあり、それらを区別する必要がある場合に役立ちます。

   * 「**[!UICONTROL 作業をする]**」をクリックして、自分に割り当てられた作業を承認します。
   * 「**[!UICONTROL 完了]**」オプション、「**[!UICONTROL ステータス]**」、「**[!UICONTROL 完了率]**」などの様々なオプションを編集します。

     「**[!UICONTROL 完了率]**」で、項目の進捗状況を示す数字と（オプションで）パーセント記号％を入力します。
   * 所有者、サイズ、添付ファイルなど、承認リクエストに関する情報を表示します。
   * 承認リクエストとドキュメントを&#x200B;**[!UICONTROL 承認]**&#x200B;または&#x200B;**[!UICONTROL 却下]**&#x200B;します。

   * アクセス権のリクエストを&#x200B;**[!UICONTROL 許可]**&#x200B;または&#x200B;**[!UICONTROL 無視]**&#x200B;します。

1. （オプション）**[!UICONTROL [!DNL Workfront]]** で「表示」をクリックして、[!DNL Workfront] の現在の作業アイテムに移動します。

* [!UICONTROL &#x200B; の「] 更新 [!DNL Workfront for Google Workspace]」タブの使用について詳しくは、[ から  [!DNL Adobe Workfront]  オブジェクトを更新  [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md) を参照してください。
* [!DNL Workfront for Google Workspace] の「[!UICONTROL ドキュメント]」タブの使用について詳しくは、[[!DNL G Suite] のドキュメントを表示および管理](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md)を参照してください。
