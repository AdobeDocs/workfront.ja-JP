---
title: 接続されたレコードの概要
description: レコードタイプ間の接続を作成したら、個々のレコードを相互に接続できます。 この記事では、Adobe Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 20%

---

# 接続されたレコードの概要

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

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

* Workspace <!--<span class="preview">and record type</span>--> に対するWorkfront Planning and View 以上のアクセス権を持つすべてのユーザーは、レコード間またはレコードと他のアプリケーションのオブジェクト間で確立した関連付けを確認できます。 そのようなユーザーは、接続先のアプリケーションの権限に関係なく、接続されたレコードとオブジェクトを表示できます。
* ワークスペースに対する管理権限を持ち、接続されたレコードがある場所に <!--<span class="preview">and record type</span>--> る場合は、他のユーザーの接続を表示および編集できます。
* 1 つのレコードを別のアプリケーションの 1 つまたは複数のオブジェクトに接続できます。これは、レコードタイプの接続時に選択した接続タイプによって異なります。 詳しくは、「接続されたレコードタイプの概要 [ の「接続タイプ」の節を参照してください ](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

## レコードを接続できる領域

次の領域で、レコードを他のレコードに接続したり、別のアプリケーションのオブジェクトに接続したりできます。

* Workfront Planning のレコードを、Planning レコードの次の領域にあるWorkfrontオブジェクトまたはExperience Manager Assetsオブジェクトに関連付けることができます。

   * Planning のレコード・タイプのテーブル・ビューの接続されたレコード・フィールド。
   * 「詳細」タブの、接続されたレコードフィールドでのレコードのプレビューまたはページ。
   * [ 接続 ] タブのレコードのプレビューまたはページ。
   * <span class="preview"> 接続されたレコードの「接続ビュー」タブでのレコードのページ </span>

* Workfrontの次の領域で、Workfront オブジェクトをWorkfront Planning レコードに関連付けることができます。

   * Workfront オブジェクトの Planning セクション。
   * <span class="preview">Workfront オブジェクトのカスタムフォームの Planning 接続フィールド</span>

  詳しくは、[Workfront オブジェクトからのレコード接続の管理 ](/help/quicksilver/planning/records/manage-records-in-planning-section.md) を参照してください。