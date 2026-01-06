---
product-area: projects
navigation-topic: convert-issues
title: 解決されたオブジェクトから問題のリンクを解除する
description: イシューをプロジェクトまたはタスクに変換してプロジェクトまたはタスクを作成する場合、元のイシューを保持するオプションがあります。イシューの変換中にこのオプションを使用できるようにするには、Adobe Workfront 管理者がこの設定を有効にする必要があります。イシューをプロジェクトやタスクに変換する方法について詳しくは、Adobe Workfront でのイシューの変換の概要を参照してください。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 96%

---

# 解決オブジェクトからイシューのリンクを解除する

<!--Audited: 08/2025-->

イシューをプロジェクトまたはタスクに変換してプロジェクトまたはタスクを作成する場合、元のイシューを保持するオプションがあります。イシューの変換中にこのオプションを使用できるようにするには、Adobe Workfront 管理者がこの設定を有効にする必要があります。\
イシューをプロジェクトやタスクに変換する方法について詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

プロジェクトまたはタスクに変換されたイシューを保持することにした場合、イシューの解決はプロジェクトまたはタスクに関連付けられます。イシューはプロジェクトまたはタスクの解決可能なオブジェクトになります。プロジェクトまたはタスクは、イシューの解決オブジェクトです。

イシューを別のイシューに手動でリンクすることもできます。この場合、2 番目のイシューは最初のイシューの解決オブジェクトになります。\
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
   <td> <p>投稿者以上</p>
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>タスクおよびプロジェクトへのアクセスの表示</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>タスクまたはプロジェクトに対する表示権限</p> </td> 
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
</table>-->

## プロジェクト、タスクまたはイシューからのイシューのリンク解除

1. プロジェクト、タスクまたはイシューにリンクされているイシューに移動します。
1. 「**イシューの詳細**」セクションをクリックします。
1. 「**イシューの詳細**」セクションの&#x200B;**概要**&#x200B;エリアに移動します。
1. 「**解決者**」フィールドで、解決可能なオブジェクトタイプを削除します。\
   イシューは、プロジェクト、タスクまたはイシューによって解決できます。

   これにより、イシューの解決オブジェクトが削除されます。

1. 「**変更を**&#x200B;**保存**」をクリックします。\
   イシューがプロジェクト、タスクまたはイシューにリンクされなくなり、イシューを個別に解決できるようになりました。
