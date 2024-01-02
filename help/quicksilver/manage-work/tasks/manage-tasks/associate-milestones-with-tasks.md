---
product-area: projects
navigation-topic: manage-tasks
title: タスクへのマイルストーンの関連付け
description: マイルストーンをタスクに関連付けて、プロジェクトの有効期間中に重要なステップに達したタイミングを示すことができます。 マイルストーンをプロジェクト上のタスクに関連付ける前に、マイルストーンパスをプロジェクトに関連付ける必要があります。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# タスクへのマイルストーンの関連付け

<!--Audited: 01/2024-->

マイルストーンをタスクに関連付けて、プロジェクトの有効期間中に重要なステップに達したタイミングを示すことができます。

## アクセス要件

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
   <td> <p>新しいライセンス：標準</p> 
   <p>現在のライセンス：作業中以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクへのアクセスを編集</p> <p><b>メモ</b>

アクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

マイルストーンをタスクに関連付ける前に、次の設定が必要です。

* Workfrontの管理者は、マイルストーンパスを作成する必要があります。詳しくは、 [マイルストーンパスを作成する](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* マイルストーンパスをプロジェクトに関連付ける必要があります。

  詳しくは、 [プロジェクトを編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* マイルストーンパスをプロジェクトに関連付けるには、プロジェクトのステータスが「計画」または「現在」である必要があります。

  >[!TIP]
  >
  >マイルストーンビューを使用してプロジェクトのマイルストーンの進行状況の最適な概要を把握するには、親タスクを作成し、それらをプロジェクトの各主要フェーズに関連付ける必要があります。 次に、これらの親タスクをマイルストーンパスの各マイルストーンに関連付けます。

## マイルストーンとタスクの関連付け

マイルストーンパスをプロジェクトに関連付けた後、タスクにマイルストーンを割り当てることができます。

1. タスクに移動して、 **その他** アイコン ![](assets/more-icon.png) をタスク名の右にドラッグし、 **編集**.

   タスクとマイルストーンは 1 対 1 の関係にあります。 同じマイルストーンを複数のタスクに関連付けることはできません。 各タスクは、1 つのマイルストーンにリンクすることも、1 つのタスクにマイルストーンをマッピングすることもできます。

1. クリック **設定**」をクリックし、 **マイルストーン** タスクのフィールド。
1. 「**保存**」をクリックします。
1. （オプション）タスクのリストで、 **ステータスアイコン** 列を使用して、マイルストーンを持つタスクを特定します。 「ステータスアイコン」列にマイルストーンのひし形インジケータが表示されます。

   詳しくは、 [Adobe Workfrontでビューを作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![](assets/amwt3.png)

1. （オプション）プロジェクトのリストに移動し、 **マイルストーン** マイルストーンタスクの進行状況を特定するビュー。

   ![](assets/milestone-view-project-list.png)
