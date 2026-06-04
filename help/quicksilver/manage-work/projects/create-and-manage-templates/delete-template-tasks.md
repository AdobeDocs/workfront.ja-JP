---
product-area: templates
keywords: タスク,デフォルト,自動化,作成
navigation-topic: templates-navigation-topic
title: テンプレートタスクの削除
description: テンプレートタスクが不要になった場合は、削除できます。 削除されたテンプレートタスクは復元できません。 テンプレートタスクから作成されたプロジェクトタスクは、削除または変更されません。
author: Alina
feature: Work Management
exl-id: dd733e9f-8045-4b65-828b-fe6aa40d973f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/G4OdOAGqiLA0PNUADG9ONsN9Dc2euNHQQGCYXK6ohvA
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
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 285
ht-degree: 27%

---

# テンプレートのタスクの削除

テンプレートタスクが不要になった場合は、削除できます。 テンプレートタスクから作成されたプロジェクトタスクは、削除または変更されません。

>[!NOTE]
>
>削除されたテンプレートタスクとその追加情報（割り当て、ドキュメント、承認）は復元できません。 テンプレートを復元すると、テンプレート上のすべてのタスクも復元できます。 テンプレートタスクを削除しても（テンプレートを削除しない）、復元することはできません。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> <p>標準</p>
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>テンプレートへの編集アクセス</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p> </td> 
   <td> <p>テンプレートの権限を管理します。</p> <p>テンプレートタスクは共有できません。</p> </td> 
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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level</p></td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p> </td> 
   <td> <p>Manage permissions for a template.</p> <p>You cannot share a template task.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## テンプレートのタスクの削除

1つまたは複数のテンプレートタスクを一括で削除できます。

{{step1-to-templates}}

1. テンプレートの名前をクリックして開きます。
1. 左側のパネルの「**テンプレートタスク**」をクリックします。
1. 次のいずれかの操作を行います。
   * リスト内のテンプレートタスクの名前をクリックしてテンプレートタスクを開き、**詳細** メニュー![詳細メニュー](assets/more-icon.png)/**テンプレートタスクを削除**&#x200B;をクリックします。
   * リスト > **削除** アイコン ![削除アイコン &#x200B;](assets/delete.png)で1つまたは複数のテンプレートタスクを選択します。

   「**テンプレートタスクを削除**」ボックスが開きます。
1. 「**はい、削除**」をクリックして確認します。

   テンプレートタスクは削除され、復元できません。

>[!TIP]
>
>テンプレートタスクの左側のパネルにある「先行タスク」セクションまたは「サブタスク」セクションをクリックして、先行タスクまたはサブタスクを削除できます。
>
>上記の手順を繰り返して、テンプレートタスクの先行タスクまたはサブタスクを削除します。
