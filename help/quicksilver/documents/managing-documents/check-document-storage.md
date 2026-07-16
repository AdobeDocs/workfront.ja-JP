---
product-area: documents
navigation-topic: manage-documents
title: ドキュメントのストレージ制限のチェック
description: Adobe Workfront管理者は、お客様情報ページでドキュメントストレージの使用状況と割り当てを確認できます。 ストレージの表示方法は、組織で従来のWorkfront ストレージを使用するか、Adobe クラウドストレージを使用するかによって異なります。
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 15%

---

# ドキュメントのストレージ制限のチェック

ユーザーがWorkfront インスタンスにアップロードできる個々のファイルの種類とサイズに制限はありませんが、Workfront プランには合計ストレージ割り当てが含まれています。 Workfront管理者は、お客様情報ページの設定領域から使用状況と割り当てを監視できます。

ストレージの表示方法は、組織で従来のWorkfront ストレージを使用するか、Adobe クラウドストレージを使用するかに応じて異なります。

* 従来のWorkfront ストレージを使用している場合は、この記事の[従来のWorkfront ストレージ ](#legacy-workfront-storage)を参照してください。
* Adobe クラウドストレージを使用する場合は、この記事の「[Adobe クラウドストレージ ](#adobe-cloud-storage)」を参照してください。

  Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront プラン</td> 
   <td> <p>従来のストレージを使用してドキュメントを管理する任意のWorkfront パッケージ</p>
      <p>Adobe クラウドストレージを使用してドキュメントを管理するワークフローパッケージ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レガシー Workfront ストレージ

お客様の組織が従来のWorkfront ストレージを使用している場合、お客様の情報ページには、Workfrontに直接アップロードされたドキュメントに対する1つのストレージ割り当て量が表示されます。

従来のWorkfront ドキュメントストレージを確認するには：

{{step-1-to-setup}}

1. 左側のパネルで、**システム**／**顧客情報**&#x200B;をクリックします。
1. 「**基本情報**」セクションで「**ストレージ割当**」を探します。 ここでは、現在使用しているストレージの量と、Workfront プランに含まれるストレージの合計量を確認できます。

ストレージクォータは、最新のカウントを表示するために毎日更新されます。

>[!NOTE]
>
>この制限は、他のサードパーティサービスプロバイダー（SharePoint、Google Drive、Webdam、Box、Dropbox、またはその他のドキュメントアセット管理プロバイダー）からWorkfrontにリンクするドキュメントには適用されません。

## Adobe クラウドストレージ


組織でAdobe クラウドストレージを使用している場合、ストレージ割り当ては、Workfront ライセンスを通じてプロビジョニングされたストレージと、Frame.io Enterprise アドオンを通じてプロビジョニングされたストレージを組み合わせた1つのプール割り当てとしてレポートされます。 ストレージの使用量にハードキャップはありません。ユーザーは、使用量が割り当て量を超えた場合でもドキュメントのアップロードを続行できます。

### お客様情報でのストレージ使用状況の表示

Adobe クラウドストレージのドキュメントを確認するには：

{{step-1-to-setup}}

1. 左側のパネルで、**システム**／**顧客情報**&#x200B;をクリックします。
1. 「**ストレージの概要**」セクションに移動します。
1. 利用状況を確認しましょう。 ストレージの概要には、プールされたストレージの割り当てが表示され、使用状況は次の場所に分けられます。

   * 青いバーには、Workfrontの従来のプロジェクトとAdobe クラウドストレージプロジェクトが表示されます。
   * 緑色のバーにフレームスタンドアロンプロジェクトが表示されます。 これらのプロジェクトはWorkfrontとは別のもので、Frame.io Enterprise ライセンスをお持ちの場合にのみ使用できます。


お客様の情報](assets/storage-usage.png)での![Adobe クラウドストレージの使用状況

使用状況の数値は定期的に更新されるので、最新の数を確認できます。

### 管理者向けメール通知

使用率がストレージ割り当て量の75%、90%、または100%を超えると、Workfrontはシステム管理者にメール通知を送信します。
