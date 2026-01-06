---
product-area: projects
navigation-topic: convert-issues
title: イシューの解決を他のイシュー、タスク、プロジェクトに手動で結び付ける
description: イシューを変換せずに、イシューの解決策をプロジェクト、タスク、またはイシューの解決策に手動で結び付けることができます。イシューは、選択したプロジェクト、タスク、またはイシューの解決可能なオブジェクトの 1 つになります。これを行うと、プロジェクト、タスク、またはイシュートリガーのステータスが変更されると、元のイシューのステータスも変更されます。
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 95%

---

# イシューの解決策を他のイシュー、タスク、またはプロジェクトに手動で結び付ける

<!--Audited: 08/2025-->

イシューを変換せずに、イシューの解決策をプロジェクト、タスク、またはイシューの解決策に手動で結び付けることができます。イシューは、選択したプロジェクト、タスク、またはイシューの解決可能なオブジェクトの 1 つになります。これを行うと、プロジェクト、タスク、またはイシュートリガーのステータスが変更されると、元のイシューのステータスも変更されます。

>[!TIP]
>
>イシューの解決策を別のオブジェクトの解決策に結び付けると、元のイシューのステータスを手動で編集できなくなります。

オブジェクトの解決と解決可能なオブジェクトについて詳しくは、[解決の概要と解決可能なオブジェクト](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>投稿者以上</p> 
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシュー、タスク、プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>別のイシュー、タスク、またはプロジェクトにリンクするイシューへの権限を管理します</p> <p>既存のイシューに追加するイシュー、タスク、またはプロジェクトに対する表示以上の権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 前提条件

開始する前に、次の条件を満たす必要があります。

* 解決策を別のイシュー、タスク、またはプロジェクトの解決策に結び付けたいイシューがある

* 追加のイシュー、タスク、またはプロジェクトがある

## イシューの解決と、別のイシュー、タスクまたはプロジェクトの解決を結び付けている

1. 解決策を別のイシューの解決策またはタスクやプロジェクトの解決策に結び付けるイシューに移動します。
1. 左パネルで「**問題の詳細**」をクリックしてから、**概要**&#x200B;エリアを展開します。

   ![ 問題の詳細アイコン ](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. 「**解決者**」フィールドをクリックし、次の解決オブジェクトのタイプから選択します。

   * **プロジェクト**
   * **タスク**
   * **イシュー**

   選択したオブジェクトに応じて、次のフィールドが表示されます。

   * **解決するプロジェクト**
   * **解決するタスク**
   * **解決する問題**

1. **プロジェクトを解決中**、**タスク**、または&#x200B;**イシュー**&#x200B;フィールドに特定のプロジェクト、タスク、またはイシューの名前を入力し、リストに表示されたらクリックします。

   >[!NOTE]
   >
   >イシューの解決を、イシューが存在するタスクまたはプロジェクトに結び付けることはできません。イシューのタスクまたはプロジェクトは、「解決中のタスク」フィールドまたは「解決中のタスク」フィールドに表示されません。


1. 「**変更を保存**」をクリックします。

   元のイシューは、手順 4 と 5 で選択したプロジェクト、タスク、またはイシューの解決可能なオブジェクトになります。これは、解決オブジェクト（リンク先のプロジェクト、タスク、またはイシュー）が完了すると、元のイシューが完了することを意味します。

   >[!NOTE]
   >
   >1 つのプロジェクト、タスク、またはイシューに、解決可能なオブジェクトとして複数のイシューがある場合があります。
