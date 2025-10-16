---
product-area: projects
navigation-topic: manage-issues
title: 問題のコピー
description: イシューまたはリクエストをコピーして、同じプロジェクトまたは別のプロジェクトに保存できます。タスクから別のプロジェクトにイシューをコピーすることもできます。
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 90%

---

# イシューのコピー

<!--Audited: 08/2025-->

イシューまたはリクエストをコピーして、同じプロジェクトまたは別のプロジェクトに保存できます。タスクから別のプロジェクトにイシューをコピーすることもできます。

次のオブジェクトからイシューをコピーできます。

* プロジェクトから同じプロジェクトへ（同じプロジェクトで複製）
* タスクから同じタスクへ（同じタスクで複製）
* プロジェクトから別のプロジェクトへ
* タスクからプロジェクトへ

>[!TIP]
>
>Workfront では、「イシュー」と「リクエスト」が同じような意味で使用されます。プロジェクトとタスクの両方のイシューを記録して、対処する必要がある予期せぬ作業を示すことができます。リクエストを送信することもできます。リクエストは、リクエストキューとして指定されたプロジェクトのイシューとして記録されます。

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
   <td> 
   <ul><li><p>投稿者以上</p> </li>
   <li><p>プロジェクトの「イシュー」セクションにイシューをコピーするためのライト以上のライセンス</p></li></ul>
   または
   <ul><li><p>要求者以上</p> </li>
   <li><p>プロジェクトの「イシュー」セクションにイシューをコピーするためのレビュアー以上のライセンス</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトとタスクへのアクセス権またはそれ以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>イシューを追加する機能を使用してイシューをコピーする先の項目には、Contribute 権限が必要です。</p></td> 
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
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying the issue to with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## イシューをコピーする際の考慮事項

### イシューをコピーする際の一般的な考慮事項

コピープロセス中に、コピーしたイシューに対して、そのイシューに関連するアイテムをコピーすることを選択できます。ただし、以下のリストに示すように、一部のアイテムはデフォルトで新しいイシューにコピーされますが、それ以外のアイテムはコピーされません。

デフォルトでは、次のアイテムが新しいイシューにコピーされます。

* プライマリ連絡先
* カスタムフォームカスタムフィールドの情報は、コピー処理で「カスタムデータ」を選択した場合にのみ、新しいイシューにコピーされます。
* 承認
* 予定開始日と予定完了日

次のオブジェクトは、デフォルトでは新しいイシューにコピーされません。

* ログに記録された時間数

### ドキュメントまたはリクエストキューに関連するイシューについての考慮事項

ドキュメントを含むイシューやリクエストキューに関連付けられているイシューをコピーする際は、次の点を考慮してください。

* **イシューがリクエストキューに関連付けられている場合：**&#x200B;イシューを別のオブジェクトにコピーし、そのイシューをリクエストキューに関連付けると、コピーされたイシューは、最初のイシューが発生した元のキューには関連付けられなくなります。
* **ドキュメントがイシューに添付されている場合：**&#x200B;イシューを別のオブジェクトにコピーし、そのイシューにドキュメントが添付されている場合、ドキュメントとそのバージョンも新しいイシューに移動します。ドキュメントに関連付けられているプルーフや承認は移動しません。
* **イシューがドキュメントまたはフォルダーにリンクされている場合：** Google ドライブなどのサードパーティのサービスにリンクされたドキュメントまたはフォルダーを含むイシューをコピーすると、ドキュメントへのリンクがコピーされたイシューに転送されます。

## リスト内のイシューのコピー

1 つまたは複数のイシューをイシューのリストまたはイシューレポートからコピーできます。

1. コピーする 1 つまたは複数のイシューを含むプロジェクトに移動します。

   または

   イシューレポートに移動します。

1. プロジェクトに移動する場合は、左側のパネルで「**イシュー**」をクリックします。
1. コピーする 1 つまたは複数のイシューを選択し、イシューリストの上部にある&#x200B;**その他のメニュー**&#x200B;をクリックし、「**指定の場所にコピー**」をクリックします。

   ![ リスト内のイシューをコピー ](assets/copy-issue-in-list-nwe-350x169.png)

1. [1 つのイシューをコピー](#copy-a-single-issue)の節の説明に従って、手順 2 からイシューのコピーを続行します。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## 1 つのイシューのコピー {#copy-a-single-issue}

イシューの表示時に 1 つのイシューをコピーできます。

1. コピーするイシューに移動し、イシュー名の右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-icon.png) をクリックして、**コピー先** をクリックします。

   ![ 問題レベルでコピー ](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   **イシューをコピー**&#x200B;ボックスが表示されます。

   ![ イシューボックスをコピー ](assets/copy-issue-box-nwe-350x285.png)

1. 「**宛先プロジェクトを選択**」セクションで、イシューをコピーする先のプロジェクト名を指定します。デフォルトでは、現在のプロジェクトの名前が表示されます。

   >[!TIP]
   >
   >リストには 100 個のプロジェクトのみが表示されます。

1. （条件付き）プロジェクトにイシューをコピーするアクセス権がない場合は、「**アクセスをリクエスト**」をクリックします。
1. （条件付き）宛先プロジェクトのタスクの 1 つにイシューを追加するアクセス権がある場合は、アクセス権をリクエストせずに、引き続き選択した宛先プロジェクトにイシューをコピーします。

   ![ イシューをコピーしてアクセスをリクエスト ](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Workfront 管理者がこれらのプロジェクトにイシューを追加できない場合、選択したプロジェクトが承認待ち、完了または無効の場合にも、同様のメッセージが表示されます。詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. （オプション）「**オプション**」セクションで、以下の表に示すアイテムの選択を解除して、新しいイシューから削除します。デフォルトでは、すべてのオプションが選択されています。

   >[!NOTE]
   >
   >これは、コピーされたイシューのみに影響し、元のイシューには影響しません。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">割り当て</td> 
      <td>イシューに割り当てられているユーザー、担当業務またはチームを削除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況</td> 
      <td>イシューの完了率（存在する場合）を削除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td><span style="line-height: 1.5;">ドキュメントのバージョン、リンクされたドキュメント、フォルダーなど、「ドキュメント」タブ内のすべての項目を削除します。</span> <br>デフォルトでは、ドキュメントのプルーフと承認を別のイシューにコピーすることはできません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">権限</td> 
      <td>イシューの共有先エンティティを削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>イシューの「更新」セクションからコメントを削除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムデータ</td> 
      <td>イシューのカスタムフォームから情報を削除します。イシューに添付されたドキュメントに関連付けられたカスタムフォームに関する情報も削除します（それらのドキュメントがイシューとともにコピーされている場合）。カスタムフォームはイシューとドキュメントに添付されたままになりますが、フォームに関する情報は新しいイシューには引き継がれません。 </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「**タスクを選択**」セクションで、イシューを移動するタスクを選択します。
1. 「**イシューをコピー**」または「**複数のイシューをコピー**」（リスト内の複数のイシューを選択した場合）をクリックします。

   コピーされたイシューは、指定したプロジェクトに追加されます。


