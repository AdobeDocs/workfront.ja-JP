---
title: 履歴セクションの概要
description: AdobeMaestro のレコードの右側のパネルで、レコードに対して行われた変更や記録を確認できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 4%

---


# 履歴セクションの概要

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

レコードの右側のパネルにコメントや返信を追加することで、AdobeMaestro レコードで共同作業を行うことができます。 また、この領域で、記録に加えられた他の変更や記録を表示することもできます。

レコードの右側のパネルには、次のセクションが表示されます。

* **コメント**：ユーザーがレコードに追加したコメントおよび返信を表示します。 Maestro レコードでのコメント管理の詳細については、 [レコードコメントの管理](/help/quicksilver/maestro/records/manage-record-comments.md).
* **履歴**：ユーザーがレコードフィールドに対しておこなった、システムで記録された変更を表示します。

## レコードの履歴セクションを見つける

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

1. 次の場所からテーブルビューを選択します。 **表示** ドロップダウンメニュー。
1. テーブルビューでレコードの名前をクリックします。

   レコードの **詳細** ページが開きます。 「コメント」領域は、デフォルトでは右側のパネルに開きます。
1. 次をクリック： **履歴を表示** アイコン ![](assets/show-history-icon.png). レコードのフィールドに加えたすべての変更が、最新の変更から始まる右側のパネルに表示されます。
1. （オプション） **履歴を非表示** アイコン ![](assets/hide-history-icon.png) をクリックして、右側のパネルを閉じます。

## 「履歴」セクションに関する考慮事項

レコードのフィールドに加えた変更は、オペレーショナルレコードまたは分類の [ 詳細 ] ページの右側のパネルにある [ 履歴 ] セクションで確認できます。

![](assets/history-area-in-comments.png)

* Maestro は、次の情報を History セクションに記録します。

   * フィールドの変更

   * 値が変更されたときの、フィールドの古い値と新しい値。 古い値は取り消し線形式で表示されます。

   * 変更を加えたユーザーの氏名

   * 変更が発生した日時の日時スタンプ。

* 次のタイプのフィールドでは、常に以前の値（取り消し線形式）と新しい値が表示されます。

   * テキスト
   * 段落
   * 通貨
   * 日付
   * 数値
   * パーセンテージ
   * 単一選択

* 次のタイプのフィールドは、複数の値のうち少なくとも 1 つが削除された場合にのみ、取り消し線形式の古い値を表示します。

   * 複数選択
   * リンクされたレコードフィールド
   * 人物

  変更によってフィールドに値が追加されただけの場合、古い値は表示されず、新しいフィールド値のみが表示されます。

* チェックボックスタイプのフィールドでは、以前の値が取り消し線形式で表示されることはありません。 フィールドが編集された場合は、変更が行われた時点の現在の状態のみが表示されます。

  Maestro フィールドについて詳しくは、 [フィールドの作成](/help/quicksilver/maestro/fields/create-fields.md).

* 次のタイプのフィールドに対する変更は、「履歴」セクションには表示されません。

   * リンクされた（参照）フィールド
   * 数式
   * 作成者
   * 作成日
   * 最終変更者
   * 最終変更日

* フィールドがシステムから削除されても、そのフィールドに対しておこなわれた更新は「履歴」セクションに残ります。 レコードの「履歴」セクションでフィールドが削除されたことを示すものはありません。