---
product-area: projects
navigation-topic: financials
title: パフォーマンスインデックスメソッド (PIM) の設定
description: プロジェクトの PIM(Performance Index Method) は、Adobe Workfrontが CPI(Cost Performance Index)、CSI(Cost Schedule Performance Index)、SPI(Schedule Performance Index)、EAC(Estimate At Completion) などのプロジェクトの実績指標の計算に使用する方法を制御します。
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# パフォーマンスインデックスメソッド (PIM) の設定

プロジェクトの PIM(Performance Index Method) は、Adobe Workfrontが CPI(Cost Performance Index)、CSI(Cost Schedule Performance Index)、SPI(Schedule Performance Index)、EAC(Estimate At Completion) などのプロジェクトの実績指標の計算に使用する方法を制御します。

Workfrontは、次の値を使用してこれらの値を計算します。

* 時間
* コスト

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Workfrontでの PIM に関する考慮事項

* Workfront管理者またはグループ管理者が、パフォーマンスインデックスメソッド (PIM) を時間ベースとコストベースのどちらにするかに関するデフォルトを設定します。 パフォーマンス指標の計算は、このデフォルトの設定に応じて変わります。 PIM の計算方法のデフォルトを変更する方法の詳細については、を参照してください。 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* プロジェクトマネージャは、プロジェクトの「財務」サブタブで、個々のプロジェクトに対する PIM の設定をプロジェクトレベルで変更することもできます。 プロジェクトの「財務」サブタブを編集するには、プロジェクトに対する管理権限が必要です。

## プロジェクトのパフォーマンスインデックスメソッド (PIM) の設定

1. 自分が所有しているプロジェクトに移動します。

   >[!IMPORTANT]
   >
   >次の手順を実行するには、プロジェクトに対する管理権限が必要です。 また、プロジェクトの財務領域を変更するのは、プロジェクト所有者のみにすることをお勧めします。

1. クリック **プロジェクトの詳細** 左のパネルで、 **金融** 領域
1. 値をダブルクリックし、 **パフォーマンスインデックスメソッド** フィールドを編集します。
1. 次のオプションから選択します。 **パフォーマンスインデックスメソッド** フィールド：

   | 時間ベース | Workfrontでは、プロジェクトの CPI と EAC の計算に「計画時間」が使用され、プロジェクトの EAC は時間単位の数値で表示されます。 |
   |---|---|
   | コスト ベース | Workfrontは、プロジェクトの CPI と EAC の計算に計画労務費を使用し、EAC は通貨値として表示されます。 このオプションを選択する場合は、タスクの担当者（ジョブの役割またはユーザー）がコスト率に関連付けられていることを確認します。 |

   {style=&quot;table-layout:auto&quot;}

1. クリック **保存** **変更点**.
