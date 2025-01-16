---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion のアグリゲータモジュール
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 60%

---

# [!UICONTROL [!DNL Adobe Workfront Fusion] でのアグリゲーター]モジュール

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [Aggregator モジュール ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/aggregator-module.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

アグリゲーターモジュールは、複数のデータバンドルを 1 つのバンドルに結合するように設計されたモジュールの一種です。

モジュールの種類について詳しくは、[モジュールの種類](../../workfront-fusion/modules/module-types.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

+++

## [!UICONTROL Aggregator] モジュールの概要

[!UICONTROL アグリゲーター]モジュールが実行されると、次の処理が行われます。

* 単一のソースモジュールの操作中に受け取ったすべてのバンドルを蓄積します。
* 蓄積された各バンドルごとに 1 つの項目を含む配列を持つ単一のバンドルを出力します。配列の項目の内容は、特定の[!UICONTROL アグリゲーター]モジュールとその設定によって異なります。

次の画像は、[!UICONTROL アグリゲーター]モジュールの通常の設定を表示します。

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source Module]</p> </td> 
   <td> <p>バンドル集計が開始するモジュール。 ソースモジュールは、通常、一連のバンドルを出力するイテレータまたは検索モジュールです。</p><p>アグリゲーターのソースモジュールを設定する（およびアグリゲーターの設定を閉じる）と、集計の開始と終了を明確に確認できるように、ソースモジュールおよびアグリゲーターモジュール間のルートがグレーのエリアでラップされます。 
   </p> <p>イテレーターについて詳しくは、<a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> の [!UICONTROL Iterator] モジュールを参照してください。</p> <p>検索モジュールについて詳しくは、<a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">モジュールの種類</a>でのモジュールの検索を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>（[!UICONTROL 配列アグリゲータ ] モジュールにのみ適用） データが集計されるターゲット構造。 デフォルトのオプション [!UICONTROL Custom] を使用すると、[!UICONTROL Array aggregator] の出力バンドルの <code>Array </code>item：に集計する項目を選択できます。</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>[!UICONTROL 配列 aggregator] モジュールの後にさらにモジュールを接続し、モジュールの設定に戻ると、[!UICONTROL Target] 構造体型ドロップダウンメニューには、[!DNL Slack] &gt;[!UICONTROL メッセージの作成 ] モジュールの [!UICONTROL 添付ファイル ] フィールドに表示されるように、次のすべてのモジュールと、「コレクションの配列」型のフィールドが含まれます。</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>集計モジュールの出力に含めるフィールド。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>アグリゲーターの出力は、[!UICONTROL Group by] フィールドの助けを借りて、複数のグループに分割できます。[!UICONTROL Group by] フィールドには、各アグリゲーターの入力バンドルについて評価される式を含めることができます。次に、アグリゲーターは、個々の明確な数式の値ごとに 1 つのバンドルを出力します。各バンドルには、次の 2 つの項目が含まれます。</p> 
    <ul> 
     <li><code>Key </code>特定の値が含まれます。</li> 
     <li><code>Array </code>式が <code>Key </code> 値に評価されたバンドルからの集計データが含まれます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>空の集計後に処理を停止</p> </td> 
   <td> <p>[!UICONTROL Aggregator] モジュールは、バンドルが [!UICONTROL Aggregator] モジュールに到達しなかった場合でも（途中でバンドルがすべてフィルタリングされた場合など）、デフォルトで集計の結果を出力します。[!UICONTROL Stop processing after an empty aggregation] オプションが有効だと、この場合は [!UICONTROL Aggregator] モジュールが出力バンドルを生成せず、フローが停止します。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>ソースモジュールと[!UICONTROL アグリゲーター]モジュールの間にあるモジュールによって生成されたバンドルは、[!UICONTROL アグリゲーター]モジュールによって出力されないため、[!UICONTROL アグリゲーター]の後のフローでモジュールがアクセスできません。ソースモジュールと[!UICONTROL アグリゲーター]モジュールの間にあるモジュールによって出力されたバンドルのデータが必要な場合は、指定した項目を[!UICONTROL アグリゲーター]モジュールの設定に必ず含めます（[!UICONTROL 配列アグリゲーター]モジュールの設定の「[!UICONTROL 集計フィールド]」フィールドと同様）。


## アグリゲータの動作のシナリオの例

このサンプルシナリオでは、すべてのメール添付ファイルを zip で圧縮し、その ZIP ファイルを [!DNL Dropbox] にアップロードする方法を示します。

![](assets/dropbox-archive-350x87.png)

以下のシナリオでは、次の方法を示します。

* 最初のモジュールは、受信メールのメールボックスを監視します。[!UICONTROL Email] >[!UICONTROL Watch emails] トリガーは、アイテム `Attachments[]` を含むバンドルを出力します。これは、メールのすべての添付ファイルを含む配列です。

* 2 つ目のモデルは、メールの添付ファイルを反復します。[!UICONTROL  メール ] >[!UICONTROL  添付ファイルを反復 ] イテレータは、`Attachments[]` 配列から項目を 1 つずつ取得し、それらを別のバンドルとしてさらに送信します。

* 3 番目のモジュールは、[!UICONTROL Email] >[!UICONTROL Iterate attachments] モジュールによって出力されたバンドルを集計します。[!UICONTROL Archive] >[!UICONTROL Create an archive aggregator] 受信したすべてのバンドルを蓄積し、ZIP ファイルを含む単一のバンドルを出力します。

* 最後のモジュールは、結果の ZIP ファイルを [!DNL Dropbox] にアップロードします。[!DNL Dropbox]/[!UICONTROL  ファイルをアップロード ][!UICONTROL  アーカイブ ]/[!UICONTROL  アーカイブを作成 ] モジュールから ZIP ファイルを取得し、[!DNL Dropbox] にアップロードします。



以下に、[!UICONTROL アーカイブ]／[!UICONTROL アーカイブを作成]アグリゲーターの設定例を示します。

![](assets/archive-create-an-archive-350x484.png)
