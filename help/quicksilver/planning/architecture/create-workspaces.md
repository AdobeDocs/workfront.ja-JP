---
title: ワークスペースを作成
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。レコードタイプは、ワークスペースのセクション別に整理されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 73%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースを作成

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

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
 <td role="rowheader"><p>Adobe Workfront 契約</p></td>
   <td>
<p>Workfront Planning の早期アクセス段階に登録されている必要があります </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>新規：標準</p>
   または
   <p>現在：プラン</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>作成したワークスペースに対する管理権限が付与されます。 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Planning エリアをレイアウトテンプレートに追加する必要があります。詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

アクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## ワークスペースに関する考慮事項

* 各部署の固有の仕事の仕方に合わせて、組織内の特定の部署単位でワークスペースを作成できます。
* ワークスペースに含まれるレコードタイプは、組織の部署単位の作業のライフサイクルを反映する必要があります。
* あるユーザーがワークスペースを作成した場合、そのユーザーだけがワークスペースにアクセスし、管理する権限を有します。他のユーザーと同じスペースで共同作業を行うには、他のユーザーとワークスペースを共有する必要があります。詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。システム管理者は、自分が作成していないワークスペースも含め、すべてのワークスペースを管理できます。
* 管理できるのは次のとおりです。

   * 1 つのワークスペースに最大 50 セクション。
   * 1 つのワークスペースのすべてのセクションから合計で最大 1,000 のレコードタイプ。すべてのレコードタイプは、各ワークスペースに固有です。<!--this might change-->
   * 組織の Workfront インスタンスに最大 1,000 のワークスペース。


## ワークスペースの作成

ワークスペースを作成し、それにレコードタイプを追加して、Workfront Planning でオブジェクトを整理できます。 ワークスペースの編集の詳細については、を参照してください。 [ワークスペースを編集](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

<!--replace the snippet with the new snippet with the landing page The Workfront Planning landing page opens. 
    ![](assets/planning-landing-page-admin.png)
    1. (Optional) Click the **My workspaces** tab to view workspaces you created
    Or
    Click the **Other workspaces** tab to view workspaces shared with you. 
    -->

1. （条件付き）利用する環境にワークスペースがない場合、「**ワークスペースを作成**」をクリックします。

   または、既存のワークスペースから、ワークスペース名の右側にある下向き矢印をクリックし、 **ワークスペースを作成**.

   ![](assets/workspace-drop-down-right-menu.png)


1. （オプションおよび条件付き）次の事前定義済みのワークスペーステンプレートのいずれかで「**プレビュー**」をクリックします。

   * マーケティング管理
   * セールス管理
   * 製品管理

   運用中のレコードタイプ、分類および各テンプレートに関連付けられているフィールドの数が示されます。

   ![](assets/previewing-a-workspace-template.png)

   Workfront Planning ワークスペーステンプレートについて詳しくは、[ワークスペーステンプレートのリスト](/help/quicksilver/planning/architecture/workspace-templates.md)を参照してください。

1. 「**テンプレートを使用**」をクリックして、選択したテンプレートからワークスペースの作成を開始します。

   または

   「**ワークスペースを作成**」をクリックして、ワークスペースを最初から作成します。

   次のタイプのワークスペースの 1 つが作成されます。

   * という空のワークスペース **無題のワークスペース** ワークスペースを最初から作成する際に、レコードタイプの手動での追加を開始できます。
   * サンプルレコードタイプが入力される、選択したテンプレートにちなんで名前が付けられたワークスペース。 レコードタイプとワークスペースをさらにカスタマイズできます。

1. 新しいワークスペースのヘッダーでワークスペースの名前の内側をクリックして名前を変更し、Enter キーを押します。

1. （オプションおよび条件付き）ワークスペースをテンプレートから作成した場合は、「**運用中のレコードタイプ**」または「**分類**」セクションの名前内をクリックします。

   または

   セクションの名前にポインタを合わせ、**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックし、「**名前を変更**」をクリックして、セクションの名前を変更します。

   >[!TIP]
   >
   >セクションを作成していない場合でも、任意のワークスペースから任意のセクションの名前を変更できます。

   ワークスペース セクションの編集など、ワークスペースの編集の詳細については、を参照してください。 [ワークスペースを編集](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. （オプション）「**レコードタイプを追加**」をクリックして、任意のセクションのワークスペースにレコードタイプを追加します。

   詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   ワークスペースでのレコードタイプの編集および削除について詳しくは、を参照してください。 [ワークスペースを編集](/help/quicksilver/planning/architecture/edit-workspaces.md).


