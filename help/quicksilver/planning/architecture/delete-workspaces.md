---
title: ワークスペースの削除
description: 関係がなくなったワークスペースは削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 74%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースの削除

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

不要になったワークスペースは削除できます。

ワークスペースを削除する前に、そのワークスペースに関連付けられているレコードタイプ、レコード、フィールド、ビューの一部またはすべてを、別のワークスペースで再作成することをお勧めします。

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
   <td> <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

*アクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## ワークスペースの削除に関する考慮事項

* ワークスペースを削除すると、すべてのレコードタイプ、レコード、そのフィールドおよびビューも削除されます。
* 削除したワークスペースとそれらに含まれる情報は復元できません。

## ワークスペースの削除

{{step1-to-planning}}

1. （条件付き）Workfront管理者の場合は、「**マイワークスペース** **」をクリックして作成したワークスペースにアクセスするか、「その他のワークスペース** をクリックして自分と共有されている他のワークスペースにアクセスします。<!--change it to Workspaces I'm on-->

1. 削除するワークスペースのカードをクリックします。

   Workspace ページが表示されます。

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To delete a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **De,ete**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,******to the step below****-->

1. ワークスペース名の横にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックし「**削除**」を選択します。

   ![](assets/permanently-delete-workspace-confirmation.png)

1. 表示されたスペースに「**削除**」と入力し、「**完全に削除**」をクリックします。 これは、大文字と小文字を区別しません。

   ワークスペースは削除され、復元できません。レコードタイプ、レコード、フィールドおよびそれらに関連付けられているビューも削除されます。<!--ensure this is right at or before GA-->
