---
title: レポートキャンバスでの円グラフビジュアライゼーションの設定
description: レポートキャンバスでの円グラフビジュアライゼーションの設定
hidefromtoc: true
hide: true
exl-id: 0497edb5-9322-406a-b53b-ec498afdd96e
source-git-commit: f994a3f79df0594ea190a3dd77853c4b4ea89afb
workflow-type: ht
source-wordcount: '289'
ht-degree: 100%

---

# レポートキャンバスでの円グラフビジュアライゼーションの設定

円グラフのビジュアライゼーションを使用すると、相対比率を示すウェッジの付いた円形のグラフィックで重要な情報をハイライト表示することで、データに関するストーリーをすばやく示すことができます。

## 前提条件

開始する前に、レポートキャンバス Beta に登録する必要があります。詳しくは、[レポートキャンバス Beta：概要](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)を参照してください。

## 円グラフのビジュアライゼーションを設定

>[!TIP]
>
>レポートのブロックを作成および編集すると、すべての変更が自動的に保存されます。

1. まず、[レポートキャンバスでのビジュアライゼーションブロックの追加または編集](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md)の説明に従って、**円グラフ**&#x200B;ビジュアライゼーションタイプのビジュアライゼーションブロックをレポートに追加します。

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
         <td role="rowheader">ウェッジ</td>
         <td>個々のウェッジが表すデータを選択します。</td>
        </tr>
        <tr>
         <td role="rowheader">値</td>
         <td><p>左のドロップダウンメニューで、各ウェッジに表示する値を選択します。</p><p>右側のドロップダウンメニューで、これらの値をディスプレイで計算する方法を選択します。</p>
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
