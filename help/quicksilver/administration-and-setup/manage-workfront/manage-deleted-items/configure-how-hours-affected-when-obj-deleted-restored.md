---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: オブジェクトが削除および復元された場合の時間数に対する動作の設定
description: 時間数を記録する対象となるプロジェクト、タスク、またはイシューが削除されたときの時間数に対する動作を設定できます。選択したオプションによって、プロジェクト、タスク、またはイシューが後で復元された場合の時間数に対する動作も設定できます。（Workfront での項目の復元について詳しくは、「削除した項目の復元」を参照してください）。
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '412'
ht-degree: 100%

---

# オブジェクトが削除および復元された場合の時間数に対する動作の設定

時間数を記録する対象となるプロジェクト、タスク、またはイシューが削除されたときの時間数に対する動作を設定できます。選択したオプションによって、プロジェクト、タスク、またはイシューが後で復元された場合の時間数に対する動作も設定できます。（Workfront での項目の復元について詳しくは、[削除した項目の復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください）。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 項目が削除および復元された場合の時間数の管理方法の設定

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**設定** ![](assets/gear-icon-settings.png)」の順にクリックします。

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
