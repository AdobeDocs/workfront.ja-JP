---
product-area: projects
navigation-topic: financials
title: パフォーマンスインデックスメソッド（PIM）の設定
description: プロジェクトのパフォーマンスインデックスメソッド（PIM）は、Adobe Workfront がコスト効率指数（CPI）、コストスケジュール効率指数（CSI）、スケジュール効率指数（SPI）、完成時総コスト見積り（EAC）などのプロジェクトの実績指標の計算に使用する方法を制御します。
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '469'
ht-degree: 100%

---

# パフォーマンスインデックスメソッド（PIM）の設定

プロジェクトのパフォーマンスインデックスメソッド（PIM）は、Adobe Workfront がコスト効率指数（CPI）、コストスケジュール効率指数（CSI）、スケジュール効率指数（SPI）、完成時総コスト見積り（EAC）などのプロジェクトの実績指標の計算に使用する方法を制御します。

Workfront は、次の値を使用してこれらの値を計算します。

* 時間
* コスト

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## Workfront での PIM に関する考慮事項

* Workfront 管理者またはグループ管理者が、パフォーマンスインデックスメソッド（PIM）を時間ベースとコストベースのどちらにするかに関するデフォルトを設定します。パフォーマンス指標の計算は、このデフォルトの設定に応じて変わります。PIM の計算方法のデフォルトを変更する方法について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
* プロジェクトマネージャーは、プロジェクトの「財務」サブタブで、個々のプロジェクトに対する PIM の設定をプロジェクトレベルで変更することもできます。プロジェクトの「財務」サブタブを編集するには、プロジェクトに対する管理権限が必要です。

## プロジェクトのパフォーマンスインデックスメソッド（PIM）を設定

1. 自分が所有するプロジェクトに移動します。

   >[!IMPORTANT]
   >
   >次の手順を実行するには、プロジェクトに対する管理権限が必要です。また、プロジェクトの財務情報エリアを変更するのは、プロジェクト所有者のみにすることをお勧めします。

1. 左側のパネルで「**プロジェクト詳細**」をクリックして、**財務情報**&#x200B;エリアに移動します。
1. 「**パフォーマンスインデックスメソッド**」フィールドの値をダブルクリックして編集します。
1. 「**パフォーマンスインデックスメソッド**」フィールドの次のオプションから選択します。

   | 時間ベース | Workfront では、プロジェクトの CPI と EAC の計算に予定時間数が使用され、プロジェクトの EAC は時間単位の数値で表示されます。 |
   |---|---|
   | コストベース | Workfront は、プロジェクトの CPI と EAC の計算に予定労力コストを使用し、EAC は通貨の値で表示されます。このオプションを選択する場合は、タスクの担当者（業務担当またはユーザー）がコスト率に関連付けられていることを確認します。 |

   {style="table-layout:auto"}

1. 「**変更**&#x200B;を&#x200B;**保存**」をクリックします。
