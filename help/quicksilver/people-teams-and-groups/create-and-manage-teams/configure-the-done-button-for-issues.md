---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 問題が発生しないように「完了」ボタンを設定します
description: 「完了」ボタンを使用して、タスクまたはイシューのステータスを自動的に設定できます。 デフォルトでは、Adobe Workfrontは、担当者が作業項目で「完了」をクリックすると、問題を「解決済み」とマークします。
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 1%

---

# の設定 [!UICONTROL 完了] ボタン

この [!UICONTROL 完了] ボタンを使用して、タスクまたはイシューのステータスを自動的に設定できます。 デフォルトでは、 [!DNL Adobe Workfront] 問題を次のようにマーク [!UICONTROL 解決済み] 担当者が [!UICONTROL 完了] を設定します。

## 概要

特定の権限を持つユーザーは、 [!UICONTROL 完了] ボタンを使用して、特定のステータスをシステムに反映させることができます。 次の 3 つの方法があります。 [!UICONTROL 完了] ボタンが [!DNL Workfront]:

* ユーザーに [!UICONTROL ホームチーム], a [!DNL Workfront] 管理者または [!UICONTROL プラン] ライセンスは、 [!UICONTROL 完了] ボタンを使用して、チームメンバーに特定のステータスを反映させます。 詳しくは、 [の設定 [!UICONTROL 完了] チームのボタン](#configure-the-uicontrol-done-button-for-a-team) 」を参照してください。
* ユーザーが [!UICONTROL ホームチーム] 割り当て済み、 [!UICONTROL 完了] 問題のボタンは、システムで生成された [!UICONTROL 解決済み] 3 文字のコードを持つステータス [!UICONTROL RLV]. このシナリオで使用できる設定オプションはありません。 この [!UICONTROL 完了] ボタンは、自動的にこのステータスに設定されます。
* この [!UICONTROL 解決済み] ([!UICONTROL RLV]) ステータスが削除され、ユーザーが問題を「 」としてマークします。 [!UICONTROL 完了] 次がない [!UICONTROL ホームチーム]の場合、デフォルトの問題ステータスは、 [!UICONTROL クローズ] 問題が属するプロジェクトに割り当てられたグループの場合。 Workfrontの管理者は、グループのシステム全体のデフォルト設定を構成できます。 詳しくは、 [の設定 [!UICONTROL 完了] ボタン [!UICONTROL 解決済み] ステータスは削除されました](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 」を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL プラン ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td>[!UICONTROL 解決済み ] ステータスが削除された場合に [!UICONTROL 完了 ] ボタンを設定するには、システム管理者のアクセス権が必要です</td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## の設定 [!UICONTROL 完了] チームのボタン

作業項目に適用されるステータスは、 [!UICONTROL 完了] 」ボタンをクリックします。 また、複数のステータスを設定し、適切なステータスをユーザーが選択できるようにすることもできます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL チーム]**.

1. 次をクリック： **[!UICONTROL チームの切り替え]** アイコンをクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。
1. 次をクリック： **[!UICONTROL 詳細]** メニュー、次に「 **[!UICONTROL 編集]**.
1. 次を検索： **[!UICONTROL 完了ボタン]** の一番下のセクション **[!UICONTROL チーム設定]** ページ。

1. 各作業項目タイプに対して 1 つ以上のステータスを選択します。

   >[!NOTE]
   >
   >タスクまたは問題のステータスを選択する際は、次の点を考慮してください。
   >
   >* 作業項目の種類ごとに 1 つのステータスを選択すると、ユーザーがクリックすると、タスクまたは問題のステータスがそのステータスに設定されます [!UICONTROL 完了] を選択します。 作業項目のタイプごとに複数のステータスを設定した場合、 [!UICONTROL 完了] 」ボタンをクリックし、作業項目のステータスを変更するには、ステータスを選択する必要があります。
   >* システムレベルのステータスのみを [!UICONTROL 完了] 」ボタンをクリックします。 グループ固有のステータスを作業項目のステータスに関連付けることはできません。
   >* アイテムに割り当てられたユーザーが、アイテムを [!UICONTROL 完了] ボタンをクリックすると、項目は [!UICONTROL 完了] 選択したステータスが [!UICONTROL 完了] または [!UICONTROL クローズ] ステータスまたは作業ステータス。

   >   
   >   
   >  例えば、 [!UICONTROL 完了] ボタンをクリックすると、作業項目が [!UICONTROL 完了] ステータスを「新規」から「処理中」に変更するユーザーのステータスを表示します。
   >   
   >* 問題のタイプはカスタマイズ可能で、環境によっては、以下に示すように異なる名前が付けられる場合があります。\
      >  デフォルトのタスクと問題のタイプは次のとおりです。
      >     
      >   * [!UICONTROL タスク]
      >   * [!UICONTROL 問題]
      >   * [!UICONTROL リクエスト]
      >   * [!UICONTROL 変更依頼]
      >   * [!UICONTROL バグ報告書]


   タスクまたはイシューが複数のユーザーに割り当てられている場合は、「[!UICONTROL 私の部分で完了]」オプションが表示されます。

1. クリック **[!UICONTROL 変更を保存]**.

## ユーザをホームチームに関連付ける

を変更するには、以下を実行します。 [!UICONTROL 完了] ボタン機能をユーザに表示するには、ユーザのホームチームを変更したチームに設定します。

ユーザーをホームチームに関連付けるには：

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront].

