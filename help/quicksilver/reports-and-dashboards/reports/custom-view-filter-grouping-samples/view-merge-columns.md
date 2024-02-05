---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：複数の列の情報を 1 つの共有列に結合」
description: 複数の異なる列に表示される情報を結合し、1 つの共有列に表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 94%

---

# 表示：複数の列の情報を 1 つの共有列に結合

<!-- Audited: 1/2024 -->

複数の異なる列に表示される情報を結合し、1 つの共有列に表示できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p> 現在： 
   <ul>
   <li>表示の変更をリクエスト</li> 
   <li>レポートを変更するためのプラン</li>
   </ul>
     </p>
     <p> 新規： 
   <ul>
   <li>ビューを変更する寄稿者</li> 
   <li>レポートを変更するための標準</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 列を共有または結合する際の考慮事項

* 隣接する 2 つの列を結合して、改行で区切られた各列の情報を表示するか、隣接する 2 つの列に情報を結合して、各列の情報を区切らずに表示できます。
* この記事で説明する同じ構文を既に共有されている列と隣接する列に適用すると、2 つ以上の列の情報を結合できます。
* `valueformat=HTML` 行は共有列で必須です。そうでない場合、レポートが Adobe Workfront から書き出される際に、列に情報が含まれません（空白になります）。
* 条件付き形式は、結合された列ではサポートされない場合があります。

  次の例外があります。

   * Workfront で情報を表示する場合、結合された列を構成する列の形式が互いに異なる場合、最初の列の形式は維持され、他のすべての列の形式は無視されます。
   * ビューを PDF ファイルに書き出す場合、条件付き形式は結合された列の最初の列に適用されます。
   * ビューを Excel ファイルに書き出す場合、結合された列は別々の列として表示されます。個々の列には、それぞれの条件付き形式ルールも表示されます。

* **viewalias** 属性を持つ列は、結合できる列の数を制限できます。これらの制限を回避するには、**viewalias** 属性の使用を回避します。列に **viewalias** 属性を含める必要がある場合、それが列の最後の項目であることを確認します。

* 共有列を含むリストを Excel またはタブ区切り形式で書き出す場合、これらの列は書き出されたファイル内に分割されます。

* いずれかの列または両方に `tile` タイプフィールドが表示されている場合、強制改行が結合された列に自動的に挿入されます。例えば、形式が適用されたテキストフィールドは `tile` タイプフィールドになります。この場合、テキストモードで列を表示すると、`type=tile` の行コードが存在します。

## 改行なしで 2 列のデータを結合

複数の異なる列のデータを結合して、各列の値の間に改行やスペースを入れずに 1 列に表示できます。

>[!TIP]
>
>同じレコードに値を同時に表示できない 2 列を結合する場合は、この方法をお勧めします。例えば、作業アイテムレポートでは、改行なしでイシュー名列およびタスク名列を結合できます。これは、作業アイテムはイシュー名とタスク名を同時に持つことができないためです。作業アイテムは、Workfront でイシューまたはタスクにすることができます。

改行のない 2 つの列のデータを結合するには、次の手順を実行します。

1. ビューのテキストモードを使用して、結合する最初の列に次のテキストを追加します。

   `sharecol=true`

   リストまたはレポートの最初の 2 列を結合する場合、Workfront は 1 列目のオブジェクトに関する情報を含むテキストの各行の前に `column.0.`、2 列目のオブジェクトに関する情報を含むテキストの各行の前に `column.1.` を付けます。

   最初の列の列番号の前に、その列の番号を付ける必要があります。列のカウントは、常に、`column.0.` のラベルの付いたリストまたはレポートの左端の列から開始します。

   複数の列を共有する場合は、各列の共有情報を含むコード行に列番号を必ず追加してください。

   **例：**&#x200B;次に、リストの 2 列目から始まる、異なる3 列を含む結合された列のテキストモードコードを示します。結合された値は、プロジェクト名、予定開始日およびプロジェクト所有者の名前で、次の 3 つの値の間に区切りはありません。

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.1.sharecol=true`

   `column.2.valuefield=plannedStartDate`

   `column.2.valueformat=atDate`

   `column.2.sharecol=true`

   `column.3.valuefield=owner:name`

   `column.3.valueformat=HTML`

![](assets/shared-column-no-line-breaks-350x142.png)

1. 「**保存**」、「**ビューを保存**」の順にクリックします。

## 改行付きの 2 列のデータを結合

複数の列のデータを結合して、1 つの共通列に表示し、各列の値を改行するには、次の手順を実行します。

1. 結合する 2 列の間に 3 つ目の列を追加します。

   >[!TIP]
   >
   >* 結合する列は、互いに隣接している必要があります。
   >* 結合する最初の列をクリックする必要があります。

1. 「**テキスト モードに切り替える**」をクリックして、手順 1 で追加した中央の列に次のコードを追加します。

   `value=<br>`

   `valueformat=HTML`

   `width=1`

   `sharecol=true`


1. 最初の列をクリックし、 **テキストモードに切り替え**&#x200B;次に、列に次のテキストを追加します。

   `sharecol=true`

   リストまたはレポートの最初の 2 列を結合する場合、Workfront は 1 列目のオブジェクトに関する情報を含むテキストの各行の前に `column.0.` を、共有情報を含む列の前に `column.1.` を、2 列目に関する情報を含むテキストの行の前に `column.2.` を付けます。

   組み合わせる列がビューの中央にある場合は、ビュー内の位置に応じて列に番号が付けられます。列のカウントは、常に、`column.0.` のラベルの付いたリストまたはレポートの左端の列から開始します。

   複数の列を共有する場合は、共有情報を含むコード行に列番号を必ず追加してください。

   **例：**&#x200B;次に、プロジェクト名、予定開始日および改行付きのプロジェクト所有者名を含む共有列のテキストモードコードを示します。共有列は、プロジェクトビューの 2 番目の列です。


   `column.1.displayname=Project_StartDate_Owner`

   `column.1.sharecol=true`

   `column.1.textmode=true`

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.2.value=<br>`

   `column.2.width=1`

   `column.2.valueformat=HTML`

   `column.2.sharecol=true`

   `column.3.valuefield=plannedStartDate`

   `column.3.valueformat=atDate`

   `column.3.sharecol=true`

   `column.4.value=<br>`

   `column.4.width=1`

   `column.4.valueformat=HTML`

   `column.4.sharecol=true`

   `column.5.textmode=true`

   `column.5.valuefield=owner:name`

   `column.5.valueformat=HTML`


   ![](assets/shared-column-with-line-breaks-350x199.png)


1. 「**保存**」、「**ビューを保存**」の順にクリックします。
