---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: で配列をマッピングする [!DNL Adobe] Workfront Fusion
description: 配列は、Adobe Workfront Fusion のモジュールフィールドにマッピングできます。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# で配列をマッピングする [!DNL Adobe Workfront Fusion]

配列は、次の項目を含む特別なタイプの項目です。

* 1 つ以上のテキスト値（単純配列）
* 同じタイプの 1 つ以上のコレクション（複合配列）

>[!INFO]
>
>**例：** この [!UICONTROL メールを見る] モジュールは、すべての電子メールの添付ファイルの配列を返します。 すべての添付ファイルは、名前、コンテンツ、サイズなどを含むコレクションを表します。

詳しくは、 [の項目データタイプ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## 配列のマッピング

1. ターゲットフィールドにある「 」ボタンをクリックします。

   >[!INFO]
   >
   >  **例：** 上記の例では、「 [!UICONTROL 添付ファイルを追加] ボタンをクリックします。
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. 表示されるボックスに、項目を入力します。

   パネルを使用すると、他のタイプの項目と同じ方法でフィールドをマッピングできます。 各項目に個別に入力しないで、別の配列をターゲットフィールドにマッピングする場合は、 [!UICONTROL マップ] 」ボタンをクリックします。 この場合、両方の配列（ソース配列とターゲット配列）の構造が同じであることを確認します。

   1 つの配列には、任意の数の項目を追加できます。

反復子を使用して、配列を個々のバンドルに分割できます。 詳しくは、 [[!UICONTROL 反復子] モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
