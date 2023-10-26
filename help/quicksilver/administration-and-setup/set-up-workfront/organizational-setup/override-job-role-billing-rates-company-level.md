---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社レベルでのジョブロール請求率の上書き
description: ジョブの役割を作成する際に、その役割の時間別請求率を選択することもできます。 会社に固有の時間別請求率を作成できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# 会社レベルでのジョブロール請求率の上書き

ジョブの役割を作成する際に、その役割の時間別請求率を選択することもできます。 1 つの会社に固有の複数の時間別請求率を作成できます。 各請求率は、特定の日付範囲に対して有効です。

プロジェクトレベルでは、会社レベルの請求率でプロジェクトレベルのレートを上書きするオプションを有効にできます。 詳しくは、 [プロジェクト・レベルの請求率を会社レベルの請求率で上書き](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>システム管理者でない場合の会社への管理者アクセス</p> <p>[!UICONTROL 編集 ] による金融データへのアクセス</p> <p><b>注意</b>：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 特定のジョブの役割に使用される確定済みの請求率を上書きまたは変更する

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) ～の右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL 会社]**.
1. ジョブの役割が割り当てられている会社を見つけます。
1. リストで会社名をクリックします。
1. クリック **[!UICONTROL 請求率]** をクリックします。
1. クリック **[!UICONTROL 請求率を追加] > [!UICONTROL 新しい請求率]**&#x200B;または、編集する既存のレートを選択します。
1. Adobe Analytics の [!UICONTROL 新しい請求率] ダイアログで、 [!UICONTROL **ジョブの役割**] ：の請求率を定義します。

   The [!UICONTROL **デフォルトの請求率**] このジョブロールのシステムレベルのレートを表示します。

   ![新しい請求率ダイアログ](assets/date-effective-billing-rates-for-company.png)

1. Adobe Analytics の [!DNL **請求率 1**] 「 」フィールドに、請求率を入力します。 次に、「 [!UICONTROL **保存**] ：請求率を 1 回だけ上書きします。

   または

   クリック [!UICONTROL **追加率**] 有効日を含む請求率をさらに追加する場合。

1. （条件付き）複数の請求レートを追加する場合は、次の情報を入力します。

   * **[!UICONTROL 請求率 1]、2 など**：期間の請求率の値。
   * **[!UICONTROL 開始日]**：レートが有効になった日付。
   * **[!UICONTROL 終了日]**：レートが終了する日付。

     請求レート 1 には開始日が設定されず、最後の請求レートには終了日が設定されません。 一部の日付は自動的に追加されます。 たとえば、請求レート 1 に終了日がなく、開始日が 2023 年 5 月 1 日の請求レート 2 を追加した場合、ギャップが生じないように、2023 年 4 月 30 日の終了日が請求レート 1 に追加されます。

1. 「[!UICONTROL **保存**]」をクリックします。

   >[!NOTE]
   >
   >プロジェクトで変更されたジョブの役割率は、そのプロジェクトにのみ影響します。 会社レベルで変更された率は、すべてのプロジェクトに影響を与えます。 詳しくは、 [ジョブ・ロール請求率の上書きとプロジェクトでの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
