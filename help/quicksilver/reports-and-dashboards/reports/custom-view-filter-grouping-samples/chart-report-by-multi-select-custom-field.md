---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 複数選択カスタムフィールドを使用したレポートのチャート化
description: 複数選択カスタムフィールドで選択した選択肢を取り込む追加の計算フィールドを作成した後でのみ、複数選択カスタムフィールドでレポートのグラフを作成できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: a2f0ef565b0f0dbcfec7f3f5b5fece4c7b4b1ec6
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 49%

---

# 複数選択カスタムフィールドを使用したレポートのチャート化

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

複数選択カスタムフィールドを使用してグラフを作成するのではなく、複数選択カスタムフィールドの各オプションに対して個別のフィールドを作成することをお勧めします。

複数選択カスタムフィールドの例は、次のとおりです。

* チェックボックス
* 複数選択ドロップダウンメニュー

テキストモードの使用について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)の記事を参照してください。

ただし、複数選択フィールドの各オプションに個別のフィールドを指定できない場合は、計算カスタムフィールドを使用して、複数選択フィールドから選択をグループ化し、複数選択フィールドでレポートをグラフ化できます。 その後、計算フィールド別にレポートのグラフを表示できます。

>[!NOTE]
>
>選択したいずれかの選択肢を持つ項目は、1 回だけカウントされます。
>
>たとえば、選択肢 1 と選択肢 2 をオプションとして持つチェックボックスカスタムフィールドがあり、フォームをタスクに添付すると、選択肢 1 と選択肢 2 の両方を持つタスクは、選択肢 1 と選択肢 2 のみを持つタスクとは別のグラフ要素に表示されます。
>
>選択肢 1 が選択されたタスクは、選択肢 1 と選択肢 2 が選択されたタスクと同じグラフ要素に表示されません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

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

複数選択のカスタムフィールドを参照する計算フィールドを作成するには、次の前提条件が満たされている必要があります。

* カスタムフォーム内の複数選択カスタムフィールド。\
  カスタムフォームの作成と、カスタムフォームへのカスタムフィールドの追加について詳しくは、[カスタムフォームを作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)の記事を参照してください。

* 複数選択カスタムフィールドがオブジェクトに添付されたカスタムフォーム。
* 各オブジェクトの複数選択カスタムフィールドの値。

複数選択カスタムフィールドを参照する計算カスタムフィールドを作成するには、以下のように行います。

1. カスタムフォームを作成するか、既存のフォームを編集します。

   カスタムフォームの作成については、[カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

1. カスタムフォームで使用する 1 つ以上のオブジェクトを選択します。
1. クリック **フィールドを追加**&#x200B;を、 **計算済み** 複数選択カスタムフィールドをフォームに追加する場合。

1. 「**ラベル**」ボックスで、新しい計算フィールドに名前を付け、複数選択カスタムフィールドを参照することを示します。

   例：「計算された複数選択フィールド」。

1. 「**計算**」ボックスに、以下のコードを入力します。

   `{DE:Multi-select Custom Field}`

   これにより、複数選択カスタムフィールドで選択した選択肢が計算カスタムフィールドに追加されます。 例えば、フォームがタスクに添付され、複数選択カスタムフィールドから選択 1 が選択された場合、計算カスタムフィールドには「選択 1」という値が表示されます。 別のタスクで選択 1 と選択 2 を選択した場合は、計算されたカスタムフィールドに「選択 1、選択 2」という値が表示されます。

1. 「複数選択カスタムフィールド」を、Workfront に表示される複数選択カスタムフィールドの実際の名前に置き換えます。

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （オプション）複数選択カスタムフィールドが既にこのフォームに存在し、このフォームが既にオブジェクトに添付されている場合は、 **以前の計算を（バックグラウンドで）更新する** オプション。

   これにより、複数選択カスタムフィールドの値が、既にオブジェクトに添付されているフォームに追加されるので、新しい計算フィールドに自動的に入力されます。

1. 「**完了**」をクリックします。
1. 「**保存して閉じる**」をクリックします。

   計算されたカスタムフィールドがカスタムフォームに追加されます。現在フォームがオブジェクトに添付されている場合は、複数選択カスタムフィールドの情報がフィールドに入力されます。

### 計算カスタムフィールドを参照するチャートの作成 {#build-a-chart-that-references-a-calculated-custom-field}

1. （オプション）グラフに表示するすべての計算フィールドに値を入力するには、レポートの「詳細」タブで、複数選択カスタムフィールドと計算カスタムフィールドの両方を持つカスタムフォームを含むすべてのオブジェクトを選択し、 **編集**.
1. （オプションおよび条件付き） **カスタム式の再計算** 「 」フィールドで「 」をクリックし、 **変更を保存**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >このオプションは、プロジェクトを一括編集する際には使用できなくなりました。プロジェクトリストの上部にある&#x200B;**その他**&#x200B;アイコン![](assets/more-icon-45x33.png)をクリックし、「**式の再計算**」をクリックすると、プロジェクトの式を一括で再計算することができます。

1. 複数選択カスタムフィールドを参照する計算フィールドのチャートを追加するレポートに移動します。
1. 「**レポートアクション**」、「**編集**」の順にクリックします。

1. 「<strong>グループ化</strong>」タブを選択して、「<strong>グループを追加</strong>」をクリックします。
1. 次を追加： <strong>計算された複数選択フィールド</strong> をグループ化として作成しました。
1. 「<strong>グラフ</strong>」タブを選択し、レポートにグラフを追加します。

   例えば、 **列** グラフ。
   <br>レポートへのグラフの追加について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>の記事の<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">レポートへのグラフの追加</a>の節を参照してください。
1. Adobe Analytics の **下 (X) 軸** フィールドで、 <strong>計算された複数選択フィールド</strong> をクリックしてグラフに表示します。
1. 「<strong>保存して閉じる</strong>」をクリックします。

   レポートには、計算された複数選択フィールドでグループ化された結果がグラフに表示されます。

   ![](assets/chart-multi-select-field-column-chart-example.png)