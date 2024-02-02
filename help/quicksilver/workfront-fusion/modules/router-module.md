---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion のルーターモジュール
description: ルーターモジュールを使用すると、フローを複数のルートに分岐し、データを各ルートで別々に処理できます。ルーターモジュールがバンドルを受け取ると、ルートがルーターモジュールに接続された順序で、接続されている各ルートにバンドルを転送します。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '626'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の[!UICONTROL ルーター]モジュール

[!UICONTROL ルーター]モジュールを使用すると、フローを複数のルートに分岐し、データを各ルートで別々に処理できます。[!UICONTROL ルーター]モジュールはバンドルを受け取ると、ルートが[!UICONTROL ルーター]モジュールに接続された順序で、接続されている各ルートにバンドルを転送します。

>[!NOTE]
>
>* ルートの順序を確認するには、[!UICONTROL 自動整列]アイコンをクリックします。上から下への順序に従ってルートを配置します。
>
>  順序を変更するには、[!UICONTROL ルーター]モジュールを開き、必要な順序でルートを再接続します。
>
>* ルートは、並列ではなく順番に処理されます。バンドルは、前のルートで完全に処理されるまで、次のルートに送信されません。
>



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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL ルーター]モジュールをシナリオに追加

[!UICONTROL ルーター]は、次のいずれかの方法でシナリオに追加できます。

* モジュールの後に[!UICONTROL ルーター]モジュールを接続する場合、モジュールの右ハンドルをクリックし、「**[!UICONTROL ルーター]**」と入力して検索して、表示されるモジュールのリストで&#x200B;**[!UICONTROL フロー制御]**／**[!UICONTROL ルーター]**&#x200B;を選択します。

  ![](assets/connect-the-router-350x108.png)

* 2 つのモジュール間に[!UICONTROL ルーター]モジュールを挿入する場合は、2 つのモジュールを接続するルートの下にあるレンチアイコンをクリックし（またはルートを右クリックし）、メニューから「**[!UICONTROL ルーターを追加]**」を選択します。

  ![](assets/insert-router-350x191.png)

* [!UICONTROL ルーター]モジュールを自動的に挿入することができます。例えば、下の画像で、右下隅のモジュールを左上隅のモジュールに接続するには（右上隅のモジュールに接続済み）、右下隅のモジュールの左ハンドルをドラッグして、左上モジュールにドロップします。

  ![](assets/insert-router-automatically-350x379.png)

## フィルター

[!UICONTROL ルーター]モジュールの後に、他のルートと同様にバンドルをフィルタリングすることができます。

1. ルート内のいずれかのドットをクリックします。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 表示される&#x200B;**[!UICONTROL フィルターの設定]**&#x200B;ボックスで条件を追加して、「**[!UICONTROL OK]**」をクリックし、フィルター設定を保存します。

   ![](assets/set-up-a-filter-2-350x242.png)

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md) のシナリオにフィルターを追加を参照してください。

## フォールバックルート

[!UICONTROL ルーター]モジュールに続くルートのフィルター設定には、フォールバックルートの特別なオプションがあります。

![](assets/fallback-route-350x260.png)

有効にすると、このルートは、他のルートのフィルターによってフィルターが除外され、バンドルが[!UICONTROL ルーター]モジュールから他のどのルートを通っても続行できないときに使用されます。

フォールバックルートは、[!UICONTROL ルーター]モジュール内で異なる矢印記号で区別されます。

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

フォールバックルートの一般的な使用例は、次の手順に従って、条件が満たされた場合は、あるルートでフローを続行し、満たされない場合は別のルートでフローを続行することです。

1. シナリオに[!UICONTROL ルーター]モジュールを挿入します。
1. [!UICONTROL ルーター]モジュールで両方のルートを接続します。
1. 最初のルートをクリックし、条件を指定します。

   ![](assets/set-up-a-filter-2-350x242.png)

1. 2 つ目のルートをクリックし、[!UICONTROL フォールバックルート]オプションを有効にします。

   ![](assets/enable-fallback-route-option-350x238.png)
