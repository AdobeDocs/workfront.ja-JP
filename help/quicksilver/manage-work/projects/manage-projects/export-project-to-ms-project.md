---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトの Microsoft Project へのエクスポート
description: Adobe Workfront プロジェクトを Microsoft Project に書き出すことができます。
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: ht
source-wordcount: '307'
ht-degree: 100%

---

# プロジェクトの Microsoft Project へのエクスポート

Adobe Workfront プロジェクトを Microsoft Project に書き出すことができます。 

>[!IMPORTANT]
>
>* すべての Workfront フィールドが Microsoft Project ファイルに転送されるわけではありません。\
>  Workfront と Microsoft Project の間のフィールドの互換性の詳細については、[Microsoft Project フィールドの Adobe Workfront プロジェクトへのマッピング](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md)を参照してください。
>* あるアプリケーションから別のアプリケーションにプロジェクトを転送する回数を制限することをお勧めします。 
>

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。プロジェクトへのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセスの許可</a>を参照してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> プロジェクトの表示またはそれ以上の権限</p> <p>プロジェクト権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>を参照してください。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者にお問い合わせください。

## Workfront から Microsoft Project へのプロジェクトの書き出し

プロジェクトは、Workfront のプロジェクトページ、プロジェクトリスト、レポートから書き出すことができます。

1. 書き出すプロジェクトに移動し、プロジェクト名の右側にある&#x200B;**その他**&#x200B;アイコン ![](assets/qs-more-menu.png) をクリックします。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   または

   プロジェクトリストまたはレポートに移動してプロジェクトを選択し、リスト上部にあるその他アイコン ![](assets/qs-more-menu.png) をクリックします。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 「**MS プロジェクトを書き出し**」をクリックします。

   プロジェクトが XML ファイルとしてコンピューターにダウンロードされ、Microsoft Project に読み込む準備が整います。 
