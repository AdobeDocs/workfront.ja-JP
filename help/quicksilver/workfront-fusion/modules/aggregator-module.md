---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion のアグリゲータモジュール
description: アグリゲーターモジュールは、複数のデータバンドルを 1 つのバンドルに結合するように設計されたモジュールの一種です。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '800'
ht-degree: 100%

---

# [!UICONTROL [!DNL Adobe Workfront Fusion] でのアグリゲーター]モジュール

アグリゲーターモジュールは、複数のデータバンドルを 1 つのバンドルに結合するように設計されたモジュールの一種です。

モジュールの種類について詳しくは、[モジュールの種類](../../workfront-fusion/modules/module-types.md)を参照してください。

## アクセス要件

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select]または[!UICONTROL Prime]の [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL アグリゲーター]モジュール

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
   <td> <p>モジュールは、バンドルの集計を開始します。通常、ソースモジュールは、一連のバンドルを出力するイテレーターまたは検索モジュールです。アグリゲーターのソースモジュールを設定する（およびアグリゲーターの設定を閉じる）と、集計の開始と終了を明確に確認できるように、ソースモジュールおよびアグリゲーターモジュール間のルートがグレーのエリアでラップされます。 
   </p> <p>イテレーターについて詳しくは、<a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> の [!UICONTROL Iterator] モジュールを参照してください。</p> <p>検索モジュールについて詳しくは、<a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">モジュールの種類</a>でのモジュールの検索を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target structure type]</p> </td> 
   <td> <p>（[!UICONTROL Array aggregator] モジュールにのみ適用されます。）データはターゲット構造に集計されます。デフォルトのオプションである [!UICONTROL Custom] を使用すると、[!UICONTROL Array Aggregator] の出力バンドルの <code>Array </code> 項目に集計される項目を選択できます。</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>[!UICONTROL Array aggregator] モジュールの後にさらにモジュールを接続し、モジュールの設定に戻ると、[!DNL Slack] の [!UICONTROL Attachments] フィールド／[!UICONTROL Create a Message] モジュールに示すように、[!UICONTROL Target] 構造タイプドロップダウンには、コレクションの配列タイプである次のモジュールとそのフィールドがすべて含まれます。</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td>アグリゲーターモジュールの出力に含めるフィールドを選択します。</td> 
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


>[!INFO]
>
>**例：**&#x200B;ユースケース：すべてのメール添付ファイルを圧縮し、その ZIP ファイルを [!DNL Dropbox] にアップロードします
>
>以下のシナリオでは、次の方法を示します。
>
>* 受信メール用のメールボックスを監視：[!UICONTROL メール]／[!UICONTROL メールを監視]トリガーは、メールのすべての添付ファイルをすべて含む配列である、`Attachments[]` 項目を含むバンドルを出力します。
>
>* メールの添付ファイルを反復：[!UICONTROL メール]／[!UICONTROL 添付ファイルを反復]イテレーターは、`Attachments[]` 配列の項目を 1 つずつ取得し、それらをさらに別々のバンドルとして送信します。
>
>* [!UICONTROL メール]／[!UICONTROL 添付ファイルを反復]モジュールによって出力されたバンドルを集約：[!UICONTROL アーカイブ]／[!UICONTROL アーカイブの集約の作成]は、受け取ったすべてのバンドルを蓄積し、ZIP ファイルを含む単一のバンドルを出力します。
>
>* 結果の ZIP ファイルを [!DNL Dropbox] にアップロード：[!DNL Dropbox]／[!UICONTROL ファイルをアップロード]は ZIP ファイルを[!UICONTROL アーカイブ]／[!UICONTROL アーカイブを作成]モジュールから取得し、[!DNL Dropbox] にアップロードします。
>
>![](assets/dropbox-archive-350x87.png)
>
>以下に、[!UICONTROL アーカイブ]／[!UICONTROL アーカイブを作成]アグリゲーターの設定例を示します。
>
>![](assets/archive-create-an-archive-350x484.png)
