---
product-area: projects
navigation-topic: task-duration
title: シンプル期間タイプを使用して、タスクの予定時間と期間を更新する
description: デフォルトでは、予定時間数に基づいてシンプル期間タイプでタスクの期間が計算されます。 ただし、Workfront の特定のエリアでは、予定時間数タスクとシンプル期間のタスクの期間を手動で編集することもできます。
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SLemiOnFj-dOnWtXjH6gNzHZdVaXfp47qB0xzVJkRck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 450
ht-degree: 78%

---

# タスクの予定時間数と期間のシンプルな期間タイプでの更新

デフォルトでは、予定時間数に基づいてシンプル期間タイプでタスクの期間が計算されます。 ただし、Workfront の特定のエリアでは、予定時間数タスクとシンプル期間のタスクの期間を手動で編集することもできます。

タスクの予定時間数と期間は、「割り当て」のシンプル期間タイプのインラインまたはタスクレベルで編集できます。

情報をインラインで編集する方法について詳しくは、[Adobe Workfront のリスト内の項目のインライン編集](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)を参照してください。

この記事では、「割り当て」のタスクレベルでシンプル期間タイプを使って、タスクの予定時間数と期間を更新する方法について説明します。

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
   <td><p>Standard以上</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p> <p>タスクへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクへのアクセスを管理 </p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Old:

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## タスクの予定時間数と期間のシンプルな期間タイプでの更新

>[!IMPORTANT]
>
>シンプルな期間タスクで期間を手動で更新すると、予定時間数に基づく期間の計算が停止します。

「高度な割り当て」ボックスでシンプル期間タイプを使って、タスクの予定時間数と期間を編集するには：

1. タスクのリストで、期間タイプを変更するタスクの名前をクリックします。
1. 次のいずれかの操作を行います。

   * タスク名の横にあるオブジェクト ![&#128279;](assets/qs-more-icon-on-an-object.png)の&#x200B;**詳細** アイコン 詳細アイコンをクリックし、**編集**、**割り当て**&#x200B;をクリックします。
   * タスク ヘッダーの「**割り当て先**」または「割り当て先」セクションの割り当て名をクリックし、「**詳細**」をクリックします。

1. すべての割り当ての **予定時間数**&#x200B;の合計値を入力します（例：10 時間）。 予定時間数の合計は、タスクに割り当てられたすべてのリソースに均等に配分されます。
1. （オプション）タスクに割り当てられた各リソースの予定時間数を手動で調整します。 タスク更新の予定時間数の合計数は、リソースに個別に割り当てられた新しい時間を反映します。
1. タスクの&#x200B;**期間**&#x200B;の値を入力します（例：2 日）。

   ![高度な割り当て単純期間、複数のリソース &#x200B;](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 「**保存**」をクリックします。
