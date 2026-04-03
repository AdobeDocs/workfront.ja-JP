---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Adobe エンタープライズストレージを有効にする
description: Adobe エンタープライズストレージを有効にすると、すべてのAdobe製品に対して統合ストレージソリューションを使用できるようになります。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 11%

---

# Adobe エンタープライズストレージを有効にする

Adobeエンタープライズストレージは、Adobeのあらゆるアプリケーションに対応する、統合ストレージソリューションです。 Adobeのクラウドベースのストレージソリューションであり、エンタープライズ製品全体のアセットの中央リポジトリとして機能します。

Adobe エンタープライズストレージは、新規のお客様に対してデフォルトで有効になっており、契約更新時に既存のお客様に対して有効にすることができます。

Adobe エンタープライズ ストレージについて詳しくは、[Adobe エンタープライズ ストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

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

Adobe エンタープライズストレージを有効にするには、次の手順に従います。

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。
1. **ストレージの環境設定** セクションまでスクロールします。
1. デフォルト ドロップダウンメニューで、**Adobe エンタープライズストレージ**&#x200B;を選択します。
1. （オプション）Adobe エンタープライズストレージと従来のWorkfront ストレージを組み合わせて使用する場合は、「**ユーザーがストレージプロバイダーを選択することを許可する**」チェックボックスをオンにします。

   >[!NOTE]
   >
   >このオプションを有効にすると、ユーザーは新しいプロジェクトの作成時にストレージプロバイダーを選択できます。 エンタープライズストレージは、デフォルトのストレージプロバイダーであるため、「新しいプロジェクト」というラベルが付けられます。 従来のWorkfront ストレージは、「従来のプロジェクト」とラベル付けされます。
   >
   >![新しいプロジェクトと従来のプロジェクトのオプション &#x200B;](assets/new-esm-project.png)

1. 「適用先」ドロップダウンメニューで、次のいずれかのオプションを選択します。

   - **組織全体**：このオプションは、デフォルトのストレージプロバイダーをWorkfront環境全体に適用します。 ユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます。
   - **特定のグループ**：このオプションは、組織内の特定のグループにのみデフォルトのストレージプロバイダーを適用します。 指定したグループのユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます

1. 「**保存**」をクリックします。
