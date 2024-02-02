---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion でのフロー制御
description: シナリオを作成または編集する際、シナリオ内でのデータの流れを制御する設定を行うことができます。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '637'
ht-degree: 100%

---

# Adobe Workfront Fusion でのフロー制御

シナリオを作成または編集する際、シナリオ内でのデータの流れを制御する設定を行うことができます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランの場合、この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## リピーター

[!UICONTROL リピーター]モジュールを使用すると、タスクを指定した回数繰り返すことができます。[!UICONTROL リピーター]モジュールは、次々にバンドルを生成します。

例えば、[!UICONTROL リピーター]モジュールを使用して「こんにちは 1」、「こんにちは 2」などの件名のメールを 5 通送信するには、**[!UICONTROL メール]／[!UICONTROL 自分にメール]**&#x200B;モジュールを[!UICONTROL リピーター]モジュールに接続します。

[!UICONTROL リピーター]モジュールを使用するには：

1. 画面の下部の[!UICONTROL フロー制御]アイコン ![](assets/flow-control-icon.gif) をクリックし、表示されるメニューで「**[!UICONTROL リピーター]**」をクリックします。
1. [!UICONTROL リピーター]バンドルをクリックし、表示されるボックスで「**[!UICONTROL 自動的に接続]**」をクリックします。
1. 表示される[!UICONTROL フロー制御]ボックスで、**[!UICONTROL 繰り返し]**&#x200B;ボックスに必要な繰り返し（出力バンドル）の回数を入力します。

   ここでのメールの例では、「5」と入力します。

   ![](assets/repeater-2-350x207.png)

   アイテムの値は、繰り返されるごとに、**[!UICONTROL ステップ]**&#x200B;フィールドで指定したこの数ずつ増加します。この値は、**[!UICONTROL 詳細設定を表示]**&#x200B;を選択すると表示できます。この数値は、デフォルトでは 1 です。

1. 「**[!UICONTROL OK]**」をクリックして、**[!UICONTROL フロー制御]**&#x200B;ボックスを閉じます。

1. [!UICONTROL リピーター]モジュールに接続されているアプリまたはサービスモジュールをクリックします。
1. 表示されるボックスに、繰り返す情報を入力します。

   ここでのメールの例では、[!UICONTROL 件名]ボックスに「こんにちは」と入力し、リピーターモジュールから `i` をマッピングします。

   ![](assets/repeater-3-350x207.png)

| 項目 | 説明 |
|---|---|
| [!UICONTROL 初期値] | 最初の繰り返しでモジュールが `i` として設定する数値を入力またはマッピングします。デフォルト値は 1 です。 |
| [!UICONTROL 繰り返し] | モジュールが繰り返す回数を入力またはマッピングします。この数は、0 以上 10,000 以下である必要があります。 |
| [!UICONTROL ステップ] | モジュールは、`i` の値を、この数だけ増分します。デフォルト値は 1 です。 |

{style="table-layout:auto"}

>[!NOTE]
>
>繰り返し回数は、プログラミングのループとは異なり、`i` の値によって決まるわけではありません。モジュールは、[!UICONTROL 繰り返し]フィールドに指定された回数だけ繰り返します。値 `i` は [!DNL repeater] モジュールのイテレーションごとに変化し、後のモジュールにマッピングできます。ここでの例では、`i` の値を「こんにちは」メッセージにマッピングすると、「こんにちは 1」、「こんにちは 2」などのメッセージが表示されます。

## [!UICONTROL イテレーター]

[!UICONTROL イテレーター]は、配列を一連のバンドルに変換する特別なタイプのモジュールです。配列の各項目は、[!UICONTROL イテレーター]モジュールの出力では個別のバンドルになります。詳しくは、[[!UICONTROL  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) のイテレーター]モジュールを参照してください。

## 配列アグリゲーター

配列アグリゲーターは、複数のバンドルを 1 つのバンドルに結合できる特別なタイプのモジュールです。詳しくは、[[!UICONTROL Adobe Workfront Fusion のアグリゲーター]モジュール](../../workfront-fusion/modules/aggregator-module.md)を参照してください。

## [!UICONTROL ルーター]

[!UICONTROL ルーター]モジュールを使用すると、フローを複数のルートに分岐し、データを各ルートで別々に処理できます。[!UICONTROL ルーター]モジュールはバンドルを受け取ると、ルートが[!UICONTROL ルーター]モジュールに接続された順序で、接続されている各ルートにバンドルを転送します。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md) のルーターモジュールを参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
