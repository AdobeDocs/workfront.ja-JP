---
title: ワークスペースを作成
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。 Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。 レコードタイプは、ワークスペースのセクション別に整理されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 12%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースを作成

{{maestro-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画するための一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。 Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>AdobeWorkfront のクローズ済ベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス*</p></td>
   <td>
   <p>新規：標準</p>
   または
   <p>現在：プラン</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセス レベルの制御はありません</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>作成したワークスペースに対する管理権限を受け取ります。 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>計画エリアをレイアウトテンプレートに追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

アクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## ワークスペースについての考慮事項

* 組織内の特定の組織単位に対して、各単位の一意の動作方法に一致するワークスペースを作成できます。
* ワークスペースに含まれるレコードタイプは、組織単位の作業ライフサイクルを反映する必要があります。
* ワークスペースを作成した場合、ワークスペースにアクセスして管理する権限を持っているのはユーザーのみです。 同じスペースで他のユーザーと共同作業するには、そのユーザーと共有する必要があります。 詳しくは、を参照してください [ワークスペースの共有](/help/quicksilver/maestro/access/share-workspaces.md). システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースを管理できます。
* 以下を設定できます。

   * 1 つのワークスペースに最大 50 個のセクションを含めることができます。
   * 1 つのワークスペース内のすべてのセクションから合計で最大 1,000 個のレコードタイプ。 すべてのレコードタイプは、各ワークスペースに固有です。 <!--this might change-->
   * 組織のWorkfront インスタンス内の最大 1,000 個のワークスペース。


## ワークスペースの作成

ワークスペースを作成し、それにレコードタイプを追加して、Workfront Planning でオブジェクトを整理できます。 ワークスペースの編集の詳細については、を参照してください。 [ワークスペースを編集](/help/quicksilver/maestro/architecture/edit-workspaces.md).

{{step1-to-maestro}}

これにより、Workfront Planning の「ワークスペース」領域が開きます。

1. （条件付き）環境内にワークスペースがない場合は、 **ワークスペースを作成**

   または、既存のワークスペースから、ワークスペース名の右側にある下向き矢印をクリックし、 **ワークスペースを作成**.

   ![](assets/workspace-drop-down-right-menu.png)


1. （オプションおよび条件付き）クリック **プレビュー** 次の事前定義済みのワークスペーステンプレート内：

   * マーケティング管理
   * 営業管理
   * 製品管理

   どの運用中のレコードタイプ、分類、および各テンプレートに関連付けられているフィールド数が示されます。

   ![](assets/previewing-a-workspace-template.png)

   Workfront Planning Workspace のテンプレートについては、を参照してください。 [ワークスペーステンプレートのリスト](../architecture/workspace-templates.md).

1. クリック **テンプレートを使用** 選択したテンプレートからのワークスペースの作成を開始するには

   または

   クリック **ワークスペースを作成** ワークスペースを最初から作成する。

   次のタイプのワークスペースが 1 つ作成されます。

   * という空のワークスペース **無題のワークスペース** ワークスペースを最初から作成する際に、レコードタイプの手動での追加を開始できます。
   * サンプルレコードタイプが入力される、選択したテンプレートにちなんで名前が付けられたワークスペース。 レコードタイプとワークスペースをさらにカスタマイズできます。

1. 新しいワークスペースのヘッダーでワークスペースの名前の内側をクリックして名前を変更し、Enter キーを押します。

1. （オプションおよび条件付き）ワークスペースをテンプレートから作成した場合は、の名前内をクリックします **運用中のレコードタイプ** または **分類** セクション

   または

   セクションの名前にポインタを合わせ、 **詳細** メニュー ![](assets/more-menu.png)を選択し、 **名前を変更** セクションの名前を変更します。

   >[!TIP]
   >
   >セクションを作成していない場合でも、任意のワークスペースから任意のセクションの名前を変更できます。

   ワークスペース セクションの編集など、ワークスペースの編集の詳細については、を参照してください。 [ワークスペースを編集](/help/quicksilver/maestro/architecture/edit-workspaces.md).

1. （任意）クリック **レコードタイプを追加** をクリックして、任意のセクションのワークスペースにレコードタイプを追加します。

   詳しくは、[リクエストタイプの作成](../architecture/create-record-types.md)を参照してください。

   ワークスペースでのレコードタイプの編集および削除について詳しくは、を参照してください。 [ワークスペースを編集](/help/quicksilver/maestro/architecture/edit-workspaces.md).


