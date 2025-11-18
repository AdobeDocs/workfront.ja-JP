---
title: Adobe Workfront Planning のアクセスの概要
description: Adobe Workfront Planning を使用する際、組織内のすべてのユーザーが同じアクセス権と権限を持っているわけではありません。 ここでは、Adobe Workfront Planning の機能を使用するために必要になるアクセス権およびアクセス権について説明します。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 26%

---


# Adobe Workfront Planning のアクセスの概要

<!--leave the global record type reference in yellow till Jan 2026-->

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

>[!IMPORTANT]
>
>この記事では、Adobe Workfrontの追加機能であるAdobe Workfront Planning について説明します。
>
>Workfront Planning が機能にアクセスするには、会社がパッケージを追加購入する必要があります。
>
>詳しくは、アカウントマネージャーにお問い合わせください
>
>Adobe Workfront Planning の詳細については、[Workfront Planning の基本を学ぶ ](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

Adobe Workfront Planning を使用するには、ライセンスと共有権限の制約があります。

ここでは、Workfront Planning の機能を使用するために必要なアクセス権と設定について説明します。

## アクセス要件

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Workfront Planning を使用するには、次のアクセス権が必要です：

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
   <p>任意のWorkfrontおよび Planning パッケージ</p>
   <p>任意のワークフローおよび計画パッケージ</p>

<p><b>メモ</b></p>

<p>接続可能なレコードタイプへのアクセスの場合：</p>
   <ul><li><p>任意のWorkfront パッケージと Planning パッケージ</p></li>
   <li><p>任意のワークフローと Planning PrimeおよびUltimate パッケージ</p></li></ul>

<div class="preview">
   <p>グローバルレコードタイプへのアクセスの場合：</p>
   <ul><li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
   <li><p>任意のワークフローパッケージと Planning PrimeおよびUltimate パッケージ</p></li></ul> </td></tr>
   </div>
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p>
   <p><b>重要</b></p>
   <p>Adobe Identity Management System （IMS）に追加されたユーザーのみが、権限を付与され、計画フィールドに追加できます。</p>
   <p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
   <ul><li><p>すべて（Workfront計画情報を表示する場合）</p></li>
   <li><p>標準：ワークスペースとビューを作成します。</p></li></ul>
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
   <li><p>自分が作成していないワークスペース、レコード タイプ、およびビューに対して、それらおよびオブジェクトにアクセスするための表示以上の権限。</p></li>
   <li><p>作成しなかったワークスペースおよびレコードの種類に対する投稿以上のアクセス許可を編集し、レコードの種類およびレコードを作成、編集、または削除します。</p></li>
   <li><p>自分が作成していないビューに対する投稿以上の権限、ビューの編集、削除、共有</p>
   </li>
    <li><p>システム管理者は、自分が作成していないワークスペースを管理できます。 </p></li>
    <li><p>システム管理者は、自分が作成していないビューにアクセスすることはできません。 </p></li></ul>
   <p>Workfront Planning オブジェクトの共有権限について詳しくは、
<a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a>を参照してください。 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> 
<p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p>
<p> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、次の領域に Planning オプションを含むレイアウト テンプレートを割り当てる必要があります。</p>
   <ul><li>メインメニュー</li>
   <li>プロジェクト、ポートフォリオおよびプログラムの左側のパネル</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


## レイアウトテンプレートを使用した計画エリアの共有

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

標準ユーザーとシステム管理者は、次の領域で、デフォルトで Planning 領域を有効にします。

* メインメニュー
* プロジェクト、ポートフォリオまたはプログラムの左側のパネル

他のWorkfront ライセンスがあり、Workfront Planning の作業にコントリビューションする必要がある場合は、システム管理者から Planning エリアを追加してもらう必要があります。

管理者は、ユーザーを変更してレイアウト・テンプレートに割り当てることにより、プランニング・オプションを次の領域に追加できます。

* メインメニュー
* ランディングページ
* プロジェクト、ポートフォリオおよびプログラムの左側のパネル
* ピン留め

Workfront インスタンスのユーザーからWorkfront Planning エリアを追加または削除するには、次の手順に従います。

1. Workfront 管理者として **Workfront** にログインします。

1. **メインメニュー**/**設定**/**インターフェイス**/**レイアウトテンプレート** に移動して、レイアウトテンプレートを開くか作成します。

   レイアウトテンプレートのカスタマイズについて詳しくは、[ レイアウトテンプレートの作成と管理 ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) を参照してください。

1. Workfront Planning へのアクセス権を付与するユーザーにレイアウトテンプレートを割り当てます。

   詳しくは、[レイアウトテンプレートにユーザーを割り当て](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

   テンプレートに割り当てられたすべてのユーザーは、メインメニューから Workfront Planning にアクセスできるようになります。

   ユーザーは、ワークスペース、レコードタイプ、レコードおよびフィールドの作成を開始できます。

## ユーザーへのライセンスの割り当て

ユーザーの編集または作成時にアクセスレベルを設定する際に、ユーザーにライセンスを割り当てることができます。

詳しくは、[ ユーザープロファイルの編集 ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) を参照してください。

## アクセスレベルを設定

Workfront Planning には、Workfrontのアクセスレベル制御はありません。

あらゆるタイプのWorkfront ライセンスを持つユーザーは、Workfront Planning にアクセスできます。

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 権限の付与

Workfront Planning の次のエンティティに権限を付与できます。

* ワークスペース
* レコードタイプ
* ビュー

詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

Adobe WorkfrontのライセンスタイプはWorkfront Planning 権限と連携し、Workfront Planning オブジェクトの表示、投稿、管理に対するアクセス権を付与します。

ライセンスタイプが Workfront Planning オブジェクトの権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。


