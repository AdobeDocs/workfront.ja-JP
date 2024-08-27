---
title: フィールドの概要
description: 組織のライフサイクルを反映する新しいフィールドを Adobe Workfront Planning に追加できます。フィールドは、レコードタイプの属性です。
author: Alina
feature: Workfront Planning
role: User, Admin
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 98%

---


# フィールドの概要

{{planning-important-intro}}

組織のライフサイクルを反映する新しいフィールドを Adobe Workfront Planning に追加できます。フィールドは、レコードタイプの属性です。


## Adobe Workfront の計画フィールドに関する考慮事項

* レコードを作成できるのは、レコードタイプのページのテーブルビューのみです。フィールドは、テーブルビューで列として表示されます。レコードタイプに関連付けられているすべてのフィールドは、レコードページにも表示されます。

  テーブルの列（またはレコードフィールド）の管理については、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

  フィールドの管理については、以下の記事も参照してください。

   * [フィールド設定を編集](/help/quicksilver/planning/fields/edit-fields.md)
   * [フィールドを削除](/help/quicksilver/planning/fields/delete-fields.md)

* レコードタイプに関連付けられたフィールドは、そのタイプのすべてのレコードに関連付けることができます。<!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* レコードタイプに関連付けられたフィールドは、別のレコードタイプに追加できません。<!-- this will change when they open the Field library tab when creating a field-->

* 以下の方法で、手動または自動でフィールドを作成できます。

   * 手動：

      * レコードタイプのページのテーブルビューに列を追加にして。テーブルの列は、レコードタイプに関連付けられるフィールドです。これらは、レコードのページに表示されるフィールドと同じです。

        フィールドは、レコードのページから作成することはできません。

      * レコードタイプを接続する。2 つのレコードタイプ間で、または、1 つのレコードタイプと他のアプリケーションのオブジェクトタイプとの間で新しい接続を追加する際に、リンクされるレコードフィールドを作成できます。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        レコードタイプの接続について詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

     <!--* By importing record types using an Excel or CSV file. For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). -->

   * 自動：

     新規のレコードタイプごとにデフォルトで作成される標準フィールドを次に示します。

      * 名前
      * 説明
      * 開始日
      * 終了日
      * ステータス。レコードのステータスのデフォルト値を以下に示します。
         * 開発
         * 予定
         * アクティブ
         * 完了
         * 保留中

        値をさらに追加したり、既存の値の名前を変更したりできます。

     Workfront Planning では、ワークスペースをテンプレートから作成する際にレコードタイプのフィールドが作成されます。詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

* Workfront Planning フィールドには Workfront からアクセスできません。

* レコードタイプを Workfront オブジェクトタイプと関連付け、Workfront オブジェクトからリンクされたフィールドまたは参照フィールドを追加した場合にのみ、Workfront Planning から Workfront フィールドにアクセスできます。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

* フィールドが属するワークスペースに対する管理権限を持っている場合は、自分または他のユーザーが作成したフィールドの設定を表示および更新できます。

* 1 つのレコードタイプに対して最大 500 個のフィールドを設定できます。

* フィールド名は最大 250 文字まで指定できます。

* レコードタイプまたはワークスペースを削除すると、それらに関連付けられたすべてのフィールドとフィールドの値も削除され、復元できなくなります。<!-- this might change with a possible recycle bin solution?!-->
