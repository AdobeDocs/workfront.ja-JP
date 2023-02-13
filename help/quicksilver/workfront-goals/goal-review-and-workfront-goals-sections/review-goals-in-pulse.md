---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront目標パルスの節で目標を確認する
description: 所有者が誰であるかに関係なく、組織内のすべての目標を表示できます。 目標の作成について詳しくは、「Adobe Workfront目標で目標を作成する」を参照してください。
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# Adobe Workfront目標パルスの節で目標を確認する

>[!IMPORTANT]
> 
>この記事で説明する機能は、23.1 リリースからWorkfrontから削除されました。\
>この記事は、2023 年初頭の 23.1 リリースの直後にも削除されます。 現時点では、ブックマークを適宜更新することをお勧めします。


所有者が誰であるかに関係なく、組織内のすべての目標を表示できます。 目標の作成について詳しくは、 [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md).

Adobe Workfront目標のパルスセクションを共同作業ツールとして使用できます。このツールでは、自分、チーム、グループまたは組織に属する現在の目標に関する更新のストリームを確認し、参加して、目標を常に最新の状態に保つことができます。 Workfront目標は、進行状況の更新、コメント、編集履歴を、「パルス」セクションの目標別にグループ化します。

## アクセス要件

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、 Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront目標の使用要件</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>目標へのアクセス権を表示またはそれ以上に設定</p> <p>メモ:  <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront目標へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標に対する権限の表示以上</p> 
     <p>目標の共有について詳しくは、 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront目標での目標の共有</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

を起動する前に、次の条件を満たす必要があります。

* メインメニューの目標領域を含むレイアウトテンプレート。

## Pulse セクションで目標の更新とコメントを管理 

>[!TIP]
>
>少なくとも 1 回、チェックインした目標のみが「パルス」セクションに表示されます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) > **目標** をクリックします。

   「Workfront目標」領域が開きます。

   デフォルトでは、すべての目標が表示されます。

1. クリック **パルス** をクリックします。

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   目標のリストが表示されます。 リストには、各目標に関する情報を含む次の列が含まれています。

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">目標</td> 
         <td>目標名。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">所有者</td> 
         <td>目標所有者の名前。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">期間</td> 
         <td>目標がスケジュールされる期間。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">進捗状況</td> 
         <td>目標の進捗状況インジケーター。通常は割合 (%) の値です。</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>ステータス（整列アイコンを含む）</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>次のいずれかの目標のステータス。</p> 
         <ul> 
         <li>アクティブ</li> 
         <li>下書き</li> 
         <li>非アクティブ</li> 
         <li>クローズ</li> 
         </ul> <p>整列アイコンは、他の目標に合わせた目標に表示されます。 目標の調整について詳しくは、 <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">目標をAdobe Workfront目標に結び付けて整列させる</a>.</p>

   <p>「ステータス」列には、目標に対する各チェックインに伴う、結果またはアクティビティごとの増分更新も含まれます。</p>

   例えば、目標に手動で進行状況バーアクティビティが 1 つあり、目標をチェックインしてアクティビティを 50%に更新した場合、「ステータス」列には、その目標のアクティビティの 50%が表示されます。 後で、同じアクティビティを 60%に更新する場合があります。 この場合、10%の同じアクティビティの同じ目標の下に、新しい行が表示されます。これは、アクティビティの進行状況に 10%を追加しただけなのです。
   </td>
   </tr> 
      </tbody> 
      </table>

1. （オプション）「パルス」セクションの右上隅にあるフィルターを更新して、表示する情報のタイプを選択します。

   パルスリストには、選択したフィルターの条件に一致する目標と更新された履歴が表示されます。

   目標のフィルタリングについて詳しくは、 [Adobe Workfront目標での情報のフィルター](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 目標名の左側にある右向き矢印をクリックして目標を展開し、各目標の更新に関する追加情報を表示します。

   以下の情報は、各目標の下の Pulse セクションに表示されます。

   * 結果の名前と所有者。 結果について詳しくは、 [Adobe Workfront目標の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * アクティビティ名と所有者。 アクティビティについて詳しくは、 [Adobe Workfront目標での目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * 結果およびアクティビティのプログレスバーと進捗状況ステータス Workfront目標での目標の進捗の計算方法について詳しくは、 [Adobe Workfront目標の目標の達成状況と条件の概要](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. クリック **コメントを追加** 目標にコメントを追加するには、 **投稿**. コメントは、チェックイン領域と、目標の詳細パネルの「更新」タブに表示されます。 「パルス」セクションを使用して、しばらく更新されていない目標についてコメントし、目標の所有者に更新を依頼することをお勧めします。

1. （オプション）「 **すべての更新を表示** すべての目標の更新を表示します。 右側の目標の詳細パネルに「更新」タブが開きます。
1. 目標の名前をクリックして、 **目標の詳細** 右側のパネルをクリックし、目標に関する詳細を確認し、目標とその結果およびアクティビティを管理します。 個々の目標の確認について詳しくは、 [Adobe Workfront目標の「目標の詳細」節の目標を更新します](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. （オプションおよび条件付き）「 **整列アイコン** ![](assets/align-icon.png) 目標が他の目標に合わされている場合は、目標揃えセクションで目標を開きます。

1. （オプション） **1 ページの目標** ドロップダウンメニューから「 」を選択し、追加の目標を表示します。

   * 20. これはデフォルトの選択です。
   * 50
   * 100


