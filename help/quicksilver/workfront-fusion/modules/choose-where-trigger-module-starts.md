---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion でトリガーモジュールを開始する場所を選択
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 80%

---

# [!DNL Adobe Workfront Fusion] でトリガーモジュールを開始する場所を選択

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [トリガーモジュールの開始位置の選択 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/choose-where-trigger-module-starts.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

一部のトリガーモジュールでは、バンドルの取得を開始する最初のバンドルを選択できます。

また、すべてのバンドルを取得するか、特定の日付以降のバンドルのみを取得するかを指定することもできます。

トリガーモジュールについて詳しくは、[モジュールの種類](../../workfront-fusion/modules/module-types.md)の記事で[トリガーモジュール](../../workfront-fusion/modules/module-types.md#triggers)の節を参照してください。

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

## トリガーモジュールの開始場所を選択

1. トリガーモジュールを保存します。

   または

   [[!UICONTROL Adobe Workfront Fusion でモジュールの設定を行う]](../../workfront-fusion/modules/configure-a-modules-settings.md)の説明に従って、トリガーモジュールの設定を変更します。

   または

   [ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成の説明に従って、[!UICONTROL シナリオエディター]でトリガーモジュールのアイコンを右クリックします。

1. 表示される&#x200B;**[!UICONTROL 開始場所を選択]**&#x200B;ボックスでオプションを選択します。

   ![](assets/choose-where-to-start-350x346.jpg)

   表示されるオプションは、特定のサービスの可能性に応じて異なります。含まれる可能性のあるものは、次のとおりです。

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on]（デフォルト）</td>
            <td>以降、追加または更新されたすべてのバンドルを（設定に応じて）取得します。</td>
        </tr>
        <tr>
            <td>[!UICONTROL From after a specific date]</td>
            <td>指定された日時以降に（設定に応じて）追加または更新されたすべてのバンドルを取得します</td>
        </tr>
        <tr>
            <td>[!UICONTROL With ID greater than or equal to a specific value]</td>
            <td>指定された ID 以上の ID を持つすべてのバンドルを取得します</td> 
        </tr>
        <tr>
            <td>[!UICONTROL All bundles]</td>
            <td>使用可能なすべてのバンドルを取得します</td>
        </tr>
        <tr>
            <td>[!UICONTROL Select the first bundle]</td>
            <td>バンドルの取得を開始する最初のバンドルを選択できます</td>
        </tr>
   </table>
