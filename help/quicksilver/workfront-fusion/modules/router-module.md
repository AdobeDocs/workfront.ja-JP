---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion のルーターモジュール
description: ルータモジュールを使用すると、フローを複数のルートに分岐し、各ルート内のデータを異なる方法で処理できます。 ルータモジュールがバンドルを受け取ると、ルートがルータモジュールに接続された順に、各接続ルートに転送されます。
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL 発送担当] モジュール [!DNL Adobe Workfront Fusion]

この [!UICONTROL 発送担当] モジュールを使用すると、フローを複数のルートに分岐し、各ルート内のデータを別々に処理できます。 1 回： [!UICONTROL 発送担当] モジュールはバンドルを受け取り、ルートが [!UICONTROL 発送担当] モジュール。

>[!NOTE]
>
>* ルートの順序を確認するには、 [!UICONTROL 自動整列] アイコン。上から下への順序に従ってルートを配置します。
>
>  順序を変更するには、 [!UICONTROL 発送担当] モジュールを開き、必要な順序でルートを再接続します。
>
>* ルートは、並列ではなく順番に処理されます。 バンドルは、前のルートで完全に処理されるまで、次のルートに送信されません。
>



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

## の追加 [!UICONTROL 発送担当] シナリオへのモジュール

A [!UICONTROL 発送担当] は、次のいずれかの方法でシナリオに追加できます。

* 接続する [!UICONTROL 発送担当] モジュールの後にモジュールの右ハンドルをクリックし、入力を開始します **[!UICONTROL ルータ]** を選択して、 **[!UICONTROL フロー制御]** > **[!UICONTROL 発送担当]** をクリックします。

  ![](assets/connect-the-router-350x108.png)

* を [!UICONTROL 発送担当] 2 つのモジュール間のモジュールで、2 つのモジュールを接続するルートの下のレンチアイコンをクリックし（またはルートを右クリック）、を選択します。 **[!UICONTROL 発送担当の追加]** を選択します。

  ![](assets/insert-router-350x191.png)

* 次の項目を挿入できます： [!UICONTROL 発送担当] モジュールが自動的に追加されます。 例えば、下の画像で、右下隅のモジュールを左上隅のモジュールに接続するには（右上隅のモジュールに既に接続されている）、右下隅のモジュールの左ハンドルをドラッグして、左上モジュールにドロップします。

  ![](assets/insert-router-automatically-350x379.png)

## フィルター

次の [!UICONTROL 発送担当] 他のルートと同様にバンドルをフィルタリングするモジュール：

1. ルート内のドットの 1 つをクリックします。

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. 内 **[!UICONTROL フィルターの設定]** 表示されるボックスで、条件を追加して、 **[!UICONTROL OK]** をクリックして、フィルター設定を保存します。

   ![](assets/set-up-a-filter-2-350x242.png)

詳しくは、 [のシナリオにフィルターを追加する [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## フォールバックルート

ルートの次のルートに対するフィルター設定 [!UICONTROL 発送担当] モジュールには、次の特殊なオプションが含まれます。フォールバックルート：

![](assets/fallback-route-350x260.png)

有効にした場合、バンドルが [!UICONTROL 発送担当] 他のルートのフィルターによってフィルターが除外されたので、他のルートを介したモジュール。

フォールバックルートは、 [!UICONTROL 発送担当] モジュール：

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

フォールバックルートの一般的な使用例は、次の手順に従って、条件が満たされた場合は 1 つのルートでフローを続行し、満たされない場合は別のルートでフローを続行することです。

1. 挿入 [!UICONTROL 発送担当] モジュールを設定します。
1. 両方のルートを [!UICONTROL 発送担当] モジュール。
1. 最初のルートをクリックし、条件を指定します。

   ![](assets/set-up-a-filter-2-350x242.png)

1. 2 番目のルートをクリックし、 [!UICONTROL 代替ルート] オプション：

   ![](assets/enable-fallback-route-option-350x238.png)
