---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: ' [!DNL Slack] の共有リンクからの [!DNL Adobe Workfront] オブジェクトへのアクセス'
description: ' [!DNL Adobe Workfront] オブジェクトへのリンクが Slack チャネルで共有されると、 [!DNL Workfront] をインストールして Slack 用に設定した後で、それらに関する追加情報が Slack に表示されます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 587c6ac7-cc56-480f-852d-f0bd36b3f3cf
source-git-commit: eeb90d8f80b1680d880d07f41e9d80c0658495fa
workflow-type: ht
source-wordcount: '1118'
ht-degree: 100%

---

# [!DNL Slack] の共有リンクからの [!DNL Adobe Workfront] オブジェクトへのアクセス

[!DNL Adobe Workfront] オブジェクトへのリンクが [!DNL Slack] チャネルで共有されると、[!DNL Workfront for Slack] をインストールして設定した後で、それらに関する追加情報が [!DNL Slack] に表示されます。

[!DNL Workfront for Slack] の設定について詳しくは、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

[!DNL Slack] からリンクを開いたり、これらのオブジェクトに対して追加のアクションを実行したりするには、別のブラウザータブで [!DNL Workfront] にログインする必要があります。

ユーザーが [!DNL Workfront] 内のオブジェクトへのリンクを共有している場合、そのオブジェクトに関する追加情報がリンクと共に表示される場合があります。これらの追加情報を [!DNL Slack] に表示するには、リンクを送信するユーザーに、少なくともオブジェクトの[!UICONTROL 表示]権限が必要です。

## アクセス要件

この記事で説明されている機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Slack] から、最近使用した項目とお気に入りにアクセスするには、まず以下が必要です。

* [!DNL Workfront for Slack] の設定\
   [!DNL Workfront for Slack] の設定の手順については、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

## [!DNL Slack] からのプロジェクトへのアクセス

1. [!DNL Slack] インスタンスにログインし、[!DNL Workfront from Slack.] にログインします。

   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Adobe Workfront from Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) へのアクセスの「[!DNL Workfront from Slack] へのログイン」の節を参照してください。

1. [!DNL Workfront] プロジェクトへのリンクを含んだメッセージに移動します。

   >[!NOTE]
   >
   >リンクを共有しているユーザーがプロジェクトに関する追加情報を参照するには、少なくともプロジェクトの[!UICONTROL 表示]権限が必要です。

1. （オプション）プロジェクトの名前をクリックして、新しいブラウザータブで [!DNL Workfront] にプロジェクトを開きます。
1. プロジェクトに関する次の追加情報を確認することを検討します。

   * **[!UICONTROL ステータス]：**&#x200B;プロジェクトステータスについて詳しくは、[システムプロジェクトステータスのリストへのアクセス](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)を参照してください。

   * **[!UICONTROL 予定完了日]**：予定完了日について詳しくは、[プロジェクトの予定完了日の設定](../../manage-work/projects/planning-a-project/project-planned-completion-date.md)を参照してください。

   * **[!UICONTROL ポートフォリオ]**&#x200B;名：ポートフォリオについて詳しくは、[Adobe Workfront のポートフォリオの概要](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)を参照してください。

   * **[!UICONTROL 状況]**：プロジェクト状況について詳しくは、[プロジェクト状況と状況タイプの概要](../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)を参照してください。

   * **[!UICONTROL 完了率]**：プロジェクトの完了率の値について詳しくは、[プロジェクトの完了率の概要](../../manage-work/tasks/task-information/project-percent-complete.md)を参照してください。

   * **[!UICONTROL 参照番号]**：オブジェクトの参照番号について詳しくは、[オブジェクトの参照番号の使用](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)を参照してください。

1. （オプション）「**[!UICONTROL 登録]**」をクリックして、プロジェクトに登録します。

   プロジェクトに正常に登録されたことを示す確認メッセージが表示されます。

## [!DNL Slack] からのタスクへのアクセス

1. [!DNL Slack] インスタンスにログインし、[!DNL Workfront from Slack] にログインします。

   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Adobe Workfront from Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) へのアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. [!DNL Workfront] タスクへのリンクを含んだメッセージに移動します。

   >[!NOTE]
   >
   >リンクを共有しているユーザーがタスクに関する追加情報を参照するには、少なくともタスクの[!UICONTROL 表示]権限が必要です。

1. （オプション）タスクの名前をクリックして、新しいブラウザータブで [!DNL Workfront] にタスクを開きます。
1. タスクに関する次の追加情報を確認することを検討します。

   * **[!UICONTROL 状態]**

     タスク状態について詳しくは、[システムタスク状態のリストへのアクセス](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)を参照してください。

   * **[!UICONTROL 完了率]**
   * **[!UICONTROL 名前の割り当て]**
   * **[!DNL Planned Completion Date]**
   * **[!UICONTROL プロジェクト名]**&#x200B;または&#x200B;**[!UICONTROL 親タスク名]**
   * **[!UICONTROL 参照番号]**

     オブジェクトの参照番号について詳しくは、[オブジェクトの参照番号の使用](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)を参照してください。

1. （オプション）「**[!UICONTROL 登録]**」をクリックして、タスクに登録します。

   タスクに正常に登録されたことを示す確認メッセージが表示されます。

