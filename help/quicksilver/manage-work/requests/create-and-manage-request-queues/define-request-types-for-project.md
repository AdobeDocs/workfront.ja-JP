---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: プロジェクトの要求タイプの定義
description: Adobe Workfrontにログインする問題やリクエストの種類は、リクエストのタイプ別に整理できます。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 2%

---

# プロジェクトの要求タイプの定義

Adobe Workfrontにログインする問題やリクエストの種類は、リクエストのタイプ別に整理できます。

この組織は、レポートの理由を知るのに役立ち、プロジェクトの存続期間中に予期しない作業が発生した可能性があることをユーザーが理解するのに役立ちます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a>*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">ライセンスの概要</a>*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

開始する前に、次の操作を行う必要があります。

* プロジェクトを作成する

  プロジェクトの作成について詳しくは、 [プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md).

## リクエストタイプに関する考慮事項

* プロジェクトにログオンできる問題や要求の種類は、 **キューの詳細** プロジェクトの領域。
* プロジェクトの要求タイプを定義するために、プロジェクトを要求キューにする必要はありません。 プロジェクトに関してログに記録される問題には、別のリクエストタイプのラベルを付けることができます。
* プロジェクトにキュートピックを追加する場合、新しい問題やリクエストを追加する際に表示するリクエストタイプを各キュートピックに定義する必要があります。 詳しくは、 [キュートピックを作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## プロジェクトの問題または要求タイプを定義する

1. クリック **プロジェクト** をクリックします。 ![](assets/main-menu-icon.png)

1. プロジェクトの名前をクリックして開きます。
1. 左側のパネルで、 **キューの詳細**.
1. 内 **キューのプロパティ** セクションで、 **リクエストタイプ** プロジェクトに必要です。

   >[!NOTE]
   >
   >少なくとも 1 つのリクエストタイプを選択する必要があります。 複数のリクエストタイプを選択できます。

   次のタイプから選択します。

   * バグレポート
   * 変更依頼
   * 問題
   * リクエスト

   >[!TIP]
   >
   >Workfront管理者が、これらのオプションの一部の名前を変更している可能性があります。 詳しくは、 [リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. 「**保存**」をクリックします。

   指定したリクエストタイプは、タスクやプロジェクトに新しいイシューを入力する際、またはプロジェクトがリクエストキューとして有効な場合は、プロジェクトに新しいリクエストを送信する際に選択できます。
