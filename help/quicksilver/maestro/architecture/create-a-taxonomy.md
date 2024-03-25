---
title: 分類レコードタイプの作成
description: テンプレートを使用してワークスペースを作成する場合、レコード・タイプは「Operational Record Types」セクションと「Taxonomies」セクションに作成されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 9%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 分類レコードタイプの作成

{{maestro-important-intro}}

テンプレートを使用してワークスペースを作成する場合、次のセクションでレコードタイプが作成されます。

* 運用中のレコードタイプ
* 分類

ワークスペースの「分類」セクションのレコード・タイプは、同じワークスペースの「オペレーショナル・レコード・タイプ」セクションのレコード・タイプに関する属性を取得します。

例えば、キャンペーンはオペレーショナルレコードタイプにすることができます。 Campaign レコードタイプに関する属性を取得する分類を次に示します：地域、オーディエンス、国。

レコードの種類の詳細については、「 [レコードタイプの概要](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>レコードタイプをExperience Manager Assetsに接続するには、Adobe Experience Manager Assetsライセンスが必要です。組織のWorkfrontインスタンスをAdobeビジネスプラットフォームまたはAdobe Admin Consoleにオンボーディングする必要があります。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Adobe Workfront Planning クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Adobe Workfront Planning には、アクセスレベルの制御はありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
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

* ワークスペースの「分類」セクションでレコード・タイプを作成する前に、テンプレートを使用してワークスペースを作成する必要があります。

  ワークスペースについて詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).
* 次のいずれかの操作を行って、ワークスペースの「分類」セクションでレコードタイプを作成できます。
   * テンプレートを使用してワークスペースを作成する際に、自動的に作成します。 詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).
   * ワークスペースの「分類」セクションで、一から手動で作成します。

* 新しく作成されたすべての分類には、デフォルトで次のフィールドがあります。

   * 名前
   * 説明
   * 開始日
   * 終了日
   * ステータス

  さらに、分類にカスタムフィールドを追加できます。 詳しくは、 [フィールドの作成](../fields/create-fields.md).

  >[!NOTE]
  >
  >    ワークスペーステンプレートの使用時に作成される分類レコードタイプには、追加のフィールドがあります。

## 分類レコードタイプの作成

分類レコードタイプの作成は、レコードタイプの作成と似ています。

詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).
