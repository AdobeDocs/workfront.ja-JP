---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion の Iterator モジュール
description: Iterator モジュールは、配列を一連のバンドルに変換する特殊なタイプのモジュールです。 各配列項目は、別々のバンドルとして出力されます。
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# [!UICONTROL 反復子] モジュール [!DNL Adobe Workfront Fusion]

An [!UICONTROL 反復子] モジュールは、配列を一連のバンドルに変換する特殊なタイプのモジュールです。 各配列項目は、別々のバンドルとして出力されます。

詳しくは、 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md) および [Adobe Workfront Fusion で配列をマッピングする](../../workfront-fusion/mapping/map-an-array.md).

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明する機能を使用するには、Adobe Workfront Fusion とAdobe Workfrontを購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 反復子] モジュール構成

次の項目を設定しました。 [!UICONTROL 反復子] モジュールは、他のモジュールの設定と同じです。 この [!UICONTROL 配列] フィールドには、変換または分割する別々のバンドルの配列が含まれます。

![](assets/set-up-iterator-350x190.jpg)

詳しくは、 [Adobe Workfront Fusion でのモジュールの設定](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**例:**
>
>* 以下のシナリオでは、添付ファイルを含む E メールを取得し、添付ファイルを選択した 1 つのファイルとして保存する方法を示します [!DNL Dropbox] フォルダー。
>
>   E メールには、添付ファイルの配列を含めることができます。 この [!UICONTROL 反復子] 最初のモジュールの後に挿入されたモジュールを使用すると、各添付ファイルを個別に処理できます。 この [!UICONTROL 反復子] モジュールは、添付ファイルの配列を 1 つのバンドルに分割します。 各バンドルは、1 つの添付ファイルを持ち、選択した 1 つのバンドルに 1 つずつ保存されます [!DNL Dropbox] フォルダー。 この [!UICONTROL 反復子] モジュールの設定は、上記のとおりです。の [!UICONTROL 配列] フィールドには `Attachments` 配列。
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* 多くの方がご都合の良いように [!DNL Workfront Fusion] アプリに特化した [!UICONTROL 反復子] モジュールを簡単に設定できます。 例えば、 [!UICONTROL 電子メール] アプリに特別な [!UICONTROL 反復子] モジュール [!UICONTROL 電子メール] > [!UICONTROL 添付ファイルを繰り返し] それは一般と同じ結果を生む [!UICONTROL 反復子] モジュール。
>
>   ![](assets/specialized-iterators-350x135.jpg)


## トラブルシューティング：マッピングパネルで、次の下にマッピング可能な項目が表示されない [!UICONTROL 反復子] モジュール

実行時に [!UICONTROL 反復子] モジュールは、配列の項目の構造に関する情報を持っていません。 [!UICONTROL 反復子] モジュールは、次の 2 つの項目のみを表示します [!UICONTROL 反復子] モジュール：`Total number of bundles` および `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

これは、各モジュールが出力する項目に関する情報を提供し、後続のモジュールのマッピングパネルにそれらの項目を適切に表示できるようにするためです。 ただし、場合によっては、複数のモジュールでこの情報を提供できないことがあります。例： [!UICONTROL JSON] > [!UICONTROL JSON を解析] または [!UICONTROL ウェブフック] > [!UICONTROL カスタムウェブフック] モジュールにデータ構造がありません。

解決策は、シナリオを手動で実行し、出力する項目についてモジュールに学習させ、次のモジュールに情報を提供できるようにすることです。

例えば、 [!UICONTROL JSON] > [!UICONTROL JSON を解析] モジュールに以下のようなデータ構造が含まれていません。

![](assets/json-parse-json-350x285.png)

次に、 [!UICONTROL 反復子] モジュールを使用すると、モジュールの出力を、セットアップパネルの「配列」フィールドにマッピングできなくなります。 [!UICONTROL 反復子] モジュール：

![](assets/connect-iterator-module-350x146.png)

これを解決するには、シナリオエディターでシナリオを手動で開始します。 モジュールのリンクを解除するには、 [!UICONTROL JSON] > [!UICONTROL JSON を解析] モジュールを使用して、フローがこれ以上続くのを防ぎます。 または、 [!UICONTROL JSON] > [!UICONTROL JSON を解析] モジュールと選択 **[!UICONTROL このモジュールのみを実行]** コンテキストメニューから [!UICONTROL JSON] > [!UICONTROL JSON を解析] モジュール。

次の場合に [!UICONTROL JSON] > [!UICONTROL JSON を解析] を実行すると、出力する項目について学習し、この情報を Iterator モジュールを含むすべての後続モジュールに提供します。 次に、Iterator の設定のマッピングパネルに、次の項目が表示されます。

![](assets/mapping-panel-displays-items-350x131.png)

さらに、 [!UICONTROL 反復子] モジュールは、配列の項目に含まれる項目を表示します。

![](assets/items-contained-in-array-350x156.png)

モジュールのマッピングパネルに一部の項目が表示されない場合は、シナリオを 1 回実行して、すべてのモジュールが出力する項目について学習し、次のモジュールにこの情報を提供できるようにします。
