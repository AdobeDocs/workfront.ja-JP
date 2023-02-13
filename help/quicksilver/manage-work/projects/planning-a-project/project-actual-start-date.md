---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの概要実績開始日
description: プロジェクト、タスクおよびタスクは、Adobe Workfrontで実際の開始日を持ちます。 タスクおよび問題については、この日付が「処理中」とマークされています。 プロジェクトの場合は、プロジェクトの最初のタスクが [ 進行中 ] としてマークされるか、完了した日付です。
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# プロジェクトの概要実績開始日

プロジェクト、タスクおよびタスクは、Adobe Workfrontで実際の開始日を持ちます。 タスクおよび問題については、この日付が「処理中」とマークされています。 プロジェクトの場合は、プロジェクトの最初のタスクが [ 進行中 ] としてマークされるか、完了した日付です。

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
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセス権を表示または高くする</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限以上</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Workfrontの実際の開始日に関する考慮事項

* 実際の開始日は、プロジェクト、タスクおよびタスクの詳細セクションにあります。 
* プロジェクト、タスク、またはタスクの実際の開始日は、これらの項目を作成する際に入力されません。
* [ 実績開始日 ] は、プロジェクト、タスク、またはタスクで実際に作業が開始したときに設定されます。
* プロジェクトの作業がまだ開始されていない場合、[ プロジェクトの詳細 ] タブに [ 実際の開始日 ] が表示されません。

   [ 実績開始日 ] タブと [ タスクの詳細 ] タブには、まだ作業が開始されていない場合は空白で表示されます。

* タスクやイシューの実際の開始日は手動で変更できますが、プロジェクトの実際の開始日は変更できません。

## プロジェクトの実際の開始日に関する考慮事項

* Workfrontは、次のいずれかが発生すると、プロジェクトの実際の日付を自動的に設定します。

   * タスクの担当者がタスクのステータスを *新規* 等しくない他のステータスに *新規*.

   * タスクの担当者がタスクの完了率を変更します。

      >[!IMPORTANT]
      >
      >プロジェクトが「現在」とマークされている場合、「プロジェクトの実際の開始日」には入力されません。 実績作業時間は、プロジェクトの実績開始日が設定される前に、プロジェクトのタスクで開始する必要があります。

      この場合、プロジェクトの「実績開始日」は、プロジェクトの最も早いタスクに対してこれらのアクションが実行された日時に設定されます。 これは、プロジェクトが実際にこの日時に開始されたことを示します。

## プロジェクトの実際の開始日を見つける

プロジェクトの実際の開始日は、次の領域で確認できます。

* （プロジェクトの詳細セクション）。
* プロジェクトのレポートまたはビューで、レポートのオブジェクト Project の実績開始日を追加する場合。

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

プロジェクトの「詳細」セクションで実際の開始日を検索する手順は、次のとおりです。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **プロジェクト**.
1. 実際の開始日を表示するプロジェクトをクリックします。
1. クリック **プロジェクトの詳細** 左のパネルで、 **概要** 」セクションに入力します。

   実際の開始日は、他のプロジェクト日付と共に表示されます。

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
