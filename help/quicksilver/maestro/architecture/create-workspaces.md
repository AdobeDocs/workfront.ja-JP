---
title: ワークスペースの作成
description: ワークスペースは、チームが使用するオペレーショナルレコードタイプと分類の集まりで、チームの作業ライフサイクルを表します。 Maestro でワークスペースを完全にカスタマイズできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースの作成

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

AdobeMaestro では、ワークスペースはチームが作業を計画するための一元化された場所です。

ワークスペースは、チームが使用するオペレーショナルレコードタイプと分類の集まりで、チームの作業ライフサイクルを表します。 Maestro でワークスペースを完全にカスタマイズできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
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
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level*</p></td>
   <td> <p>System Administrator</p>  
   <p>The following license types:</p>
   <ul><li>New: Standard</li>
   <li>Current: Worker or higher </li></ul>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Maestro area to your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver\administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->




<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## ワークスペースに関する考慮事項

* 各単位の固有の動作方法に合わせて、組織内の特定の組織単位のワークスペースを作成できます。
* ワークスペースに含まれるレコードタイプと分類は、組織単位の作業ライフサイクルを反映する必要があります。
* ワークスペースを作成すると、組織内の全員がワークスペースを表示、編集または削除できます。  <!--this will change with access levels and permissions-->
* 組織内には最大 1,000 個のワークスペースを持つことができます。
* ワークスペースには、各ワークスペースに固有のレコードタイプが含まれます。 <!--this might change-->

## ワークスペースの作成

1. （条件付き）システムにワークスペースがない場合、 **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅、または **メインメニュー** アイコン ![](assets/main-menu-shell.png)  左上隅にある場合は、「 **マエストロ** ![](assets/maestro-icon.png).

   または、既存のワークスペースから、ワークスペース名の右側を下向きでクリックし、 **ワークスペースを作成**.

   ![](assets/workspace-drop-down-right-menu.png)

   これにより、Maestro の Workspaces 領域が開きます。
1. （オプションおよび条件付き）「 **プレビュー** 次の事前定義済みの workspace テンプレートのいずれかに含まれます。

   * マーケティング管理
   * セールス管理
   * 製品管理

   オペレーショナル・レコードのタイプ、分類、および各テンプレートに関連付けられているフィールドの数を示します。

   ![](assets/previewing-a-workspace-template.png)

   Maestro Workspace テンプレートについて詳しくは、 [Workspace テンプレートのリスト](../architecture/workspace-templates.md).

1. クリック **テンプレートを使用** 選択したテンプレートからワークスペースの作成を開始するには

   または

   クリック **ワークスペースを作成** をクリックして、ワークスペースをゼロから作成します。

   次のタイプのワークスペース用の 1 つが作成されます。

   * レコードタイプの手動で追加を開始できる空のワークスペース。
   * サンプルレコードタイプが設定されたワークスペースです。このレコードタイプはさらにカスタマイズできます。

1. 新しいワークスペースのヘッダーにあるワークスペース名の中をクリックして名前を変更し、Enter キーを押します。

   または

   次をクリック： **その他** メニュー ![](assets/more-menu.png)をクリックし、 **名前を変更**.

1. （オプション）「 **レコードタイプを追加** をクリックして、レコードタイプをワークスペースに追加します。

   詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

1. （オプション）「 **分類を追加** ワークスペースに分類を追加するには、次の手順に従います。

   詳しくは、 [分類の作成](../architecture/create-a-taxonomy.md).
