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
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 会社レベルでのジョブロール請求率の上書き

ジョブの役割を作成する際に、その役割の時間別請求率を選択することもできます。 会社に固有の時間別請求率を作成できます。

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
   <td> <p>システム管理者でない場合の会社への管理者アクセス</p> <p>[!UICONTROL 編集 ] による金融データへのアクセス</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 特定のジョブの役割に使用される確定済みの請求率を上書きまたは変更する

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL 会社]**.
1. ジョブの役割が割り当てられている会社を見つけます。
1. クリック **[!UICONTROL 会社を編集]** をクリックします。
1. 内 **[!UICONTROL 請求率]** 「 」セクションで、編集するジョブロールを選択し、そのジョブロールの新しい請求率を「 」に入力します **[!UICONTROL 会社の請求率]** ボックス

   >[!NOTE]
   >
   >プロジェクトで変更されたジョブの役割率は、そのプロジェクトにのみ影響します。 会社レベルで変更された率は、すべてのプロジェクトに影響を与えます。 詳しくは、 [ジョブ・ロール請求率の上書きとプロジェクトの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
