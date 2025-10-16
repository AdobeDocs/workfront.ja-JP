---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: オブジェクトが削除および復元された際の時間への影響を設定
description: 時間数を記録する対象となるプロジェクト、タスク、またはイシューが削除されたときの時間数に対する動作を設定できます。選択したオプションによって、プロジェクト、タスク、またはイシューが後で復元された場合の時間数に対する動作も設定できます。（Workfront での項目の復元について詳しくは、「削除した項目の復元」を参照してください）。
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 90%

---

# オブジェクトが削除および復元された場合の時間への影響を設定する

時間数を記録する対象となるプロジェクト、タスク、またはイシューが削除されたときの時間数に対する動作を設定できます。選択したオプションによって、プロジェクト、タスク、またはイシューが後で復元された場合の時間数に対する動作も設定できます。（Workfront での項目の復元について詳しくは、[削除した項目の復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください）。

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

## 項目が削除および復元された場合の時間数の管理方法の設定

{{step-1-to-setup}}

1. 「**タイムシートと時間**」を展開し、「**環境設定**」をクリックします。

1. 「**プロジェクト、タスク、またはイシューの削除の環境設定**」セクションを見つけます。
1. （条件付き）プロジェクトが削除された場合の時間数の管理方法を設定するには、**プロジェクトを削除する場合**&#x200B;セクションに記載される次のオプションのいずれかを選択します。

   * タイムシートに既に追加されているログ時間を一般的な時間として保持する（プロジェクトが後で復元された場合、時間はタイムシートに残ります）\
     このオプションはデフォルトで選択されています。
   * ログ時間をすべて削除する（プロジェクトが後で復元された場合、ログ時間はプロジェクトに復元されます）

1. （条件付き）タスクまたはイシューが削除された場合の時間の管理方法を設定するには、**タスクまたは問題を削除する場合**&#x200B;のセクションで、次のいずれかのオプションを選択します。

   * プロジェクトのログ時間をすべて、タスクまたはイシューがある場所に移動する（後でこのタスクまたはイシューが復元された場合、時間はプロジェクトに残ります）\
     このオプションはデフォルトで選択されています。
   * ログ時間を削除する（このタスクまたはイシューが後で復元された場合、ログ時間はタスクまたはイシューに復元されます）

1. 「**保存**」をクリックします。
