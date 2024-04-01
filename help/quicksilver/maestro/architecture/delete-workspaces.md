---
title: ワークスペースの削除
description: 関係がなくなったワークスペースは削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 9%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# ワークスペースの削除

{{maestro-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画するための一元化された場所です。 詳しくは、 [ワークスペースの作成](../architecture/delete-workspaces.md).

不要になったワークスペースは削除できます。

削除する前に、別のワークスペースで削除するワークスペースに関連付けられているレコードの種類、レコード、フィールド、ビューの一部またはすべてを再度作成することをお勧めします。

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
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Workfron Planning ベータプログラムにAdobeする必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <p>現在：プラン</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセスレベルの制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*アクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## ワークスペースの削除に関する考慮事項

* ワークスペースを削除すると、すべてのレコードタイプ、レコード、そのフィールド、ビューも削除されます。
* 削除したワークスペースとそれらに含まれる情報は復元できません。

## ワークスペースの削除

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、削除するワークスペースを選択します。
1. 次をクリック： **その他** メニュー ![](assets/more-menu.png) ワークスペース名の横にある「 」をクリックし、 **削除**.
1. 「**削除**」をクリックして確定します。

   ワークスペースは削除され、復元できません。 レコードタイプ、レコード、フィールド、およびそれらに関連付けられたビューも削除されます。 <!--ensure this is right after closed beta-->
