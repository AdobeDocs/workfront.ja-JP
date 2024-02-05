---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社レベルでの担当業務請求率の上書き
description: 担当業務を作成する際に、その役割の時間単位の請求率を選択するオプションがあります。会社に固有の時間単位の請求率を作成できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 72%

---

# 会社レベルでの担当業務請求率の上書き

担当業務を作成する際に、その役割の時間単位の請求率を選択するオプションがあります。1 つの会社に固有の複数の時間別請求率を作成できます。 各請求率は、特定の日付範囲に対して有効です。

プロジェクトレベルでは、会社レベルの請求率でプロジェクトレベルの請求率を上書きするオプションを有効にできます。詳しくは、[プロジェクトレベルの請求率を会社レベルの請求率で上書きする](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>システム管理者でない場合の会社への管理者アクセス</p> <p>財務データへの [!UICONTROL Edit] アクセス</p> <p><b>メモ</b>：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 特定の担当業務に使用される確定済みの請求率を上書きまたは変更する

1. [!DNL Adobe] Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![](assets/main-menu-icon.png)をクリックし、次に「**[!UICONTROL 設定]**」![](assets/gear-icon-settings.png)をクリックします。

1. 「**[!UICONTROL 会社]**」をクリックします。
1. 担当業務が割り当てられている会社を見つけます。
1. リストで会社名をクリックします。
1. 左側のパネルで「**[!UICONTROL 請求料金]**」をクリックします。
1. クリック **[!UICONTROL 請求率を追加] > [!UICONTROL 新しい請求率]**&#x200B;または、編集する既存のレートを選択します。
1. Adobe Analytics の [!UICONTROL 新しい請求率] ダイアログで、 [!UICONTROL **ジョブの役割**] ：の請求率を定義します。

   The [!UICONTROL **デフォルトの請求率**] このジョブロールのシステムレベルのレートを表示します。

   ![新しい請求レートダイアログ](assets/date-effective-billing-rates-for-company.png)

1. Adobe Analytics の [!DNL **請求率 1**] 「 」フィールドに、請求率を入力します。 次に、「[!UICONTROL **保存**]」をクリックして、請求レートを 1 回だけ上書きします。

   または

   クリック [!UICONTROL **追加率**] 有効日を含む請求率をさらに追加する場合。

1. （条件付き）複数の請求レートを追加する場合は、次の情報を入力します。

   * **[!UICONTROL 請求率 1]、2 など**：期間の請求率の値。
   * **[!UICONTROL 開始日]**：レートが有効になった日付。
   * **[!UICONTROL 終了日]**：レートが終了する日付。

     請求レート 1 には開始日が設定されず、最後の請求レートには終了日が設定されません。一部の日付は自動的に追加されます。例えば、請求レート 1 に終了日がなく、開始日が 2023年5月1日の請求レート 2 を追加すると、ギャップが生じないように、請求レート 1 の終了日に 2023年4月30日が追加されます。

1. 「[!UICONTROL **保存**]」をクリックします。

   >[!NOTE]
   >
   >プロジェクトで変更された担当業務の請求率は、そのプロジェクトにのみ影響します。会社レベルで変更された請求率は、すべてのプロジェクトに影響を与えます。詳しくは、[担当業務の請求率の上書きとプロジェクトでの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)を参照してください。
