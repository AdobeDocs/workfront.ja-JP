---
product-area: projects
navigation-topic: use-the-home-area
title: ホームエリアの[!UICONTROL 作業リスト]に項目を表示
description: '[!UICONTROL ホーム]エリアの[!UICONTROL 作業リスト]には、自分に割り当てられているすべての作業項目が表示されます。表示する項目を [!UICONTROL 作業用リスト]、フィルターを使用し、作業項目をグループ化および並べ替える方法。'
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '1826'
ht-degree: 81%

---

# [!UICONTROL ホーム]エリアの[!UICONTROL 作業リスト]に項目を表示

<!-- Audited: 1/2024 -->


[!UICONTROL ホーム]エリアの[!UICONTROL 作業リスト]には、自分に割り当てられているすべての作業項目が表示されます。表示する項目を [!UICONTROL 作業用リスト]、フィルターを使用し、作業項目をグループ化および並べ替える方法。

>[!NOTE]
>
>* イシューをタスクまたはプロジェクトに変換すると、イシューに割り当てられたユーザーのホームエリアからイシューが削除されます。
>
>* タスクをプロジェクトに変換すると、タスクは削除され、タスクに割り当てられたユーザーのホームエリアから削除されます。


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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td> <p>新規：</p><ul><li>[!UICONTROL Contributor] ：承認のみ</li> <li>[!UICONTROL Standard] 以降（他のすべてのオブジェクト用）</li> <p>または</p> 
  </ul><p>現在：</p><ul><li>[!UICONTROL Review]（承認のみ）</li> <li>[!UICONTROL Work] 以上（他のすべてのオブジェクト）</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>プロジェクト、タスク、イシュー、ドキュメントに対する [!UICONTROL View] 以上のアクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>作業が必要なタスクやイシューに対する参加以上の権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## [!UICONTROL 作業リスト]のフィルタリング

[!UICONTROL 作業リスト]で項目をフィルタリングすると、特定のタイプの項目のみを表示できます。例えば、[!UICONTROL 作業リスト]をフィルタリングして、イシューまたはリクエストのみを表示できます。

