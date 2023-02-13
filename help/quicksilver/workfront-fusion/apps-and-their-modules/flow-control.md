---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion でのフロー制御
description: シナリオを作成または編集する際に、設定を構成して、シナリオ内でのデータの流れを制御できます。
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Adobe Workfront Fusion でのフロー制御

シナリオを作成または編集する際に、設定を構成して、シナリオ内でのデータの流れを制御できます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## リピーター

以下の [!UICONTROL リピーター] モジュールを使用して、指定された回数のタスクを繰り返します。 A [!UICONTROL リピーター] モジュールは、次々にバンドルを生成します。

例えば、 [!UICONTROL リピーター] モジュールを使用して、「Hello 1」、「Hello 2」などの件名を含む 5 つの E メールを送信する場合、 **[!UICONTROL 電子メール] >[!UICONTROL メールを送信]** モジュールを [!UICONTROL リピーター] モジュール。

次の手順で [!UICONTROL リピーター] モジュール：

1. 次をクリック： [!UICONTROL フロー制御] アイコン ![](assets/flow-control-icon.gif) 画面の下部で、「 **[!UICONTROL リピーター]** をクリックします。
1. 次をクリック： [!UICONTROL リピーター] バンドルを選択し、「 **[!UICONTROL 自動接続]** をクリックします。
1. 内 [!UICONTROL フロー制御] 表示されるボックスに、 **[!UICONTROL 繰り返し]** ボックス

   この電子メールの例では、「 5 」と入力します。

   ![](assets/repeater-2-350x207.png)

   項目の値は、 **[!UICONTROL 手順]** 「 」フィールドを選択します。このフィールドは、「 **[!UICONTROL 詳細設定を表示]**. この数値はデフォルトで 1 です。

1. クリック **[!UICONTROL OK]** 閉じる **[!UICONTROL フロー制御]** ボックス

1. 次に接続されているアプリまたはサービスモジュールをクリックします： [!UICONTROL リピーター] モジュール。
1. 表示されるボックスに、繰り返す情報を入力します。

   この電子メールの例では、「Hello」と入力して、 [!UICONTROL 件名] ボックス、次にマップ `i` をリピータモジュールから。

   ![](assets/repeater-3-350x207.png)

| アイテム | 説明 |
|---|---|
| [!UICONTROL 初期値] | モジュールを設定する番号を入力またはマッピングします `i` 最初の反復で デフォルト値は 1 です。 |
| [!UICONTROL 繰り返し] | モジュールの繰り返し回数を入力またはマッピングします。 この数は、0 以上 10,000 以下である必要があります。 |
| [!UICONTROL ステップ] | これは、モジュールが `i`. デフォルト値は 1 です。 |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>繰り返しの数は `i`プログラミングではループになるように このモジュールは、 [!UICONTROL 繰り返し] フィールドに入力します。 値 `i` の各反復で変更 [!DNL repeater] モジュールに追加し、後のモジュールにマッピングできます。 上記の例では、 `i` 「Hello」メッセージに入力すると、「Hello 1」、「Hello 2」などのメッセージが表示されます。

## [!UICONTROL 反復子]

An [!UICONTROL 反復子] は、配列を一連のバンドルに変換する特殊なタイプのモジュールです。 各配列項目は、 [!UICONTROL 反復子] モジュール出力。 詳しくは、 [[!UICONTROL 反復子] モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 配列の集約

配列集約は、複数のバンドルを 1 つのバンドルに結合できる特殊なタイプのモジュールです。 詳しくは、 [[!UICONTROL 集約] Adobe Workfront Fusion のモジュール](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 発送担当]

この [!UICONTROL 発送担当] モジュールを使用すると、フローを複数のルートに分岐し、各ルート内のデータを別々に処理できます。 1 回： [!UICONTROL 発送担当] モジュールはバンドルを受け取り、ルートが [!UICONTROL 発送担当] モジュール。 詳しくは、 [のルーターモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