1. クリック **[!UICONTROL ユーザー]**&#x200B;をクリックし、ホームチームに関連付ける 1 人または複数のユーザを選択します。
1. 次をクリック： **[!UICONTROL 詳細]** メニューから、 **[!UICONTROL 編集]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 内 **[!UICONTROL 組織]** セクションで、 **[!UICONTROL ホームチーム]** フィールドに入力します。 設定をユーザーに関連付けるチームの名前を入力します。 リストにチームの名前が表示されたら、そのチームの名前をクリックします。

1. クリック **[!UICONTROL 変更を保存]**.\
   選択したユーザがホームチームに関連付けられます。
チーム設定 ( [!UICONTROL 完了] ボタンが表示されるようになりました。

## の設定 [!UICONTROL 完了] ボタン [!UICONTROL 解決済み] ステータスは削除されました

ユーザーがホームチームを持たず、システム全体のデフォルトが [!UICONTROL 解決済み] ([!UICONTROL RLV]) が削除された場合、 [!DNL Workfront] 管理者は、 [!UICONTROL クローズ] プロジェクトに対するグループのステータス。 [!DNL Workfront] ユーザーが [!DNL Done] 」ボタンをクリックします。

### プロジェクトに関連付けられているグループを検索します

ユーザーがプロジェクトを作成すると、そのユーザーのホームグループが自動的にプロジェクトに割り当てられます。 次を持つユーザー： [!UICONTROL 管理] プロジェクトへのアクセスで、 [!UICONTROL プロジェクトの詳細] セクションに含めることができます。 ステータスを理解するには [!DNL Workfront] この場合、が完了した問題を使用するには、問題が関連付けられているプロジェクトに関連付けられているグループと、問題のデフォルトのステータスを理解する必要があります [!UICONTROL クローズ] このグループには、問題の情報が含まれています。

プロジェクトに関連付けられているグループを検索するには、次の手順に従います。

1. プロジェクトに移動します。
1. ページの左側で、 **[!UICONTROL プロジェクトの詳細]**.
1. を **[!UICONTROL プロジェクトの関連付け]** セクション、 **[!UICONTROL グループ]**.\
   これは、「設定」(Setup) 領域でステータスを確認するために使用する必要があるグループ名です。 特定のグループのデフォルトのステータスを更新する方法については、次の節を参照してください。

### 特定のグループのデフォルトのステータスを更新する

As a [!UICONTROL Workfront] 管理者は、特定のグループのステータスを更新できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 左側のパネルで、 **[!UICONTROL プロジェクト環境設定]**&#x200B;を、 **[!UICONTROL ステータス]**.

1. クリック **[!UICONTROL 問題]**&#x200B;をクリックし、 **[!UICONTROL システムステータス]** 右側の検索ボックス

1. グループを選択します。
1. 次をクリック： **[!UICONTROL デフォルトのステータスの設定]** ドロップダウンメニューから、 [!UICONTROL クローズ]. [!DNL Workfront] ユーザーが [!UICONTROL 完了] 」ボタンをクリックします。

   >[!IMPORTANT]
   >
   >このステータスは、ユーザーがホームチームを割り当てておらず、 [!UICONTROL RLV] のステータスが削除されました。

1. 「**[!UICONTROL 保存]**」をクリックします。
