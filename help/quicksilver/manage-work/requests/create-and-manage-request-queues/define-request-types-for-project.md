---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: プロジェクトのリクエストタイプの定義
description: Adobe Workfront に記録されるイシューやリクエストの種類を、リクエストタイプごとに整理できます。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: ht
source-wordcount: '430'
ht-degree: 100%

---

# プロジェクトのリクエストタイプの定義

Adobe Workfront に記録されるイシューやリクエストの種類を、リクエストタイプごとに整理できます。

これは、理由を報告したり、プロジェクトの全期間中にどのような予期せぬ作業が発生する可能性があるのかを把握するのに役立ちます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront プラン</a>*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">ライセンスの概要</a>*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対して権限を管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

始める前に、以下を行う必要があります。

* プロジェクトを所有または作成

  プロジェクトの作成について詳しくは、[プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md)を参照してください。

## リクエストタイプに関する考慮事項

* プロジェクトの&#x200B;**キューの詳細**&#x200B;領域を設定するときに、プロジェクトに記録できるイシューやリクエストのタイプを指定できます。
* プロジェクトのリクエストタイプを定義できるようにするために、プロジェクトをリクエストキューとして有効にする必要はありません。プロジェクトに関して記録されるイシューには、別のリクエストタイプのラベルを付けることができます。
* プロジェクトにキュートピックを追加する場合、新しいイシューやリクエストを追加するときに表示されるように、それぞれのキュートピックでリクエストタイプを定義する必要があります。詳しくは、[キュートピックの作成](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。

## プロジェクトのイシュータイプまたはリクエストタイプを定義

1. メインメニュー ![](assets/main-menu-icon.png) で「**プロジェクト**」をクリックします。

1. プロジェクトの名前をクリックして開きます。
1. 左側のパネルで、「**キューの詳細**」をクリックします。
1. 「**キューのプロパティ**」セクションで、プロジェクトに必要な&#x200B;**リクエストタイプ**&#x200B;を選択します。

   >[!NOTE]
   >
   >少なくとも 1 つのリクエストタイプを選択する必要があります。複数のリクエストタイプを選択できます。

   次のタイプから選択します。

   * バグレポート
   * 変更依頼
   * イシュー
   * リクエスト

   >[!TIP]
   >
   >Workfront 管理者が、これらのオプションの一部の名前を変更している可能性があります。詳しくは、[リクエストタイプの設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)を参照してください。

1. 「**保存**」をクリックします。

   プロジェクトがリクエストキューとして有効になっている場合、タスクやプロジェクトに新しいイシューを入力するとき、またはプロジェクトに新しいリクエストを送信するときに、指定したリクエストタイプを選択できるようになります。
