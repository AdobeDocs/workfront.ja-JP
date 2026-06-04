---
product-area: projects
navigation-topic: financials
title: パフォーマンスインデックスメソッド（PIM）の設定
description: プロジェクトのパフォーマンスインデックスメソッド（PIM）は、Adobe Workfront がコスト効率指数（CPI）、コストスケジュール効率指数（CSI）、スケジュール効率指数（SPI）、完成時総コスト見積り（EAC）などのプロジェクトの実績指標の計算に使用する方法を制御します。
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
TQID: https://experienceleague.adobe.com/g4FYe8k1psS9xuL6Z40teAyJ-SV4UD6ThnWvnvl8au4
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
source-wordcount: 418
ht-degree: 97%

---

# パフォーマンスインデックスメソッド（PIM）の設定

プロジェクトのパフォーマンスインデックスメソッド（PIM）は、Adobe Workfront がコスト効率指数（CPI）、コストスケジュール効率指数（CSI）、スケジュール効率指数（SPI）、完成時総コスト見積り（EAC）などのプロジェクトの実績指標の計算に使用する方法を制御します。

Workfront は、次の値を使用してこれらの値を計算します。

* 時間
* コスト

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td>任意 </td> 
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
   <td>一般財務を編集する権限を持つプロジェクトの権限を管理します</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront での PIM に関する考慮事項

* Workfront 管理者またはグループ管理者が、パフォーマンスインデックスメソッド（PIM）を時間ベースとコストベースのどちらにするかに関するデフォルトを設定します。 パフォーマンス指標の計算は、このデフォルトの設定に応じて変わります。 PIM の計算方法のデフォルトを変更する方法について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
* プロジェクトマネージャーは、プロジェクトの「財務」サブタブで、個々のプロジェクトに対する PIM の設定をプロジェクトレベルで変更することもできます。 プロジェクトの「財務」サブタブを編集するには、プロジェクトに対する管理権限が必要です。

## プロジェクトのパフォーマンスインデックスメソッド（PIM）を設定

1. 自分が所有するプロジェクトに移動します。

   >[!IMPORTANT]
   >
   >次の手順を実行するには、プロジェクトに対する管理権限が必要です。 また、プロジェクトの財務情報エリアを変更するのは、プロジェクト所有者のみにすることをお勧めします。

1. 左側のパネルで「**プロジェクト詳細**」をクリックして、**財務情報**&#x200B;エリアに移動します。
1. 「**パフォーマンスインデックスメソッド**」フィールドの値をダブルクリックして編集します。
1. 「**パフォーマンスインデックスメソッド**」フィールドの次のオプションから選択します。

   | 時間ベース | Workfront では、プロジェクトの CPI と EAC の計算に予定時間数が使用され、プロジェクトの EAC は時間単位の数値で表示されます。 |
   |---|---|
   | コストベース | Workfront は、プロジェクトの CPI と EAC の計算に予定労力コストを使用し、EAC は通貨の値で表示されます。 このオプションを選択する場合は、タスクの担当者（業務担当またはユーザー）がコスト率に関連付けられていることを確認します。 |

   {style="table-layout:auto"}

1. 「**変更**&#x200B;を&#x200B;**保存**」をクリックします。
