---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードの概要
description: レポートやリストを構成する要素を作成する際に標準またはテキストモードのインターフェイスを使用して、Adobe Workfront でレポートやリストを作成できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 86%

---

# テキストモードの概要

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

レポートやリストを構成する要素を作成する際に標準またはテキストモードのインターフェイスを使用して、Adobe Workfront でレポートやリストを作成できます。

標準インターフェイスでは、Workfront インターフェイスですぐに利用できるフィールドとその属性を参照できます。

テキストモードを使用すると、標準モードでは利用できないかもしれないフィールドや属性を参照できますが、Workfront データベースでは利用可能です。

クラス、ビデオ、チュートリアルなど、テキストモードを使用したレポートの作成について詳しくは、Adobe Experience League サイトの学習の節を参照してください。

## テキストモードを使用する前の考慮事項

>[!TIP]
>
>カスタムフィールドのテキストモードのバージョンを使用することによって、計算カスタムフィールドの機能を拡張することもできます。計算カスタムフィールドを作成するための構文とルールは、レポートやリストで使用するものとは異なります。計算カスタムフィールドの追加について詳しくは、[ 計算フィールドのフォームへの追加 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) を参照してください。

* レポートでテキストモードの使用を開始する前に、テキストモードの言語をより深く理解するために、高度なレポートに関するクラスを受講することを強くお勧めします。
* Workfront ソフトウェアのアップデート後も作成したレポートがそのまま残るように、標準モードを使用することをお勧めします。テキストモードでは、より複雑な表示、フィルター、グループ化を作成できますが、メンテナンスがより複雑になるため、Workfront ソフトウェアの更新時に保証されません。
* 常に標準インターフェイスですべてのレポート要素を構築し、一部の調整のみテキストモードビルダーに切り替えることをお勧めします。

  >[!TIP]
  >
  >標準ビルダーを使用することで、テキストモードでコードを修正する際に使用できる、コードの重要なビルディングブロックとパターンを使用できます。

* テキストモードで正常にレポートやリストを作成するには、一連のルールと独自の構文を使用する必要があります。開始する前に、テキストモードの Workfront 構文について理解するようにしてください。

  テキストモードの構文とルールについては、[テキストモードの構文概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)を参照してください。

* テキストモードでレポート要素をカスタマイズすると、標準モード（ビュー）に戻せなくなったり、作成した要素のコードが削除されたりする場合があります（フィルターおよびグループ内）。 これは、テキストモードでサポートされるすべてのフィールドが標準モードでサポートされているわけではないからです。

## 標準モードインターフェイス

「標準モード」インターフェイスには、レポートまたはリストに表示するアプリケーション要素をマッピングするためのフィールドが表示されます。標準モードのインターフェイスは、レポートまたはリストに表示するフィールドを選択できる一、連のドロップダウンメニューです。

標準モードインターフェイスの詳細、およびレポートやリストの作成方法については、下記を参照してください。

* [カスタムレポートを作成します](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。
* [レポート要素：フィルター、ビューおよびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## テキストモードインターフェイス

テキストモードでは、標準モードインターフェイスでは使用できないフィールドを使用できるので、より複雑なビュー、フィルター、グループ化およびプロンプトを作成できます。Workfront のテキストモードは、レポートまたはリストに表示するオブジェクトを示すコード化されたステートメントの集まりです。

すべてのレポート可能なフィールドの完全なリストについては、[API エクスプローラ](../../../wf-api/general/api-explorer.md)を参照してください。

>[!NOTE]
>
>API で利用可能な一部のフィールドは、テキストモードのインターフェイスで利用できないことがあります。テキストモードのコードで正しいフィールドを使用し、期待する結果が表示されない場合、そのフィールドは API 経由でしか報告できない可能性があります。

## レポート要素へのアクセスとテキストモードの編集 {#access-reporting-elements-and-edit-text-mode}

テキストモードインターフェイスへのアクセスは、レポートやリストからビュー、グループ化、フィルターにアクセスする場合と同様です。

ビュー、フィルター、グループ化でのテキストモードの使用については、こちらを参照してください。

* [テキストモードを使用したビューの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [テキストモードを使用したフィルターの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [テキストモードを使用したグループ化の編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

カスタムプロンプトは、テキストモードでのみ編集できます。プロンプトには、レポートからのみアクセスできます。

カスタムプロンプト用のテキストモードインタフェースへのアクセスについては、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

## テキストモードを使用する一般的な理由 {#common-reasons-to-use-text-mode}

テキストモードを使用してのみ設定できるカスタムプロンプトを作成する場合を除き、Report Builder を使用して、ビュー、フィルターおよびグループ化を作成することをお勧めします。ただし、テキストモードを使用してレポートやリストの内容を強化できる場合もあります。

テキストモードの一般的な使用法について詳しくは、[テキストモードの一般的な使用法の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)を参照してください。
