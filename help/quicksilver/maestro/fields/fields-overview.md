---
title: フィールドの概要
description: 組織のライフサイクルを反映する新しいフィールドをAdobeマエストロに追加できます。 フィールドは、レコードタイプの属性です。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6d1d3d82e15f4232ff81294d9094c2683b01ca89
workflow-type: tm+mt
source-wordcount: '539'
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

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

組織のライフサイクルを反映する新しいフィールドをAdobeマエストロに追加できます。 フィールドは、レコードタイプの属性です。


## マエストロフィールドに関する考慮事項

* フィールドは、レコードタイプのページのテーブルビューからのみ作成できます。 フィールドは、テーブル表示で列として表示されます。 レコードの種類に関連付けられているすべてのフィールドも、その種類の各レコードの詳細ページに表示されます。

  テーブルの列（またはレコードのフィールド）の管理については、 [テーブル表示の管理](../views/manage-the-table-view.md).

  フィールドの管理の詳細については、次の記事も参照してください。

   * [フィールドを編集](../fields/edit-fields.md)
   * [フィールドを削除](../fields/delete-fields.md)

* レコードタイプに関連付けられたフィールドは、そのタイプのすべてのレコードに関連付けることができます。 <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* レコードタイプに関連付けられたフィールドを別のレコードタイプに追加することはできません。 <!-- this will change when they open the Field library tab when creating a field-->

* 次の方法で、手動または自動でフィールドを作成できます。

   * 手動:

      * レコードタイプのページの [ テーブル ] ビューに列を追加する。 テーブルの列は、レコードタイプに関連付けられたフィールドです。 これらは、レコードの詳細ページに表示されるフィールドと同じです。

        レコードの詳細ページからは、フィールドを作成できません。

        この記事では、フィールドを手動で作成する方法について説明します。

      * レコードタイプを接続する。 2 つの Maestro レコードタイプ間の新しい接続を追加するときに、リンクされたレコードフィールドを作成できます。また、他のアプリケーションからレコードタイプとオブジェクトタイプを追加すると、リンクされたレコードフィールドを作成できます。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Maestro レコードタイプの接続について詳しくは、 [レコードタイプを接続](../architecture/connect-record-types.md).

      * Excel または CSV ファイルを使用してレコードタイプをインポートする。 詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

   * 自動:

      * デフォルトでは、レコードタイプを作成するたびに使用されます。

        次に、新しい各操作レコードタイプに対してデフォルトで作成される標準フィールドを示します。

         * 名前
         * 説明
         * 開始日
         * 終了日
         * ステータス. レコードのステータスのデフォルト値は次のとおりです。
            * 開発
            * 予定
            * アクティブ
            * 完了
            * 保留中

           他の値を追加したり、既存の値の名前を変更したりできます。

        以下は、新しい分類レコードタイプごとにデフォルトで作成される標準フィールドです。

         * 名前 <!--will more be added? If not, consider rephrasing this bullet-->

      * テンプレートからワークスペースを作成する場合。 テンプレートからワークスペースを作成すると、Maestro はオペレーショナルレコードタイプと分類のフィールドを作成します。 詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

* Maestro フィールドはWorkfrontからアクセスできません。

* Workfrontのフィールドは、Maestro のレコードタイプをWorkfrontのオブジェクトタイプに接続し、Workfrontのオブジェクトからリンクされたフィールドまたはルックアップフィールドを追加した場合にのみ、Maestro からアクセスできます。 詳しくは、 [レコードタイプを接続](../architecture/connect-record-types.md).

* 自分または他のユーザーが作成したフィールドの設定を表示および更新できます。 <!--this will change with access/ permissions-->

* 1 つのレコードタイプに対して最大 500 個のフィールドを指定できます。

* フィールド名は 250 文字までです。

* オペレーショナルレコードタイプ、分類、またはワークスペースを削除すると、それらに関連付けられたすべてのフィールドとフィールドの値も削除され、復元できなくなります。 <!-- this might change with a possible recycle bin solution?!-->