>[!NOTE]
>
>フィルターオプションは、ブラウザーに保存されます。同じコンピューター上で一貫して同じブラウザーを使用している（かつ、サイトのデータをクリアしない）場合、選択したフィルターは変更されません。ブラウザーまたはコンピューターを切り替えると、フィルターがデフォルトのオプションに戻り、すべてのフィルターが選択解除されます。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
1. 次をクリック： **[!UICONTROL フィルター]** ![](assets/filter-nwepng.png) ドロップダウンメニュー。 フィルターを選択している場合は、アイコンの代わりに、選択したフィルターの数が表示されます。
1. 以下のフィルターオプションから選択して、表示する項目のタイプを指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>すべての項目を表示および選択します。これには、タスク、イシュー、承認、個人タスクおよび完了したタスクとイシューが含まれます。 </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL タスク：操作 ]</strong></td> 
      <td> <p>作業中のタスクのみを表示します。これらは、「[!UICONTROL Work On It]」ボタンをクリックして自分に割り当てられたタスクです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL タスク：開始準備完了 ]</strong></td> 
      <td> 
       <div> 
        <p>開始する準備が整ったタスクのみを表示します。以下の条件の両方が成り立つ必要があります。</p> 
        <ul> 
         <li> <p>タスクとその親には、作業を妨げる先行タスクやタスク制約がない。</p> </li> 
         <li> <p>タスクの[!UICONTROL Planned Start Date]が過去の日付か、最大 2 週間後になっている。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL タスク：準備ができていません ]</strong></td> 
      <td> 
       <div> 
        <p>まだ開始する準備ができていないタスクのみを表示します。以下の条件のいずれか 1 つが成り立つ必要があります。</p> 
        <ul> 
         <li> <p>タスクとその親に、作業を妨げる先行タスクやタスク制約がある可能性がある。</p> </li> 
         <li> <p>タスクの[!UICONTROL Planned Start Date]が 2 週間以上後の日付になっている。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL の問題：操作 ]</strong></td> 
      <td> <p>現在作業中のイシューのみを表示します。このタスクは、「[!UICONTROL Work On It]」ボタンをクリックして自分に割り当てられたイシューです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL の問題：リクエスト済み ]</strong></td> 
      <td>割り当てられているが [!UICONTROL Work On It] ボタンをクリックしていないイシューのみが表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>個人用</strong></td> 
      <td>個人用タスクのみを表示します。これらは、<a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">[!UICONTROL Home] エリアから作業アイテムの作成</a>の記事の<a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">個人用タスクを作成</a>の節で説明されているように、[!UICONTROL To Do] タスクとして作成するタスクです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>自分に割り当てられた、または委任された承認と、自分が送信した承認のみを表示します。承認には、作業項目（プロジェクト、タスクおよびイシュー）に対する承認、およびドキュメント、プルーフ、アクセス要求およびタイムシートに対する承認が含まれます。承認について詳しくは、次の記事を参照してください。</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">承認を表示</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">作業承認</a> </p> </li> 
        </ul> 
        <p>メモ：自分が送信し、自分が承認者の 1 人でもある承認は2 回カウントされます。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 委任：自分が委任しました ]</strong></td> 
      <td> 
       <div> 
        <p>別のユーザーに委任した作業項目のみを表示します。</p> 
        <p>タスクの委任について詳しくは、 <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">タスクと問題を別のユーザーに委任する</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 委任：自分に委任済み ]</strong></td> 
      <td> 
       <div> 
        <p>別のユーザーによって一時的に委任された作業項目のみを表示します。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Completed]</strong></td> 
      <td> <p>完了したタスク、イシューおよび個人用のタスクのみを表示します。過去 2 週間の完了した作業が表示され、完了した週に応じて作業リストにグループ化されます。承認は含まれません。</p> <p>このフィルターを選択しない限り、完了した作業は [!UICONTROL Work List] に表示されません。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* フィルターオプションは、オブジェクト（タスク、イシュー、承認、個人用タスク）に基づきます。
   >* タスクとイシューは、作業の準備状態と関連してさらにフィルタリングされます（[!UICONTROL 作業中]、[!UICONTROL 開始準備完了]、タスクの[!UICONTROL 準備未完了]およびイシューの[!UICONTROL 作業中]と[!UICONTROL 要求済み]）。特定のステートのタスクまたはイシューを表示することを選択するか、「タスク」または「イシュー」をクリックしてすべてのステートを選択して表示できます。
   >* 完了した項目に対しては別のフィルターがあり、タスクとイシューの両方が含まれます。これには承認は含まれません。[!UICONTROL 完了]フィルターには、個人用のタスクが含まれます。
   >* 一度に 1 つの状態のみを表示するよう選択できます。 例えば、 [!UICONTROL 作業中] タスクとのみ [!UICONTROL リクエスト済み] 問題。 また、一度に複数の状態を選択することもできます。
   >* チームの 1 つに割り当てられた項目に対してフィルタを適用することはできません。また、チームの割り当ては、直接割り当てられた項目には含まれません。


1. （オプション）さらに[!UICONTROL 作業リスト]を整理するには、この記事の[日付、プロジェクト、優先度でグループ化して並べ替え](#group-and-sort-by-date-project-and-priority)の節を参照してください。

## [!UICONTROL 日付]、[!UICONTROL プロジェクト]および[!UICONTROL 優先度]によるグループ化と並び替え

[!UICONTROL 予定完了日]、[!UICONTROL コミット日]、[!UICONTROL プロジェクト]または[!UICONTROL マイ優先度]により、[!UICONTROL 作業用リスト]をグループ化して並べ替えることができます。選択するオプションにより、[!UICONTROL 作業リスト]の項目をグループ化する方法が決まります。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
1. 次をクリック： **[!UICONTROL グループ化の基準]** ![グループ化の基準](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) ドロップダウンメニュー。

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. 次のオプションから選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td> 
      <td> <p> 項目は、[!UICONTROL Planned Completion Date] に応じて、[!UICONTROL Work List] 内の次のグループ化で表示されます（各グループに含まれる項目の数は、見出しのタイトル横の括弧内に表示されます）。</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL No Planned Completion Date]</p> </li> 
        <li> <p>[!UICONTROL This Week]</p> <p>このグループ化は、デフォルトで展開されます。</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned] に続き、様々な [!UICONTROL Planned Completion Dates] が続く（複数のグループ化）</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Planned Start]</strong></td> 
      <td> <p>項目は、[!UICONTROL Planned Start Date] に応じて、[!UICONTROL Work List] 内の次のグループ化で表示されます（各グループに含まれる項目の数は、見出しのタイトル横の括弧内に表示されます）。</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL This Week] </p> <p>このグループ化は、デフォルトで展開されます。</p> </li> 
        <li> <p>[!UICONTROL Next Week]</p> </li> 
        <li> <p>[!UICONTROL Planned] に続き、様々な [!UICONTROL Planned Start Dates] が続く（複数のグループ化）</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Commit Date]</strong></td> 
      <td> <p>項目は、[!UICONTROL Work List] 内の次のグループに表示されます（各グループに含まれる項目の数は、見出しのタイトルの横に括弧で囲まれて表示されます）。</p> 
       <ul> 
        <li> <p>[!UICONTROL No Commit Date]</p> </li> 
        <li> <p>[!UICONTROL Committed Next Week]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>項目はプロジェクトに従ってグループ化され、プロジェクトは [!UICONTROL Work List] でアルファベット順に表示されます。（各グループ内に含まれる項目の数は、見出しのタイトルの横に括弧で囲まれて表示されます）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>項目は、選択した順序で表示されます。詳しくは、<a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">[!UICONTROL Home] 領域で作業を優先</a>を参照してください。</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>デフォルトの並べ替えは昇順です。 並べ替えを降順に変更すると、選択した並べ替えオプションがブラウザーに保存されます。 同じコンピューター上で同じブラウザーを一貫して使用し、サイトのデータをクリアしない場合、並べ替えは変更されませんが、ブラウザーまたはコンピューターを切り替えた場合、並べ替えはデフォルトの並べ替えに変更されます。

