---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: のシナリオにフィルターを追加する [!DNL Adobe] Workfront Fusion
description: 場合によっては、特定の条件を満たすバンドルでのみ作業する必要があります。 フィルターを使用すると、これらのバンドルを選択できます。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# のシナリオにフィルターを追加する [!DNL Adobe Workfront Fusion]

場合によっては、特定の条件を満たすバンドルでのみ作業する必要があります。 フィルターを使用すると、これらのバンドルを選択できます。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

2 つのモジュール間にフィルターを追加し、前のモジュールから受け取ったバンドルが特定のフィルター条件を満たしているかどうかを確認できます。

* その場合、バンドルはシナリオの次のモジュールに渡されます。
* そうでない場合、バンドルの処理は終了します。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

両方のモジュールをシナリオに追加してから、フィルタを追加する必要があります。

## 2 つのモジュール間にフィルターを追加します。

1. クリック **[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) 左のパネルで、シナリオを選択して開きます。
1. ウィンドウの右上隅で、 **[!UICONTROL 編集]**.
1. モジュール間の接続線をクリックします。
1. 表示されるボックスに、 **[!UICONTROL ラベル]** フィルターの
1. フィルターの定義 **[!UICONTROL 条件]**.

   2 つのボックスに、1 つまたは 2 つのオペランドを入力できます。 両方のボックスにオペランドを入力する場合は、オペランド間のドロップダウンメニューで演算子を選択して、オペランド間の関係を指定できます。

   >[!TIP]
   >
   >オペランドフィールドでは、で説明しているように、値をマッピングするのと同じ方法で入力できます。 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   例えば、フィルターで次の場所にファイルを検索する場合、 [!DNL Adobe Workfront] XML で終わり、に渡される [!DNL Dropbox]を入力し、 **[!UICONTROL ファイル名]** 」と「 」の両方を入力します。**[!UICONTROL xml]** を 2 番目のボックスに入力します。 これらの間のドロップダウンメニューで、「 **[!UICONTROL 次で終わる（大文字と小文字を区別しない）]**. このフィルターは、最初のモジュール (Workfront) からの受信バンドルに適用されます。 次のモジュール ([!DNL Dropbox]) をクリックします。

   ![](assets/set-up-filter-box-350x368.jpg)

1. クリック **[!DNL OK]**.

## フィルターのコピー

現在、シナリオエディターには、フィルターをコピーする機能は含まれていません。

>[!NOTE]
>
>フィルターの両側のモジュールをコピーすると、フィルターもコピーされます。
>
>モジュールのコピーについて詳しくは、 [でのモジュールまたはシナリオのコピー [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

モジュールをコピーせずにフィルターをコピーするには、 [!DNL Google] 次の回避策に対する Chrome:

1. のインストール [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 拡張子。
1. In [!DNL Workfront Fusion]、シナリオを開きます。
1. Chrome の 3 ドットメニューをクリックし、 *をクリックします。*[!UICONTROL その他のツール*]* > **[!UICONTROL 開発者ツール]**.

1. 内 [!UICONTROL 開発者ツール] 表示されるパネルで、上部のメニューバーの [!UICONTROL Workfront Fusion] タブをクリックします。

   ![](assets/copy-a-filter-350x174.png)

1. 次をクリック： **[!UICONTROL ツール]** アイコン ![](assets/devtools-tools-icon.png) をクリックします。

1. クリック **[!UICONTROL フィルターをコピー]**&#x200B;次に、 **[!UICONTROL フィルターをコピー]** ツールを右側のパネルに次のように設定します。

   1. を **[!UICONTROL ソースモジュール]** を追加します。
   1. を **[!UICONTROL ターゲットモジュール]** を追加します。

1. クリック **[!UICONTROL 実行]**.
