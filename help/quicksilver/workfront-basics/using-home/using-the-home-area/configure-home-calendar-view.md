---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: ホームカレンダービューの設定
description: ホームカレンダーの設定を構成して、Outlook の web ベースのバージョンと統合し、使用可能な勤務時間に対するワークロードの追跡を行うことができます。
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 79%

---

# [!UICONTROL ホームカレンダー]ビュー設定の指定

<!--Audited: 01/2024-->

[!UICONTROL  のホームカレンダー]を設定して、次の項目を実行できます。

* クラウドでホストされている [!DNL Office 365] または [!DNL Outlook Live] の web ベースバージョンの [!DNL Outlook] と統合します。Outlook の予定表のすべてのイベントと、自分で選択した関連する予定表を表示できます [!UICONTROL ホームカレンダー] Adobe Workfrontで
* 作業可能な時間に対する作業量を[!UICONTROL 配分]バーで追跡するのに役立ちます。

ホームカレンダーの詳細については、[[!UICONTROL ホームカレンダー]ビュー](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)を参照してください。

この記事では、ホームカレンダーの設定を構成し、ホームカレンダーを外部の Outlook カレンダーと統合する方法について説明します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>現在： [!UICONTROL Work] 以降</p> 
   または
   <p>新規： [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*お持ちのプランやライセンスの種類を確認するには、 [!DNL Workfront] 管理者。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## [!DNL Microsoft Outlook] カレンダーの統合について

[!DNL Microsoft Outlook] カレンダーでホームカレンダーを設定するときは、次の点を考慮してください。

* クラウドでホストされている [!DNL Office 365] または [!DNL Outlook Live] で統合できるのは、[!DNL Outlook] の web ベースバージョンのみです。

  オンプレミス [!DNL Outlook] および [!DNL Outlook] クラウドベースの企業で [!DNL Exchange] サーバーはサポートされていません。

  組織でシングルサインオンを使用している場合は、 [!DNL Microsoft 365 E3] または [!DNL E5] が必要です。

* [!DNL Outlook] のイベントに関連付けられた添付ファイルは、ホームカレンダーの [!DNL Outlook] イベントには添付されません。
* [!DNL Outlook] カレンダーとの統合は、各ユーザーごとに個別に実行する必要があります。
* [!UICONTROL 期限]バーに表示されるイベントは、[!UICONTROL 作業リスト]から [!DNL Adobe Workfront] カレンダーにドラッグしない限り、[!DNL Microsoft] カレンダーには表示されません。詳細については、[[!UICONTROL ホームカレンダー]ビュー](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)の[!UICONTROL ホームカレンダー]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view)の[[!UICONTROL 期限]バー](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar)と[作業リストを参照してください。 

* [!DNL Outlook] との統合を有効にした場合、それ以降に [!UICONTROL ホームカレンダー]にドラッグされた作業項目のみが同期されます。統合を有効にする前にホームカレンダーにあった項目は表示されません。[!DNL Outlook] に表示するには、それらの項目をホームカレンダーに再度ドラッグする必要があります。
* 共有（または共有解除）時に、 [!DNL Outlook] 他のユーザーとカレンダーを共有したり、他のユーザーと共有するカレンダーのアクセス許可レベルを変更した場合、この変更は約 30 分間カレンダーに影響を与えません。 詳しくは、 [!DNL Microsoft Outlook] ドキュメント。\
   したがって、[!DNL Workfront] カレンダーを他のユーザーと共有する [!DNL Outlook] カレンダーと統合すると、他のユーザーには [!DNL Workfront] のカレンダー項目が約 30 分間表示されなくなります。

>[!NOTE]
>
>[!DNL Outlook] カレンダー設定は、[!DNL Outlook] アドイン（[!UICONTROL [!DNL Outlook] 統合] または [!DNL Workfront Outlook]）とは完全に分離されています。カレンダーの設定にインストールする必要はありませんが、[!DNL Outlook] アドインのインストールは必要です。[!DNL Outlook] アドインの詳細については、[ の設定 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)を参照してください。

## を設定します。 [!UICONTROL ホームカレンダー] 設定を表示し、Outlook の予定表と統合する

1. Adobe Analytics の [!UICONTROL ホームカレンダー] ビューを開き、 **[!UICONTROL 設定]** 歯車アイコン ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) を開くには、右上隅に **[!UICONTROL カレンダーの設定]** パネルを右に表示します。

   [!UICONTROL ホームカレンダー]ビューへのアクセスについて詳しくは、[[!UICONTROL ホームカレンダーの表示]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)を参照してください。

