---
product-area: projects
navigation-topic: financials
title: プロジェクトの通貨の変更
description: プロジェクトマネージャーは、Adobe Workfront システムのデフォルト通貨以外の通貨を使用するようにプロジェクトを設定できます。これにより、労力コストと収益を計算する際に、プロジェクトの財務情報を目的の通貨で表示できます。
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: b16523bf6c37747702efe3b5ecfcc33801526af1
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 85%

---

# プロジェクト通貨の変更

プロジェクトマネージャーは、Adobe Workfront システムのデフォルト通貨以外の通貨を使用するようにプロジェクトを設定できます。これにより、労力コストと収益を計算する際に、プロジェクトの財務情報を目的の通貨で表示できます。

この節で説明されているように代替通貨を使用する前に、[為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)の記事の説明に従って、Workfront 管理者はまず複数の通貨を有効にして設定する必要があります。

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
   <td>プロジェクトへのアクセスを編集</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>プロジェクトの管理権限</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront でプロジェクト通貨を変更する際の考慮事項

* プロジェクトに既に財務情報が存在する場合、プロジェクト通貨は変更できません。
* 料金は、人件費、収益計算、レポート作成などに使用されます。
* 1 つのプロジェクトに異なる通貨を指定しない場合、Workfront は、そのプロジェクトの通貨がシステムのデフォルトの通貨であると見なします。システムレベルのデフォルト通貨について詳しくは、[為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。
* デフォルトでは、すべてのフルライセンスユーザーが通貨と為替レートを表示に対するアクセス権を持っています。Workfront 管理者は、ユーザーがプロジェクトに特定のレートを設定できるように、**為替レート**&#x200B;に対する追加の管理アクセス権を付与する必要があります。
* Workfront の為替レートは動的ではありません。管理者がこの値を設定し、為替レートの変動が発生した場合に更新する必要があります。
* <span class="preview">有効な日付が通貨とその為替レートに適用されている場合、プロジェクトの期間中に為替レートが変更される可能性があります。 有効期限切れの為替レートについて詳しくは、[為替レートの設定](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。</span>
* プロジェクトに通貨を反映させるレポートを作成すると、デフォルトでは、すべてのレポートがプロジェクトのデフォルト通貨でグループ化されます。異なる為替レートを持つ複数のプロジェクトでレポートを作成する場合、プロジェクトに適用したグループは、システムレベルでのデフォルトの為替レートを反映します。詳しくは、[一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)を参照してください。

## プロジェクト通貨の設定

1. デフォルトの通貨を変更するプロジェクトに移動します。

   >[!TIP]
   >
   >プロジェクトに財務情報がまだ含まれていないことを確認します。例えば、プロジェクトに予定コストまたは実際のコストが関連付けられていないことを確認します。

1. 左側のパネルで「**プロジェクト詳細**」をクリックして、**財務情報**&#x200B;エリアに移動します。
1. 「**通貨**」フィールドの「**追加**」をクリックし、プロジェクトのデフォルト通貨として使用する通貨を選択します。Workfront 管理者が Workfront インスタンスに設定したすべての通貨が表示されます。

   ![ プロジェクトの通貨](assets/currency-on-project.png)

1. （条件付き）Workfront システムに設定されているデフォルト通貨以外の通貨を選択する場合は、システムで基準通貨として設定される通貨との関連で、選択した通貨のレートを指定します。

   >[!NOTE]
   >
   ><span class="preview">このプロジェクトで「**システムから日付有効な為替レートを使用」設定がオンになっている場合、為替レートの上書きは許可されません。**&#x200B;詳しくは、[ プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。</span>

1. 「**変更を保存**」をクリックします。
