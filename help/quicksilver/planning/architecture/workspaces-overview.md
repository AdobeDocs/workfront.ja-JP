---
title: ワークスペースの概要
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planningのワークスペースは、組織部門のワークフローに合わせて完全にカスタマイズできます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 28%

---

# ワークスペースの概要

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

ワークスペースは、組織単位で使用されるレコードタイプのコレクションであり、単位の作業ライフサイクルとプロセスを表します。 Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。


![Workspaces ランディングページ管理者アカウント &#x200B;](assets/workspaces-landing-page-admin-account.png)

## ワークスペースに関する考慮事項

* 各部署の固有の仕事の仕方に合わせて、組織内の特定の部署単位でワークスペースを作成できます。
* Workfront Planningには、事前設定されたワークスペースは付属していません。 自社のニーズに応じて作成する必要があります。
* ワークスペースは、次の方法で作成できます。

   * 最初から
   * テンプレートの使用。 テンプレートには、事前設定済みのレコードタイプの数とそのフィールドが含まれています。
   * AIを活用したPlanning Designerを使用します。 この機能は現在Betaにあります。
   * <span class="preview"> マルチワークスペース テンプレート バンドルを使用しています。</span>

  詳しくは、[ワークスペースの概要](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

* ワークスペースとは、組織部門（チーム、グループ、部門、部門）が作業をおこなうフレームワークのことです。 フィールドに関連付けることはできません。 フィールドに関連付けられるのは、ワークスペース内のレコードタイプのみです。

  詳しくは、[&#x200B; レコードタイプの概要](/help/quicksilver/planning/architecture/overview-of-record-types.md)を参照してください。
* Workfront ライセンスに応じて、ワークスペースはプランニング エリアの次のタブに表示されます。

   * システム管理者の場合、ワークスペースは次のタブに表示されます。

      * **自分が所属するワークスペース**：作成したワークスペースまたは共有されているワークスペースを表示します。
      * **その他のワークスペース**：システム内のその他すべてのワークスペースが表示されます。

   * その他のすべてのユーザーに対しては、そのユーザーが作成したワークスペースと、そのユーザーと共有された他のワークスペースがワークスペース領域に表示されます。

* ワークスペースに含まれるレコードタイプは、作業ライフサイクルと組織単位の概念を反映している必要があります。

  例えば、ユニットの作業オブジェクトがキャンペーン、製品、地域の場合、そのユニットのワークスペースにはキャンペーン、製品、地域のレコードタイプを含める必要があります。
* ワークスペースを作成した場合、自分だけがワークスペースにアクセスし、管理する権限を持っています。他のユーザーが同じスペースで共同作業できるようにするには、他のユーザーと共有する必要があります。

  詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。

  システム管理者は、自分が作成していないワークスペースも含め、すべてのワークスペースを管理できます。

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Workfront Planningのインスタンスで作成できるワークスペースオブジェクトの数には制限があります。 詳しくは、[Adobe Workfront計画オブジェクト制限の概要](/help/quicksilver/planning/general/limitations-overview.md)を参照してください。
