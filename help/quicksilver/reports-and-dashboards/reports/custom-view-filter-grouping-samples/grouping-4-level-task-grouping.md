---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「グループ化：ポートフォリオ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータスに関する 4 レベルのタスクグループ化」
description: このタスクグループ化では、4 レベルのグループ化を提供します。この場合、タスクは、ポートフォリ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータス別にグループ化されます。標準インターフェイスを使用する場合は、最大 3 レベルのグループ化に限られます。第 4 レベルを追加するには、テキストモードを使用する必要があります。同時に 4 つを超える条件でレポートをグループ化することはできません。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# グループ化：ポートフォリオ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータスに関する 4 レベルのタスクグループ化

このタスクグループ化では、4 レベルのグループ化を提供します。この場合、タスクは、ポートフォリ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータス別にグループ化されます。標準インターフェイスを使用する場合は、最大 3 レベルのグループ化に限られます。第 4 レベルを追加するには、テキストモードを使用する必要があります。同時に 4 つを超える条件でレポートをグループ化することはできません。

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>グループ化を変更するためのリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、ビュー、グループ化へのアクセス権を編集して、グループ化を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ポートフォリオ所有者、プログラム所有者、プロジェクト所有者およびプロジェクトステータスに関する 4 レベルのタスクグループ化の作成

このグループ化を適用するには、次の操作を行います。

1. タスクのリストに移動します。
1. 「**グループ化**」ドロップダウンメニューで「**新規グループ化**」を選択します。

1. 「**テキスト モードに切り替える**」をクリックします。
1. **報告書のグループ化**&#x200B;エリア内のテキストを削除します。
1. 次のコードでテキストを置き換えます。
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. 「**グループ化の保存**」をクリックします。
