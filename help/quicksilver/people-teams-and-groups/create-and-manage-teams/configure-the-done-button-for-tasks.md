---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: タスクの「完了」ボタンの設定
description: 「完了」ボタンを使用して、タスクまたはイシューのステータスを自動的に設定できます。 デフォルトでは、Adobe Workfrontは、担当者が作業項目で「完了」をクリックすると、タスクを「完了」とマークします。
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# の設定 [!UICONTROL 完了] タスクのボタン

この [!UICONTROL 完了] ボタンを使用して、タスクまたはイシューのステータスを自動的に設定できます。 デフォルトでは、 [!UICONTROL Adobe Workfront] タスクを [!UICONTROL 完了] 担当者が作業項目で「完了」をクリックしたとき。

## 概要

特定の権限を持つユーザーは、 [!UICONTROL 完了] ボタンを使用して、特定のステータスをシステムに反映させることができます。 次の 2 つの方法があります。 [!UICONTROL 完了] ボタンが [!UICONTROL Workfront]:

* ユーザーがホームチームを割り当てている場合、 [!DNL Workfront] 管理者または [!UICONTROL プラン] ライセンスは、 [!UICONTROL 完了] ボタンを使用して、チームメンバーに特定のステータスを反映させます。 詳しくは、 [の設定 [!UICONTROL 完了] チームのボタン](#configure-the-uicontrol-done-button-for-a-team) 」を参照してください。
* ユーザーがホームチームを割り当てていない場合、 [!UICONTROL 完了] タスクのボタンは、完了ステータスに結び付けられます。 このシナリオで使用できる設定オプションはありません。 この [!UICONTROL 完了] ボタンは、自動的にこのステータスに設定されます。

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
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、 [!DNL Workfront] 管理者。

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
   >  例えば、 [!UICONTROL 完了] ボタン [!UICONTROL 処理中] を指定すると、作業項目は [!UICONTROL 完了] ステータスを次から変更するユーザー： [!UICONTROL 新規] から [!UICONTROL 処理中].
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
