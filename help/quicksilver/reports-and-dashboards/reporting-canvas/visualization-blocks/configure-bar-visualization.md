---
title: レポートキャンバスでの棒グラフビジュアライゼーションの設定
description: レポートキャンバスでの棒グラフビジュアライゼーションの設定
author: Nolan
feature: Reports and Dashboards
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---


# レポートキャンバスでの棒グラフビジュアライゼーションの設定

棒グラフのビジュアライゼーションを使用すると、横棒グラフを使用して重要な情報をハイライト表示し、データに関するストーリーをすばやく知るのに役立ちます。

## 前提条件

開始する前に、レポートキャンバスベータ版に登録する必要があります。 詳しくは、 [レポートキャンバスベータ版：概要](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 棒グラフのビジュアライゼーションの設定

>[!NOTE]
>
>レポートのブロックを作成および編集すると、すべての変更が自動的に保存されます。

1. 最初に、 **棒グラフ** ビジュアライゼーションタイプをレポートに追加できます。詳しくは、 [レポートキャンバスでのビジュアライゼーションブロックの追加または編集](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. ビジュアライゼーションを編集アイコンをクリックします。 ![](assets/edit-icon.png) ビジュアライゼーションの右上隅で、次のいずれかの操作をおこないます。

   1. 次の日： **設定** タブ：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">ビジュアライゼーションタイプ</td>
         <td><p>別のタイプのビジュアライゼーションに切り替えます。 この場合、メニューの後続のオプションが変わる場合があります。</p></td>
        </tr>
        <tr>
         <td role="rowheader">垂直軸</td>
         <td><p>バービジュアライゼーションの縦の左端または Y 軸に沿って表現するデータを選択します。 ビジュアライゼーションでは、横軸の各項目に従って、この軸の項目が比較されます。</p></td>
        </tr>
        <tr>
         <td role="rowheader">水平軸</td>
         <td><p>左のドロップダウンメニューで、水平または X 軸に沿って表現するデータを選択します。 この軸の項目は、値に基づいて比較バーとして表示されます。</p><p>右側のドロップダウンメニューで、ビジュアライゼーションで計算し、横軸に沿って値を表示する方法を選択します。</p>
          <ul>
           <li><p><b>カウント</b>：値の数</p></li>
           <li><p><b>合計</b>：すべての値の合計 </p></li>
           <li><p><b>平均</b>：すべての値の平均</p></li>
           <li><p><b>最小</b>：最も小さい値のみ</p></li>
           <li><p><b>最大</b>：最も大きい値のみ</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ 値を追加</td>
         <td>水平軸に沿って追跡する別のフィールドを追加します。</td>
        </tr>
       </tbody>
      </table>

   1. 次の日： **データ** タブ：

      | データソース（ドロップダウンメニュー） | ビジュアライゼーションのデータソースをレポートキャンバス上の別のテーブルに変更します。 |
      |---|---|
      | データソースを表示 | このオプションを有効にすると、レポートキャンバスにビジュアライゼーションのソーステーブルが表示されます。または、このオプションを無効にすると非表示になります。 |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. ビジュアライゼーション設定メニューの外側の任意の場所をクリックして、それを閉じます。
