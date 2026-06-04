---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: templates-navigation-topic
title: ブループリントカタログを参照し、ブループリントのインストールをリクエストする
description: ブループリントは、ビジネスと共に成長する作業管理システムを構築するために役立つ基本的な構成要素を提供します。 すべての  [!DNL Adobe Workfront]  ユーザーはブループリントのカタログを参照できます。  [!DNL Workfront]  管理者がブループリントリクエストを有効にしている場合、管理者に特定のブループリントをインストールするようリクエストすることもできます。
author: Courtney
feature: System Setup and Administration, Work Management
exl-id: 932072e4-4d52-4b4b-a045-0cd38cb882d3
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/pXahlHijtEo-hqF7Rh9OBIYAyHIIR1ZtmlrWR8SyVYo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 369
ht-degree: 95%

---

# ブループリントカタログの参照とブループリントのインストールのリクエスト

ブループリントは、ビジネスと共に成長する作業管理システムを構築するために役立つ基本的な構成要素を提供します。 すべての [!DNL Adobe Workfront] ユーザーはブループリントのカタログを参照できます。 [!DNL Workfront] 管理者がブループリントリクエストを有効にしている場合、管理者に特定のブループリントをインストールするようリクエストすることもできます。

ブループリントをインストールできるのはシステム管理者だけです。 詳しくは、[ブループリントのインストール](../../administration-and-setup/blueprints/blueprints-install.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>コントリビューター以上</p><p>依頼者以上</p>
  </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ブループリントカタログを参照

カタログには、組織で利用可能なすべてのブループリントが表示されます。 ブループリントのタイプや成熟度レベルなどのブループリントについて詳しくは、[ブループリントの概要](../../administration-and-setup/blueprints/blueprints-overview.md)を参照してください。

{{step1-to-blueprints}}

1. ブループリントのカタログを参照します。
1. 右側のフィルターパネルを使用して、次のオプションでカタログをフィルターします。

   * ユースケース（[!UICONTROL 人事]や[!UICONTROL マーケティング] など）
   * 成熟度レベル（[!UICONTROL 管理]または[!UICONTROL 統合]）
   * インストールステータス（[!UICONTROL インストール済み] また末[!UICONTROL インストール]）
   * ブループリントタイプ（[!UICONTROL ダッシュボード]、[!UICONTROL 組織構造]、[!UICONTROL プロジェクトテンプレート]<!-- above Custom Form; here, Request Queue, Setup Feature-->）

1. （オプション）ブループリントの&#x200B;**[!UICONTROL 詳細]**&#x200B;をクリックして、その仕組みを確認してください。

   [!UICONTROL 詳細]ページで利用可能なコンテンツについて詳しくは、[ブループリントの概要](../../administration-and-setup/blueprints/blueprints-overview.md)を参照してください。

## ブループリントのインストールをリクエスト

システム管理者がブループリントのリクエストを許可している場合は、ブループリントのインストールを要求できます。 詳しくは、[ブループリントへのアクセスの設定](../../administration-and-setup/blueprints/configure-access-to-blueprints.md)を参照してください。

ブループリントのインストールをリスエストすると、そのリスエストはシステム管理者に送信されます。 通知環境設定に従って、リクエストが完了すると通知が届きます。

{{step1-to-blueprints}}

1. インストールするブループリントを見つけます。 右側のパネルのフィルターを使用して、ユースケース、成熟度レベル、インストール状況、タイプごとにフィルターをかけることができます。
1. ブループリントで&#x200B;**[!UICONTROL リクエスト]**&#x200B;をクリックします。

   ブループリントに&#x200B;**[!UICONTROL リスエスト]**&#x200B;ボタンが表示されない場合は、システム管理者がリクエストを有効にしていません。

   ![ブループリントをリクエスト](assets/blueprints-non-admin-request-bp-350x283.png)
