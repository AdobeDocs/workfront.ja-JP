---
title: 分類レコードタイプの作成
description: 分類は、Adobe Workfront Maestro のオペレーショナルレコードタイプに関する属性を取得する、再利用可能なレコードタイプの一種です。
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 分類レコードタイプの作成

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなクローズドベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

分類は、レコード・タイプで、Adobe・マエストロのオペレーショナル・レコード・タイプに関する属性をキャプチャします。

例えば、キャンペーンはオペレーショナルレコードタイプにすることができます。 Campaign レコードタイプに関する属性を取得する分類を次に示します：地域、オーディエンス、国。

Maestro のレコードタイプの詳細については、 [レコード・タイプと分類の概要](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
<td>
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
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

* ワークスペースで分類を作成する前に、ワークスペースを作成する必要があります。

  ワークスペースについて詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
* 次のいずれかの操作を行って、分類レコードタイプを作成できます。
   * テンプレートを使用してワークスペースを作成する際に、自動的に作成します。 詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
   * 最初から手動で作成します。
   * 外部リストから情報を貼り付けて、手動で作成します。

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* 新しく作成されたすべての分類には、次のフィールドが含まれます。

   * 名前 <!--if there won't be any more fields, consider rephrasing this-->

  さらに、分類にカスタムフィールドを追加できます。 詳しくは、 [フィールドの作成](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    ワークスペーステンプレートを使用する際に作成された分類には、追加のフィールドがあります。

## 分類の作成

分類の作成は、最初から、またはワークスペーステンプレートから、オペレーショナルレコードタイプを作成する場合と似ています。

詳しくは、この記事の「最初からレコードタイプを作成する」を参照してください。 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

テンプレートからワークスペースを作成する際の分類の自動作成について詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
