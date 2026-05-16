---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Adobe クラウドストレージを有効にする
description: Adobe クラウドストレージを有効にすると、すべてのAdobe製品に対して統合ストレージソリューションを使用できるようになります。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 8%

---

# Adobe クラウドストレージを有効にする

Adobeクラウドストレージは、Adobeのあらゆるアプリケーションに対応する統合ストレージソリューションです。 Adobeのクラウドベースのストレージソリューションであり、エンタープライズ製品全体のアセットの中央リポジトリとして機能します。

Adobe クラウドストレージは、新規のお客様に対してデフォルトで有効になっており、契約更新時に既存のお客様に対して有効にすることができます。

Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意のワークフローパッケージ</p></td> 
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

## Adobe クラウドストレージを有効にする

Adobe クラウドストレージを有効にするには：

{{step-1-to-setup}}

1. 左側のナビゲーションで「**システム**」を選択し、「**環境設定**」を選択します。
1. **ストレージの環境設定** セクションまでスクロールします。
1. デフォルト ドロップダウンメニューで、**Adobe クラウドストレージ**&#x200B;を選択します。
1. （オプション）Adobe クラウドストレージと従来のWorkfront ストレージを組み合わせて使用する場合は、「**ユーザーがストレージプロバイダーを選択することを許可する**」チェックボックスをオンにします。

   >[!NOTE]
   >
   >このオプションを有効にすると、ユーザーは新しいプロジェクトの作成時にストレージプロバイダーを選択できます。 Adobe クラウドストレージは、デフォルトのストレージプロバイダーであるため、「新しいプロジェクト」というラベルが付けられます。 従来のWorkfront ストレージは、「従来のプロジェクト」とラベル付けされます。
   >
   >![新しいプロジェクトと従来のプロジェクトのオプション ](assets/new-esm-project.png)

1. 「適用先」ドロップダウンメニューで、次のいずれかのオプションを選択します。

   - **組織全体**：このオプションは、デフォルトのストレージプロバイダーをWorkfront環境全体に適用します。 ユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます。
   - **特定のグループ**：このオプションは、組織内の特定のグループにのみデフォルトのストレージプロバイダーを適用します。 指定したグループのユーザーが新しいプロジェクトを作成するたびに、デフォルトのストレージプロバイダーが使用されます

1. 「**保存**」をクリックします。

   >[!NOTE]
   >
   >既存のプロジェクトは、作成されたストレージモデルを保持します。 例えば、Adobe クラウドストレージを使用するプロジェクトでは、デフォルトのストレージ環境設定を変更した後も、引き続きAdobe クラウドストレージを使用します。

## サンドボックス環境でのAdobe クラウドストレージ

Adobe クラウドストレージは、[!DNL Workfront] サンドボックス環境で利用できます。本番環境でロールアウトする前に、この記事で説明した機能をテストできます。 ただし、Frame.io ビューアはサンドボックスでは利用できないため、統一されたレビューと承認のエクスペリエンスを本番環境で検証する必要があります。

カスタムリフレッシュサンドボックスがある場合は、Adobe クラウドストレージをサポートするWorkfrontのバージョンにアップグレードした後でリフレッシュする必要があります。 更新により、サンドボックスからAdobe クラウドストレージ機能にアクセスできるようになり、テストを開始できます。 詳しくは、[ カスタムリフレッシュサンドボックス環境 [!DNL Adobe Workfront] を参照してください。](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)
