---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 複数選択のカスタムフィールドによるレポートのグラフ化
description: 複数選択カスタムフィールドで選択した選択肢を取り込む追加の計算フィールドを作成した後でのみ、複数選択カスタムフィールドでレポートのグラフを作成できます。
author: Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 82%

---

# 複数選択カスタムフィールドを使用したレポートのチャート化

<!--Audited: 11/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

複数選択カスタムフィールドを使用してグラフを作成するのではなく、複数選択カスタムフィールドの各オプションに対して別々のフィールドを作成することをお勧めします。

複数選択カスタムフィールドの例は、次のとおりです。

* チェックボックス
* 複数選択ドロップダウンメニュー

テキストモードの使用について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)の記事を参照してください。

ただし、複数選択フィールドの各オプションに個別のフィールドを指定できない場合は、計算済みカスタムフィールドを使用して、複数選択フィールドから選択肢をまずグループ化すると、複数選択フィールドでレポートをグラフ化できます。その後、計算フィールド別にレポートのグラフを表示できます。

>[!NOTE]
>
>いずれかの選択肢が選択された項目は、1 回だけカウントされます。
>
>たとえば、あるチェックボックスカスタムフィールドにオプションとして選択肢 1 と選択肢 2 があり、そのフォームをタスクに添付すると、選択肢 1 と選択肢 2 の両方を持つタスクは、選択肢 1 または選択肢 2 のいずれかのみが選択されたタスクとは別のグラフ要素に表示されます。
>
>選択肢 1 が選択されたタスクは、選択肢 1 と選択肢 2 が選択されたタスクと同じグラフ要素に表示されません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 前提条件

開始する前に、複数選択カスタムフィールドで選択した値を表示する計算カスタムフィールドを作成する必要があります。詳しくは、この記事にある[複数選択カスタムフィールドを参照する計算カスタムフィールドの作成](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)の節を参照してください。

## 複数選択カスタムフィールドを使用したレポートのチャート化

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

複数選択カスタムフィールドを参照して、レポート内にチャートを作成することはできません。その代わり、特定のオブジェクトの複数選択カスタムフィールドの値を記録する計算フィールドを作成し、計算フィールドごとにグループ化することができます。 

* [複数選択カスタムフィールドを参照する計算カスタムフィールドの作成](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [計算カスタムフィールドを参照するチャートの作成](#build-a-chart-that-references-a-calculated-custom-field)

### 複数選択カスタムフィールドを参照する計算カスタムフィールドの作成 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

複数選択カスタムフィールドを参照する計算フィールドを作成するには、以下の前提条件が満たされている必要があります。

* カスタムフォームの複数選択カスタムフィールド\
  カスタムフォームの作成と、カスタムフォームへのカスタムフィールドの追加について詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

* 複数選択カスタムフィールドがオブジェクトに添付されたカスタムフォーム。
* 各オブジェクトの複数選択カスタムフィールドの値。

複数選択カスタムフィールドを参照する計算カスタムフィールドを作成するには、以下のように行います。

1. カスタムフォームを作成するか、既存のフォームを編集します。

   カスタムフォームの作成について詳しくは、「[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

1. カスタムフォームで使用する 1 つ以上のオブジェクトを選択します。
1. **フィールドを追加**／**計算**&#x200B;をクリックして、複数選択カスタムフィールドをフォームに追加します。

1. 「**ラベル**」ボックスで、新しい計算フィールドに名前を付け、複数選択カスタムフィールドを参照することを示します。

   例：「計算複数選択フィールド」

1. 「**計算**」ボックスに、以下のコードを入力します。

   `{DE:Multi-select Custom Field}`

   これにより、複数選択カスタムフィールドで選択した選択肢が計算済みカスタムフィールドに追加されます。例えば、フォームがタスクに添付され、複数選択カスタムフィールドから選択肢 1 が選択された場合、計算済みカスタムフィールドには「選択肢 1」という値が表示されます。別のタスクで選択肢 1 と選択肢 2 を選択した場合は、計算済みカスタムフィールドに「選択肢 1、選択肢 2」という値が表示されます。

1. 「複数選択カスタムフィールド」を、Workfront に表示される複数選択カスタムフィールドの実際の名前に置き換えます。

   ![&#x200B; 計算複数選択カスタムフィールド &#x200B;](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （オプション）複数選択のカスタムフィールドがこのフォームに既に存在し、このフォームが既にオブジェクトに添付されている場合は、「**既存の計算に適用**」オプションを有効にします。

   これにより新しい計算フィールドには、既にオブジェクトに添付されているフォームに追加された複数選択カスタムフィールドの値がそのまま自動的に入力されるようになります。

1. 「**適用**」をクリックします。
1. 「**保存して閉じる**」をクリックします。

   計算済みカスタムフィールドがカスタムフォームに追加されます。現在フォームがオブジェクトに添付されている場合は、複数選択カスタムフィールドの情報がフィールドに入力されます。

### 計算カスタムフィールドを参照するチャートの作成 {#build-a-chart-that-references-a-calculated-custom-field}

1. （オプション）グラフで表示したいすべての計算フィールドに値が入力されるようにするには、レポートの「詳細」タブで、複数選択カスタムフィールドと計算済みカスタムフィールドの両方を含むオブジェクトをすべて選択して、「**編集**」をクリックします。
1. （オプションおよび条件付き）「**カスタム式の再計算**」フィールドを有効にし、次に「**変更を保存**」をクリックします。\
   ![&#x200B; カスタム式の再計算 &#x200B;](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >このオプションは、プロジェクトを一括編集する際には使用できなくなりました。プロジェクトリストの上部にある **その他** アイコン ![&#x200B; その他のアイコン &#x200B;](assets/more-icon-45x33.png) をクリックしてから、「式を再計算 **をクリックすると、プロジェクトの式を一括で再計算** ることができます。

1. 複数選択カスタムフィールドを参照する計算フィールドのチャートを追加するレポートに移動します。
1. 「**レポートアクション**」、「**編集**」の順にクリックします。

1. 「<strong>グループ化</strong>」タブを選択して、「<strong>グループを追加</strong>」をクリックします。
1. グループ化として作成した <strong> 計算複数選択フィールド </strong> を追加します。
1. 「<strong>グラフ</strong>」タブを選択し、レポートにグラフを追加します。

   例えば、**列**&#x200B;のグラフを選択します。
   <br>レポートへのグラフの追加について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>の記事の<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">レポートへのグラフの追加</a>の節を参照してください。
1. **下（X）軸** フィールドで、グラフに表示する <strong> 計算複数選択フィールド </strong> を選択します。
1. 「<strong>保存して閉じる</strong>」をクリックします。

   レポートは、複数選択の計算フィールドでグループ化された結果をグラフで表示します。

   ![&#x200B; グラフの複数選択フィールド &#x200B;](assets/chart-multi-select-field-column-chart-example.png)
