---
product-area: projects
navigation-topic: convert-issues
title: 解決中のオブジェクトからイシューのリンク解除
description: イシューをプロジェクトまたはタスクに変換してプロジェクトまたはタスクを作成する場合、元のイシューを保持するオプションがあります。 イシューの変換中にこのオプションを使用できるようにするには、Adobe Workfront 管理者がこの設定を有効にする必要があります。 イシューをプロジェクトやタスクに変換する方法について詳しくは、Adobe Workfront でのイシューの変換の概要を参照してください。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-JK3YabXxWdvaEdgTvertsshm0G1EhJqif714zFPOEo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 429
ht-degree: 97%

---

# 解決オブジェクトからイシューのリンクを解除する

<!--Audited: 08/2025-->

イシューをプロジェクトまたはタスクに変換してプロジェクトまたはタスクを作成する場合、元のイシューを保持するオプションがあります。 イシューの変換中にこのオプションを使用できるようにするには、Adobe Workfront 管理者がこの設定を有効にする必要があります。\
イシューをプロジェクトやタスクに変換する方法について詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

プロジェクトまたはタスクに変換されたイシューを保持することにした場合、イシューの解決はプロジェクトまたはタスクに関連付けられます。 イシューはプロジェクトまたはタスクの解決可能なオブジェクトになります。 プロジェクトまたはタスクは、イシューの解決オブジェクトです。

イシューを別のイシューに手動でリンクすることもできます。 この場合、2 番目のイシューは最初のイシューの解決オブジェクトになります。\
解決オブジェクトの詳細については、[解決オブジェクトと解決可能なオブジェクトの概要](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)を参照してください。

>[!TIP]
>
>イシューのステータスは、解決オブジェクトのステータスに応じて自動的に変化するので、変更できません。

イシューからプロジェクト、タスク、またはイシューを削除することで、イシューの解決とプロジェクト、タスク、またはイシューの解決のリンクを解除できます。

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
   <td> <p>コントリビューター以上</p>
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>タスクとプロジェクトへのアクセスを表示</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>タスクまたはプロジェクトに対する表示権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## プロジェクト、タスクまたはイシューからのイシューのリンク解除

1. プロジェクト、タスクまたはイシューにリンクされているイシューに移動します。
1. 「**イシューの詳細**」セクションをクリックします。
1. 「**イシューの詳細**」セクションの&#x200B;**概要**&#x200B;エリアに移動します。
1. 「**解決者**」フィールドで、解決可能なオブジェクトタイプを削除します。\
   イシューは、プロジェクト、タスクまたはイシューによって解決できます。

   これにより、イシューの解決オブジェクトが削除されます。

1. 「**変更を****保存**」をクリックします。\
   イシューがプロジェクト、タスクまたはイシューにリンクされなくなり、イシューを個別に解決できるようになりました。