## 遅れた項目を表示する

[!DNL Adobe Workfront] は、次の日付を使用して、作業リクエストが遅れているかどうかを判断します。

* **タスク**：[!UICONTROL 予定完了日]
* **イシュー**：[!UICONTROL 予定完了日]
* **ドキュメント**：[!UICONTROL 送信日]
* **タイムシート**：[!UICONTROL 送信日]
* **承認**：[!UICONTROL 送信日]
* **プルーフの承認**：[!UICONTROL プルーフの期限]

## [!UICONTROL 作業リスト]を検索します。

[!UICONTROL 作業リスト]を検索する場合、割り当てられた項目は検索で返されます（現在画面に読み込まれていない項目も検索で返されます）。[!UICONTROL 完了済みを表示]オプションが選択されている場合は、過去 2 週間以内に完了としてマークした項目も返されます。

また、作業項目の名前のみが検索されます（作業項目内の情報は検索されず、作業項目が存在するプロジェクトの名前も検索されません）。

[!UICONTROL 作業リスト]を検索するには、以下を実行します。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
1. （オプション） [!UICONTROL 作業用リスト]を参照してください。 [フィルター [!UICONTROL 作業用リスト]](#filter-the-work-list) および [日付、プロジェクト、優先度でグループ化および並べ替え](#group-and-sort-by-date-project-and-priority).

1. （オプション）既に完了している作業アイテムを検索する場合は、検索する前に、完了した項目を表示するように[!UICONTROL 作業リスト]を設定する必要があります。

1. 検索アイコンをクリックします。 ![検索](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. 検索する項目名の入力を開始します。\
   [!UICONTROL 作業リスト]は、一致する名前を持つ項目を含むように自動的にフィルタリングされます。

## 作業リストのサイズを変更する

[!UICONTROL 作業リスト]のサイズを変更して、ホームエリアの約 4 分の 1 から[!UICONTROL ホーム]エリアの約半分の間で使用することができます。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
1. [!UICONTROL 作業リスト]の右端にマウスを合わせ、作業リストが希望のサイズになるまで左または右にドラッグします。

## グループ化を折りたたみ、展開する

[!UICONTROL 作業リスト]内の項目はグループ化内に表示されます。グループ化を折りたたんだり展開したりして、特定の時点でページに表示する情報の量を制御できます。

[!UICONTROL 作業リスト]内のグループ化を折りたたんだり展開したりして、表示される情報をより適切に制御できます。\
デフォルトでは、[!UICONTROL 今週]のグループ化が展開され、その他のグループ化はすべて折りたたまれます。加えた変更は、次回ホームエリアにアクセスしたときに記憶されます。

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。
1. 展開または折りたたむグループ化の横にある「**[!UICONTROL 展開]**」または「**[!UICONTROL 折りたたむ]**」矢印をクリックします。

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   または\
   すべてのグループ化を同時に展開または折りたたむには、[!UICONTROL Shift] キーを押しながら、グループ化の横にある「**[!UICONTROL 展開]**」または「**[!UICONTROL 折りたたむ]**」矢印をクリックします。
