---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの優先度の更新
description: タスクの優先度を定義して、タスクの重要度を指定できます。
author: Alina
feature: Work Management
exl-id: 653b62fe-6195-4288-ac05-f89e4a6113fd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/e7FZhg09w3el3xMbi-kjB52x6WUf4p2XzUi1HOqTSHk
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
source-wordcount: 277
ht-degree: 93%

---

# タスクの優先度の更新

タスクの優先度を定義して、タスクの重要度を指定できます。

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
   <td><p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限</p></td> 
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
   <td> <p>Manage permissions to a task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## タスクの優先度の概要

タスクの優先度を使用する際は、次の点に注意してください。

* Adobe Workfront の管理者は、Workfront 内で優先度ラベルを変更したり、新しい優先度を作成したりできます。 その結果、Workfront インスタンスでの「優先度」フィールドのオプションが、下記のオプションと異なる場合があります。 インスタンスでの優先度名のカスタマイズについては、[優先度の作成とカスタマイズ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)を参照してください。
* それぞれの優先度ラベルには、変更できない番号が関連付けられています。

  組織で使用されている優先度の番号付け順序を熟知している必要があります。

  例えば、優先度のラベルが変更されている場合、組織では緊急のタスクに言及するために数字の 1 を使用するかもしれません。

  それぞれのデフォルト優先度ラベルとそれに対応する数字については、次の表を参照してください。

  | **優先度ラベル（変更可能）** | **優先度番号（変更不可）** |
  |---|---|
  | なし | 0 |
  | 低 | 1 |
  | 標準 | 2 |
  | 高 | 3 |
  | 緊急 | 4 |



## タスクの優先度の変更

1. 優先度を変更するタスクに移動します。
1. 左パネルでの「**タスクの詳細**」をクリックします。
1. **編集** アイコン ![編集アイコン &#x200B;](assets/qs-edit-icon.png)をクリックし、**概要**&#x200B;領域で、**優先度** フィールドの値を選択します。
1. 「**変更を**&#x200B;**保存**」をクリックします。
