---
product-area: projects
navigation-topic: manage-issues
title: イシューを削除
description: 適切なアクセス権や権限を持っている場合は、Adobe Workfront でイシューやリクエストを削除できます。
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 90%

---

# イシューを削除

<!--Audited: 01/2024-->

適切なアクセス権や権限を持っている場合は、Adobe Workfront でイシューやリクエストを削除できます。

>[!TIP]
>
>Workfront では、「イシュー」と「リクエスト」が同じような意味で使用されます。プロジェクトとタスクの両方のイシューを記録して、対処する必要がある予期せぬ作業を示すことができます。リクエストを送信することもできます。リクエストは、リクエストキューとして指定されたプロジェクトのイシューとして記録されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新規：寄稿者以上</p>
   <p>現在：リクエスト以降</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベルの設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトとタスクへのアクセス権またはそれ以上の権限</p>  <p>アクセスレベルの問題へのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">問題へのアクセス権の付与</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>プロジェクトまたはタスクに対する参加以上の権限</p> <p> イシューに関する権限の付与については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。 アクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## イシューの削除に関する考慮事項

* Workfront 管理者またはグループ管理者は、ステータスが完了のプロジェクトのイシューの削除を、プロジェクトの環境設定領域で有効にする必要があります。プロジェクトの環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

* イシューにログに記録された時間がある場合、Workfront 管理者またはグループ管理者は、Workfront インスタンスでタスクとイシューの環境設定を指定することで、これらのイシューの削除を許可する必要があります。これは、時間が記録されたイシューがあるプロジェクトを削除しようとした場合も該当します。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  時間が記録されたイシューの削除を有効にする方法について詳しくは、[システム全体のタスクとイシューの環境設定を行う](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

## イシューの削除による影響

イシューを削除すると、そのイシューにリンクされている他のオブジェクトに影響を与えます。

イシューを削除すると、イシューに添付されている次のオブジェクトも削除されます。

* ドキュメント

  チェックアウトされたドキュメントが添付されたイシューは削除できません。ドキュメントのチェックアウトについて詳しくは、[ドキュメントのチェックアウト](../../../documents/managing-documents/check-out-documents.md)を参照してください。

* メモ
* 承認

Workfront インスタンスの&#x200B;**タイムシートおよび時間設定**&#x200B;で、Workfront 管理者またはグループ管理者が指定したプロジェクト、タスクまたはイシューの削除に関する環境設定によって、イシューに記録される時間は、イシューを削除する際に次のいずれかの方法で処理されます。

* イシューが後で復元された場合、プロジェクトに移動しても、イシューで復元されない。
* イシューが後で復元された場合は、削除され、イシューで復元される。

  これは、時間が記録されたタスクを持つプロジェクトを削除しようとした場合にも該当します。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  イシューに時間が記録されている場合の削除の環境設定について詳しくは、[タイムシートおよび時間設定の指定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

* イシューまたはイシューの承認に割り当てられたユーザーは、プロジェクトチームに残ります。\
  プロジェクトチームについて詳しくは、[プロジェクトチームの概要](../../../manage-work/projects/planning-a-project/project-team-overview.md)を参照してください。

## イシューを削除

* [プロジェクト内の複数のイシューを同時に削除](#delete-multiple-issues-in-a-project-simultaneously)
* [単一のイシューを削除](#delete-a-single-issue)

### プロジェクト内の複数のイシューを同時に削除  {#delete-multiple-issues-in-a-project-simultaneously}

1. **メインメニュー**&#x200B;に移動します。
1. 「**プロジェクト**」をクリックします。
1. 削除するイシューを含むプロジェクト名をクリックします。
1. 左側のパネルで「**イシュー**」をクリックします。
1. イシューを選択し、リストの上部で&#x200B;**削除**&#x200B;アイコン ![](assets/delete.png) をクリックします。

1. 削除が許可されている場合は、「**はい、削除します**」をクリックします。\
   時間が記録されたイシューの削除を Workfront 管理者が許可していない場合があります。\
   イシューの削除に必要なアクセスおよび権限について詳しくは、[イシューを削除](#access-and-permissions-needed)を参照してください。

### 単一のイシューを削除 {#delete-a-single-issue}

{{step1-to-projects}}

1. 削除するイシューを含むプロジェクト名をクリックします。
1. 左側のパネルで「**イシュー**」をクリックします。

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 削除するイシューの名前をクリックします。
1. 次をクリック： **その他** 問題名の右側にあるメニュー。

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. クリック **問題を削除**.
1. 削除が許可されている場合は、「**はい、削除します**」をクリックします。

   時間が記録されたイシューの削除を Workfront 管理者が許可していない場合があります。\
   イシューの削除に必要なアクセスおよび権限について詳しくは、[イシューを削除](#access-and-permissions-needed)を参照してください。

## 削除されたイシューを復元

Workfront またはグループ管理者は、イシューを削除してから 30 日以内に復元できます。Workfront での項目の復元について詳しくは、[削除した項目を復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。
