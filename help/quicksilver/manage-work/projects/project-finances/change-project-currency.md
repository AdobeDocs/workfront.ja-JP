---
product-area: projects
navigation-topic: financials
title: プロジェクト通貨を変更
description: プロジェクトマネージャーは、Adobe Workfrontシステムでデフォルトの通貨以外の通貨を使用するようにプロジェクトを設定できます。 これにより、人件費と売上高を計算する際に、プロジェクトの財務情報を目的の通貨で表示できます。
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# プロジェクト通貨を変更

プロジェクトマネージャーは、Adobe Workfrontシステムでデフォルトの通貨以外の通貨を使用するようにプロジェクトを設定できます。 これにより、人件費と売上高を計算する際に、プロジェクトの財務情報を目的の通貨で表示できます。

この節で説明するように代替通貨を使用するには、まずWorkfront管理者が複数の通貨を有効にして設定する必要があります（記事を参照） [為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

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
   <td> <p>プロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Workfrontでプロジェクトの通貨を変更する際の考慮事項

* プロジェクトに財務情報がある場合、プロジェクトの通貨は変更できません。
* 賃率は労務費に使用されます。売上高の計算およびは、今後レポート目的で使用されます。
* 1 つのプロジェクトに異なる通貨を指定しない場合、Workfrontは、そのプロジェクトの通貨がシステムのデフォルトの通貨であると見なします。 システムレベルのデフォルト通貨について詳しくは、 [為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* デフォルトでは、すべてのフルライセンスユーザーが通貨と為替レートを表示する権限を持っています。 Workfront管理者は、 **為替レート** ユーザーがプロジェクトに対して特定の率を設定できるようにする。
* Workfrontの為替レートは動的ではありません。 この値は管理者が設定し、為替レートの変更が発生した場合に更新する必要があります。
* 通貨をプロジェクトに反映するレポートを作成する場合、デフォルトでは、すべてのレポートはプロジェクトのデフォルト通貨でグループ化されます。 異なる為替レートを持つ複数のプロジェクトでレポートを作成する場合、プロジェクトに適用したグループは、システムレベルでのデフォルトの為替レートを反映します。 詳しくは、 [一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## プロジェクトの通貨の設定

1. デフォルトの通貨を変更するプロジェクトに移動します。

   >[!TIP]
   >
   >プロジェクトに財務情報がまだ含まれていないことを確認します。 たとえば、プロジェクトに「計画原価」または「実績原価」が関連付けられていないことを確認します。

1. クリック **プロジェクトの詳細** 左のパネルで、 **金融** 領域
1. クリック **追加** 内 **通貨** 「 」フィールドで、プロジェクトのデフォルト通貨として使用する通貨を選択します。 Workfront管理者がWorkfrontインスタンスに設定したすべての通貨が表示されます。

   ![](assets/currency-on-project-expanded-nwe.png)

1. （条件付き）Workfrontシステムに設定されているデフォルト通貨以外の通貨を選択する場合は、選択した通貨のレートを指定します。通貨は、システムでベース通貨として設定されている通貨に関連します。
1. クリック **変更を保存**.