1. （オプション）[!DNL Microsoft Outlook] カレンダーを統合するには、**[!UICONTROL カレンダー設定]**&#x200B;パネルの右上隅にある「**[!UICONTROL アカウントを追加]**」をクリックします。次に、プロンプトが表示された場合は、 [!DNL Microsoft Outlook] ログイン情報を入力します。複数の [!DNL Outlook] アカウントを追加するには、この手順を繰り返します。

   >[!NOTE]
   >
   >[!DNL Outlook] カレンダーにアクセスするには [!DNL Workfront] にアクセス許可を与える必要があります。権限を付与すると、[!DNL Workfront] はカレンダーデータへのアクセスを維持し、[!DNL outlook] プロファイルを読み取り、[!DNL Microsoft] カレンダーを読み取り、更新することができます。

1. ブラウザーウィンドウを更新すると、カレンダーと [!UICONTROL カレンダー設定]パネルに [!DNL Outlook] アカウントの情報が表示されます。
1. 右上隅にある&#x200B;**[!UICONTROL 設定]**&#x200B;歯車アイコンをもう一度クリックすると、**[!UICONTROL カレンダー設定]**&#x200B;パネルが開きます。![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. （オプション）前の手順で追加した各 [!DNL Microsoft] アカウントで、「**[!UICONTROL 表示]**」または「**[!UICONTROL 同期]**」を選択します。

   * **[!UICONTROL 表示]**：[!UICONTROL ホームカレンダー]に [!DNL Microsoft] のカレンダーイベントを表示する読み取り専用オプションです。
   * **[!UICONTROL 同期]**：このオプションを使用すると、[!DNL Microsoft] カレンダーと [!UICONTROL ホーム]カレンダーの間で双方向の同期が可能になります。つまり、リアルタイムで、[!DNL Workfront] [!UICONTROL ホーム カレンダー]の項目が [!DNL Microsoft] カレンダーに書き出され、[!DNL Microsoft] カレンダーの項目が Workfront [!UICONTROL ホーム カレンダー]に読み込まれます。

     ![](assets/view-sync-checkboxes-qs.png)

1. （オプション）[!DNL Workfront] アカウントまたは統合アカウントの下で、[!UICONTROL ホームカレンダー]に表示したい関連カレンダー（有給休暇、誕生日、休日カレンダーなど）を選択し、ブラウザーの[!UICONTROL 更新]または[!UICONTROL 再読み込み]ボタンをクリックして変更内容を確認します。

1. （オプション）**[!UICONTROL 一般]**&#x200B;セクションの&#x200B;**[!UICONTROL 週の開始日]**&#x200B;の下で、ホームカレンダーの勤務週の最初の日として表示する日を選択します。

   ![](assets/general-section-home-calendar-settings-panel.png)

1. 次のオプションを設定します。

   * **[!UICONTROL 勤務日]：** 勤務日を選択します。
   * **[!UICONTROL 通常の開始時刻]：** 勤務日に勤務を開始する時刻を選択します。
   * **[!UICONTROL 通常の終了時刻]：** 勤務日に勤務を終了する時間を選択します。

   [!DNL Workfront] は、これら 3 つの設定を使用して、1 週間の勤務時間数を計算します。 この数は、[!UICONTROL 配分]バーに影響し、使用可能な勤務時間に対するワークロードの追跡に役立ちます。 詳しくは、[[!UICONTROL ホームカレンダー]ビュー](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)の[[!UICONTROL 配分]バー](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time)を参照してください。

1. の外側をクリック **[!UICONTROL カレンダーの設定]** 領域を閉じます。

   [!DNL Workfront] では、ユーザーの変更内容を自動的に保存します。

[!UICONTROL カレンダー]ビューを使用して仕事の割り当てと統合されたカレンダーイベントを管理する方法については、[[!UICONTROL ホームカレンダー]ビューの使用](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md)を参照してください。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
