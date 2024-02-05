---
product-area: projects
navigation-topic: update-work-in-a-project
title: イシューのステータスの更新
description: イシューのステータスを更新して、イシューの発生場所と進行状況を他の人に知らせることができます。
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 66%

---

# イシューのステータスの更新

<!--Audited: 01/2024-->

イシューのステータスを更新して、イシューの発生場所と進行状況を他の人に知らせることができます。

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
   <td> <p>新しいライセンス：寄稿者以上</p>
   または
   <p>現在のライセンス：リクエスト以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## イシューのステータス

Workfront のイシューのデフォルトのステータスは次のとおりです。

* 新規
* 処理中
* フィードバック待ち
* 保留中
* 解決されない
* 再オープン
* クローズ
* 解決済み

Adobe Workfront 管理者は、組織のイシューに対してカスタムステータスを追加できます。また、イシューのタイプに応じて、ステータスを使用可能にすることもできます。

カスタムステータスとイシューのタイプについて詳しくは、次の記事を参照してください。

* [ステータスを作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [イシューの作成](../../../manage-work/issues/manage-issues/create-issues.md)

イシューのステータスは、手動で更新することも、特定のアクションが実行されたときに Workfront で自動的に更新することもできます。

## イシューのステータスを手動で更新

Workfrontの次の領域で、問題のステータスを更新できます。

* タスクページの発行ヘッダーです。
* イシューの編集時の「イシューの編集」ボックス。
* 問題ページの「詳細」セクション。
* イシューリストまたはレポートで、ステータスフィールドがビューに表示されている場合。
* （問題の Summary パネル）。

問題ヘッダーで問題ステータスを手動で更新するには：

1. ステータスを更新するイシューに移動します。
1. イシューのヘッダーの「**ステータス**」フィールドをクリックし、新しいステータスを選択します。
1. 問題の完了を視覚的に示すには、下のバブルをドラッグまたはダブルクリックします **完了率** （問題のヘッダー内）

   または

   イシューのヘッダーのバブル内をクリックして、割合を入力します。

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. （オプション）更新に関する追加情報を提供するには、次のいずれかの操作を行います。

   * 更新に関するメモを追加するには、 **更新** 「 」セクションで、「 」をクリックします。 **新しいコメント**&#x200B;メモを入力します。

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 更新を特定のユーザーに通知するには、ユーザー名を **担当者またはチームのタグ付け** コメントを入力すると表示されるフィールド。 詳しくは、[更新時の他のユーザーへのタグ付け](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。
   * 問題のコミット日を更新するには、 **問題の詳細**」、「 **コミット日** フィールドに入力します。 詳しくは、 [問題の編集](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  割り当て先がコミット日を更新できるのは、問題の担当者のみです。



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## イシューのステータスを自動的に更新

Workfront は、以下の表に示すアクションが発生すると、イシューの既存のステータスを別のステータスに自動的に更新します。

>[!NOTE]
>
>以下の表のステータスは、デフォルトのシステムステータスです。Workfront 管理者またはグループ管理者は、Workfront のインスタンスでステータスの名前を変更できます。Workfront でのステータスの作成と管理について詳しくは、[ステータスを作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>アクション</b></td> 
   <td><b>元のステータス</b></td> 
   <td><b>新しいステータス</b></td> 
  </tr> 
  <tr> 
   <td>イシューの完了率を 100％に更新</td> 
   <td>新規または進行中</td> 
   <td>クローズ</td> 
  </tr> 
  <tr> 
   <td>イシューの完了率を 100％から低い数に更新</td> 
   <td>クローズ </td> 
   <td>処理中</td> 
  </tr> 
  <tr> 
   <td>イシューに関連付けられた解決オブジェクトのステータスを更新</td> 
   <td>各種ステータス</td> 
   <td> <p>各種ステータス</p> <p>オブジェクトの解決とイシューのステータスに対する影響について詳しくは、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決中オブジェクトと解決可能オブジェクトの概要</a>の記事の「解決中オブジェクトの状態と解決可能オブジェクトの状態の同期」の節を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>「イシューの取り組みを開始」ボタンをクリックして、割り当てられたイシューの作業を確認します</span> </td> 
   <td><span>新規</span> </td> 
   <td> <p>ホームチーム設定の「イシューの取り組みを開始」ボタンに関連するステータス。 </p> <p>「作業をする」ボタンを「イシューの取り組みを開始」ボタンに置き換える方法について詳しくは、<span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業をする」ボタンを「イシューの取り組みを開始」ボタンに置き換える</a></span>を参照してください<span>。</span> </p> <p>ヒント：「イシューの取り組みを開始」をクリックした後に「<span data-mc-conditions="QuicksilverOrClassic.Quicksilver">元に戻す</span>」ボタンをクリックすると、ステータスが新規に戻ります。 </p> </td> 
  </tr> 
 </tbody> 
</table>
