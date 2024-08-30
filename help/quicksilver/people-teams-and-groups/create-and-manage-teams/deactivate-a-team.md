---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: チームの非アクティブ化
description: 関連する履歴データを保持したまま、使用しなくなったチームを非アクティブ化できます。Adobe Workfront 管理者は、設定のチームエリアからいつでもチームを再アクティブ化できます。
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 95%

---

# チームの非アクティブ化

関連する履歴データを保持したまま、使用しなくなったチームを非アクティブ化できます。[!DNL Adobe Workfront] 管理者は、設定のチームエリアからいつでもチームを再アクティブ化できます。チームを非アクティブ化すると、チームは以下のエリアに表示されなくなります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>カスタムフォームの先行入力フィールド</p> </li> 
    </ul> 
    <ul> 
     <li> <p>オブジェクトの共有ダイアログ</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] エリアのメイン選択ドロップダウンメニュー</p> </li> 
     <li> <p>[!UICONTROL Assignments] 先行入力</p> </li> 
     <li> <p>プロジェクトの [!UICONTROL Add to Kanban] ボードダイアログ</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

非アクティブ化されたチームは、チームを検索するときに表示されませんが、ユーザーが非アクティブ化前にチームに割り当てられていた場合は、[!UICONTROL ホームチーム]およびその他のチームには引き続き表示されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## チームの非アクティブ化

非アクティブ化する前にチームに割り当てられた作業は、すべて割り当てられたままです。チームを非アクティブ化する前に、作業を再割り当てすることをお勧めします。

>[!TIP]
>
>非アクティブ化されたチームがまだ割り当てられているタスクやイシューをフィルタリングして特定するレポートを作成できます。

リクエストキューを使用する場合、ルーティングルールでデフォルトチームとして割り当てられたチームを非アクティブ化しても、そのチームはそのまま残り、リクエストは非アクティブ化されたチームに引き続きルーティングされます。チームを非アクティブ化する前に、アクティブなチームでルーティングルールをアップデートすることをお勧めします。

{{step1-to-team}}

1. **[!DNL Switch team]** アイコンをクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。
1. **[!UICONTROL その他]**&#x200B;メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

   ![](assets/edit-team-settings-350x205.png)

1. 「**[!UICONTROL アクティブ]**」チェックボックスをオフにします。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

## 既知の制限事項

非アクティブ化されたチームは、以下のエリアに表示されます。

* [!DNL Workfront Goals] の所有者フィールドこれには、追加の [!DNL Adobe Workfront Goals] ライセンスが必要です。詳しくは、[概要 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md)を参照してください。
