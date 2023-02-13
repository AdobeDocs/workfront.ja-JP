---
product-area: projects
navigation-topic: use-predecessors
title: タスクを連結して先行タスク関係を作成
description: Adobe Workfrontでは、複数の方法で先行関係を作成できます。 1 つの方法は、タスクを連結することです。
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# タスクを連結して先行タスク関係を作成

Adobe Workfrontでは、複数の方法で先行関係を作成できます。 1 つの方法は、タスクを連結することです。

先行タスクの詳細については、 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

タスクを連結すると、各タスクに手動で関係を作成する代わりに、選択したタスクで先行関係を自動的に作成できます。 タスク間では、別の先行関係タイプを引き続き使用できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 先行関係を作成するためのチェーンタスク

1. チェーンするタスクを含むプロジェクトに移動します。
1. クリック **タスク** をクリックします。
1. （条件付き）選択 **自動保存** タスクリストの右上隅で、連結するタスクを選択します。

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >タスクに対する変更を手動で保存する場合や、タスクを保存する場合にタイムライン計画モードを使用する場合は、タスクリスト内のタスクを連結できません。

1. 選択したタスクを右クリックし、 **チェーン**.
1. 次の依存関係タイプから選択します。

   * **終了 - 開始**
   * **終了 - 終了**
   * **開始 - 開始**
   * **開始 - 終了**

   先行依存タイプの詳細については、「 [タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. （オプション）「 **チェーン解除** （一部のタスクが以前にチェーンされている場合）。

   >[!CAUTION]
   >
   >一括編集タスクの場合は、連結解除オプションを使用して連続先行タスクのみが削除されます。

   選択したタスクは、先行タスクの関係によってリンクされます。
