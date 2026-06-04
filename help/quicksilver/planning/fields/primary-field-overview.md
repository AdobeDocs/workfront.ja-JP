---
title: プライマリフィールドの概要
description: Adobe Workfront Planningのレコードタイプのテーブルビューでは、1行のテキスト、数値、または数式フィールドをプライマリフィールドとして指定できます。 プライマリフィールドは、そのタイプのレコードのタイトルになります。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LAxXoG6cLqWJfEn5FQQDVQ7JO9-Fql0o56Q9qUIi2Gs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 307
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

![ プライマリフィールドとしてハイライト表示された別のテキストフィールド ](assets/another-text-field-as-a-primary-field-highlighted.png)

フィールドをプライマリフィールドとして指定する方法について詳しくは、[ テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

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
