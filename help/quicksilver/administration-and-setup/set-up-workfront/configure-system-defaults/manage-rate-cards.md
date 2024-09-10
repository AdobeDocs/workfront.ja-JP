---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 評価カードの管理
description: レートカードを使用すると、場所に基づいて、役割ごとに複数の請求レートを定義できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 97%

---

# 評価カードを管理

{{highlighted-preview-article-level}}

レートカードを使用すると、場所に基づいて、役割ごとに複数の請求レートを定義できます。例えば、パリを拠点とするデザイナーとニューヨークを拠点とする別のデザイナーの 2 つの担当業務を持ち、それぞれに異なる請求レートで設定できます。ただし、レートカードの担当業務に場所は必要ありません。レートカードの担当業務（場所が含まれる場合もあります）の請求レートには、有効日付を含めることもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規：[!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL Financial Data] への編集アクセス権</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>共有されているレートカードを編集するには、レートカードの管理権限が必要です。</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レートカードを追加

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. 「[!UICONTROL **新しいレートカード**]」をクリックし、「[!UICONTROL 新しいレートカード]」ボックスにレートカード名を入力して、「無題のレートカード」を置き換えます。
1. （オプション）レートカードの詳細画面で、[!UICONTROL **説明**]&#x200B;を追加します。
1. （オプション）レートカードにカスタムフォームを添付するには、右上隅にある「[!UICONTROL **カスタムフォームを追加**]」フィールドをクリックし、表示されるリストからカスタムフォームを選択します。

   カスタムフォームの添付について詳しくは、[オブジェクトへのカスタムフォームの追加](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

1. 左側のナビゲーションパネルで「[!UICONTROL **担当業務とレート**]」をクリックします。
1. レートカードの担当業務とレート画面で、「[!UICONTROL **担当業務を追加**]」をクリックします。
1. ダイアログで、請求レートを定義する&#x200B;[!UICONTROL **担当業務**]&#x200B;を選択します。

   「既定の請求レート」には、この担当業務のシステムレベルのレートが表示されます（定義されている場合）。

   ![新しい請求レートダイアログ](assets/location-rate-for-rate-card.png)

1. 担当業務の&#x200B;[!UICONTROL **通貨**]&#x200B;を選択します。
1. （オプション）担当業務の&#x200B;[!UICONTROL **場所**]&#x200B;を選択します。
1. 「[!UICONTROL **請求レート 1**]」フィールドに、この場所の請求レートを入力します。次に、「[!UICONTROL **保存**]」をクリックして、請求レートを 1 回だけ上書きします。

   または

   「[!UICONTROL **レートを追加**]」をクリックして、有効日付と共に場所固有の請求レートを追加します。

1. （条件付き）この場所に複数の請求レートを追加する場合は、次の情報を入力します。

   * **[!UICONTROL 請求レート 1]、2 など：**&#x200B;期間の請求レートの値。
   * **[!UICONTROL 開始日]：**&#x200B;レートの上書きを開始する日付。
   * **[!UICONTROL 終了日]：**&#x200B;レートの上書きを終了する日付。

     請求レート 1 には開始日が設定されず、最後の請求レートには終了日が設定されません。一部の日付は自動的に追加されます。例えば、請求レート 1 に終了日がなく、開始日が 2023年5月1日の請求レート 2 を追加すると、ギャップが生じないように、請求レート 1 の終了日に 2023年4月30日が追加されます。

1. 「[!UICONTROL **保存**]」をクリックします。
1. （オプション）別の場所の同じ担当業務または別の担当業務に対して別の請求レートを追加するには、「[!UICONTROL **担当業務を追加**]」をクリックします。
1. （オプション）レートカードを編集するには、「設定」のレートカードリストでレートカード名をクリックします。請求レートを編集するには、レートカードの左側のナビゲーションパネルで「[!UICONTROL **担当業務とレート**]」をクリックします。次に、レートを選択し、**編集**&#x200B;アイコン ![編集アイコン](assets/edit-icon.png) をクリックします。

## レートカードをコピー

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. リスト内のレートカードの横にあるチェックボックスを選択し、**コピー**&#x200B;アイコン ![コピーアイコン](assets/copy-icon.png) をクリックします。
1. 「[!UICONTROL レートカードをコピー]」ボックスにレートカード名を入力して、「無題のレートカード」を置き換えます。次に、「**保存**」をクリックします。

   新しいレートカードが保存されます。必要に応じて、レートカードの詳細、担当業務、レートを編集します。

## レートカード全体を削除する

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. リスト内のレートカードの横にあるチェックボックスを選択し、**削除** アイコン ![削除アイコン](assets/delete.png) をクリックします。

   >[!NOTE]
   >
   >プロジェクトに添付されている評価カードが、プロジェクトから削除されます。
