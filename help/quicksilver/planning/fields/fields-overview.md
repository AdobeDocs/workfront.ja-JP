---
title: フィールドの概要
description: 組織のライフサイクルを反映する新しいフィールドを Adobe Workfront Planning に追加できます。フィールドは、レコードタイプの属性です。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 74%

---


# フィールドの概要

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


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

      * レコードタイプページのテーブル表示で列を追加する場合。 テーブルの列は、レコードタイプに関連付けられるフィールドです。これらは、レコードのページに表示されるフィールドと同じです。

        フィールドは、レコードのページから作成することはできません。

      * レコードタイプを接続する場合。 2 つのレコードタイプ間で、または、1 つのレコードタイプと他のアプリケーションのオブジェクトタイプとの間で新しい接続を追加する際に、リンクされるレコードフィールドを作成できます。

        レコードタイプの接続について詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

      * Workfrontから既存のフィールドを読み込む場合。

        詳しくは、[Adobe Workfrontからのフィールドの読み込み ](/help/quicksilver/planning/fields/import-fields-from-workfront.md) を参照してください。


   * 自動：

      * レコードタイプを作成する場合：

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

        さらに値を追加したり、既存の値の名前を変更したりできます。

      * テンプレートからワークスペースを作成する場合

        詳しくは、[ワークスペースの概要](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

      * Excel または CSV ファイルを使用してレコードタイプを読み込む場合。

        詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

* Workfront Planning フィールドには Workfront からアクセスできません。

* レコードタイプを Workfront オブジェクトタイプと関連付け、Workfront オブジェクトからリンクされたフィールドまたは参照フィールドを追加した場合にのみ、Workfront Planning から Workfront フィールドにアクセスできます。詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

* 自分または他のユーザーが作成したフィールドの設定を表示および更新できます（フィールドが属するワークスペース <span class="preview"> およびレコードタイプ </span> に対する管理権限がある場合）。

* 1 つのレコードタイプに対して最大 500 個のフィールドを設定できます。

* フィールド名は最大 250 文字まで指定できます。

* レコードタイプまたはワークスペースを削除すると、それらに関連付けられたすべてのフィールドとフィールドの値も削除され、復元できなくなります。<!-- this might change with a possible recycle bin solution?!-->
