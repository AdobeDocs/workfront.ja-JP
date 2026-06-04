---
product-area: projects
navigation-topic: financials
title: プロジェクトレベルの請求レートの会社レベルの請求率での上書き
description: プロジェクトレベルの請求レートの会社レベルの請求率での上書き
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
TQID: https://experienceleague.adobe.com/GQSQGGHBZsBLtI8IEUltVXzxmEtOxue0iE6fpHmYWP4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 475
ht-degree: 89%

---

# プロジェクトレベルの請求レートの会社レベルの請求率での上書き

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

プロジェクトレベルの請求料金の代わりに会社レベルの請求料金を使用するようにプロジェクトを設定できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>プロジェクトおよび財務データへのアクセスを編集する</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>請求レートと一般財務を編集する権限を持つプロジェクトへの権限を管理します</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 会社レベルの請求料金上書きオプションの有効化

会社がプロジェクトに関連付けられ、このオプションが有効になっている場合、会社レベルの請求料金を変更すると、プロジェクトで設定されている請求料金が上書きされます。

ユーザーがプロジェクトの財務を手動で再計算すると、会社レベルの請求料金に対する変更がすべて適用されます。 収益計算の履歴も、請求済みとしてマークされていない限り上書きされます。

1. プロジェクトに移動します。
1. ヘッダーのプロジェクト名の横にある&#x200B;**詳細** メニュー![詳細メニュー](assets/qs-more-icon-on-an-object.png)をクリックし、**編集**&#x200B;をクリックします。
1. 「**財務**」セクションで、「**会社レベルでの請求料金によるプロジェクトレベルの請求料金の上書きを許可**」を有効にします。

   >[!CAUTION]
   >
   >このオプションを有効にすると、請求済みとしてマークされていない限り、収益計算の履歴が上書きされます。 請求記録を作成することで、収益計算の履歴を保持できます。 詳しくは、[請求記録を作成](../../../manage-work/projects/project-finances/create-billing-records.md)の記事を参照してください。

1. 「**変更を保存**」をクリックします。

## 会社レベルの請求料金を更新してプロジェクトに適用

プロジェクトで会社レベルの請求料金上書きオプションを有効にした後、会社の請求料金に加えた変更は、財務が再計算されるたびにプロジェクトに適用されます。

>[!NOTE]
>
>会社レベルの請求料金を更新するには、ユーザーは自分のアクセスレベルで会社にアクセスできる必要があります。

{{step-1-to-setup}}

1. 「**会社**」をクリックします。
1. 会社レベルの請求料金の上書きを有効にしたプロジェクトに関連付けられている会社の名前をクリックします。
1. 左側のパネルで「**請求料金**」をクリックします。
1. **会社の請求料**&#x200B;と、既存の担当業務の開始日と終了日を更新し、Enter を押します。

   新しい日付の有効な会社の請求料を追加するには、担当業務の請求率を選択して「**編集**」をクリックします。 日付が有効な会社の請求料金について詳しくは、 [会社レベルでの担当業務請求料金の上書き](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)を参照してください。

1. 1 つ以上のプロジェクトの会社の料金を更新するには、次のいずれかの操作を行います。

   * 複数のプロジェクト：

      1. プロジェクトのリストに移動します。
      1. 更新するプロジェクトに合わせてチェックボックスを選択します。
      1. 「**編集**」をクリックします。
      1. 「設定」セクションで、「**コストおよび収益の再計算**」オプションを有効にします。
      1. 「**変更を保存**」をクリックします。

   * 単一のプロジェクト：

      1. 会社レベルの請求料金の上書きを有効にしたプロジェクトに移動します。
      1. ヘッダーのプロジェクト名の横にある&#x200B;**詳細** メニュー![詳細メニュー](assets/qs-more-icon-on-an-object.png)をクリックし、「**財務を再計算**」をクリックします。
