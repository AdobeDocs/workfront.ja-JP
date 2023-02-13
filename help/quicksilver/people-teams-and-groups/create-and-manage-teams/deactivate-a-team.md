---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: チームを非アクティブ化
description: 関連する履歴データを保持したまま、使用しなくなったチームを非アクティブ化できます。 Adobe Workfrontの管理者は、セットアップの「チーム」領域からいつでもチームを再アクティブ化できます。
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# チームを非アクティブ化

関連する履歴データを保持したまま、使用しなくなったチームを非アクティブ化できます。 [!DNL Adobe Workfront] 管理者は、セットアップの「チーム」領域からいつでもチームを再アクティブ化できます。 チームを非アクティブ化すると、チームは次の領域に表示されなくなります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>カスタムフォームの先頭に入力するフィールド</p> </li> 
    </ul> 
    <ul> 
     <li> <p>オブジェクトの共有ダイアログ</p> </li> 
     <li> <p>[!UICONTROL ユーザープロファイル ]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL チーム ] 領域のメイン選択ドロップダウンメニュー</p> </li> 
     <li> <p>[!UICONTROL 割り当て ] typeahead</p> </li> 
     <li> <p>プロジェクトの [!UICONTROL かんばんに追加 ] ボードダイアログ</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

非アクティブなチームは、チームを検索しても表示されませんが、には表示されます [!UICONTROL ホームチーム] およびその他のチーム（非アクティブ化の前にユーザーがチームに割り当てられた場合）

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>計画</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、 [!DNL Workfront] 管理者。

## チームを非アクティブ化

アクティベーションを解除する前にチームに割り当てられた作業は、すべて割り当てられたままになります。 チームを非アクティブ化する前に、作業を再割り当てすることをお勧めします。

>[!TIP]
>
>非アクティブなチームが割り当てられたままのタスクや問題をフィルタリングするレポートを作成できます。

リクエストキューを使用する場合、ルーティングルールでデフォルトチームとして割り当てられたチームを非アクティブ化しても、チームはそのまま残り、リクエストは非アクティブなチームにルーティングされます。 チームを非アクティブ化する前に、アクティブなチームでルーティングルールを更新することをお勧めします。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL チーム]**.
1. 次をクリック： **[!DNL Switch team]** アイコンをクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。
1. 次をクリック： **[!UICONTROL 詳細]** メニューから、 **[!UICONTROL 編集]**.

   ![](assets/edit-team-settings-350x205.png)

1. をクリア **[!UICONTROL アクティブ]** チェックボックスをオンにします。
1. クリック **[!UICONTROL 変更を保存]**.

## 既知の制限事項

非アクティブなチームは、次の領域に表示されます。

* の「所有者」フィールド [!DNL Workfront Goals]. 追加のライセンスが必要です。 [!DNL Adobe Workfront Goals]. 詳しくは、 [の基本を学ぶ [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
