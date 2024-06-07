---
title: 履歴セクションの概要
description: Adobe Workfront Planning のレコードの右パネルで、レコードに対して行われ、システムによって記録された変更を確認できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 93%

---

# 履歴セクションの概要

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードに関する共同作業を行うことができます。また、レコードに加えられた他の変更やシステムにより記録された他の変更を、このエリアに表示することもできます。

レコードの右側のパネルには、次のセクションが表示されます。

* **コメント**：ユーザーがレコードに追加したコメントおよび返信を表示します。Workfront Planning レコードでのコメントの管理について詳しくは、[レコードのコメントの管理](/help/quicksilver/planning/records/manage-record-comments.md)を参照してください。
* **履歴**：ユーザーがレコードのフィールドに対して行い、システムで記録された変更を表示します。

## レコードの履歴セクションを見つける

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、カードにレコードタイプが表示されます。

1. レコードタイプのカードをクリックします。
レコードタイプのページが開き、そのタイプのすべてのレコードが表示されます。

1. 「**表示**」ドロップダウンメニューからテーブルビューを選択します。
1. テーブルビューでレコードの名前をクリックします。

   レコードのページが開きます。コメントエリアがデフォルトで右パネルに開きます。
1. **履歴を表示**&#x200B;アイコン ![](assets/show-history-icon.png) をクリックします。レコードのフィールドに加えられたすべての変更が、最新の変更を先頭にして右パネルに表示されます。
1. （オプション）**履歴を非表示**&#x200B;アイコン ![](assets/hide-history-icon.png) をクリックすると、右パネルが閉じます。

## 履歴セクションに関する考慮事項

レコードのフィールドに加えた変更は、レコードのページの右パネルにある「履歴」セクションで確認できます。

![](assets/history-area-in-comments.png)

* Workfront Planning は、次の情報を「履歴」セクションに記録します。

   * フィールドの変更

   * 値が変更されたときの、フィールドの古い値と新しい値。古い値は、打ち消し線付きで表示されます。

   * 変更を加えたユーザーのフルネーム

   * 変更が発生した日時スタンプ

* 次のタイプのフィールドでは、常に古いの値（打ち消し線付きの形式）と新しい値が表示されます。

   * テキスト
   * 段落
   * 通貨
   * 日付
   * 数値
   * パーセンテージ
   * 単一選択

* 次のタイプのフィールドは、複数の値のうち少なくとも 1 つが削除された場合にのみ、打ち消し線付きの形式で古い値を表示します。

   * 複数選択
   * リンクされたレコードフィールド
   * ユーザー

  変更によってフィールドに値が追加されただけの場合、古い値は表示されず、新しいフィールド値のみが表示されます。

* チェックボックスタイプのフィールドでは、以前の値が打ち消し線付きの形式で表示されることはありません。フィールドが編集された場合は、変更が行われた時点の状態のみが表示されます。

  Workfront Planning フィールドについて詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

* 次のタイプのフィールドに対する変更は、「履歴」セクションに表示されません。

   * リンクされた（ルックアップ）フィールド
   * 式
   * 作成者
   * 作成日
   * 最終変更者
   * 最終変更日

* フィールドがシステムから削除されても、そのフィールドに対して行われた更新は「履歴」セクションに残ります。レコードの「履歴」セクションでフィールドが削除されたことを示すものはありません。
