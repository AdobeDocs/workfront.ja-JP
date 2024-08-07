---
title: ワークスペースを作成
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。レコードタイプは、ワークスペースのセクション別に整理されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 56%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースを作成

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

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

+++

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
* Workfront ライセンスに応じて、ワークスペースは計画領域の次のタブに表示されます。

   * システム管理者の場合、ワークスペースは次のタブに表示されます。

      * **マイワークスペース**：作成したワークスペースが表示されます。<!--Replace with: Workspaces I'm on: Displays workspaces you created or workspaces that are shared with you.-->
      * **その他のワークスペース**：共有されているワークスペースを含む、システム内のその他すべてのワークスペースを表示します。 &lt;! – 置換後：その他のワークスペース：システム内のその他すべてのワークスペースを表示します。>

   * その他のすべてのユーザーについては、作成したワークスペースと、共有している他のユーザーのワークスペースが「ワークスペース」領域に表示されます。

* ワークスペースに含まれるレコードタイプは、組織の部署単位の作業のライフサイクルを反映する必要があります。
* あるユーザーがワークスペースを作成した場合、そのユーザーだけがワークスペースにアクセスし、管理する権限を有します。他のユーザーと同じスペースで共同作業を行うには、他のユーザーとワークスペースを共有する必要があります。詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。システム管理者は、自分が作成していないワークスペースも含め、すべてのワークスペースを管理できます。
* 管理できるのは次のとおりです。

   * 1 つのワークスペースに最大 50 セクション。
   * 1 つのワークスペースのすべてのセクションから合計で最大 1,000 のレコードタイプ。すべてのレコードタイプは、各ワークスペースに固有です。<!--this might change-->
   * 組織の Workfront インスタンスに最大 1,000 のワークスペース。


## ワークスペースの作成

ワークスペースを作成し、それにレコードタイプを追加して、Workfront Planning でオブジェクトを整理できます。 ワークスペースの編集について詳しくは、[ ワークスペースの編集 ](/help/quicksilver/planning/architecture/edit-workspaces.md) を参照してください。

{{step1-to-planning}}

1. **ワークスペースを作成** をクリックします

   ワークスペースを作成ボックスが表示されます。 ワークスペースは、最初から作成することも、使用可能なテンプレートの 1 つを使用して作成することもできます。

1. （オプションおよび条件付き）次の事前定義済みのワークスペーステンプレートのいずれかで「**プレビュー**」をクリックします。

   * 基本：マーケティング管理
   * 詳細：マーケティング管理
   * エンタープライズ：マーケティング管理
   * セールス管理
   * 製品管理

   テンプレートのプレビューボックスが開きます。

   運用中のレコードタイプ、分類および各テンプレートに関連付けられているフィールドの数が示されます。

   ![](assets/previewing-a-workspace-template.png)

   Workfront Planning ワークスペーステンプレートについて詳しくは、[ワークスペーステンプレートのリスト](/help/quicksilver/planning/architecture/workspace-templates.md)を参照してください。

1. テンプレートプレビューボックスで「**テンプレートを使用**」をクリックして、選択したテンプレートからワークスペースの作成を開始します

   または

   「**戻る**」をクリックし、「**新しいワークスペース**」をクリックしてワークスペースを最初から作成します。

   次のタイプのワークスペースの 1 つが作成されます。

   * ワークスペースをゼロから作成する際にレコードタイプの手動追加を開始できる **名称未設定Workspace** という空のワークスペース。
   * サンプルレコードタイプが入力される、選択したテンプレートにちなんで名前が付けられたワークスペース。 レコードタイプとワークスペースをさらにカスタマイズできます。

   Workfront管理者の場合、新しいワークスペースが「**マイワークスペース**」タブに表示されます。<!--replace this with: Workspaces I'm on tab-->
1. 新しいワークスペースのヘッダーでワークスペースの名前の内側をクリックして名前を変更し、Enter キーを押します。

1. （オプションおよび条件付き）ワークスペースをテンプレートから作成した場合は、「**運用中のレコードタイプ**」または「**分類**」セクションの名前内をクリックします。

   または

   セクションの名前にポインタを合わせ、**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックし、「**名前を変更**」をクリックして、セクションの名前を変更します。

   >[!TIP]
   >
   >セクションを作成していない場合でも、任意のワークスペースから任意のセクションの名前を変更できます。

   「ワークスペース」セクションの編集を含む、ワークスペースの編集の詳細については、「[ ワークスペースの編集 ](/help/quicksilver/planning/architecture/edit-workspaces.md)」を参照してください。

1. （オプション）「**レコードタイプを追加**」をクリックして、任意のセクションのワークスペースにレコードタイプを追加します。

   詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   ワークスペース内のレコードの種類の編集および削除の詳細については、「[ ワークスペースの編集 ](/help/quicksilver/planning/architecture/edit-workspaces.md)」を参照してください。


