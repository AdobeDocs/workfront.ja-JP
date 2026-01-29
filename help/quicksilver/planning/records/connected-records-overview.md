---
title: 接続されたレコードの概要
description: レコードタイプ間の接続を作成したら、個々のレコードを相互に接続できます。 この記事では、Adobe Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 8%

---

# 接続されたレコードの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。

この記事では、Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。

レコードを相互に、または別のオブジェクトに接続する方法については、「[&#x200B; レコードの接続 &#x200B;](/help/quicksilver/planning/records/connect-records.md)」を参照してください。

## 前提条件

Workfront Planning でレコードを接続する前に、次を接続する必要があります：

* 2 つのレコードタイプ
* 別のアプリケーションからのオブジェクトを持つレコードタイプ

詳しくは、[&#x200B; 接続されたレコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。


## レコードの接続に関する考慮事項

* レコードタイプを接続すると、接続されたレコードタイプは、リンク元のレコードタイプのテーブルの接続フィールドおよびレコードのページに表示されます。
* リンクされたレコードフィールドから、リンクされたレコードタイプやオブジェクトタイプのレコードやオブジェクトを参照し、追加することができます。
* リンク元のレコードタイプのテーブルに、リンクされたレコードタイプのフィールド（参照フィールド）を追加できます。

  また、リンク元のレコードタイプのフィールド（ルックアップフィールド）を、リンク先のレコードタイプのテーブルに追加することもできます。

  例えば、キャンペーンのレコードタイプから製品のレコードタイプにリンクすると、キャンペーンの製品フィールドと製品のキャンペーンフィールドを表示できます。
* リンク元のレコードの参照フィールドの値を手動で更新することはできません。

  参照フィールドの値は、元のレコードまたはオブジェクトで更新された後、自動リンク元のWorkfront Planning レコードに入力されます。

* ワークスペースおよびレコードタイプに対するWorkfront Planning and View 以上のアクセス権を持つユーザーは誰でも、レコード間またはレコードと他のアプリケーションのオブジェクト間で確立した関連付けを確認できます。 そのようなユーザーは、接続先のアプリケーションの権限に関係なく、接続されたレコードとオブジェクトを表示できます。
* ワークスペースに対する管理権限と、接続されたレコードがあるレコードタイプを持っている場合は、他のユーザーの接続を表示および編集できます。
* 1 つのレコードを別のアプリケーションの 1 つまたは複数のオブジェクトに接続できます。これは、レコードタイプの接続時に選択した接続タイプによって異なります。 詳しくは、「接続されたレコードタイプの概要 [&#x200B; の「接続タイプ」の節を参照してください &#x200B;](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。
* 接続されたレコードタイプが階層の一部である場合は、レコードのページから階層内の任意のオブジェクトタイプにアクセスできます。 詳しくは、[&#x200B; 階層とパンくずリストの概要 &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md) を参照してください。
* 接続されたレコード タイプが階層の一部である場合、子レコード タイプから 1 つのレコードを親レコード タイプから最大 10 個のレコードに接続できます。 詳しくは、[&#x200B; 階層とパンくずリストの概要 &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md) を参照してください。

## レコードを接続できる領域

Workfrontでレコードを手動または自動で接続できます。

### レコードの手動接続

次の領域で、レコードを他のレコードまたは別のアプリケーションのオブジェクトに手動で接続できます。

* Workfront Planning のレコードを、Planning レコードの次の領域にあるWorkfrontオブジェクト、Experience Manager AssetsオブジェクトまたはGenStudioブランドに関連付けることができます。

   * Planning のレコード・タイプのテーブル・ビューの接続されたレコード・フィールド。
   * レコードのプレビューページまたは詳細ページの接続済みレコードフィールド。
   * レコードの接続済みレコードページ上のレコードのプレビューまたは詳細ページ。

* Workfrontの次の領域で、Workfront オブジェクトをWorkfront Planning レコードに関連付けることができます。

   * Workfront オブジェクトの Planning セクション。
   * Workfront オブジェクトのカスタムフォームの Planning 接続フィールド。

  詳しくは、[Workfront オブジェクトからのレコード接続の管理 &#x200B;](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。

### レコードを自動的に接続

レコードの種類を別のアプリケーションから相互に接続したり、レコードの種類を別のアプリケーションからオブジェクトの種類に接続したりすると、次の方法でレコードとオブジェクトを自動的に接続できます。

* 自動化の使用

  オートメーションを構成する計画レコードから、レコードまたはWorkfrontオブジェクトを作成できます。

  定義した条件が満たされると、レコードまたはオブジェクトが作成され、自動処理をトリガーするレコードに自動的に接続されます。

  詳しくは、[Adobe Workfront Planning の自動設定の構成 &#x200B;](/help/quicksilver/planning/records/configure-automations-to-create-records.md) を参照してください。

* リクエストフォームを使用したレコードの作成

  Planning 要求を発行する際に、レコードを作成できます。 リクエストとレコードは自動的に接続されます。

  >[!NOTE]
  >
  >レコードを元のリクエストから切断することはできません。

  詳しくは、[&#x200B; レコードを作成するためのAdobe Workfront Planning リクエストの発行 &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) を参照してください。
