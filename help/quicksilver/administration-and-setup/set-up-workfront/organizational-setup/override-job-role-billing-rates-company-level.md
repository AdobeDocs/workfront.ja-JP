---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社レベルでの担当業務請求率の上書き
description: 担当業務を作成する際に、その役割の時間単位の請求率を選択するオプションがあります。会社に固有の時間単位の請求率を作成できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 94%

---

# 会社レベルでの担当業務請求率の上書き

担当業務を作成する際に、その役割の時間単位の請求率を選択するオプションがあります。1 つの会社に固有の複数の時間単位の請求レートを作成できます。各請求レートは、特定の日付範囲に対して有効です。

プロジェクトレベルでは、会社レベルの請求率でプロジェクトレベルの請求率を上書きするオプションを有効にできます。詳しくは、[プロジェクトレベルの請求率を会社レベルの請求率で上書きする](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>システム管理者でない場合の会社への管理者アクセス</p>
   <p>財務データへのアクセスの編集</p> </td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 特定の担当業務に使用される確定済みの請求率を上書きまたは変更する

{{step-1-to-setup}}

1. 「**[!UICONTROL 会社]**」をクリックします。
1. 担当業務が割り当てられている会社を見つけます。
1. リストで会社名をクリックします。
1. 左側のパネルで「**[!UICONTROL 請求料金]**」をクリックします。
1. **[!UICONTROL 請求レートを追加]／[!UICONTROL 新規請求料金]**&#x200B;をクリックするか、編集する既存のレートを選択します。
1. [!UICONTROL 新規請求料金]ダイアログで、請求レートを定義する&#x200B;[!UICONTROL **担当業務**]&#x200B;を選択します。

   [!UICONTROL **既定の請求レート**]&#x200B;には、この担当業務のシステムレベルのレートが表示されます。

   ![新しい請求レートダイアログ](assets/date-effective-billing-rates-for-company.png)

1. 「[!DNL **請求レート 1**]」フィールドに請求レートを入力します。次に、「[!UICONTROL **保存**]」をクリックして、請求レートを 1 回だけ上書きします。

   または

   「[!UICONTROL **レートを追加**]」をクリックして、有効な日付と請求レートをさらに追加します。

1. （条件付き）複数の請求レートを追加する場合は、次の情報を入力します。

   * **[!UICONTROL 請求率 1]、2 など**：期間の請求レートの値。
   * **[!UICONTROL 開始日]**：レートが有効になる日付。
   * **[!UICONTROL 終了日]**：レートが終了する日付。

     請求レート 1 には開始日が設定されず、最後の請求レートには終了日が設定されません。一部の日付は自動的に追加されます。例えば、請求レート 1 に終了日がなく、開始日が 2023年5月1日の請求レート 2 を追加すると、ギャップが生じないように、請求レート 1 の終了日に 2023年4月30日が追加されます。

1. 「[!UICONTROL **保存**]」をクリックします。

   >[!NOTE]
   >
   >プロジェクトで変更された担当業務の請求率は、そのプロジェクトにのみ影響します。会社レベルで変更された請求率は、すべてのプロジェクトに影響を与えます。詳しくは、[担当業務の請求率の上書きとプロジェクトでの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)を参照してください。
