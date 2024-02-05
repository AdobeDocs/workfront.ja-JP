---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトの共有
description: Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにオブジェクトの表示や編集のアクセス権を付与します。オブジェクトへのアクセス権の付与について詳しくは、カスタムアクセスレベルの作成または変更を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 61%

---

# オブジェクトの共有

<!--Audited: 01/2024-->

Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにオブジェクトの表示や編集のアクセス権を付与します。オブジェクトへのアクセス権の付与について詳しくは、[カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

ユーザーに付与されるアクセスレベルに加えて、自分が作成した特定のオブジェクトや、自分が共有のアクセス権を持つ特定のオブジェクトを表示または編集する権限をユーザーに付与することもできます。アクセスレベルと権限について詳しくは、[アクセスレベルと権限の連携方法](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

オブジェクトに対する共有権限について詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

>[!NOTE]
>
>Workfront 管理者は、システム内のすべてのユーザーに対して、システム内のアイテムに対する権限の追加や削除を、それらのアイテムの所有者にならなくても行うことができます。

この記事では、次のオブジェクトを共有する方法について説明します。

* プロジェクト、タスク、イシュー
* ポートフォリオ、プログラム
* ドキュメント

Workfront で他のすべてのオブジェクトを共有する方法について詳しくは、次の記事も参照してください。

* テンプレートについては、[プロジェクトテンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md)を参照してください。
* プルーフについては、[Workfront Proof でのプルーフの共有](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)を参照してください。
* レポート、ダッシュボード、カレンダーについては、次の記事を参照してください。

   * [Adobe Workfront でのレポートの共有](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [ダッシュボードの共有](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [カレンダーレポートの共有](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

  また、 [レポート、ダッシュボード、カレンダーの共有](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) レポート、ダッシュボード、カレンダーの共有に関する一般情報を参照してください。

* フィルター、ビューおよびグループ化については、[フィルター、ビューまたはグループ化の共有](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)を参照してください。
* ドキュメントフォルダーについては、[ドキュメントフォルダーの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)を参照してください。
* プランについては、[シナリオプランナーでのプランの共有](../../scenario-planner/share-a-plan.md)を参照してください。

  追加のライセンスが必要です。

* 目標については、[Workfront Goals での目標の共有](../../workfront-goals/workfront-goals-settings/share-a-goal.md)を参照してください。追加のライセンスが必要です。

## アクセス要件

オブジェクトを共有するには、次の条件を満たしている必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新しいライセンス：標準</p> 
   または
   <p>現在のライセンス：作業中以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>共有するオブジェクトに対する表示以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>共有するオブジェクトに対する表示またはそれ以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 単一のオブジェクトの共有 {#share-a-single-object}

1. 共有するオブジェクトに移動します。

   共有可能なオブジェクトについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。
1. プロジェクト、タスク、イシューの場合：

   オブジェクト名の横にある「**共有**」ボタンをクリックします。

   ![](assets/new-share-button.png)

   または

   ドキュメント、ポートフォリオおよびプログラムの場合：

   次をクリック： **その他** アイコン ![](assets/more-icon.png)オブジェクト名の横にあるをクリックし、 **共有** または **共有。**

   ![](assets/share-a-document-350x160.png)

1. Adobe Analytics の **&lt; オブジェクト名 > へのアクセス権を付与** ボックス（ドキュメント、ポートフォリオ、プログラムの場合）、または **&lt; オブジェクト名 > へのアクセスを許可** ボックス（プロジェクト、タスク、タスク、問題の場合）に、オブジェクトを共有するユーザー、チーム、役割、グループ、または会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   例えば、プロジェクトを共有している場合、 **へのプロジェクトアクセス権の付与** フィールドに入力します。

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

   ![](assets/nwe-project-sharing-modal-350x456.png)

   >[!TIP]
   >
   >同様の名前を持つ複数のエンティティが存在する場合は、それらすべてがタイプの下に表示されます。エンティティの名前はアルファベット順に表示されます。ただし、エンティティタイプが表示される順序はランダムです。
   >
   >
   >![](assets/sharing-entities-named-similarly-in-sharing-box-350x179.png)   >
   >

1. （オプション）オブジェクトへのアクセスを許可するユーザー、チーム、役割またはグループごとに、手順 3 を繰り返します。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: esnure this stays accurate; in the editor it looks like step 4 but one step is conditioned entirely for one version or another)
   </MadCap:conditionalText>
   -->

1. 手順 3 で追加した各ユーザー、チーム、役割、グループまたは会社に対する権限を指定するには、ドロップダウンメニューをクリックし、付与する権限レベルを選択します。

   オブジェクトからの権限の削除については、 [オブジェクトから権限を削除](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   次のオプションを使用できます。

   * **表示：** ユーザーは項目を確認し、共有できます。
   * **Contribute**：ユーザーは、更新、ログ情報の記録、マイナーな編集、共有のほか、すべての表示権限をおこなうことができます。

     >[!TIP]
     >
     >以下のオブジェクトに対してのみ、Contribute の権限を付与できます。
     >
     >   
     >   
     >   * プロジェクト
     >   * タスク
     >   * イシュー
     >   
     >

   * **管理：** ユーザーは、管理権限を持たずにオブジェクトに対する完全なアクセス権を持ちます（管理権限はアクセスレベルで付与されます）。 また、すべての表示および投稿権限も持っています。

     >[!NOTE]
     >
     >Workfront管理者またはオブジェクト作成者は、これらのエンティティから権限を削除できます。

     ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

1. （オプション）「 **詳細オプション** ：オブジェクトに対する特定の権限を設定します。

   表示、管理および参加の詳細設定オプションは、選択したオブジェクトに応じて異なります。\
   権限レベルについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. （オプション）このオブジェクトをシステム内のすべてのユーザーが使用できるようにするには、 **ギア** アイコン ![](assets/gear-icon-settings-with-dn-arrow.jpg) を選択し、ドロップダウンメニューで「 **この機能をシステム全体で表示する**.

   すべてのユーザーは、設定した権限に基づいてオブジェクトを表示できます。

1. （オプションおよび条件付き）プロジェクトを共有する場合、 **ギア** アイコン ![](assets/gear-icon-settings-with-dn-arrow.jpg)を選択し、ドロップダウンメニューで「 **自分のプロジェクトアクセステンプレートとして設定** 権限をテンプレートとして設定する場合。\
   1 つのプロジェクトに対して権限を定義した後、次回プロジェクトをゼロから作成する際に、同じ権限が自動的に適用されます。

   >[!NOTE]
   >
   >プロジェクトアクセステンプレートは、アクセスレベルで Workfront 管理者が付与した共有のデフォルトよりも優先されます。\
   >アクセスレベルでプロジェクトの共有の既定を指定する方法の詳細については、「 [プロジェクトへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->

   テンプレートを共有する際に、テンプレートから作成されるプロジェクトに対する権限を指定できます。 詳しくは、 [プロジェクトテンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. （オプション）オブジェクトをパブリックにするには、「**これを外部ユーザーに公開**」をクリックします。

   >[!TIP]
   >
   >このオプションは、一部のオブジェクトでは利用できません。

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png)

1. （条件付き）オブジェクトを外部ユーザーに公開した場合、 **リンクをコピー**&#x200B;をクリックし、外部ユーザーにリンクを配布します。\
   リンクを使用してすべてのユーザーがオブジェクトを表示できます。

   >[!CAUTION]
   >
   >機密情報を含んだオブジェクトを外部ユーザーと共有する場合は、注意することをお勧めします。Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

1. 「**保存**」をクリックします。

## オブジェクトを一括共有

オブジェクトのリストから、複数のオブジェクトを一度に他のユーザー、チーム、グループ、担当業務または会社と共有できます。

>[!IMPORTANT]
>
>オブジェクトを一括で共有する場合、個々のオブジェクトに対する権限を持つエンティティの名前は表示されません。オブジェクトを一括で共有する場合、共有リストに追加するエンティティは、選択したオブジェクトに追加されます。個々のオブジェクトに関連付けられたエンティティは上書きされません。

オブジェクトを一括で共有するには：

1. オブジェクトのリストに移動します。
1. リスト内の 2 つ以上のオブジェクトを選択します。
1. **共有**&#x200B;アイコン ![](assets/share-icon.png) をクリックします。\
   オブジェクトへのアクセス権を持つユーザーは、一括共有時に使用可能として表示されません。

   >[!NOTE]
   >
   >選択したオブジェクトを共有する権限がない場合、「**共有**」ボタンは表示されません。

1. Adobe Analytics の **&lt; オブジェクト名 > アクセスを編集** フィールドに、権限を付与するユーザー、チーム、グループ、ジョブの役割、または会社の名前を入力します。

   例えば、プロジェクトを共有している場合、 **次のプロジェクトへのアクセスを許可** フィールドに入力します。

   ![](assets/share-multiple-projects-people-box-nwe-350x480.png)

1. この記事にある[単一のオブジェクトの共有](#share-a-single-object)セクションの手順 4～9 に従って、選択したオブジェクトの共有を続行します。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure these steps stay accurate; always look at them in the viewer; because of condiitoning, the steps numbers in the editor are different!!!!!!*****)
   </MadCap:conditionalText>
   -->

1. 「**保存**」をクリックします。
