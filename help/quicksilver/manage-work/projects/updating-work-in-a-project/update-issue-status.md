---
product-area: projects
navigation-topic: update-work-in-a-project
title: 問題ステータスを更新
description: 問題のステータスを更新して、問題の発生場所と進行状況を他の人に知らせることができます。
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 2%

---

# 問題ステータスを更新

<!--Audited: 01/2024-->

問題のステータスを更新して、問題の発生場所と進行状況を他の人に知らせることができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>新しいライセンス：寄稿者以上</p>
   または
   <p>現在のライセンス：リクエスト以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>問題へのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>問題に対する権限の管理</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 問題のステータス

Workfrontの問題のデフォルトのステータスは次のとおりです。

* 新規
* 処理中
* フィードバック待ち
* 保留中
* 解決されない
* 再オープン
* クローズ
* 解決済み

Adobe Workfront管理者は、組織の問題に対してカスタムステータスを追加できます。 また、問題のタイプに応じて、ステータスを使用可能にすることもできます。

カスタムステータスと問題のタイプについて詳しくは、次の記事を参照してください。

* [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [イシューの作成](../../../manage-work/issues/manage-issues/create-issues.md)

問題のステータスは、手動で更新することも、特定のアクションが実行されたときにWorkfrontで自動的に更新することもできます。

## 問題ステータスを手動で更新

Workfrontの次の領域で、問題のステータスを更新できます。

* タスクページの発行ヘッダーです。
* イシューの編集時の「イシューの編集」ボックス。
* 問題ページの「詳細」セクション。
* イシューリストまたはレポートで、ステータスフィールドがビューに表示されている場合。
* （問題の Summary パネル）。

問題ヘッダーで問題ステータスを手動で更新するには：

1. ステータスを更新するイシューに移動します。
1. 次をクリック： **ステータス** 「 」フィールドに値を入力し、新しいステータスを選択します。
1. 問題の完了を視覚的に示すには、下のバブルをドラッグまたはダブルクリックします **完了率** （問題のヘッダー内）

   または

   問題のヘッダーのバブル内をクリックして、割合を入力します。

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. （オプション）更新に関する追加情報を提供するには、次のいずれかの操作を行います。

   * 更新に関するメモを追加するには、 **更新** 「 」セクションで、「 」をクリックします。 **新しいコメント**&#x200B;メモを入力します。

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 更新を特定のユーザーに通知するには、ユーザー名を **担当者またはチームのタグ付け** コメントを入力すると表示されるフィールド。 詳しくは、 [更新時の他のユーザーへのタグ付け](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
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

## 問題ステータスを自動的に更新

Workfrontは、以下の表に示すアクションが発生すると、問題の既存のステータスを別のステータスに自動的に更新します。

>[!NOTE]
>
>次の表に、デフォルトのシステムステータスを示します。 Workfront管理者またはグループ管理者は、Workfrontのインスタンスでステータスの名前を変更できます。 Workfrontでのステータスの作成と管理について詳しくは、 [ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td>問題の割合を 100%に更新</td> 
   <td>新規または進行中</td> 
   <td>クローズ</td> 
  </tr> 
  <tr> 
   <td>問題の完了率を 100%から低い数に更新します</td> 
   <td>クローズ </td> 
   <td>進行状況</td> 
  </tr> 
  <tr> 
   <td>問題に関連付けられた解決オブジェクトのステータスを更新します</td> 
   <td>各種ステータス</td> 
   <td> <p>各種ステータス</p> <p>オブジェクトの解決と問題の状態に対する影響の詳細については、この記事の「解決可能なオブジェクトの状態と解決可能なオブジェクトの状態の同期」を参照してください。 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>「問題の開始」ボタンをクリックして、割り当てられた問題の作業を承認します</span> </td> 
   <td><span>新規</span> </td> 
   <td> <p>ホームチーム設定の [ 問題の開始 ] ボタンに関連するステータス。 </p> <p>「Work On It」ボタンを「Start Issue」ボタンに置き換える方法については、 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業対象」ボタンを「開始」ボタンに置き換えます</a></span><span>.</span> </p> <p>ヒント：クリック <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">取り消しボタン</span> 「問題を開始」をクリックすると、ステータスが「新規」に戻ります。 </p> </td> 
  </tr> 
 </tbody> 
</table>
