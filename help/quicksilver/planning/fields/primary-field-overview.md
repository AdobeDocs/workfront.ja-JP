---
title: プライマリフィールドの概要
description: Adobe Workfront Planning のレコード・タイプのテーブル・ビューで、1 行のテキスト、数値または式フィールドをプライマリ・フィールドとして指定できます。 プライマリフィールドは、そのタイプのレコードのタイトルになります。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 11%

---


# プライマリフィールドの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

主フィールドは、Adobe Workfront Planning のレコードタイプのテーブルビューの最初の列に表示されるフィールドです。

デフォルトでは、名前フィールドはプライマリフィールドです。 ただし、次のタイプのフィールドをレコードのプライマリフィールドとして指定できます。

* 1 行のテキストフィールド
* 数値
* 式

![](assets/another-text-field-as-a-primary-field-highlighted.png)

プライマリフィールドとしてフィールドを指定する方法については、「[ テーブルビューの管理 ](/help/quicksilver/planning/views/manage-the-table-view.md)」を参照してください。

## プライマリフィールドの概要

* プライマリとして指定されたフィールド内の情報は、レコードのタイトルになります。

  >[!NOTE]
  >
  >    Workfront Planning では、「主なフィールド」と「レコードタイトル」という名前は同義語です。 テーブルビューでレコードを表示する場合は、「プライマリフィールド」をお勧めします。


* レコードのタイトルは、次の領域に表示されます。

   * レコードのページとプレビューボックスのヘッダー領域
   * 接続されたレコードフィールド
   * ビュー
* テーブル ビューで主フィールドの移動、非表示、削除を行うことはできません。ただし、別のフィールドを主フィールドとして指定した場合を除きます。
* プライマリフィールドは常にロックされ、テーブルビューの水平スクロールには含まれません。
* テーブルビューのプライマリフィールドを変更すると、それを選択した他のすべてのユーザーのビューに影響します。
* テーブル ビューの主フィールドを変更すると、レコード タイプのすべてのテーブル ビューに影響します。
* プライマリフィールドにリスト表示される値は、レコードのページに常にハイパーリンクされます。
* Workspace <!--<span class="preview">and record type</span>--> に対する投稿以上の権限を持っている場合は、数式フィールドを除くプライマリフィールドの値を編集できます。 数式は、自動的に更新される計算です。
