---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: カンバンボードのストーリーにフラグを使用する
description: ' [!DNL Kanban]  ボードで、フラグは、ストーリーが次のステータスに移行する準備ができていることを視覚的に示します。 これにより、かんばんチームは、ステータス間でストーリーを移動する際に、「プッシュ」アプローチではなく「プル」アプローチを使用できます。'
author: Courtney
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zyfrbteuJy-xfPZL75ElkfotVrJWLHF78hDsIwkouko
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 458
ht-degree: 85%

---

# [!UICONTROL かんばん]ボードのストーリーにフラグを使用

[!DNL Kanban] ボードで、フラグは、ストーリーが次のステータスに移行する準備ができていることを視覚的に示します。 これにより、[!UICONTROL かんばん]チームは、ステータス間でストーリーを移動する際に、「プッシュ」アプローチではなく「プル」アプローチを使用できます。

**例：**「プル」アプローチを使用するチームの例を考えてみましょう。チームのグラフィックデザイナーである Olivia が作業を終了し、ストーリーフラグを「[!UICONTROL プル準備完了]」に設定します。 このフラグは、チームのコピーライターである Tony に対し、ストーリーが次のステータスに移る準備ができていることを視覚的に示します。 Tony は、作業を始める準備が整ったら、次のステータスに進みます。

ストーリーでフラグを使用する際は、次の点に注意してください。

* フラグはステータスではなく、チームの別のメンバーがストーリーを次のステータスに移す準備ができていることを視覚的に示します。
* [!UICONTROL バックログ]列または[!UICONTROL 完了]列（または列のステータスが[!UICONTROL 完了]に等しい列）にあるストーリーカードにはフラグが表示されません。

  ストーリーのステータスについて詳しくは、[かんばんボード上のストーリーでのフラグの使用](#updating-the-status-of-stories-and-subtasks)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL かんばん]ボードのストーリーでフラグを使用

ストーリーのフラグを変更するには：

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しい[!UICONTROL かんばん]チームを選択するか、検索バーでチームを検索します。

1. ストーリーのステータスを変更する[!UICONTROL かんばん]ボードに移動します。
1. ストーリータイルを展開して、フラグを表示します。
デフォルトでは、各ストーリーの&#x200B;**[!UICONTROL トラック]**&#x200B;にフラグが設定されています。
   ![かんばんカード](assets/agile-storycard-kanban-2021-350x308.png)

1. 現在のフラグをクリックし、次のフラグオプションから選択します。

   * **[!UICONTROL トラック &#x200B;]:** ストーリーは適切なステータスであり、現時点ではアクションを実行する必要はありません。

     かんばんボードの各ストーリーの既定のフラグです。
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL ブロック済み]：**&#x200B;ストーリーは次のステータスに進めません。 ストーリーにこのフラグを設定した場合、ストーリーは WIP 制限にカウントされません。 （WIP制限について詳しくは、[&#x200B; カンバンの設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)を参照してください）。

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL 引き出す準備ができました]:** ストーリーは、チームの別のメンバーによって次のステータスに移動する準備ができています。

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
