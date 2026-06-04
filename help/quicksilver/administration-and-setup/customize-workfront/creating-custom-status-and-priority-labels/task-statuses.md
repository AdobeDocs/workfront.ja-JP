---
title: システム タスク ステータスのリストへのアクセス
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: タスクのステータスを使用して、タスクが特定の時点で開発のどのステージにあるかユーザーに示すことができます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2cdedc67-b7b0-4e83-a446-d71e3afe255c
TQID: https://experienceleague.adobe.com/7-c15nhRYvTmQOL7NRBywrhUazdPzppKScZVH5bB-1Y
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 259
ht-degree: 96%

---

# システムタスクステータスのリストへのアクセス

タスクのステータスを使用して、タスクが特定の時点で開発のどのステージにあるかユーザーに示すことができます。

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
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タスクステータスへのアクセス

システムステータスの編集または新しいカスタムステータスの作成について詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

{{step-1-to-setup}}

1. **プロジェクトの環境設定**／**ステータス**&#x200B;をクリックします。

1. 「**タスク**」タブをクリックします。

   Workfront で使用できるタスクステータスがこのタブに表示されます。

   ![&#x200B; タスクの状態](assets/task-status.png)

   ビルトインの各システムタスクステータスについて詳しくは、[システムタスクステータス](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-task-statuses.md)を参照してください。

## カスタムタスクステータスの作成について

Workfront 管理者は、カスタムのシステムタスクステータスを Workfront に追加できます。

グループの所有者は、グループにカスタムタスクステータスを追加できます。

カスタムタスクステータスを作成する場合は、新しいステータスと既存のシステムのステータスを同じにする必要があります。 カスタムステータスをどのステータスとみなすのが適切かを知るには、システムステータスの動作を理解する必要があります。 同じステータスを選択した後は変更できません。

カスタムステータスの作成、システムステータスの編集、タスクの新しいデフォルトステータスの選択について詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。
