---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Adobe Workfront でのレポートの共有
description: Adobe Workfront 管理者は、ユーザーにアクセスレベルを割り当てる際に、レポートの表示や編集を行えるアクセス権を付与します。イシューに対するアクセス権の付与の詳細については、レポート、ダッシュボード、カレンダーへのアクセス権の付与を参照してください。
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: ht
source-wordcount: '807'
ht-degree: 100%

---

# Adobe Workfront でのレポートの共有

Adobe Workfront 管理者は、ユーザーにアクセスレベルを割り当てる際に、レポートの表示や編集を行えるアクセス権を付与します。イシューに対するアクセス権の付与について詳しくは、[レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)を参照してください。

ユーザーに付与するアクセスレベルに加えて、自分が共有を行うアクセス権を持っている特定のレポートを、表示、管理する権限をユーザーに付与することもできます。アクセスレベルと権限について詳しくは、[アクセスレベルと権限の連携方法](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

>[!NOTE]
>
>Workfront 管理者は、システム内のすべてのユーザーに対して、システム内のアイテムに対する権限の追加や削除を、それらのアイテムの所有者にならなくても行うことができます。

## アクセス要件

オブジェクトを共有するには、次の条件を満たしている必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権またはそれ以上の権限を表示</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートの表示以上以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## レポートの共有に関する考慮事項

以下の考慮事項に加えて、[レポート、ダッシュボード、カレンダーを共有](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)も参照してください。

* 作成したレポートを、他の個人、チーム、グループ、担当業務や会社と共有できます。他の人が作成し、自分と共有したレポートを共有することもできます。
* また、組織全体と共有したり、公開したりすることもできます。レポートを公開すると、他のユーザーと共有できる URL が生成されます。
* 個々のレポートを共有したり、レポートのリストから複数のレポートを共有したりすることができます。

## レポートを共有する方法

以下の方法で、Workfront でレポートを共有できます。

* 手動（[レポートを共有](#share-a-report)の節を参照）。
* 自動（共有されているレポートを含むダッシュボードから表示権限を継承することにより）。オブジェクトに対する継承された権限の表示について詳しくは、[オブジェクトの継承された権限を表示](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)を参照してください。

## レポートを共有 {#share-a-report}

リストから 1 つのレポートを共有することも、複数のレポートを共有することも同じです。

1. レポートのリストに移動し、1 つまたは複数のレポートを選択して、「**共有**」をクリックします。

   または

   1 つのレポートの名前をクリックし、**「レポートのアクション」、**「**共有**」の順にクリックします。

   ![](assets/qs-report-actions-sharing.png)

1. 表示されるボックスで、「**担当者、チーム、役割、グループや会社を追加…**」フィールドに、レポートを共有するユーザー、チーム、担当業務、グループや会社の名前を入力し、名前が表示されたら **Enter** を押します。

1. 追加した名前のアクセスレベルを調整するには、名前の右側にあるドロップダウンメニューをクリックし、以下のオプションの 1 つを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">それを表示</td> 
      <td> <p>受信者がアクセスして<strong>レポート</strong> <img src="assets/reports-in-main-menu.png">エリアでレポートを表示し、実行できるようにします。</p> <p>「<strong>詳細設定</strong>」をクリックして、ユーザーがシステム内の誰とでも<strong>共有</strong>できるようにするかどうかを指定します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">それを管理</td> 
      <td> <p>受信者にレポートへの完全な編集アクセス権を許可します。</p> <p>「<strong>詳細設定</strong>」をクリックして、ユーザーがシステムからレポートを<strong>削除</strong>して、システム内の誰とでも<strong>共有</strong>できるようにするかどうかを指定します。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）上記の 2 つの手順を繰り返して、リストに他の名前を追加し、そのオプションを設定します。
1. （オプション）右上隅の共有ボックスの&#x200B;**ギア**&#x200B;アイコン ![](assets/gear-icon-settings-with-dn-arrow.jpg)をクリックし、次のいずれかのオプションを選択します。

   * **これを外部ユーザーに公開：**&#x200B;他のユーザーと共有できる URL を生成する場合は、このオプションを選択します。URL を知っているユーザーは誰でも、Adobe Workfront のライセンスを持っていなくてもレポートにアクセスできます。

     >[!CAUTION]
     >
     >機密情報を含んだオブジェクトを外部ユーザーと共有する場合は、注意することをお勧めします。Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

     >[!NOTE]
     >
     >レポートにプロンプトがあり、それを公開共有する場合、レポートを実行するユーザーがプロンプトを使用してレポートを実行できるようにするには、Workfront にログインする必要があります。Workfront にログインできない場合は、プロンプトが適用されないレポートが表示されます。プロンプトを使用したレポートの共有に関する制限について詳しくは、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)の記事にある[プロンプトレポートの共有に関する制限](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports)を参照してください。

   * **これをシステム全体で表示：**&#x200B;レポートへのアクセス権を持つ Workfront 内の全員がレポートを表示できるようにするには、このオプションを選択します。

1. 「**保存**」をクリックします。
