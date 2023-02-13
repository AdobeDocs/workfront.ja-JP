---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの共有
description: Adobe Workfront管理者がアクセスレベルを割り当てる際に、ダッシュボードの表示や編集のためのアクセス権をユーザーに付与します。 ユーザーに付与されるアクセスレベルに加えて、共有する特定のダッシュボードを表示または管理する権限をユーザーに付与することもできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# ダッシュボードの共有

Adobe Workfront管理者がアクセスレベルを割り当てる際に、ダッシュボードの表示や編集のためのアクセス権をユーザーに付与します。 問題へのアクセス権の付与について詳しくは、 [レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

ユーザーに付与されるアクセスレベルに加えて、共有する特定のダッシュボードを表示または管理する権限をユーザーに付与することもできます。 アクセスレベルと権限の詳細については、 [アクセスレベルと権限の連携](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

>[!NOTE]
>
>Workfront管理者は、システム内のすべてのユーザーに対して、それらの項目の所有者にならずに、システム内の項目に対する権限を追加または削除できます。

## アクセス要件

オブジェクトを共有するには、次の条件を満たす必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権以上の表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードの表示権限以上</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ダッシュボードを共有するには、まずダッシュボードを作成する必要があります。

ダッシュボードの作成について詳しくは、 [ダッシュボードの作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## ダッシュボードの共有に関する考慮事項

以下の考慮事項に加えて、 [レポート、ダッシュボード、カレンダーの共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* ダッシュボードの作成者には、デフォルトで、ダッシュボードに対する管理権限が付与されています。

* 自分で作成したダッシュボードを、他の個人、チーム、グループ、職務上の役割、会社と共有できます。 また、自分が作成し、自分と共有していたダッシュボードを他のユーザーと共有することもできます。
* また、システム全体で表示できるようにすることで、組織全体と共有することもできます。
* 個々のダッシュボードを共有することも、リストから複数のダッシュボードを共有することもできます。
* ダッシュボードを共有する場合、ユーザーは、デフォルトで、ダッシュボード上のすべてのレポートオブジェクトに対して表示権限を継承します。

   Workfrontのオブジェクトの階層について詳しくは、 [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   継承された権限の表示については、 [オブジェクトの継承された権限の表示](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## ダッシュボードの共有

1 つのダッシュボードまたはリストから複数のダッシュボードを共有する操作は同じです。

1. ダッシュボードのリストに移動し、1 つまたは複数のダッシュボードを選択して、 **共有** ![](assets/share-icon.png).

   または

   1 つのダッシュボードの名前をクリックし、「**ダッシュボードのアクション/**」をクリックします。**共有**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. 内 **担当者、チーム、役割、グループ、会社の追加…** フィールドに、ダッシュボードを共有するユーザー、チーム、役割、グループまたは会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。
1. （オプション）システム内のすべてのユーザーがダッシュボードにアクセスできるようにするには、 **設定** 共有ダイアログボックスの右上隅にあるアイコンをクリックし、 **この機能をシステム全体で表示**.

1. 「**保存**」をクリックします。
