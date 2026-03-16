---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 組織に合わせたAdobe エンタープライズストレージの有効化
description: Adobeのエンタープライズストレージを有効にすると、すべてのAdobe製品で統合ストレージソリューションを使用できるようになります。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
source-git-commit: e70a65447fe508d055809271edad399d823f66dd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 11%

---

# Adobe エンタープライズストレージを有効にする

Adobe エンタープライズストレージは、すべてのAdobe製品向けの統合ストレージソリューションです。 これは、Adobeのエンタープライズ製品全体でアセットの中央リポジトリとして機能するクラウドベースのストレージソリューションです。

Adobe エンタープライズストレージは、新規のお客様に対してはデフォルトで有効になっており、既存のお客様に対しては契約更新時に有効にすることができます。

Adobe エンタープライズストレージについて詳しくは、[Adobe エンタープライズストレージの概要 ](/help/quicksilver/review-and-approve-work/esm-overview.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Adobe エンタープライズストレージを有効にする

Adobeのエンタープライズストレージを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。
1. 「**ストレージ環境設定**」セクションまでスクロールします。
1. デフォルト ドロップダウンメニューから、「**Adobe エンタープライズストレージ**」を選択します。
1. （オプション）Adobe エンタープライズストレージと従来のWorkfront ストレージの組み合わせを使用する場合は、「**ストレージプロバイダーの選択を許可**」チェックボックスを選択します。

   >[!NOTE]
   >
   >このオプションを有効にすると、ユーザーは新しいプロジェクトを作成する際にストレージプロバイダーを選択できます。 エンタープライズストレージはデフォルトのストレージプロバイダーなので、「新規プロジェクト」というラベルが付いています。 従来のWorkfront ストレージには、「従来のプロジェクト」というラベルが付けられます。
   >
   >![ 新規プロジェクトおよび従来のプロジェクトオプション ](assets/new-esm-project.png)

1. 適用先ドロップダウンメニューで、次のいずれかのオプションを選択します。

   - **組織全体**：このオプションは、デフォルトのストレージプロバイダーをWorkfront環境全体に適用します。 ユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます。
   - **特定のグループ**：このオプションは、デフォルトのストレージプロバイダーを組織内の特定のグループにのみ適用します。 指定したグループのユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます

1. 「**保存**」をクリックします。
