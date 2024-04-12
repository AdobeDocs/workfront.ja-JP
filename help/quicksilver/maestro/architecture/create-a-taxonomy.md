---
title: 分類レコードタイプの作成
description: テンプレートを使用してワークスペースを作成すると、運用中のレコードタイプおよび分類セクションでレコードタイプが作成されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 44%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 分類レコードタイプの作成

{{maestro-important-intro}}

テンプレートを使用してワークスペースを作成する場合、レコードタイプは次のセクションで作成されます。

* 運用中のレコードタイプ
* 分類

ワークスペースの「分類」セクションのレコードタイプは、同じワークスペースの「運用中のレコードタイプ」セクションにあるレコードタイプに関する属性を取り込みます。

例えば、キャンペーンを運用中のレコードタイプにすることができます。以下は、キャンペーンレコードタイプに関する属性をキャプチャする分類です：地域、オーディエンス、国。

レコードタイプについて詳しくは、を参照してください。 [レコードタイプの概要](../architecture/overview-of-record-types-and-taxonomies.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <p> Adobe Workfront</p> <p>レコードタイプをExperience Manager Assetsと連携するには、Adobe Experience Manager Assets ライセンスが必要で、組織のWorkfront インスタンスがAdobeの Business Platform またはAdobe Admin Consoleにオンボーディングされている必要があります。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning クローズドベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセス レベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限を管理</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 分類の作成に関する考慮事項

* ワークスペースの分類セクションでレコードタイプを作成するには、テンプレートを使用してワークスペースを作成する必要があります。

  ワークスペースについて詳しくは、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。
* 次のいずれかの操作を行うことで、ワークスペースの分類セクションにレコードタイプを作成できます。
   * テンプレートを使用してワークスペースを作成する際に、自動的に作成します。詳しくは、[ワークスペースの作成](../architecture/create-workspaces.md)を参照してください。
   * ワークスペースの「分類」セクションで、ゼロから手動で分類を作成します。

* 新しく作成された分類には、デフォルトで次のフィールドがあります。

   * 名前
   * 説明
   * 開始日
   * 終了日
   * ステータス

  さらに、分類にカスタムフィールドを追加することができます。詳しくは、[フィールドの作成](../fields/create-fields.md)を参照してください。

  >[!NOTE]
  >
  >    ワークスペーステンプレートの使用時に作成される分類レコードタイプには、追加のフィールドがあります。

## 分類レコードタイプの作成

分類レコードタイプの作成は、レコードタイプの作成と似ています。

詳しくは、[リクエストタイプの作成](../architecture/create-record-types.md)を参照してください。
