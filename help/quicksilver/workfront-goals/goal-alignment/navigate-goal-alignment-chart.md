---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront Goals の目標の整合性セクションに移動
description: 「目標の整合性」セクションを使用して、組織全体の目標揃えの全体像をフローチャートに表示します。整合させた目標は、階層ツリー内で相互に接続するカードに表示されます。
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 91%

---

# Adobe Workfront Goals の目標の整合性セクションに移動

「目標の整合性」セクションを使用して、組織全体の目標揃えの全体像をフローチャートに表示します。整合させた目標は、階層ツリー内で相互に接続するカードに表示されます。

目標の整合性とその達成方法については、次の記事も参照してください。

* [Adobe Workfront Goals の整合性の概要](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [目標を Adobe Workfront Goals で相互に関連付けて整合させる方法](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## アクセス要件

この記事で説明するアクティビティを実行するには、次の操作が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
 <tr>
 <td role="rowheader">Adobe Workfront プラン*</td>
 <td>
 <p>新規計画：以上を選択</p>
 または
 <p>現在のプラン：Pro 以上</p>
 
 </td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront ライセンス*</td>
 <td>
 <p>新規ライセンス：コントリビューター以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p>  </td>
 </tr>
 <tr>
 <td role="rowheader">製品*</td>
 <td>
 <p> 新製品の要件は、次のいずれかです。 </p>
<ul>
<li>Select または Prime Adobe Workfront プランと、追加のAdobe Workfront Goals ライセンス。</li>
<li>Workfront Goals をデフォルトで含む究極のWorkfront プラン。 </li></ul>
 <p>または</p>
 <p>現在の必要な製品：Workfront プランとAdobe Workfront Goals の追加ライセンス。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
 <div>
 <p>目標の表示には表示権限以上が必要</p>
 <p>目標に対する編集権限を管理</p>
 <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
 </div> </td>
 </tr>
<tr>
<td role="rowheader"><p>レイアウトテンプレート</p></td>
<td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
</tr>
 </tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 目標の関連付けページへの移動

1. 右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![メインメニュー](../goal-alignment/assets/dots-main-menu-icon.png)アイコン、次に「**目標**」をクリックします。
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 左パネルの「**目標の整合性**」をクリックします。
1. 整合性グラフの右上隅にあるフィルターを使用して、重要な目標のみを選択します。Workfront Goals でのフィルターの使用について詳しくは、[Adobe Workfront Goals での情報のフィルター](../../workfront-goals/goal-management/filter-information-wf-goals.md)を参照してください。

   フィルターに一致する目標は、カードの整合性グラフに表示されます。

   次の情報が目標カードに表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期間の日付 </td> 
      <td> <p>これは、目標がオープンとなっている期間です。目標は、期間の終了日までに達成する必要があります。Workfront Goals は、目標の期間と現在の日付に基づいて目標の進捗を計算します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況インジケーター</td> 
      <td>目標の進行状況インジケーターの数。進捗インジケーターは、目標、結果、活動、またはアクティビティを関連付けることができます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者名</td> 
      <td>目標の所有者として指定されたユーザー、チーム、グループまたは組織の名前。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目標名</td> 
      <td>目標の名前。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目標進捗バー<span>および進捗</span></td> 
      <td> <p>目標の進捗は、現在達成されている目標の量を示します。これは、目標の期間の開始以降の経過時間に基づいて、目標に関連するすべての目標、結果およびアクティビティの進捗の平均を自動計算します。目標の進捗の計算について詳しくは、<a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront Goals の目標進捗と条件の概要</a>を参照してください。 </p> 
       <div> 
        <p>現在の日付までの目標の実際の進捗。次の進行状況の値と色は、目標が時間通りに達成される可能性を示します。 </p> 
        <ul> 
         <li><span>目標どおり</span>（緑のインジケーター）：目標まで時間通りに進捗しており、時間通りに達成されるでしょう。</li> 
         <li> <span>危険あり</span>（黄色のインジケーター）：目標までの進捗は予定より遅れており、時間通りに達成されない可能性があります。</li> 
         <li> <span>トラブル発生中</span>（赤いインジケーター）：目標が時間通りに達成されない危険性があります。 </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td><span>すべてのステータスの目標は、目標の整合性セクションに表示されます。</span> </td> 
     </tr> 
    </tbody> 
   </table>

   他の目標に整合させた目標は、その数が目標カードの下に表示されます。

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. 目標の下の&#x200B;**下向き矢印**&#x200B;アイコンをクリックして、子目標をさらに展開し表示します。

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >子目標を整合させた目標は、整合させた目標の数がそれぞれのカードの下に表示されます。

1. （条件付き）現在のフィルターでアラインメントに関与する一部の目標が除外されている場合は、すべての目標が表示されるというわけではないことを示す警告メッセージが表示されます。

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. 「**表示**」をクリックして、現在フィルターによって削除されている目標を表示します。

   次のようにアラインメントチャートが変更されます。

   * 以前フィルターで削除された連結目標が、アラインメントチャートに表示されるようになりました。
   * 右上隅のフィルターは黄色で囲まれていますが、これは現在適用されていないことを示しています。

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     フィルター名の左側に、フィルターを再適用リンクが表示されます。

1. （オプション）「**フィルターを再適用**」をクリックして元の結果に戻り、目標の階層を表示します。
1. （オプション）進行状況のインジケーターの上にポインタを合わせて、現在の 1 日の目標の進行状況を把握します。

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   次の情報が表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">本日時点</td> 
      <td>進捗ステータスは常に現在のものです。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>実際</span> </td> 
      <td>目標に関するすべての進捗指標を考慮して計算された、現在の日付までの目標の実際の進捗状況（パーセンテージ）。目標の進捗状況インジケーターは、目標、アクティビティおよび結果と一致します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予測</td> 
      <td> <p>目標を時間通りに達成すると仮定した、現在の日付までの目標の期待される進捗状況（パーセンテージ）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 目標カードをクリックして、目標ページを開きます。既存の目標の編集について詳しくは、[Adobe Workfront Goals で目標を編集](../../workfront-goals/goal-management/edit-goals.md)を参照してください。目標の進捗状況のアップデートについて詳しくは、[Adobe Workfront Goals で目標の進捗状況をアップデート](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md)を参照してください。

1. 現在のレベルの目標の上向き矢印をクリックして、グラフの階層の前のレベルに戻ります。

   または

   （オプション）「**目標の階層を終了**」をクリックし、現在のフィルターに一致するすべてのゴールのカードを、相互の接続を表示せずに表示します。


