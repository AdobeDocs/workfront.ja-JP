---
title: レポートキャンバスでの円グラフのビジュアライゼーションの設定
description: レポートキャンバスでの円グラフのビジュアライゼーションの設定
author: Nolan
feature: Reports and Dashboards
exl-id: 0497edb5-9322-406a-b53b-ec498afdd96e
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 1%

---


# レポートキャンバスでの円グラフのビジュアライゼーションの設定

円グラフのビジュアライゼーションを使用すると、相対的な比率を示すくさび付きの円形のグラフィックで重要な情報をハイライト表示し、データに関するストーリーをすばやく示すことができます。

## 前提条件

開始する前に、レポートキャンバスベータ版に登録する必要があります。 詳しくは、 [レポートキャンバスベータ版：概要](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 円グラフのビジュアライゼーションの設定

>[!TIP]
>
>レポートのブロックを作成および編集すると、すべての変更が自動的に保存されます。

1. 最初に、 **円グラフ** ビジュアライゼーションタイプをレポートに追加できます。詳しくは、 [レポートキャンバスでのビジュアライゼーションブロックの追加または編集](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

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
         <td role="rowheader">ウェッジ</td>
         <td>個々のウェッジを表すデータを選択します。</td>
        </tr>
        <tr>
         <td role="rowheader">値</td>
         <td><p>左のドロップダウンメニューで、各ウェッジに表示する値を選択します。</p><p>右側のドロップダウンメニューで、これらの値をディスプレイで計算する方法を選択します。</p>
          <ul>
           <li><p><b>カウント</b>：値の数</p></li>
           <li><p><b>合計</b>：すべての値の合計 </p></li>
           <li><p><b>平均</b>：すべての値の平均</p></li>
           <li><p><b>最小</b>：最も小さい値のみ</p></li>
           <li><p><b>最大</b>：最も大きい値のみ</p></li>
          </ul></td>
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
