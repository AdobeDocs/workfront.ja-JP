---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: かんばんボード上でストーリーのフラグを使用
description: ' [!DNL Kanban]  ボードで、フラグは、ストーリーが次のステータスに移行する準備ができていることを視覚的に示します。これにより、かんばんチームは、ステータス間でストーリーを移動する際に、「プッシュ」アプローチではなく「プル」アプローチを使用できます。'
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: ht
source-wordcount: '536'
ht-degree: 100%

---

# [!UICONTROL かんばん]ボードのストーリーにフラグを使用

[!DNL Kanban] ボードで、フラグは、ストーリーが次のステータスに移行する準備ができていることを視覚的に示します。これにより、[!UICONTROL かんばん]チームは、ステータス間でストーリーを移動する際に、「プッシュ」アプローチではなく「プル」アプローチを使用できます。

**例：**「プル」アプローチを使用するチームの例を考えてみましょう。チームのグラフィックデザイナーである Olivia が作業を終了し、ストーリーフラグを「[!UICONTROL プル準備完了]」に設定します。このフラグは、チームのコピーライターである Tony に対し、ストーリーが次のステータスに移る準備ができていることを視覚的に示します。Tony は、作業を始める準備が整ったら、次のステータスに進みます。

ストーリーでフラグを使用する際は、次の点に注意してください。

* フラグはステータスではなく、チームの別のメンバーがストーリーを次のステータスに移す準備ができていることを視覚的に示します。
* [!UICONTROL バックログ]列または[!UICONTROL 完了]列（または列のステータスが[!UICONTROL 完了]に等しい列）にあるストーリーカードにはフラグが表示されません。

  ストーリーのステータスについて詳しくは、[かんばんボード上のストーリーでのフラグの使用](#updating-the-status-of-stories-and-subtasks)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!UICONTROL かんばん]ボードのストーリーでフラグを使用

ストーリーのフラグを変更するには：

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**[!UICONTROL ボード]**」の順にクリックします。

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しい[!UICONTROL かんばん]チームを選択するか、検索バーでチームを検索します。

1. ストーリーのステータスを変更する[!UICONTROL かんばん]ボードに移動します。
1. ストーリータイルを展開して、フラグを表示します。\
   デフォルトでは、各ストーリーに対してフラグは「**[!UICONTROL 順調]**」に設定されます。\
   ![かんばんカード](assets/agile-storycard-kanban-2021-350x308.png)

1. 現在のフラグをクリックし、次のフラグオプションから選択します。

   * **[!UICONTROL 順調]：**&#x200B;ストーリーのステータスは適切で、現時点では何のアクションも実行する必要はありません。\

     かんばんボードの各ストーリーの既定のフラグです。\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL ブロック済み]：**&#x200B;ストーリーは次のステータスに進めません。ストーリーにこのフラグを設定した場合、ストーリーは WIP 制限にカウントされません。（WIP 制限について詳しくは、[かんばんの設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)の記事を参照してください。\

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL プル準備完了]：**&#x200B;このストーリーは、チームの別のメンバーが次のステータスに移動する準備が整いました。\

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
