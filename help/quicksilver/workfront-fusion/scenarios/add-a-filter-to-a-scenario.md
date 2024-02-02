---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe]  Workfront Fusion のシナリオにフィルターを追加'
description: 場合によっては、特定の条件を満たすバンドルのみで作業する必要があります。フィルターを使用すると、そのようなバンドルを選択できます。
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '576'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] のシナリオにフィルターを追加

場合によっては、特定の条件を満たすバンドルのみで作業する必要があります。フィルターを使用すると、そのようなバンドルを選択できます。

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

2 つのモジュール間にフィルターを追加すると、前のモジュールから受け取ったバンドルが特定のフィルター条件を満たしているかどうかを確認できます。

* 満たしている場合、バンドルはシナリオ内の次のモジュールに渡されます。
* 満たしていない場合、バンドルの処理は終了します。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を、組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

両方のモジュールをシナリオに追加した後で、それらの間にフィルターを追加する必要があります。

## 2 つのモジュール間にフィルターを追加します。

1. 左側のパネルで&#x200B;**[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックし、シナリオを選択して開きます。
1. ウィンドウの右上隅で「**[!UICONTROL 編集]**」をクリックします。
1. モジュール間を接続する線をクリックします。
1. 表示されるボックスに、フィルターの&#x200B;**[!UICONTROL ラベル]**&#x200B;を入力します。
1. フィルターの&#x200B;**[!UICONTROL 条件]**&#x200B;を定義します。

   2 つのボックスに、1 つまたは 2 つのオペランドを入力できます。両方のボックスにオペランドを入力する場合は、オペランド間のドロップダウンメニューで演算子を選択すると、オペランド間の関係を指定できます。

   >[!TIP]
   >
   >オペランドフィールドでは、値をマッピングするのと同じ方法で入力できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) のモジュール間で情報をマッピングを参照してください。

   例えば、XML で終わる [!DNL Adobe Workfront] 内のファイルをフィルターで検索し、それらを [!DNL Dropbox] に渡す場合は、**[!UICONTROL ファイル名]**&#x200B;を最初のボックスに入力し、2 番目のボックスに「.**[!UICONTROL xml]**」と入力します。それらの間のドロップダウンメニューで、「**[!UICONTROL 次で終わる（大文字と小文字を区別しない）]**」を選択します。このフィルターは、最初のモジュール（Workfront）からの受信バンドルに適用されます。XML ファイルを含むバンドルのみが、次のモジュール（[!DNL Dropbox]）に渡されます。

   ![](assets/set-up-filter-box-350x368.jpg)

1. **[!DNL OK]** をクリックします。

## フィルターをコピー

現在、シナリオエディターには、フィルターをコピーする機能は含まれていません。

>[!NOTE]
>
>フィルターのどちらかの側のモジュールをコピーすると、フィルターもコピーされます。
>
>モジュールのコピーについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md) でのモジュールまたはシナリオのコピーを参照してください。

モジュールをコピーせずにフィルターをコピーするには、[!DNL Google] Chrome を使用して以下の回避策を行います。

1. [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 拡張機能をインストールします。
1. [!DNL Workfront Fusion] でシナリオを開きます。
1. Chrome の 3 ドットメニューをクリックし、**[!UICONTROL その他のツール*]*／**[!UICONTROL 開発者ツール]**&#x200B;をクリックします。

1. 表示される[!UICONTROL 開発者ツール]パネルの上部のメニューバーで、「[!UICONTROL Workfront Fusion]」タブをクリックします。

   ![](assets/copy-a-filter-350x174.png)

1. 左側のサイドバーの&#x200B;**[!UICONTROL ツール]**&#x200B;アイコン ![](assets/devtools-tools-icon.png) をクリックします。

1. 「**[!UICONTROL フィルターをコピー]**」をクリックし、右側のパネルの&#x200B;**[!UICONTROL フィルターをコピー]**&#x200B;ツールを次のように設定します。

   1. コピーするフィルターの直後のモジュールとして「**[!UICONTROL ソースモジュール]**」を設定します。
   1. **[!UICONTROL ターゲットモジュール]**&#x200B;を、コピーするフィルターの直前のモジュールとして設定します。

1. 「**[!UICONTROL 実行]**」をクリックします。
