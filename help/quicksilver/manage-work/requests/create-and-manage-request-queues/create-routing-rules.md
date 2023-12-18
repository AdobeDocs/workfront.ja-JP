---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: ルーティングルールの作成
description: ルーティングルールは、リクエストキューに問題を送信する際のAdobe Workfrontの処理を制御します。 リクエストキューの作成の詳細は、「リクエストキューの作成」を参照してください。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: e971f08a1ee9bbf27a78916dbec57ca729407c03
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 1%

---

# ルーティングルールの作成

<!-- Audited: 12/2023 -->

ルーティングルールは、リクエストキューに問題を送信する際のAdobe Workfrontの処理を制御します。 リクエストキューの作成について詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

ルーティングルールは、送信された問題やリクエストを解決するのに最適な方法を備えた特定のユーザーまたはジョブロールに問題を送信します。 ルーティングルールは通常、キュートピックに関連付けられ、問題または要求に適用されるルーティングルールを制御するために使用されます。

## アクセス要件

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>
    <p>新規：標準</p>
    <p>または</p>
    <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p> プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## ルーティングルールの作成

1. リクエストのルーティングルールを追加するプロジェクトに移動します。
1. クリック **ルーティングルール** をクリックします。 クリックが必要になる場合があります。 **表示を増やす**&#x200B;を、 **ルーティングルール**.
1. クリック **新しいルーティングルール** 」をクリックして新しいルールを追加します。
1. ルーティング・ルールに次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名前</strong> </td> 
      <td>ルーティングルールの名前。 プロジェクトにこの情報を表示するアクセス権がある場合は、ルーティングルールを表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>ルーティングルールの説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>デフォルトの担当者*</strong> </td> 
      <td>新しい問題を割り当てる必要があるアクティブなユーザーまたはアクティブなジョブの役割を追加します。 このフィールドには、デフォルトの担当者を 1 人だけ指定できます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>デフォルトのチーム*</strong> </td> 
      <td>新しいイシューを割り当てる必要があるアクティブなチームを追加します。 このフィールドで使用できるデフォルトのチームは 1 つだけです。

   <p><b>メモ</b></p>

   問題の送信後、その割り当てを編集し、他のユーザー、ロールまたはチームを割り当てることができます。 詳しくは、  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">問題の割り当て</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プロジェクトへのルート</strong> </td> 
      <td>これは、問題が追加されるプロジェクトです。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*ルーティングルールに関連付けられた後にユーザー、ジョブロール、またはチームが非アクティブ化された場合、リクエストは引き続きそのユーザーにルーティングされます。 すべてのルーティングルールのインベントリを定期的に作成し、非アクティブな割り当てをアクティブな割り当てに置き換える必要があります。

   イシューをプロジェクトにルーティングすると、そのイシューに対する権限を持つユーザーは、そのプロジェクトに設定された権限を受け取ります。 プロジェクトに対する権限の設定については、 [Adobe Workfrontでプロジェクトを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![[ 新しいルーティング規則 ] ボックス](assets/new-routing-rule-box.png)

1. 「**保存**」をクリックします。

   このプロセスは、ルーティング規則のみを定義します。 問題がリクエストキューに送信されたときに確実にルーティングされるようにするには、 **キューの詳細** 下のタブ **デフォルトのルート**.

   リクエストキューへのデフォルトルートの追加については、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   複数のルーティング・ルールをリクエスト・キューに関連付ける場合は、複数のキュー・トピックを作成し、各トピックを個別のルーティング・ルールに関連付ける必要があります。 キューのトピックの作成について詳しくは、 [キュートピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
