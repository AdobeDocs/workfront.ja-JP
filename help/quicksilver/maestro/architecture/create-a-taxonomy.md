---
title: 分類レコードタイプの作成
description: 分類は、Adobe Workfront Maestro のオペレーショナルレコードタイプに関する属性を取得する、再利用可能なレコードタイプの一種です。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 7%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 分類レコードタイプの作成

{{maestro-important-intro}}

分類レコードタイプは、AdobeMaestro のオペレーショナルレコードタイプに関する属性をキャプチャします。

例えば、キャンペーンはオペレーショナルレコードタイプにすることができます。 Campaign レコードタイプに関する属性を取得する分類を次に示します：地域、オーディエンス、国。

Maestro のレコードタイプの詳細については、 [レコード・タイプと分類の概要](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>Maestro のレコードタイプをExperience Manager Assetsに接続するには、Adobe Experience Manager Assetsライセンスが必要です。組織のWorkfrontインスタンスをAdobeビジネスプラットフォームまたはAdobe Admin Consoleにオンボーディングする必要があります。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Maestro のアクセスレベルコントロールはありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています
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

* ワークスペースで分類レコードタイプを作成する前に、ワークスペースを作成する必要があります。

  ワークスペースについて詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).
* 次のいずれかの操作を行って、分類レコードタイプを作成できます。
   * テンプレートを使用してワークスペースを作成する際に、自動的に作成します。 詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).
   * 最初から手動で作成します。

* 新しく作成された分類レコードタイプには、すべて次のフィールドが含まれます。

   * 名前 <!--if there won't be any more fields, consider rephrasing this-->

  さらに、分類にカスタムフィールドを追加できます。 詳しくは、 [フィールドの作成](../fields/create-fields.md).

  >[!NOTE]
  >
  >    ワークスペーステンプレートの使用時に作成される分類レコードタイプには、追加のフィールドがあります。

## 分類レコードタイプの作成

分類レコードタイプの作成は、最初から、またはワークスペーステンプレートから、運用レコードタイプを作成する場合と似ています。

詳しくは、この記事の「最初からレコードタイプを作成する」を参照してください。 [レコードタイプの作成](../architecture/create-record-types.md).

テンプレートからワークスペースを作成する際の分類の自動作成について詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).
