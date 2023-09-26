---
title: Workspace テンプレートのリスト
description: ワークスペースは、チームが使用するオペレーショナルレコードタイプと分類の集まりで、チームの作業ライフサイクルを表します。 Maestro には、ワークスペースの作成時に基本的なレコードタイプ、分類、フィールドを使い始めるための一連のテンプレートが用意されています。
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: List of available workspace templates
description: You can use templates to create workspaces. This article provides a list of available workspace templates
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
---

-->

# Workspace テンプレートのリスト

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Adobe・マエストロでは、ワークスペースは、チームが使用する操作レコード・タイプと分類の集まりで、チームの作業ライフサイクルを表します。

Maestro には、ワークスペースの作成時に基本的なレコードタイプ、分類、フィールドを使い始めるための一連のテンプレートが用意されています。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).

この記事では、Maestro で使用できる Workspace テンプレートについて説明します。

## Maestro テンプレートに関する考慮事項

* 各テンプレートには、一連のオペレーショナル・レコード・タイプと分類が用意されています。 詳しくは、 [レコード・タイプと分類の概要](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).
* 各オペレーショナルレコードタイプと分類には、一連のフィールドが用意されています。 これらのフィールドの一部は、他の Maestro レコードタイプとの接続です。
* 任意のテンプレートをカスタマイズできます。

<!-- I modeled this article by the "List of available Blueprints" and that articles does not have an Access area

## Access requirements

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

-->

## Maestro Workspace テンプレート

以下は、Maestro の Workspace テンプレートと、それらが含むフィールドの数です。

* **マーケティング管理**：このテンプレートを使用すると、すべてのマーケティングキャンペーンを管理できます。 テンプレートには次の機能が付属しています。

   * オペレーショナルレコードのタイプ：

      * **マーケティングプラン**: 7 個のフィールドと 5 個のリンクフィールド
      * **Campaign**: 9 フィールドおよび 7 リンクフィールド
      * **プログラム**: 9 フィールドおよび 5 リンクフィールド
      * **アクティビティ**: 6 個のフィールドと 5 個のリンクフィールド
   * 分類:
      * **対象ユーザ**: 3 フィールドおよび 3 リンクフィールド
      * **セグメント**: 5 フィールド、1 リンクフィールド
      * **顧客ジャーニー**: 4 フィールド
      * **製品提供**: 3 フィールド、1 リンクフィールド
      * **地域**: 1 フィールド
      * **戦術**: 1 フィールド
      * **チャネル**: 1 フィールド、1 リンクフィールド
      * **ビジネスユニット**: 1 フィールド
      * **関数**: 1 フィールド

* **セールス管理**：販売プロセスを合理化し、効率を高める包括的な販売システムを構築できます。 テンプレートには次の機能が付属しています。

   * オペレーショナルレコードのタイプ：

      * **商談**: 7 個のフィールドと 4 個のリンクフィールド
      * **アクティビティ**: 4 フィールド、5 リンクフィールド
      * **Campaign**: 5 フィールド、3 リンクフィールド
   * 分類:
      * **アカウント**: 4 フィールドと 3 リンクフィールド
      * **リード**:12 フィールドと 2 つのリンクされたフィールド
      * **連絡先**:10 個のフィールドと 2 個のリンクされたフィールド
      * **地域**: 1 個のフィールドと 2 個のリンク済みフィールド
      * **業界**: 1 フィールド
      * **購買センター**: 1 フィールド
      * **製品/サービス**: 1 フィールド
      * **競合他社**: 1 フィールド

* **製品管理**：このテンプレートを使用して、構造化された効率的な製品管理プロセスを作成できます。 テンプレートには次の機能が付属しています。

   * オペレーショナルレコードのタイプ：

      * **テーマ**: 8 個のフィールドと 2 個のリンク済みフィールド
      * **Initiative**: 8 個のフィールドと 2 個のリンク済みフィールド
      * **叙事詩**: 9 フィールドおよび 3 リンクフィールド
      * **ユーザーストーリー**: 9 フィールドおよび 2 リンクフィールド

   * 分類:

      * **顧客**: 6 個のフィールドと 1 個のリンク済みフィールド
      * **スプリント**: 7 個のフィールドと 1 個のリンクフィールド
      * **製品チーム**: 3 フィールド
      * **機能リクエスト**: 8 個のフィールドと 1 個のリンクフィールド
      * **業界**: 1 フィールド、1 リンクフィールド


