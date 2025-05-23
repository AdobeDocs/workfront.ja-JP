---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: かんばんボード上のストーリーに関するフラグの使用
description: ' [!DNL Kanban]  ボードで、フラグは、ストーリーが次のステータスに移行する準備ができていることを視覚的に示します。これにより、かんばんチームは、ステータス間でストーリーを移動する際に、「プッシュ」アプローチではなく「プル」アプローチを使用できます。'
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 84%

---

# [!UICONTROL かんばん]ボードのストーリーにフラグを使用

[!DNL Kanban] ボードで、フラグは、ストーリーが次のステータスに移行する準備ができていることを視覚的に示します。これにより、[!UICONTROL かんばん]チームは、ステータス間でストーリーを移動する際に、「プッシュ」アプローチではなく「プル」アプローチを使用できます。

**例：**「プル」アプローチを使用するチームの例を考えてみましょう。チームのグラフィックデザイナーである Olivia が作業を終了し、ストーリーフラグを「[!UICONTROL プル準備完了]」に設定します。このフラグは、チームのコピーライターである Tony に対し、ストーリーが次のステータスに移る準備ができていることを視覚的に示します。Tony は、作業を始める準備が整ったら、次のステータスに進みます。

ストーリーでフラグを使用する際は、次の点に注意してください。

* フラグはステータスではなく、チームの別のメンバーがストーリーを次のステータスに移す準備ができていることを視覚的に示します。
* [!UICONTROL バックログ]列または[!UICONTROL 完了]列（または列のステータスが[!UICONTROL 完了]に等しい列）にあるストーリーカードにはフラグが表示されません。

  ストーリーのステータスについて詳しくは、[かんばんボード上のストーリーでのフラグの使用](#updating-the-status-of-stories-and-subtasks)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p> 
   または
   <p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL かんばん]ボードのストーリーでフラグを使用

ストーリーのフラグを変更するには：

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しい[!UICONTROL かんばん]チームを選択するか、検索バーでチームを検索します。

1. ストーリーのステータスを変更する[!UICONTROL かんばん]ボードに移動します。
1. ストーリータイルを展開すると、フラグが表示されます。
デフォルトでは、各ストーリーに対してフラグは「**[!UICONTROL 順調]**」に設定されます。
   ![かんばんカード](assets/agile-storycard-kanban-2021-350x308.png)

1. 現在のフラグをクリックし、次のフラグオプションから選択します。

   * **[!UICONTROL 順調 &#x200B;]:** ストーリーは適切なステータスにあり、現時点では、何もする必要はありません。

     かんばんボードの各ストーリーの既定のフラグです。
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL ブロック済み]：**&#x200B;ストーリーは次のステータスに進めません。ストーリーにこのフラグを設定した場合、ストーリーは WIP 制限にカウントされません。（WIP 制限について詳しくは、「かんばんの設定 [ を参照し ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) ください。

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 取り込み準備完了 &#x200B;]:** ストーリーを、チームの別のメンバーが次のステータスに移動する準備が整いました。

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
