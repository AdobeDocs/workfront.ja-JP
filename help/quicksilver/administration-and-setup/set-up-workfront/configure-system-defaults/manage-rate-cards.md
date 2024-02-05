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
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 72%

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
   <td><p>新しいプラン： [!UICONTROL Standard] </p>
       <p>または</p> 
       <p>現在のプラン： [!UICONTROL プラン ] </p>
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
1. クリック [!UICONTROL **新しい料金カード**]」をクリックし、 [!UICONTROL **料金カード**] フィールドに貼り付け、「無題レートカード」に置き換えます。
1. カード画面で、 [!UICONTROL **ジョブの役割を追加**].
1. ダイアログで、 [!UICONTROL **ジョブの役割**] ：請求率を定義します。

   「デフォルト請求レート」には、このジョブ・ロールが定義されている場合に、システム・レベルのレートが表示されます。

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
1. （オプション）別の場所の同じジョブの役割または別のジョブの役割に対して、別の請求率を追加するには、 [!UICONTROL **ジョブの役割を追加**].
1. （オプション）請求率を編集するには、料金カードで料金を選択し、 **編集** アイコン。

## レートカードをコピー

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. リスト内の料金カードの横にあるチェックボックスを選択し、 **コピー** アイコン ![コピーアイコン](assets/copy-icon.png).

   レートカードのコピーが追加されます。リスト内のレートカードの名前をクリックして、名前を変更します。

## レートカード全体を削除する

{{step-1-to-setup}}

1. 左側のパネルで、「[!UICONTROL **レートカード**]」をクリックします。
1. リスト内の料金カードの横にあるチェックボックスを選択し、 **削除** アイコン ![削除アイコン](assets/delete.png).

   >[!NOTE]
   >
   >プロジェクトに添付されている評価カードが、プロジェクトから削除されます。
