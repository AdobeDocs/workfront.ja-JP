---
title: Adobe Workfront Planning のアクセスの概要
description: Adobe Workfront Planning を使用する際、組織内のすべてのユーザーが同じアクセス権と権限を持っているわけではありません。 ここでは、Adobe Workfront Planning の機能を使用するために必要になるアクセス権およびアクセス権について説明します。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 3550d7addcc0bb790f15d141d9470e0b75f940a6
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 28%

---


# Adobe Workfront Planning のアクセスの概要

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

>[!IMPORTANT]
>
>この記事では、Adobe Workfrontの追加機能であるAdobe Workfront Planning について説明します。
>
>Workfront Planning が機能にアクセスするには、会社がライセンスを追加購入する必要があります。
>
>詳しくは、アカウントマネージャーにお問い合わせください
>
>Workfront計画の詳細については、[Adobe Workfront計画の概要 ](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

Adobe Workfront Planning を使用するには、ライセンスと共有権限の制約があります。

ここでは、Workfront Planning の機能を使用するために必要なアクセス権と設定について説明します。

## アクセス要件

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Workfront Planning にアクセスするには、次のアクセス権が必要です：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfrontの計画<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
<p>次のいずれかのWorkfront プラン：</p>
<ul><li>選択</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td>
   <td>
<p>次のいずれかのWorkfront計画</p>
<ul><li>プラン</li>
<li>Planning Plus</li>
</ul>
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p>
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <ul><li><p>標準、ライト、またはコントリビューター：Workfrontのプランニング情報を表示します</p></li>
   <li><p>標準：ワークスペースとビューを作成します。</p></li></ul>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>オブジェクト権限</p></td>
   <td>
   <ul>
   <li><p>自分が作成していないワークスペース、<span class="preview"> レコードタイプ </span> およびビューに対して、それらおよびオブジェクトにアクセスするための表示以上の権限。</p></li>
   <li><p>作成しなかったワークスペース <span class="preview"> およびレコード タイプ </span> に対する投稿以上の権限を編集し、レコード タイプおよびレコードを作成、編集、または削除します。</p></li>
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
   <td> <div class="preview">
<p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p>
<p> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、次の領域に Planning オプションを含むレイアウト テンプレートを割り当てる必要があります。</p>
   <ul><li>メインメニュー</li>
   <li>プロジェクト、ポートフォリオおよびプログラムの左側のパネル</li>
   </ul>
   <p>詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">レイアウトテンプレートを作成および管理</a>を参照してください。</p>
   </div>
   <p><b>メモ</b></p>
   <p>実稼動環境では、システム管理者を含むすべてのユーザーを、計画領域を含むレイアウトテンプレートに割り当てる必要があります。</p>
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


## レイアウトテンプレートを使用した計画エリアの共有

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

Workfront Planning ライセンスの追加購入後、システム管理者はユーザーを変更してレイアウト・テンプレートに割り当てることにより、次の領域に Planning オプションを追加できます。

* メインメニュー
* ランディングページ
* プロジェクト、ポートフォリオおよびプログラムの左側のパネル
* ピン留め

<div class="preview">

標準ユーザーとシステム管理者は、次の領域で、デフォルトで Planning 領域を有効にします。

* メインメニュー
* プロジェクト、ポートフォリオまたはプログラムの左側のパネル

</div>

Workfront インスタンスのユーザーからWorkfront Planning エリア </span> 追加または削除するには、<span class="preview"> を行います。

1. Workfront 管理者として **Workfront** にログインします。

1. **メインメニュー**/**設定**/**インターフェイス**/**レイアウトテンプレート** に移動して、レイアウトテンプレートを開くか作成します。

   レイアウトテンプレートのカスタマイズについて詳しくは、[ レイアウトテンプレートの作成と管理 ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) を参照してください。

1. Workfront Planning へのアクセス権を付与するユーザーにレイアウトテンプレートを割り当てます。

   詳しくは、[レイアウトテンプレートにユーザーを割り当て](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

   テンプレートに割り当てられたすべてのユーザーは、メインメニューから Workfront Planning にアクセスできるようになります。

   ユーザーは、ワークスペース、レコードタイプ、レコードおよびフィールドの作成を開始できます。

## アクセスを許可

Workfront Planning には、Workfrontのアクセス制御はありません。

あらゆるタイプのWorkfront ライセンスを持つユーザーは、Workfront Planning にアクセスできます。

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 権限の付与

ユーザーがWorkfront Planning のワークスペースおよびビューにアクセスするための権限をユーザーに付与する必要があります。

詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

Adobe WorkfrontのライセンスタイプはWorkfront Planning 権限と連携し、Workfront Planning オブジェクトの表示、投稿、管理に対するアクセス権を付与します。

ライセンスタイプが Workfront Planning オブジェクトの権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。


