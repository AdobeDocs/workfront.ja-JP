---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの共有
description: Adobe Workfront 管理者は、ユーザーにアクセスレベルを割り当てるときに、ダッシュボードを表示または編集するためのアクセス権を付与します。ユーザーに付与するアクセスレベルに加えて、自分が共有を行うアクセス権を持っている特定のダッシュボードを、表示、管理する権限をユーザーに付与することもできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 78%

---

# ダッシュボードの共有

<!-- Audited: 1/2025 -->

Adobe Workfront 管理者は、ユーザーにアクセスレベルを割り当てるときに、ダッシュボードを表示または編集するためのアクセス権を付与します。イシューに対するアクセス権の付与について詳しくは、[レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)を参照してください。

ユーザーに付与するアクセスレベルに加えて、自分が共有を行うアクセス権を持っている特定のダッシュボードを、表示、管理する権限をユーザーに付与することもできます。アクセスレベルと権限について詳しくは、[アクセスレベルと権限の連携方法](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

>[!NOTE]
>
>Workfront 管理者は、システム内のすべてのユーザーに対して、システム内のアイテムに対する権限の追加や削除を、それらのアイテムの所有者にならなくても行うことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

オブジェクトを共有するには、次の条件を満たしている必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
    <td> 
      <p>新規：</p>
         <ul>
         <li><p>ライト以上</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>レビュー以上</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>報告書、ダッシュボード、カレンダーへのアクセスを表示する（またはそれ以上）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードの表示権限またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

ダッシュボードを共有するには、まずダッシュボードを作成する必要があります。

ダッシュボードの作成について詳しくは、[ダッシュボードを作成](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)を参照してください。

## ダッシュボードの共有に関する考慮事項

以下の考慮事項に加えて、[レポート、ダッシュボード、カレンダーを共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)も参照してください。

* ダッシュボードの作成者には、デフォルトでタスクの管理権限が付与されています。

* 作成したダッシュボードを、他の個人、チーム、グループ、担当業務や会社と共有できます。他の人が作成し、自分と共有したダッシュボードを共有することもできます。
* また、システム全体で表示できるようにすることで、組織全体と共有することもできます。
* 個々のダッシュボードを共有することも、リストから複数のダッシュボードを共有することもできます。
* ダッシュボードを共有する場合、ユーザーは、デフォルトで、ダッシュボード上のすべてのレポートオブジェクトに対して表示権限を継承します。

  Workfront のオブジェクトの階層について詳しくは、[Adobe Workfront のオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)を参照してください。

  継承された権限の表示について詳しくは、[オブジェクトの継承された権限を表示](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)を参照してください。

## ダッシュボードの共有

リストから 1 つのダッシュボードを共有することも、複数のダッシュボードを共有することも同じです。

1. ダッシュボードのリストに移動し、1 つまたは複数のダッシュボードを選択して、**共有** ![](assets/share-icon.png) をクリックします。

   または

   ダッシュボードの名前をクリックし、**ダッシュボードアクション**/**共有** をクリックします。

   ![](assets/unshimmed-share-dashboard.png)

1. **ユーザー、チーム、役割、グループ、または会社を追加** フィールドに、ダッシュボードを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示される名前をクリックします。
1. （オプション）システム内のすべてのユーザーがダッシュボードにアクセスできるようにするには、共有ダイアログボックスの **招待されたユーザーのみがアクセスできる** ドロップダウンメニューをクリックし、**システム内の全員が表示できる** を選択します。

1. **保存**&#x200B;をクリックします。
