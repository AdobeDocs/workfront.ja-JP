---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion の集約モジュール
description: 集積モジュールは、複数のデータバンドルを 1 つのバンドルに結合するように設計されたモジュールの一種です。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL 集約] モジュール [!DNL Adobe Workfront Fusion]

集積モジュールは、複数のデータバンドルを 1 つのバンドルに結合するように設計されたモジュールの一種です。

モジュールタイプの詳細については、 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 集約] モジュール

実行時に [!UICONTROL 集約] モジュールが実行されると、次の処理が行われます。

* 単一のソースモジュールの操作中に受け取ったすべてのバンドルを蓄積します。
* 蓄積されたバンドルごとに 1 つの項目を含む配列を持つ単一のバンドルを出力します。 配列の項目の内容は、特定の [!UICONTROL 集約] モジュールとその設定。

次の図は、 [!UICONTROL 集約] モジュール：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL ソースモジュール ]</p> </td> 
   <td> <p>バンドルの集約を開始するモジュール。 通常、ソースモジュールは、一連のバンドルを出力する反復子または検索モジュールです。 集約のソース・モジュールを設定する（および集約の設定を閉じる）と、集約の開始と終了を明確に確認できるように、ソース・モジュールと集約モジュールの間のルートが灰色の領域に囲まれます。 
   </p> <p>イテレーターの詳細については、 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] モジュール ( [!DNL Adobe Workfront Fusion]</a></p> <p>検索モジュールの詳細については、「 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">モジュールのタイプ</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Target 構造の種類 ]</p> </td> 
   <td> <p>（[!UICONTROL 配列集約 ] モジュールにのみ適用されます） データを集計するターゲット構造。 デフォルトのオプションである [!UICONTROL カスタム ] を使用すると、A[!UICONTROL Rray Aggregator] の出力バンドルに集計する項目を選択できます <code>Array </code>項目：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>[!UICONTROL 配列集約 ] モジュールの後にさらにモジュールを接続し、モジュールの設定に戻ると、[!UICONTROL Target] 構造タイプドロップダウンには、次のすべてのモジュールと、コレクションの配列のフィールドが含まれます ( [!DNL Slack] &gt;[!UICONTROL メッセージを作成 ] モジュール：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 集計フィールド ]</td> 
   <td>集約モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>集計の出力は、[!UICONTROL Group by] フィールドを使用して、複数のグループに分割できます。 [!UICONTROL Group by] フィールドには、各集約の入力バンドルに対して評価される数式を含めることができます。 次に、集約器は、個々の数式の値ごとに 1 つのバンドルを出力します。 各バンドルには、次の 2 つの項目が含まれます。</p> 
    <ul> 
     <li><code>Key </code>にはユニーク値が含まれます。</li> 
     <li><code>Array </code>には、 <code>Key </code>の値です。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>空の集計後に処理を停止</p> </td> 
   <td> <p>[!UICONTROL Aggregator] モジュールは、バンドルが [!UICONTROL Aggregator] モジュールに到達しなかった場合（バンドルが途中でフィルタリングされた場合など）でも、デフォルトで、集計の結果を出力します。 [!UICONTROL Stop processing after an empty aggregation] オプションが有効な場合、[!UICONTROL Aggregator] モジュールはこの場合、出力バンドルを生成せず、フローが停止します。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>ソースモジュールと [!UICONTROL 集約] モジュールが [!UICONTROL 集約] モジュールの後にフロー内のモジュールからアクセスできない [!UICONTROL 集約]. ソースモジュールと [!UICONTROL 集約] モジュールの場合、指定した項目を [!UICONTROL 集約] モジュールの設定 ( [!UICONTROL 集計フィールド] 設定のフィールド [!UICONTROL 配列の集約] モジュール )。


>[!INFO]
>
>**例：** 使用例：すべての電子メール添付ファイルを圧縮し、ZIP をにアップロード [!DNL Dropbox]
>
>次のシナリオに、以下の方法を示します。
>
>* 受信メールのメールボックスを監視する： [!UICONTROL 電子メール] >[!UICONTROL メールを見る] トリガーは、項目を含むバンドルを出力します `Attachments[]`：電子メールの添付ファイルをすべて含む配列。
>
>* 電子メールの添付ファイルを繰り返し処理します。 [!UICONTROL 電子メール] >[!UICONTROL 添付ファイルを繰り返し] iterator は、 `Attachments[]` 配列を 1 つずつ配列し、それらを別々のバンドルとしてさらに送信します。
>
>* が出力したバンドルを集計 [!UICONTROL 電子メール] >[!UICONTROL 添付ファイルを繰り返し] モジュール： [!UICONTROL アーカイブ] >[!UICONTROL アーカイブ集約の作成] は、受け取ったすべてのバンドルを蓄積し、ZIP ファイルを含む 1 つのバンドルを出力します。
>
>* 結果の ZIP ファイルをにアップロードします。 [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL ファイルのアップロード] は、 [!UICONTROL アーカイブ] > [!UICONTROL アーカイブの作成] をモジュール化し、にアップロードします。 [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>以下に、 [!UICONTROL アーカイブ] > [!UICONTROL アーカイブの作成] 集約：
>
>![](assets/archive-create-an-archive-350x484.png)
