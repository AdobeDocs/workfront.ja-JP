---
title: フィールドの概要
description: 組織のライフサイクルを反映した新しいフィールドをAdobe Workfront Planning に追加できます。 フィールドは、レコードタイプの属性です。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 2%

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

{{maestro-important-intro}}

組織のライフサイクルを反映した新しいフィールドをAdobe Workfront Planning に追加できます。 フィールドは、レコードタイプの属性です。


## Adobe Workfront Planning フィールドに関する考慮事項

* フィールドは、レコードタイプのページのテーブルビューからのみ作成できます。 フィールドは、テーブル表示で列として表示されます。 レコードタイプに関連付けられているすべてのフィールドも、レコードページに表示されます。

  テーブルの列（またはレコードのフィールド）の管理については、 [テーブル表示の管理](../views/manage-the-table-view.md).

  フィールドの管理の詳細については、次の記事も参照してください。

   * [フィールドを編集](../fields/edit-fields.md)
   * [フィールドを削除](../fields/delete-fields.md)

* レコードタイプに関連付けられたフィールドは、そのタイプのすべてのレコードに関連付けることができます。 <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* レコードタイプに関連付けられたフィールドを別のレコードタイプに追加することはできません。 <!-- this will change when they open the Field library tab when creating a field-->

* 次の方法で、手動または自動でフィールドを作成できます。

   * 手動：

      * レコードタイプのページのテーブルビューに列を追加する。 テーブルの列は、レコードタイプに関連付けられたフィールドです。 これらは、レコードのページに表示されるフィールドと同じです。

        レコードのページからフィールドを作成することはできません。

      * レコードタイプを接続する。 2 つのレコードタイプ間の新しい接続を追加するときに、リンクされたレコードフィールドを作成できます。また、他のアプリケーションからレコードタイプとオブジェクトタイプを追加すると、リンクされたレコードフィールドを作成できます。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        レコードタイプの接続の詳細については、「 [レコードタイプを接続](../architecture/connect-record-types.md).

      * Excel または CSV ファイルを使用してレコードタイプをインポートする。 詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

   * 自動：

     次に、新しいレコードタイプごとにデフォルトで作成される標準フィールドを示します。

      * 名前
      * 説明
      * 開始日
      * 終了日
      * ステータス。 レコードのステータスのデフォルト値は次のとおりです。
         * 開発
         * 予定
         * アクティブ
         * 完了
         * 保留中

        他の値を追加したり、既存の値の名前を変更したりできます。

     Workfront Planning では、テンプレートからワークスペースを作成する際に、レコードタイプ用のフィールドが作成されます。 詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

* Workfront Planning フィールドにWorkfrontからアクセスできません。

* WorkfrontのフィールドにWorkfront Planning からアクセスできるのは、レコードタイプをWorkfrontのオブジェクトタイプに接続し、Workfrontのオブジェクトからリンクされたフィールドや参照フィールドを追加する場合のみです。 詳しくは、 [レコードタイプを接続](../architecture/connect-record-types.md).

* フィールドが属するワークスペースに対する管理権限を持っている場合は、自分または他のユーザーが作成したフィールドの設定を表示および更新できます。

* 1 つのレコードタイプに対して最大 500 個のフィールドを指定できます。

* フィールド名は 250 文字までです。

* レコードタイプまたはワークスペースを削除すると、それらに関連付けられているすべてのフィールドとフィールドの値も削除され、復元できなくなります。 <!-- this might change with a possible recycle bin solution?!-->
