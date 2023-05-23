---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'グループ化：リストに 4 つ目のグループを追加'
description: マトリックスレポートでは、4 つのグループを作成できます。 マトリックスレポートの詳細については、「マトリックスレポートの作成」を参照してください。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# グループ化：リストに 4 番目のグループを追加

マトリックスレポートでは、4 つのグループを作成できます。 マトリックスレポートの詳細については、 [マトリックスレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

標準インターフェイスを使用した標準レポートでは、3 つのグループのみを作成できます。 標準レポートに 4 番目のグループを追加するには、テキストモードを使用する必要があります。

![Four_groupings_in_a_standard_report.png](assets/four-groupings-in-a-standard-report-350x59.png)

たとえば、プロジェクト名、進捗状況ステータス、計画完了日別にグループ化されたタスクレポートがあり、そのレポートを [ 割り当て先の名前 ] 別にグループ化するとします。

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

## リストに 4 番目のグループを追加

4 番目のグループを追加するには：

1. タスクのリストに移動します。
1. 次の **グループ化**&#x200B;ドロップダウンメニューで、「 **新しいグループ化**.

1. クリック **テキストモードに切り替え**.
1. 空きスペースに、次のコードを追加します。

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. クリック **完了**&#x200B;を、 **グループ化を保存**.
