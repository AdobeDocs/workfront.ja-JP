---
title: レポートキャンバスでの列の可視化を設定
description: レポートキャンバスでの列の可視化を設定
hidefromtoc: true
hide: true
exl-id: 5a0cdcd4-b44b-4a63-964e-1c570cd9ff77
source-git-commit: f994a3f79df0594ea190a3dd77853c4b4ea89afb
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 100%

---

# レポートキャンバスでの列の可視化を設定

列の可視化を使用すると、垂直方向の列を使用して重要な情報をハイライト表示し、データに関するストーリーをすばやく知るのに役立ちます。

## 前提条件

開始する前に、レポートキャンバス Beta に登録する必要があります。詳しくは、[レポートキャンバス Beta：概要](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)を参照してください。

## 列の可視化の設定

>[!TIP]
>
>レポートのブロックを作成および編集すると、すべての変更が自動的に保存されます。

1. 最初に、**列**&#x200B;の可視化タイプを備えた可視化ブロックをレポートに追加します。詳しくは、[レポートキャンバスでの視覚化ブロックの追加または編集](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md)を参照してください。

1. ビジュアライゼーションの右上隅にあるビジュアライゼーションの編集アイコン ![](assets/edit-icon.png) をクリックし、次のいずれかの操作を実行します。

   1. 「**設定**」タブ：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">ビジュアライゼーションタイプ</td>
         <td><p>別のタイプのビジュアライゼーションに切り替えます。これを行うと、その後のメニューのオプションが変更される可能性があります。</p></td>
        </tr>
        <tr>
         <td role="rowheader">水平軸</td>
         <td><p>列の可視化の水平または X 軸に沿って表現するデータを選択します。可視化では、縦軸の各項目に従って、この軸の項目が比較されます。</p></td>
        </tr>
        <tr>
         <td role="rowheader">垂直軸</td>
         <td><p>左のドロップダウンメニューで、水平または Y 軸に沿って表現するデータを選択します。可視化では、この軸の項目が、値に基づいて比較対象の列として表示されます。</p><p>右側のドロップダウンメニューで、これらの値をディスプレイで計算する方法を選択します。</p>
          <ul>
           <li><p><b>カウント</b>：値の数</p></li>
           <li><p><b>合計</b>：すべての値の合計 </p></li>
           <li><p><b>平均</b>：すべての値の平均</p></li>
           <li><p><b>最小</b>：最小値のみ</p></li>
           <li><p><b>最大</b>：最大値のみ</p></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

   1. **データ**&#x200B;タブ上：

      | データソース（ドロップダウンメニュー） | ビジュアライゼーションのデータソースをレポートキャンバス上の別のテーブルに変更します。 |
      |---|---|
      | データソースを表示 | レポートキャンバスにビジュアライゼーションのソーステーブルを表示するにはこのオプションを有効にし、非表示にするにはオプションを無効にします。 |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. ビジュアライゼーション設定メニューの外側をクリックして閉じます。
