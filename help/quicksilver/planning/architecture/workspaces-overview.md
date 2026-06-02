---
title: ワークスペースの概要
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。 Adobe Workfront Planningのワークスペースは、組織部門のワークフローに合わせて完全にカスタマイズできます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: bd1c8dfc4b03b4b8d9948da278406addf801d226
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 25%

---

# ワークスペースの概要

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

ワークスペースは、組織単位で使用されるレコードタイプのコレクションであり、単位の作業ライフサイクルとプロセスを表します。 Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

<!--update screenshot with production, it was broken at Preview-->

![Workspaces ランディングページ管理者アカウント &#x200B;](assets/workspaces-landing-page-admin-account.png)

## ワークスペースに関する考慮事項

* 各部署の固有の仕事の仕方に合わせて、組織内の特定の部署単位でワークスペースを作成できます。
* Workfront Planningには、事前設定されたワークスペースは付属していません。 自社のニーズに応じて作成する必要があります。
* ワークスペースは、次の方法で作成できます。

   * 最初から
   * テンプレートの使用。 テンプレートには、事前設定済みのレコードタイプの数とそのフィールドが含まれています。
   * AIを活用したPlanning Designerを使用します。 この機能は現在Betaにあります。
   * マルチワークスペーステンプレートバンドルの使用。

  詳しくは、[ワークスペースの概要](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

* ワークスペースとは、組織部門（チーム、グループ、部門、部門）が作業をおこなうフレームワークのことです。 フィールドに関連付けることはできません。 フィールドに関連付けられるのは、ワークスペース内のレコードタイプのみです。

  詳しくは、[&#x200B; レコードタイプの概要](/help/quicksilver/planning/architecture/overview-of-record-types.md)を参照してください。
* ワークスペースは、プランニング領域の次のタブに表示されます。

   * **自分が所属するワークスペース**：作成したワークスペースまたは共有されているワークスペースを表示します。
   * **その他のワークスペース**：システム内のその他すべてのワークスペースが表示されます。 これは、システム管理者のみが使用できます。

  <div class="preview">

   * **サンプルワークスペース**：ベストプラクティスワークスペースの組み込み例を表示します。 ワークスペース、レコードタイプを編集したり、レコードやフィールドを追加したりすることはできませんが、他のユーザーとビューを追加、編集、共有することはできます。

  </div>

  >[!NOTE]
  >
  ><span class="preview"> サンプル ワークスペースを編集するのではなく、サンプル ワークスペースを参照して独自のワークスペースを作成することをお勧めします。 マルチワークスペーステンプレートバンドルを使用して、「サンプルワークスペース」タブにリストされているワークスペースと同じワークスペースを作成します。 詳しくは、[&#x200B; ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)の記事の「ベストプラクティスのマルチワークスペーステンプレートバンドルを使用した複数のワークスペースの作成」の節を参照してください。</span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* ワークスペースに含まれるレコードタイプは、作業ライフサイクルと組織単位の概念を反映している必要があります。

  例えば、ユニットの作業オブジェクトがキャンペーン、製品、地域の場合、そのユニットのワークスペースにはキャンペーン、製品、地域のレコードタイプを含める必要があります。
* ワークスペースを作成した場合、自分だけがワークスペースにアクセスし、管理する権限を持っています。 他のユーザーが同じスペースで共同作業できるようにするには、他のユーザーと共有する必要があります。

  詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。

  システム管理者は、自分が作成していないワークスペースも含め、すべてのワークスペースを管理できます。

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Workfront Planningのインスタンスで作成できるワークスペースオブジェクトの数には制限があります。 詳しくは、[Adobe Workfront計画オブジェクト制限の概要](/help/quicksilver/planning/general/limitations-overview.md)を参照してください。
