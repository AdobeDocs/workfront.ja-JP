---
title: 接続されたレコードの概要
description: レコードタイプ間の接続を作成したら、個々のレコードを相互に接続できます。 この記事では、Adobe Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 30%

---


<!--update metadata at GA-->

# 接続されたレコードの概要

{{planning-important-intro}}

Adobe Workfront Planning レコードを相互に接続したり、他のアプリケーションのオブジェクトに接続したりできます。

この記事では、Adobe Workfront Planning でレコードを接続する際に考慮する必要がある考慮事項について説明します。

レコードを相互に、または別のオブジェクトに接続する方法については、「[ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md)」を参照してください。


## レコードの接続に関する考慮事項

* レコードタイプを接続すると、接続されたレコードタイプが、リンク元のレコードタイプのテーブルおよびレコードのページにリンクされたレコードフィールドとして表示されます。
* リンクされたレコードフィールドから、リンクされたレコードタイプやオブジェクトタイプのレコードやオブジェクトを参照し、追加することができます。
* リンク元のレコードタイプのテーブルに、リンクされたレコードタイプのフィールド（参照フィールド）を追加できます。

  リンク元のレコードタイプのフィールド（ルックアップフィールド）を、リンク先のレコードタイプのテーブルに追加できます。

  例えば、キャンペーンのレコードタイプから製品のレコードタイプにリンクする場合、キャンペーンの製品フィールドと製品のキャンペーンフィールドを表示できます。
* リンク元のレコードの参照フィールドの値を手動で更新することはできません。

  参照フィールドの値は、元のレコードまたはオブジェクトで更新された後、自動リンク元のWorkfront Planning レコードに入力されます。

* Workfront Planning へのアクセス権と、ワークスペースへの表示以上の権限を持つユーザーは誰でも、レコード間に、またはレコードと他のアプリケーションのオブジェクトの間に作成する接続を表示できます。そのようなユーザーは、接続先のアプリケーションの権限に関係なく、接続されたレコードとオブジェクトを表示できます。
* 接続されているレコードが存在するワークスペースに対する管理権限を持っている場合は、他のすべてのユーザーの接続を表示および編集できます。
* 1 つのレコードを別のアプリケーションの 1 つまたは複数のオブジェクトに接続できます。<!--For more information, see the "Connections types" section in the article [Connected record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md). -->

## レコードを接続できる領域

次の領域で、レコードを他のレコードに接続したり、別のアプリケーションのオブジェクトに接続したりできます。

* 次の領域で、Workfront Planning のレコードをWorkfront オブジェクトに関連付けることができます。
   * テーブルビューの接続されたフィールドのWorkfront Planning の Planning レコードから。
   * レコードのプレビューまたは接続されたレコードフィールドのページで、Workfront Planning の計画レコードから。
  <!--
  * From a Planning record in Workfront Planning in the record preview or page in the connected record fields on the Details tab.
  * From a Planning record in the record's preview or page on the Connections tab.  -->

* 次の領域で、Workfrontの計画レコードをExperience Manager Assetsに接続できます。

   * テーブル表示のWorkfront計画の計画レコードから。
  <!--* From a Planning record in the Connections tab on the record's preview or page.  -->

* 次の領域で、Workfront オブジェクトをWorkfront Planning レコードに関連付けることができます。

   * Workfront オブジェクトの「計画」セクションから。

