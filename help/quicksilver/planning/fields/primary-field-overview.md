---
title: プライマリフィールドの概要
description: Adobe Workfront Planningのレコードタイプのテーブルビューでは、1行のテキスト、数値、または数式フィールドをプライマリフィールドとして指定できます。 プライマリフィールドは、そのタイプのレコードのタイトルになります。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 12%

---


# プライマリフィールドの概要

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

プライマリフィールドは、Adobe Workfront Planningのレコードタイプのテーブルビューの最初の列に表示されるフィールドです。

デフォルトでは、「名前」フィールドがプライマリフィールドになります。 ただし、次のタイプのフィールドは、レコードのプライマリフィールドとして指定できます。

* 1行テキストフィールド
* 数値
* 式

![&#x200B; プライマリフィールドとしてハイライト表示された別のテキストフィールド &#x200B;](assets/another-text-field-as-a-primary-field-highlighted.png)

フィールドをプライマリフィールドとして指定する方法について詳しくは、[&#x200B; テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

## プライマリフィールドの概要

* プライマリとして指定されたフィールド内の情報は、レコードのタイトルになります。

  >[!NOTE]
  >
  >    「プライマリフィールド」および「レコードタイトル」という名前は、Workfront Planningでは同義語です。 「プライマリフィールド」は、テーブルビューでレコードを表示する場合に適しています。


* レコードのタイトルは、次の領域に表示されます。

   * レコードのページとプレビューボックスのヘッダー領域
   * 接続されたレコードフィールド
   * ビュー
* 別のフィールドをプライマリフィールドとして指定しない限り、テーブルビューのプライマリフィールドを移動、非表示、または削除することはできません。
* プライマリフィールドは常にロックされ、テーブルビューの水平スクロールには含まれません。
* テーブルビューのプライマリフィールドを変更すると、それを選択した他のすべてのユーザーのビューに影響します。
* テーブルビューのプライマリフィールドを変更すると、レコードタイプのすべてのテーブルビューに影響します。
* プライマリフィールドにリスト表示される値は、レコードのページに常にハイパーリンクされます。
* ワークスペースおよびレコードタイプに対するContribute以上の権限がある場合は、数式フィールドを除くプライマリフィールドの値を編集できます。 式は、自動的に更新される計算です。
