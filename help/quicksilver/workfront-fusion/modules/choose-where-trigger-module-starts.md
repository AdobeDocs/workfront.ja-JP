---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion でトリガーモジュールが開始する場所を選択
description: 一部のトリガーモジュールでは、バンドルの取得を開始する最初のバンドルを選択できます。
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# トリガーモジュールの開始場所を選択 [!DNL Adobe Workfront Fusion]

一部のトリガーモジュールでは、バンドルの取得を開始する最初のバンドルを選択できます。

また、特定の日付の後に、すべてのバンドルを取得するか、またはバンドルのみを取得するかを指定することもできます。

モジュールの詳細については、「トリガーモジュール」の節を参照してください。 [トリガーモジュール](../../workfront-fusion/modules/module-types.md#triggers) 記事内 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md).

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

## トリガー・モジュールの開始場所の選択

1. モジュールをトリガーします。

   または

   トリガーモジュールの設定を変更します。詳しくは、 [でのモジュールの設定 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   または

   次に示すように、 [!UICONTROL シナリオエディター]( [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 「 **[!UICONTROL 開始場所を選択]** 」ボックスが表示されます。

   ![](assets/choose-where-to-start-350x346.jpg)

   表示されるオプションは、特定のサービスの可能性に応じて異なります。 次のものが含まれます。

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL 今後 ]（デフォルト）</td>
            <td>以降、追加または更新されたすべてのバンドルを（設定に応じて）取得します。</td>
        </tr>
        <tr>
            <td>[!UICONTROL 指定した日付以降 ]</td>
            <td>指定された日時以降に（設定に応じて）追加または更新されたすべてのバンドルを取得します</td>
        </tr>
        <tr>
            <td>[!UICONTROL 特定の値以上の ID を持つ ]</td>
            <td>指定された ID 以上の ID を持つすべてのバンドルを取得します</td> 
        </tr>
        <tr>
            <td>[!UICONTROL すべてのバンドル ]</td>
            <td>使用可能なすべてのバンドルを取得します</td>
        </tr>
        <tr>
            <td>[!UICONTROL 最初のバンドルを選択 ]</td>
            <td>バンドルの取得を開始する最初のバンドルを選択できます</td>
        </tr>
   </table>
