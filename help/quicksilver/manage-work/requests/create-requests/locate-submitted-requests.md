---
product-area: requests
navigation-topic: create-requests
title: 送信されたリクエストの検索
description: 自分または他のユーザーが送信したリクエストや、未送信でドラフトとして保存されていたリクエストを検索できる Adobe Workfront のエリアについて説明します。
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: 0ffae8ed285f6e9164a239552feb90465bea3cca
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 83%

---

# 送信されたリクエストを見つける

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

次のタイプのリクエストのうち、自分または他のユーザーが送信したものや、開始したが送信を完了していないものを検索できます。これらのリクエストは、Adobe Workfront の次のエリアで検索できます。

* Workfrontのリクエスト エリアの **Workfront** タブ：次の節で、Workfront リクエストキューに送信されたリクエストを確認します。
   * **「送信済み」セクション**：自分または他のユーザーが送信し、自分が表示以上のアクセス権を持っているすべてのリクエスト。
   * **「ドラフト」セクション**：開始したが、未完成で送信していないすべてのリクエスト。ドラフトリクエストについて詳しくは、[Adobe Workfront リクエストの作成と送信](../../../manage-work/requests/create-requests/create-submit-requests.md)を参照してください。

  >[!TIP]
  >
  >自分のドラフトリクエストのみを表示できます。

* Workfrontの「要求」エリアの「**計画**」タブ：Workfrontの計画リクエストフォームに送信された要求を検索します。 Workfront Planning パッケージを購入する必要があります。 詳しくは、次の記事を参照してください。

   * [Adobe Workfront Planning でのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)
   * [レコードを作成するためのAdobe Workfront Planning 要求の発行](/help/quicksilver/planning/requests/submit-requests.md)


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：Contributor 以上</p>
   または
   <p>現在：Request 以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>イシューへのアクセス権を編集</p></td> 
  </tr>
  <tr>
   <td role="rowheader">オブジェクト権限</td> 
   <td><p>リクエストに対する権限以上を表示</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 製品</td> 
   <td> <ul><li>Adobe Workfront</li><li>計画リクエストまたはリクエストフォームを表示するには、Adobe Workfront Planning が必要です。</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 送信されたリクエストを見つける

自分または他のユーザーが送信したリクエストを検索するには、次の手順に従います。

{{step1-to-requests}}

1. （条件付き）Workfront Planning パッケージを購入した場合は、「**Workfront**」タブをクリックしてWorkfront リクエストを表示します。
1. 左パネルの「**送信済み**」をクリックして、送信されたすべてのリクエストを表示します。

   最大 2,000 件のリクエストを表示でき、リクエストは複数のページにわたって表示される可能性があります。

   >[!TIP]
   >
   >送信済みリクエストリストの列はカスタマイズできません。

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


1. 次の列がデフォルトで表示されます。

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">名前</td> 
         <td> <p>リクエストの名前。</p> <p>リクエストの名前をクリックすると、リクエストが開きます。 </p> <p><b>ヒント</b>

   タスクまたはプロジェクトに変換したときにイシューが保持されなかった場合は、イシューの名前が淡色表示になり、クリックできなくなります。イシューの変換については、<a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Adobe Workfront におけるイシューの変換の概要</a>を参照してください。 </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">変換先</td> 
         <td> <p>リクエストの変換先の解決オブジェクト（タスクまたはプロジェクト）の名前。 </p> <p>タスクまたはプロジェクトの名前をクリックすると、そのオブジェクトが開きます。 </p> <p>リクエストが変換されなかった場合、このフィールドは空です。 </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">パス</td> 
         <td>リクエストが最初に送信されたリクエストキュー、トピックグループおよびキュートピックの名前。 </td> 
      </tr> 
      <tr> 
         <td role="rowheader">ステータス</td> 
         <td>リクエストまたは解決オブジェクト（タスクまたはプロジェクト）の現在のステータス</td> 
      </tr> 
      <tr> 
         <td role="rowheader">エントリ日</td> 
         <td>リクエストが送信された日付（変換時にリクエストが削除された場合は、解決オブジェクトが作成された日付）。 </td> 
      </tr> 
      <tr> 
         <td role="rowheader">最終更新日</td> 
         <td> <p>リクエストが最後に更新された日付。</p> <p>送信済みリクエストのリストは、デフォルトで、このフィールドで並べ替えられます。 </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. （オプション）並べ替える列のヘッダーをクリックします。

   >[!TIP]
   >
   >送信済みリクエストのリストから移動したとき、選択された並べ替えオプションが保持されます。

1. （オプション）リストからリクエストを選択し、**概要を開く**&#x200B;アイコン ![](assets/open-summary-with-text-nwe.png) をクリックして概要パネルを開き、リクエストに関する追加情報を表示したり、コメントやドキュメントを追加したり、割り当てたりします。概要パネルについて詳しくは、[概要の概要](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください。

   >[!TIP]
   >
   >概要パネルが既に開いている場合は、概要を開くアイコンが、概要を閉じるアイコンに変わります。

1. （オプションおよび条件付き）右上隅にある&#x200B;**X** アイコンか、**概要を閉じる** アイコン ![](assets/close-summary-with-text-nwe.png) をクリックし、概要パネルを閉じます。

   イシューがタスクまたはプロジェクトに変換され、変換処理でイシューが削除された場合、概要パネルは空白になります。イシューの変換について詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

1. リストの右上の&#x200B;**フィルターアイコン** ![](assets/filter-nwepng.png) から、次の表に示すフィルターのいずれかを選択します。

   >[!TIP]
   >
   >リクエストエリアの「送信済み」セクションでは、フィルターを変更できません。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべて</td> 
      <td>ステータスや送信者に関係なく、すべての送信済みリクエスト。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">開く</td> 
      <td> <p>送信者に関係なく、現在オープンであるすべての送信済みリクエスト。自分で送信しなかった場合は、表示以上の権限を持っているリクエストのみが表示されます。 </p> <p>実際の完了日がないリクエスト、または解決オブジェクトに実際の完了日が設定されていないリクエストは、「オープン」サブタブに表示されます。</p> <p><b>ヒント</b>

   ステータスがクローズに等しくないリクエストは、オープンと見なされます。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">マイリクエスト</td> 
      <td>ステータスに関係なく、送信したリクエスト。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">マイオープンリクエスト</td> 
      <td> <p>送信したリクエストで、まだオープンのもの。 </p> <p>実際の完了日がないリクエスト、または解決オブジェクトに実際の完了日が設定されていないリクエストは、「マイオープンリクエスト」サブタブに表示されます。 </p> <p><b>ヒント</b>

   ステータスがクローズに等しくないリクエストは、オープンと見なされます。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. （オプション）リストの上部にある&#x200B;**ページをフィルター**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、名前でリクエストを検索します。リストは、検索条件に一致する結果で更新されます。

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. 「**ドラフト**」をクリックして、すべてのドラフトリクエストを表示します。Workfront は、このフォルダー内の各リクエストキューに対して無制限の数のドラフトを保存します。既にドラフトのあるキュートピックの新しいリクエストを入力すると、既存のドラフトを使用するように求められます。詳しくは、[ドラフトからリクエストを作成](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)を参照してください。

1. （オプションおよび条件付き）Workfront Planning パッケージを購入した場合は、左側のパネルで「**Planning**」タブをクリックし、「**送信済み**」をクリックしてWorkfront Planning 要求を表示します。

   **フィルター** および **列** を使用して、Planning 要求リスト内の情報を更新します。

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   詳しくは、[ レコードを作成するためのAdobe Workfront Planning リクエストの発行 ](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。


