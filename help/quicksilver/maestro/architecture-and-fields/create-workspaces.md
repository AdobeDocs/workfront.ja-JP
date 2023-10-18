---
title: ワークスペースの作成
description: ワークスペースは、チームが使用するオペレーショナルレコードタイプと分類の集まりで、チームの作業ライフサイクルを表します。 Maestro でワークスペースを完全にカスタマイズできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースの作成

>[!IMPORTANT]
>
>この記事の情報は、Adobe・マエストロに関して、Adobeからの新しいオファーです。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
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

## ワークスペースに関する考慮事項

* 各単位の固有の動作方法に合わせて、組織内の特定の組織単位のワークスペースを作成できます。
* ワークスペースに含まれるレコードタイプと分類は、組織単位の作業ライフサイクルを反映する必要があります。
* ワークスペースを作成すると、組織内の全員がワークスペースを表示、編集または削除できます。  <!--this will change with access levels and permissions-->
* 組織内には最大 1,000 個のワークスペースを持つことができます。
* ワークスペースには、各ワークスペースに固有のレコードタイプが含まれます。 <!--this might change-->

## ワークスペースの作成

1. （条件付き）システムにワークスペースがない場合、 **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅に <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 次に、「 **マエストロ** ![](assets/maestro-icon.png).

   または、既存のワークスペースから、ワークスペース名の右側を下向きでクリックし、 **ワークスペースを作成**.

   ![](assets/workspace-drop-down-right-menu.png)

   これにより、Maestro の Workspaces 領域が開きます。
1. （オプションおよび条件付き）「 **プレビュー** 次の事前定義済みの workspace テンプレートのいずれかに含まれます。

   * マーケティング管理
   * セールス管理
   * 製品管理

   オペレーショナル・レコードのタイプ、分類、および各テンプレートに関連付けられているフィールドの数を示します。

   ![](assets/previewing-a-workspace-template.png)

   Maestro Workspace テンプレートについて詳しくは、 [Workspace テンプレートのリスト](../architecture-and-fields/workspace-templates.md).

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

   詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

1. （オプション）「 **分類を追加** ワークスペースに分類を追加するには、次の手順に従います。

   詳しくは、 [分類の作成](../architecture-and-fields/create-a-taxonomy.md).
