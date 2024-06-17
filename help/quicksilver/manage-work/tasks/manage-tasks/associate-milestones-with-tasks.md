---
product-area: projects
navigation-topic: manage-tasks
title: タスクへのマイルストーンの関連付け
description: タスクにマイルストーンを関連付けることで、プロジェクト期間の重要なステップに達したことを示すことができます。プロジェクトのタスクにマイルストーンを関連付けるには、まずマイルストーンパスをプロジェクトに関連付ける必要があります。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 97%

---

# タスクへのマイルストーンの関連付け

<!--Audited: 01/2024-->

タスクにマイルストーンを関連付けて、プロジェクトの全期間中に重要なステップに達したときに、それを示すことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規のライセンス：標準</p> 
   <p>現在のライセンス：ワーク以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクへのアクセスを編集</p> <p><b>メモ</b>

アクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

+++

## 前提条件

タスクにマイルストーンを関連付けるには、まず以下が必要です。

* [マイルストーンパスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)の説明に従って、Workfront の管理者がマイルストーンパスを作成する必要があります。

* マイルストーンパスをプロジェクトに関連付ける必要があります。

  詳しくは、[プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* マイルストーンパスをプロジェクトに関連付けるには、プロジェクトのステータスが「計画」または「進行中」になっている必要があります。

  >[!TIP]
  >
  >マイルストーンビューを使用してプロジェクトのマイルストーンの進行状況の概要を最も適切に把握するには、親タスクを作成し、それらをプロジェクトの各主要フェーズに関連付ける必要があります。次に、これらの親タスクをマイルストーンパスの各マイルストーンに関連付けます。

## タスクにマイルストーンを関連付け

マイルストーンパスをプロジェクトに関連付けたら、タスクにマイルストーンを割り当てることができます。

1. タスクに移動し、タスク名の右にある&#x200B;**その他**&#x200B;アイコン ![](assets/more-icon.png) をクリックして「**編集**」を選択します。

   タスクとマイルストーンは 1 対 1 の関係にあります。同じマイルストーンを複数のタスクに関連付けることはできません。各タスクを 1 つのマイルストーンにリンクすることも、各マイルストーンを 1 つのタスクにマッピングすることもできます。

1. 「**設定**」をクリックし、タスクの&#x200B;**マイルストーン**&#x200B;フィールドでマイルストーンを選択します。
1. 「**保存**」をクリックします。
1. （オプション）タスクの一覧で、**ステータスアイコン**&#x200B;の列を追加して、どのタスクにマイルストーンがあるか特定します。「ステータスアイコン」の列にマイルストーンのひし形インジケーターが表示されます。

   詳しくは、[Adobe Workfront でのビューの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)を参照してください。

   ![](assets/amwt3.png)

1. （オプション）プロジェクトの一覧で、**マイルストーン**&#x200B;のビューを選択して、マイルストーンタスクの進捗状況を特定します。

   ![](assets/milestone-view-project-list.png)
