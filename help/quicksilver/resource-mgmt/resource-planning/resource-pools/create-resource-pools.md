---
product-area: resource-management
navigation-topic: resource-pools
title: リソースプールの作成
description: リソースプールは、Adobe Workfront でリソースをより簡単に管理するのに役立つユーザーのコレクションです。
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
TQID: https://experienceleague.adobe.com/jNdb4450a6iY7-mkcBOCBOVD-JH6tRUb-LrqwpD2mQE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 515
ht-degree: 71%

---

# リソースプールを作成する {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="リソース プール"
>abstract="リソースプールとは、プロジェクトの完了に同時に必要なユーザーのコレクションです。 リソースプールを作成したら、それをプロジェクトとテンプレートに関連付けることができます。"

リソースプールは、Adobe Workfront でリソースをより簡単に管理するのに役立つユーザーのコレクションです。 リソースプールについて詳しくは、[&#x200B; リソースプールの概要](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>リソースプールを管理するアクセス権を含むリソース管理へのアクセス権の編集</p> <p>プロジェクト、テンプレート、ユーザーへのアクセスの編集</p></td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>リソースプールを関連付けるプロジェクト、テンプレート、ユーザーの権限を管理します</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リソースプールの作成 {#create-a-resource-pool}

{{step1-to-resourcing}}

1. 左側のパネルで「**リソースプール**」をクリックします。
1. 「**新しいリソースプール**」をクリックします。

   ![リソースプール](assets/list-of-resource-pools.png)

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名前</strong></td>
      <td>これは、リソースプールの名前です。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>説明</strong></td>
      <td>これは、このリソースプールに関する簡単な説明です。 例えば、どのような目的でそれを使用するかを指定できます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>プールのメンバー</strong></td>
      <td><p> リソースプールにユーザーを個別に追加します。<br>または<br>一度にリソースプールに大量のユーザーを追加します。ユーザーまたはユーザーのコレクションに関連付けられている次のいずれかのエンティティを追加できます。
        <ul>
         <li><strong>チーム</strong>：チームのすべてのメンバーはリソースプールに追加されます。</li>
         <li><strong>グループ</strong>：グループのすべてのメンバーはリソースプールに追加されます。</li>
         <li><strong>役割</strong>：その役割に関連付けられているすべてのユーザーが、リソースプールに追加されます。</li>
         <li><strong>会社</strong>：会社のすべてのユーザーはリソースプールに追加されます。</li>
        </ul><p>ヒント：アクティブなユーザー、チーム、<span>役割、</span>または会社のみを追加できます。</p><br> リソースプール内のすべてのユーザーを表示するには、ダイアログを下にスクロールする必要がある場合があります。
        <p>メモ：ユーザーがグループ、チーム、会社のメンバーになった場合、またはグループ、チーム、会社、または担当業務がリソースプールに追加された後に担当業務に関連付けられた場合、新しいメンバーはリソースプールに自動的に追加されません。 <br> ユーザーが追加するチーム、グループ、会社、および担当業務に属している場合、同時にユーザーがリソースプールに1回だけ追加されます。<br> リソースプールに追加された後に非アクティブ化されたユーザーは、ユーザーのリストでグレー表示され、非アクティブ化されているとマークされます。</p></p></td>
     </tr>
    </tbody>
   </table>

1. （オプション）グループ、チーム、会社、または担当業務を通じて追加されたユーザーを削除するための&#x200B;**取り消し**&#x200B;リンクを使用します。

   >[!NOTE]
   >
   >リソースプール内のユーザー数に制限はありません。 ただし、リソース管理が課題になる可能性があるので、リソースプールに多くのユーザーを追加しすぎないようにすることをお勧めします。 ユーザーのリストには、リソースプール内の最初の 2,000 人のユーザーがアルファベット順で表示されます。

   ![&#x200B; ユーザーがリソースプールに追加されました](assets/users-in-resource-pool2.png)

1. （オプション）ユーザー名の右側にあるX アイコンをクリックして、ユーザーを削除します。 リソースプールからユーザーを削除する方法について詳しくは、[&#x200B; リソースプールからユーザーを削除](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)を参照してください。
1. （オプション）「**検索**」オプションを使用して、リソースプール内のユーザーを検索します。
1. 「**作成**」をクリックします。
