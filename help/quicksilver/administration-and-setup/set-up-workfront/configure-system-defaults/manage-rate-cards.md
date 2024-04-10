---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 評価カードを管理
description: レートカードを使用すると、場所に基づいて、役割ごとに複数の請求レートを定義できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 57%

---

# 評価カードを管理

{{highlighted-preview-article-level}}

レートカードを使用すると、場所に基づいて、役割ごとに複数の請求レートを定義できます。例えば、パリを拠点とするデザイナーとニューヨークを拠点とする別のデザイナーの 2 つの担当業務を持ち、それぞれに異なる請求レートで設定できます。ただし、レートカードの担当業務に場所は必要ありません。レートカードの担当業務（場所が含まれる場合もあります）の請求レートには、有効日付を含めることもできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規計画：[!UICONTROL 標準 ] </p>
       <p>または</p> 
       <p>現在のプラン：[!UICONTROL プラン ] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL Financial Data] への編集アクセス権</p> <p><b>メモ</b>：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>共有されているレートカードを編集するには、レートカードの管理権限が必要です。</td> 
  </tr> 
 </tbody> 
</table>

## レートカードを追加

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. クリック [!UICONTROL **新しいレートカード**]&#x200B;で、評価カードの名前を [!UICONTROL 新しいレートカード] ボックスに入力して、「名称未設定の評価カード」と置き換えます。
1. （オプション）レートカードの詳細画面で、 [!UICONTROL **説明**].
1. （オプション）評価カードにカスタムフォームを添付するには、 [!UICONTROL **カスタムフォームを追加**] 右上隅のフィールドをクリックし、表示されるリストからカスタムフォームを選択します。

   カスタムフォームの添付について詳しくは、 [カスタムフォームのオブジェクトへの追加](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. クリック [!UICONTROL **担当業務と評価**] 左側のナビゲーションパネルで以下を実行します。
1. 評価カードの担当業務と評価の画面で、をクリックします [!UICONTROL **担当業務を追加**].
1. ダイアログで、 [!UICONTROL **担当業務**] に対する請求レートを定義します。

   デフォルトの請求レートは、この担当業務のシステムレベルのレートを表示します（定義されている場合）。

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
1. （オプション）別の場所の同じ担当業務または別の担当業務に対して別の請求レートを追加するには、次のボタンをクリックします [!UICONTROL **担当業務を追加**].
1. （オプション）評価カードを編集するには、「設定」の「評価カード」リストで評価カード名をクリックします。 請求レートを編集するには、 [!UICONTROL **担当業務と評価**] 評価カードの左側のナビゲーションパネル レートを選択し、 **編集** アイコン ![編集アイコン](assets/edit-icon.png).

## レートカードをコピー

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. リストの評価カードの横にあるチェックボックスをオンにし、 **コピー** アイコン ![コピーアイコン](assets/copy-icon.png).
1. 評価カードの名前を [!UICONTROL 評価カードをコピー] ボックスに入力して、「名称未設定の評価カード」と置き換えます。 次に、 **保存**.

   新しい評価カードが保存されます。 必要に応じて、評価カードの詳細、担当業務、評価を編集します。

## 評価カード全体を削除

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. リストの評価カードの横にあるチェックボックスをオンにし、 **削除** アイコン ![アイコンを削除](assets/delete.png).

   >[!NOTE]
   >
   >プロジェクトに添付されている評価カードが、プロジェクトから削除されます。
