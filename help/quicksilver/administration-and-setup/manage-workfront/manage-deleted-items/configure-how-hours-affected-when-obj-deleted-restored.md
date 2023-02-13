---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: オブジェクトが削除され、復元される時間に対する影響を設定する
description: 誰かがプロジェクト、タスク、または時間の記録対象となる問題を削除したときの時間に対する影響を設定できます。 選択したオプションによって、プロジェクト、タスク、または問題が後で復元された場合の時間が決まります。 (Workfrontでの項目の復元について詳しくは、「削除された項目の復元」を参照してください。)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# オブジェクトが削除され、復元される時間に対する影響を設定する

誰かがプロジェクト、タスク、または時間の記録対象となる問題を削除したときの時間に対する影響を設定できます。 選択したオプションによって、プロジェクト、タスク、または問題が後で復元された場合の時間が決まります。 (Workfrontでの項目の復元について詳しくは、 [削除した項目を復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 項目が削除され、復元されたときの時間の管理方法を構成する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **タイムシートと時間**&#x200B;を選択し、「**環境設定**.

1. を **プロジェクト、タスク、または問題報告の削除環境設定** 」セクションに入力します。
1. （条件付き）プロジェクトが削除されたときの時間の管理方法を設定するには、次のいずれかのオプションを **プロジェクトを削除する場合** セクション：

   * タイムシートに既に追加された記録時間を一般時間として保持する（このプロジェクトが後で復元された場合、時間はタイムシートに残ります）\
      このオプションはデフォルトで選択されています。
   * ログに記録された時間をすべて削除する（このプロジェクトが後で復元された場合、ログに記録された時間がプロジェクトに復元されます）

1. （条件付き）タスクまたはイシューが削除された場合の時間の管理方法を設定するには、次のいずれかのオプションを **タスクまたは問題を削除する場合** セクション：

   * ログに記録された時間を、タスクまたはタスクが存在するプロジェクトに移動します（このタスクまたはタスクが後で復元された場合は、時間はプロジェクトに残ります）\
      このオプションはデフォルトで選択されています。
   * ログに記録された時間を削除する（このタスクまたは問題が後で復元された場合、ログに記録された時間がタスクまたは問題に復元されます）

1. 「**保存**」をクリックします。
