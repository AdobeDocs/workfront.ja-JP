---
title: フィールドの概要
description: 組織のライフサイクルを反映する新しいフィールドを Adobe Workfront Planning に追加できます。フィールドは、レコードタイプの属性です。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 100%

---

# フィールドの概要

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

組織のライフサイクルを反映する新しいフィールドを Adobe Workfront Planning に追加できます。フィールドは、レコードタイプの属性です。


## Adobe Workfront の計画フィールドに関する考慮事項

* レコードを作成できるのは、レコードタイプのページのテーブルビューのみです。フィールドは、テーブルビューで列として表示されます。レコードタイプに関連付けられているすべてのフィールドは、レコードページにも表示されます。

  テーブルの列（またはレコードフィールド）の管理については、[テーブルビューの管理](../views/manage-the-table-view.md)を参照してください。

  フィールドの管理について詳しくは、次の記事も参照してください。

   * [フィールドの編集](../fields/edit-fields.md)
   * [フィールドの削除](../fields/delete-fields.md)

* レコードタイプに関連付けられているフィールドを、そのタイプのすべてのレコードに関連付けることができます。<!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* レコードタイプに関連付けられたフィールドを別のレコードタイプに追加することはできません。<!-- this will change when they open the Field library tab when creating a field-->

* 以下の方法で、フィールドを手動で、または自動的に作成できます。

   * 手動：

      * レコードタイプのページのテーブルビューで列を追加する。テーブルの列は、レコードタイプに関連付けられるフィールドです。これらは、レコードのページに表示されるフィールドと同じです。

        フィールドは、レコードのページから作成することはできません。

      * レコードタイプを接続する。2 つのレコードタイプ間で、または、1 つのレコードタイプと他のアプリケーションのオブジェクトタイプとの間で新しい接続を追加する際に、リンクされるレコードフィールドを作成できます。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        レコードタイプの接続について詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

      * Excel ファイルまたは CSV ファイルを使用してレコードタイプを読み込む。詳しくは、[レコードタイプの作成](../architecture/create-record-types.md)を参照してください。

   * 自動：

     新規のレコードタイプごとにデフォルトで作成される標準フィールドを次に示します。

      * 名前
      * 説明
      * 開始日
      * 終了日
      * ステータスレコードステータスのデフォルト値は次のとおりです。
         * 開発
         * 予定
         * アクティブ
         * 完了
         * 保留中

        値をさらに追加したり、既存の値の名前を変更したりできます。

     Workfront Planning では、ワークスペースをテンプレートから作成する際にレコードタイプのフィールドが作成されます。詳しくは、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。

* Workfront Planning フィールドには Workfront からアクセスできません。

* レコードタイプを Workfront オブジェクトタイプと関連付け、Workfront オブジェクトからリンクされたフィールドまたは参照フィールドを追加した場合にのみ、Workfront Planning から Workfront フィールドにアクセスできます。詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

* ご自分または他のユーザーが作成したフィールドの設定を表示および更新できます（フィールドが属するワークスペースに対する管理権限がある場合）。

* 1 つのレコードタイプに対して最大 500 個のフィールドを持つことができます。

* フィールド名は最大 250 文字まで指定できます。

* レコードタイプまたはワークスペースを削除すると、それらに関連付けられたすべてのフィールドとフィールドの値も削除され、復元できなくなります。<!-- this might change with a possible recycle bin solution?!-->
