---
title: Adobe Workfront計画アクセスの概要
description: 組織内のすべてのユーザーが、Adobe Workfront Planningを使用するための同じアクセス権と権限を持つわけではありません。 ここでは、Adobe Workfront Planningの機能を使用するために必要なアクセス権と権限について説明します。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 31%

---


# Adobe Workfront Planning へのアクセスの概要

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfront の追加機能である Adobe Workfront Planning に関するものです。
>
>自社でWorkfront計画の機能にアクセスするには、追加のパッケージを購入する必要があります。
>
>詳しくは、アカウントマネージャーにお問い合わせください
>
>Workfront Planning について詳しくは、[Adobe Workfront Planning の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。

Adobe Workfront Planning を使用するには、ライセンスと共有権限の制約があります。

ここでは、Workfront Planningの機能を使用するために必要なアクセス権と設定について説明します。

## アクセス要件

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Workfront Planningを使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
 <tr>
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td>
   <td>
   <p>任意のWorkfrontおよびプランニングパッケージ</p>
   <p>任意のワークフローとプランニングパッケージ</p>

<p><b>メモ</b></p>

<p>接続可能なレコードタイプにアクセスする場合：</p>
   <ul><li><p>任意のWorkfront パッケージとプランニングパッケージ</p></li>
   <li><p>任意のワークフローとプランニング PrimeとUltimateのパッケージ</p></li></ul>

<p>グローバルレコードタイプにアクセスする場合：</p>
   <ul><li><p>任意のWorkfront パッケージとPlanning Plus パッケージ</p></li>
   <li><p>任意のワークフローパッケージとプランニング PrimeおよびUltimate パッケージ</p></li></ul> </td></tr>

<!--
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  -->

<tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
   <ul><li><p>任意：Workfront計画の情報を表示します</p></li>
   <li><p>標準：ワークスペースとビューを作成します</p></li></ul>
    </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <ul>
   <li><p>ワークスペース、レコードタイプ、およびワークスペースとそのオブジェクトにアクセスするために作成しなかったビューまたはそれ以上の権限。</p></li>
   <li><p>ワークスペースおよびレコードタイプを編集したり、レコードタイプおよびレコードを作成、編集または削除したりするために、作成しなかったレコードタイプおよびレコードタイプに対して、より権限の大きい権限を付与します。</p></li>
   <li><p>作成していないビューに対して権限を付与したり、編集、削除、共有したりできます</p>
   </li>
    <li><p>システム管理者は、自分が作成していないワークスペースを管理できます。 </p></li>
    <li><p>システム管理者は、作成しなかったビューにアクセスできません。 </p></li></ul>
   <p>Workfront Planning オブジェクトの共有権限について詳しくは、
<a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a>を参照してください。 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> 
<p>標準ユーザーとシステム管理者は、デフォルトでプランニング領域を有効にできます。</p>
<p> ライトまたはコントリビューターライセンスを持つユーザーには、次の領域に「計画」オプションを含むレイアウトテンプレートを割り当てる必要があります。</p>
   <ul><li>メインメニュー</li>
   <li>プロジェクト、ポートフォリオ、プログラムの左側のパネル</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


## レイアウトテンプレートを使用した計画領域の共有

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

標準ユーザーとシステム管理者は、次の領域でデフォルトで有効になっているプランニング領域を持っています。

* メインメニュー
* プロジェクト、ポートフォリオ、またはプログラムの左側のパネル

他のWorkfront ライセンスがあり、Workfront計画作業にコントリビューションする必要がある場合は、システム管理者がプランニング領域を追加する必要があります。

管理者は、レイアウトテンプレートを変更して割り当てることで、次の領域に「計画」オプションを追加できます。

* メインメニュー
* ランディングページ
* プロジェクト、ポートフォリオ、およびプログラムの左側のパネル
* ピン留め

Workfront インスタンスのユーザーにWorkfront計画領域を追加または削除するには、次の手順を実行します。

1. Workfront 管理者として **Workfront** にログインします。

1. **メインメニュー** > **セットアップ** > **インターフェイス** > **レイアウトテンプレート**&#x200B;に移動し、レイアウトテンプレートを開くか作成します。

   レイアウトテンプレートのカスタマイズについて詳しくは、[&#x200B; レイアウトテンプレートの作成と管理](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

1. Workfront Planning へのアクセス権を付与するユーザーにレイアウトテンプレートを割り当てます。

   詳しくは、[レイアウトテンプレートにユーザーを割り当て](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

   テンプレートに割り当てられたすべてのユーザーは、メインメニューから Workfront Planning にアクセスできるようになります。

   ユーザーは、ワークスペース、レコードタイプ、レコードおよびフィールドの作成を開始できます。

## ユーザーへのライセンスの割り当て

ユーザーの編集または作成中にアクセスレベルを設定するときに、ユーザーにライセンスを割り当てることができます。

詳しくは、[ユーザーのプロファイルの編集](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## アクセスレベルの設定

Workfront Planningには、Workfrontのアクセスレベル制御はありません。

任意の種類のWorkfront ライセンスを持つユーザーは、Workfront Planningにアクセスできます。

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 権限の付与

Workfront Planningでは、次のエンティティに権限を付与できます。

* ワークスペース
* レコードタイプ
* ビュー
  <!--move this above Views: * <span class="preview">Records</span>-->

詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

Adobe Workfrontのライセンスタイプは、Workfrontプランニングの権限と連携して、Workfront プランニングオブジェクトの表示、提供、管理を行う権限を付与します。

ライセンスタイプが Workfront Planning オブジェクトの権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。


