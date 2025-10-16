---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: グループ化：Portfolio所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータスの 4 レベルのタスクのグループ化
description: このタスクグループ化では、4 レベルのグループ化を提供します。この場合、タスクは、ポートフォリ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータス別にグループ化されます。標準インターフェイスを使用する場合は、最大 3 レベルのグループ化に限られます。第 4 レベルを追加するには、テキストモードを使用する必要があります。同時に 4 つを超える条件でレポートをグループ化することはできません。
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 82%

---

# グループ化：ポートフォリオ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータスに関する 4 レベルのタスクグループ化

<!--Audited: 10/2024-->

このタスクグループ化では、4 レベルのグループ化を提供します。この場合、タスクは、ポートフォリ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータス別にグループ化されます。標準インターフェイスを使用する場合は、最大 3 レベルのグループ化に限られます。第 4 レベルを追加するには、テキストモードを使用する必要があります。同時に 4 つを超える条件でレポートをグループ化することはできません。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <p>フィルターの変更者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ポートフォリオ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータスに関する 4 レベルのタスクグループ化の作成

このグループ化を適用するには、次の操作を行います。

1. タスクのリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで「**新規グループ化**」を選択します。

1. 「**テキストモードに切り替える**」をクリックします。
1. **レポートをグループ化**&#x200B;エリアのテキストを削除します。
1. 表示されたボックス内のテキストを次のコードに置き換えます。
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. 「**完了**」をクリックし、「**グループ化の保存**」をクリックします。
1. （オプション）グループ化の名前を更新し、「**グループ化を保存**」をクリックします。
