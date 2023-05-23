---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'グループ化：Portfolio所有者、プログラム所有者、プロジェクト所有者、プロジェクトステータスに関する 4 レベルのタスクグループ'
description: このタスクのグループ化は、4 つのレベルのグループ化を提供します。 この場合、タスクは、Portfolio所有者、プログラム所有者、プロジェクト所有者、プロジェクトステータス別にグループ化されます。 標準のインターフェイスを使用して、グループ化を最大 3 レベルまで設定できます。 4 番目のレベルを追加するには、[ テキストモード ] を使用する必要があります。 同時に 4 つを超える条件でレポートをグループ化することはできません。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# グループ化：Portfolio所有者、プログラム所有者、プロジェクト所有者、プロジェクトステータスの 4 レベルのタスクグループ

このタスクのグループ化は、4 つのレベルのグループ化を提供します。 この場合、タスクは、Portfolio所有者、プログラム所有者、プロジェクト所有者、プロジェクトステータス別にグループ化されます。 標準のインターフェイスを使用して、グループ化を最大 3 レベルまで設定できます。 4 番目のレベルを追加するには、[ テキストモード ] を使用する必要があります。 同時に 4 つを超える条件でレポートをグループ化することはできません。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <td> <p>グループ化を変更するリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してグループ化を変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Portfolio所有者、プログラム所有者、プロジェクト所有者、プロジェクトステータスに関する 4 レベルのタスクグループを作成する

このグループ化を適用するには：

1. タスクのリストに移動します。
1. 次の **グループ化** ドロップダウンメニューで、「 **新しいグループ化**.

1. クリック&#x200B;**テキストモードに切り替え**.
1. 内のテキストを削除します。 **レポートをグループ化** 領域
1. 次のコードに置き換えます。

   <pre>group.0.linkedname=project<br>group.0.name=Portfolio所有者<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=プログラム所有者<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. クリック **グループ化を保存**.
