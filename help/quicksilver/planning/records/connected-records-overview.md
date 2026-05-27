---
title: 接続されたレコードの概要
description: レコードタイプ間の接続を作成したら、個々のレコードを相互に接続できます。 この記事では、Adobe Workfront Planningでレコードを接続する際に考慮しなければならない考慮事項について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 8%

---

# 接続されたレコードの概要

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>
-->

{{planning-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。

この記事では、Workfront Planningでレコードを接続する際に考慮しなければならない考慮事項について説明します。

レコードを相互または別のオブジェクトに接続する方法について詳しくは、[&#x200B; レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

## 前提条件

Workfront Planningでレコードを接続するには、次の接続が必要です。

* 2 つのレコードタイプ
* 別のアプリケーションのオブジェクトを持つレコードタイプ

詳しくは、[接続されたレコードタイプの概要](/help/quicksilver/planning/architecture/connect-record-types-overview.md)を参照してください。


## レコードの接続に関する考慮事項

* レコードタイプを接続すると、接続されたレコードタイプは、レコードのページからリンクされているレコードタイプのテーブルに接続フィールドとして表示されます。
* リンクされたレコードフィールドから、リンクされたレコードタイプやオブジェクトタイプのレコードやオブジェクトを参照し、追加することができます。
* リンク元のレコードタイプのテーブルに、リンク先のレコードタイプのフィールド（ルックアップフィールド）を追加できます。

  また、リンク先のレコードタイプのテーブルに、リンク元のレコードタイプのフィールド（ルックアップフィールド）を追加することもできます。

  例えば、製品のレコードタイプをCampaignのレコードタイプからリンクする場合、キャンペーンの製品フィールドと製品のキャンペーンフィールドを表示できます。
* リンク元のレコードのルックアップフィールドの値を手動で更新することはできません。

  ルックアップフィールドの値は、元のレコードまたはオブジェクトで更新された後、自動的にリンクするWorkfront Planning レコードに入力されます。

* Workfront Planning and Viewへのアクセス権と、ワークスペースおよびレコードタイプに対するアクセス権を持つすべてのユーザーは、レコード間またはレコードと他のアプリケーションのオブジェクト間で行う接続を確認できます。 そのようなユーザーは、接続先のアプリケーションの権限に関係なく、接続されたレコードとオブジェクトを表示できます。
* ワークスペースに対する管理権限と、接続されたレコードがあるレコードタイプがある場合は、他のユーザーの接続を表示および編集できます。
* 1つのレコードを別のアプリケーションから1つまたは複数のオブジェクトに接続できます。これは、レコードタイプの接続時に選択した接続のタイプに応じて異なります。 詳しくは、記事[接続レコードタイプの概要](/help/quicksilver/planning/architecture/connect-record-types-overview.md)の「接続タイプ」の節を参照してください。
* 接続されたレコードタイプが階層の一部である場合、レコードのページから階層内の任意のオブジェクトタイプにアクセスできます。 詳しくは、[階層とパンくずリストの概要](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)を参照してください。
* 接続されたレコードタイプが階層の一部である場合、子レコードタイプの1つのレコードを、親レコードタイプの最大10件のレコードに接続できます。 詳しくは、[階層とパンくずリストの概要](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)を参照してください。

## レコードを接続できる領域

Workfrontでは、レコードを手動または自動で接続できます。

### レコードを手動で接続する

レコードを他のレコードまたは別のアプリケーションのオブジェクトに手動で接続するには、次の領域があります。

* Workfront Planningのレコードを、Planning レコードの次の領域のWorkfront オブジェクト、Experience Manager Assets オブジェクト、またはGenStudio ブランドに接続できます。

   * Planningのレコードタイプのテーブルビューの接続レコードフィールド。
   * レコードのプレビューページまたは詳細ページの接続されたレコードフィールド。
   * レコードの接続レコードページにあるレコードのプレビューまたは詳細ページ。

* Workfront オブジェクトは、Workfrontの次の領域のWorkfront計画レコードに接続できます。

   * Workfront オブジェクトの「計画」セクション。
   * Workfront オブジェクトのカスタムフォームのPlanning接続フィールド。

  詳しくは、[Workfront オブジェクトからのレコード接続の管理](/help/quicksilver/planning/records/manage-records-in-planning-section.md)を参照してください。

### レコードを自動的に接続し

他のアプリケーションからレコードタイプを相互に、またはレコードタイプをオブジェクトタイプに接続すると、次の方法でレコードとオブジェクトを自動的に接続できます。

* 自動処理の利用

  自動処理を設定するPlanning レコードから、レコードまたはWorkfront オブジェクトを作成できます。

  定義した条件が満たされると、レコードまたはオブジェクトが作成され、オートメーションのトリガー元となるレコードに自動的に接続されます。

  詳しくは、[Adobe Workfront Planningの自動処理の設定](/help/quicksilver/planning/records/configure-automations-to-create-records.md)を参照してください。

* リクエストフォームを使用したレコードの作成

  Planning リクエストを送信するときにレコードを作成できます。 リクエストとレコードは自動的に接続されます。

  >[!NOTE]
  >
  >レコードを元のリクエストから切断することはできません。

  詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront計画リクエストの送信](/help/quicksilver/planning/requests/submit-requests.md)を参照してください。
