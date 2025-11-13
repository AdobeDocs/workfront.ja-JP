---
title: 接続されたレコードの概要
description: レコードタイプ間の接続を作成したら、個々のレコードを相互に接続できます。 この記事では、Adobe Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 16%

---

# 接続されたレコードの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>  -->

{{planning-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。

この記事では、Adobe Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。

レコードを相互に、または別のオブジェクトに接続する方法については、「[ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md)」を参照してください。


## レコードの接続に関する考慮事項

* レコードタイプを接続すると、接続されたレコードタイプが、リンク元のレコードタイプのテーブルおよびレコードのページにリンクされたレコードフィールドとして表示されます。
* リンクされたレコードフィールドから、リンクされたレコードタイプやオブジェクトタイプのレコードやオブジェクトを参照し、追加することができます。
* リンク元のレコードタイプのテーブルに、リンクされたレコードタイプのフィールド（参照フィールド）を追加できます。

  また、リンク元のレコードタイプのフィールド（ルックアップフィールド）を、リンク先のレコードタイプのテーブルに追加することもできます。

  例えば、キャンペーンのレコードタイプから製品のレコードタイプにリンクすると、キャンペーンの製品フィールドと製品のキャンペーンフィールドを表示できます。
* リンク元のレコードの参照フィールドの値を手動で更新することはできません。

  参照フィールドの値は、元のレコードまたはオブジェクトで更新された後、自動リンク元のWorkfront Planning レコードに入力されます。

* ワークスペースおよびレコードタイプに対するWorkfront Planning and View 以上のアクセス権を持つユーザーは誰でも、レコード間またはレコードと他のアプリケーションのオブジェクト間で確立した関連付けを確認できます。 そのようなユーザーは、接続先のアプリケーションの権限に関係なく、接続されたレコードとオブジェクトを表示できます。
* ワークスペースに対する管理権限と、接続されたレコードがあるレコードタイプを持っている場合は、他のユーザーの接続を表示および編集できます。
* 1 つのレコードを別のアプリケーションの 1 つまたは複数のオブジェクトに接続できます。これは、レコードタイプの接続時に選択した接続タイプによって異なります。 詳しくは、「接続されたレコードタイプの概要 [ の「接続タイプ」の節を参照してください ](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

## レコードを接続できる領域

次の領域で、レコードを他のレコードに接続したり、別のアプリケーションのオブジェクトに接続したりできます。

* Workfront Planning のレコードを、Planning レコードの次の領域にあるWorkfrontオブジェクト、Experience Manager AssetsオブジェクトまたはGenStudioブランドに関連付けることができます。

   * Planning のレコード・タイプのテーブル・ビューの接続されたレコード・フィールド。
   * 「詳細」タブの、接続されたレコードフィールドでのレコードのプレビューまたは詳細ページ。
   * 「接続」タブのレコードのプレビューまたは詳細ページ。
   * 接続されたレコードの「接続されたレコード」ページタブ内のレコードのページ。

* Workfrontの次の領域で、Workfront オブジェクトをWorkfront Planning レコードに関連付けることができます。

   * Workfront オブジェクトの Planning セクション。
   * Workfront オブジェクトのカスタムフォームの Planning 接続フィールド。

  詳しくは、[Workfront オブジェクトからのレコード接続の管理 ](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。
