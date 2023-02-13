---
product-area: reporting
navigation-topic: reporting-elements
title: 列の幅と順序を変更する
description: この記事では、列の幅のガイドラインと、Workfrontで列の幅と順序を変更する方法について説明します。
author: Lisa
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# 列の幅と順序を変更する

Adobe Workfrontでの列の幅の仕組みに関するガイドラインを次に示します。

* Workfrontは、デフォルトでリストとレポートの列の幅を定義します。
* Workfrontは、 `valueformat`列のテキストモードで特に指定されていない限り、すべてのリストおよびレポートの情報。

   >[!NOTE]
   >
   >Workfrontでは、 `valueformat` 「設定」領域と「レポート」領域で使用できるリストの情報を示します。

   この `valueformat` 値は、列に表示する情報の種類を定義します。 例えば、数値を表示する列は、「説明」フィールドを表示する列よりも狭くなります。

* 列に表示する情報の種類に応じて、Workfrontのリストとレポートの列の幅をニーズに合わせてカスタマイズできます。

   列の幅は、一時的に、リストやレポートを表示しているときに変更することも、ビュービルダーで列の幅を調整して永久的に変更することもできます。 列の幅を一時的に変更する方法については、 [列の幅と順序を一時的に変更する際の考慮事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) 」の節を参照してください。

* 組み込みビューで表示される列には、Workfrontで定義されている幅が含まれ、ハードコードされています。 これらの幅を変更するには、ビュービルダーのテキストモードを使用して、これらの列の幅を手動で更新する必要があります。

   テキストモードでの列の変更について詳しくは、 [表示：列の幅を永続的に編集する](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートのビューを編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>レポートの表示を編集するための、レポートに対する権限の管理</p> <p>ビューに対する権限を管理して編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 列の幅と順序を変更する

レポートの列の幅と順序は、次の方法で変更できます。

* [列の幅と順序を一時的に変更する](#modify-width-and-order-of-columns-temporarily)
* [列の幅と順序を恒久的に変更する](#modify-width-and-order-of-columns-permanently)

### 列の幅と順序を一時的に変更する {#modify-width-and-order-of-columns-temporarily}

列の境界線をドラッグして列のサイズを変更したり、列をドラッグ&amp;ドロップして、Workfrontサイト全体のほとんどのリストで一時的に並べ替えることができます。 これには、レポート、ビュー、ダッシュボードに関するレポート、ガントビューが含まれます。

Workfrontリストについて詳しくは、 [Adobe Workfrontのリストの概要](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [列の幅と順序を一時的に変更する際の考慮事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [列のサイズを一時的に変更する](#resize-columns-temporarily)
* [列を一時的に並べ替え](#reorder-columns-temporarily)

#### 列の幅と順序を一時的に変更する際の考慮事項 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

リスト内の列の幅と順序は、ビューを編集せずに一時的に変更できます。

列のサイズを一時的に変更して並べ替える際は、次の点に注意してください。

* 列のサイズを変更すると、新しい列のサイズはブラウザのローカルストレージに保存され、デフォルトで保存されます。 別のブラウザーを使用する場合や、キャッシュや参照データをクリアする場合は、列のサイズがデフォルトに戻ります。 ページを更新すると、列の幅に加えた変更が保持されます。
* 列を並べ替える場合、選択した順序は、リストから移動するか、ブラウザーページを更新するまで維持されません。 リストから移動したり、ブラウザーページを更新した後、列はデフォルトの順序に戻ります。
* 最適なパフォーマンスを得るために、並べ替える列のリスト項目数は 100 個以下にする必要があります。
* 列のサイズを変更すると、変更は現在使用しているビューにのみ適用され、自分だけに表示されます。 ビューを別のユーザーと共有しても、定義した列サイズは共有されません。
* 列の境界線を右にドラッグして列のサイズを変更すると、次の点を除き、隣の列の幅が保持されます。

   * 設定領域
   * レポート領域
   * ドキュメントリストとレポート

   >[!NOTE]
   >
   >リスト内で、列の左の境界線を隣の列の左の境界線よりも後に移動することはできません。

* リストをファイルにエクスポートする場合、列の一時的な順序はエクスポートされたファイルに転送されません。 エクスポートされたファイルは、列が並べ替えられる前の、元のリスト内の列の順序を表示します。

リストおよびレポートからデータをエクスポートする方法の詳細については、「 [データを書き出し](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### 列のサイズを一時的に変更する {#resize-columns-temporarily}

1. 変更するリストに移動します。
1. 列の境界線をドラッグして、目的のサイズにします。\
   ![](assets/column-resize-350x124.png)

#### 列を一時的に並べ替え {#reorder-columns-temporarily}

1. 変更するリストに移動します。
1. 別の場所に移動する列をクリックして、その列を選択します。
1. 列を正しい位置にドラッグします。
1. 列を位置にドロップして移動します。

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>これは、ガントチャートとリスト表示を同時に表示する場合に特に便利です。 ガントチャートを表示すると、列が非表示になる場合があります。 ガントチャートが表示されている間に列を表示するには、表示する列をドラッグして、ページの左側に表示します。

### 列の幅と順序を恒久的に変更する {#modify-width-and-order-of-columns-permanently}

列を永続的に並べ替えるには、「 [標準ビューの作成またはカスタマイズ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) 記事内 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

列の幅は、テキストモードを使用してのみ恒久的に変更できます。

テキストモードの使用と、列の幅の永久的な変更について詳しくは、この記事を参照してください [テキストモードの一般的な使用例の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