1. （オプション）「**[!UICONTROL ユーザーに割り当て]**」をクリックして、タスクをユーザーに割り当てます。
1. （条件付き）「**[!UICONTROL ユーザーに割り当て]**」をクリックした場合は、ユーザーの名前を入力し始めます。

   [!DNL Slack] からタスクを担当業務またはチームに割り当てることはできません。

## [!DNL Slack] からイシューにアクセス

1. [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。

   [!DNL Slack] から Workfront へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの[!DNL Slack] から [!DNL Workfront] へのログインの節を参照してください。

1. [!DNL Workfront] イシューへのリンクを含むメッセージに移動します。

   >[!NOTE]
   >
   >リンクを共有しているユーザーは、イシューに関する追加情報を表示するために、イシューに対する[!UICONTROL 表示]以上の権限を持っている必要があります。

1. （オプション）イシューの名前をクリックして、新しいブラウザータブの [!DNL Workfront] でタスクを開きます。
1. タスクに関する次の追加情報を確認することを検討します。

   * **[!UICONTROL ステータス]**：イシューのステータスについて詳しくは、[システムイシューステータスのリストへのアクセス](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)を参照してください。

   * **[!UICONTROL 割り当て先の名前]**
   * **[!UICONTROL 予定完了日]**
   * **[!UICONTROL プロジェクト名]**
   * **[!UICONTROL 参照番号]**：オブジェクトの参照番号について詳しくは、[オブジェクトの参照番号を使用](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)を参照してください。

1. （オプション）「**[!UICONTROL 登録]**」をクリックしてイシューに登録します。

   イシューに正しく登録されたことを示す確認メッセージが表示されます。

1. （オプション）「**[!UICONTROL ユーザーに割り当て]**」をクリックして、イシューをユーザーに割り当てます。
1. （条件付き）「**[!UICONTROL ユーザーに割り当て]**」をクリックした場合は、ユーザー名を入力し始めます。

   [!DNL Slack] から担当業務またはチームにイシューを割り当てることはできません。

## [!DNL Slack] からポートフォリオへのアクセス

1. [!DNL Slack] インスタンスにログインし、[!DNL Slack] から [!DNL Workfront] にログインします。

   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から [!DNL Adobe Workfront] へのアクセス の [!DNL Slack] から [!DNL Workfront] へのログインの節を参照してください。

1. [!DNL Workfront] ポートフォリオへのリンクを含むメッセージに移動します。

   >[!NOTE]
   >
   >リンクを共有しているユーザーは、ポートフォリオに関する追加情報を表示するには、ポートフォリオに対する[!UICONTROL 表示]以上の権限を持っている必要があります。

1. （オプション）ポートフォリオの名前をクリックして、新しいブラウザータブの [!DNL Workfront] でポートフォリオを開きます。
1. ポートフォリオに関する次の追加情報を確認することを検討します。

   * **[!UICONTROL ポートフォリオマネージャーの名前]**
   * **[!UICONTROL 予定通り]**
   * **[!UICONTROL ROI]**
   * **[!UICONTROL 純価]**
   * **[!UICONTROL ステータス]**
   * **[!UICONTROL 予算通り]**
   * **[!UICONTROL 整合済み]**

     [!UICONTROL ROI]、[!UICONTROL 純価]、[!UICONTROL アライメント]、[!UICONTROL オンタイム]、[!UICONTROL 予算内]の値などのポートフォリオ指標について詳しくは、[[!UICONTROL ポートフォリオオプティマイザーについて]を参照してください。](../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## [!DNL Slack] からプログラムへのアクセス

1. [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。

   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から [!DNL Adobe Workfront] へのアクセス の [!DNL Slack] から [!DNL Workfront] へのログインの節を参照してください。

1. [!DNL Workfront] プログラムへのリンクを含むメッセージに移動します。

   >[!NOTE]
   >
   > リンクを共有しているユーザーは、プログラムに関する追加情報を表示するために、プログラムに対する[!UICONTROL 表示]以上の権限を持っている必要があります。

1. （オプション）プログラムの名前をクリックして、新しいブラウザータブの [!DNL Workfront] でプログラムを開きます。
1. プログラムに関する次の追加情報を確認することを検討します。

   * **[!UICONTROL 説明]**
   * **[!UICONTROL ポートフォリオ名]**
   * **[!UICONTROL プログラムマネージャーの名前]**

     プログラムについて詳しくは、[プログラムの作成と管理](../../manage-work/portfolios/create-and-manage-programs/create-and-manage-programs.md)を参照してください。

## [!DNL Slack] からレポートへのアクセス

1. [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。

   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から [!DNL Adobe Workfront] へのアクセス の [!DNL Slack] から [!DNL Workfront] へのログインの節を参照してください。

1. [!DNL Workfront] レポートへのリンクを含むメッセージに移動します。

   >[!NOTE]
   >
   >リンクを共有しているユーザーは、レポートに関する追加情報を表示するために、レポートに対する[!UICONTROL 表示]以上の権限を持っている必要があります。

1. （オプション）レポートの名前をクリックして、新しいブラウザータブの [!DNL Workfront] でレポートを開きます。
