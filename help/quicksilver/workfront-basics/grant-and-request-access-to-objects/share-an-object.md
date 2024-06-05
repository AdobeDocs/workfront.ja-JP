---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトの共有
description: Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにオブジェクトの表示や編集のアクセス権を付与します。オブジェクトへのアクセス権の付与について詳しくは、カスタムアクセスレベルの作成または変更を参照してください。
author: Alina, Nolan
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 91371c862be6f3b99f0450ff359f601dc913dc0c
workflow-type: tm+mt
source-wordcount: '1962'
ht-degree: 72%

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

  また、レポート、ダッシュボードおよびカレンダーの共有に関する一般情報については、[レポート、ダッシュボード、カレンダーを共有](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)を参照してください。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規のライセンス：標準</p> 
   または
   <p>現在のライセンス：ワーク以上</p>
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

*ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## プロジェクト、タスクまたはイシューをそのページから共有する

1. 共有するプロジェクト、タスクまたは問題のページに移動します。

   共有可能なオブジェクトについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. オブジェクト名の横にある「**共有**」ボタンをクリックします。

   ![](assets/new-share-button.png)

1. が含まれる **&lt; オブジェクト名 > へのアクセス権の付与先** ボックスに、オブジェクトを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示される名前をクリックします。

   ![](assets/new-share-button-add-people.png) {width=&quot;350&quot; }

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

   >[!TIP]
   >
   >同様の名前を持つ複数のエンティティが存在する場合は、それらすべてがタイプの下に表示されます。エンティティの名前はアルファベット順に表示されます。ただし、エンティティタイプが表示される順序はランダムです。
   >

1. （オプション）オブジェクトへのアクセスを許可するユーザー、チーム、役割またはグループごとに、手順 3 を繰り返します。

1. 手順 3 で追加した各ユーザー、チーム、役割、グループ、または会社に対するアクセス許可を指定します。それには、ユーザー名の右側にあるドロップダウン メニューをクリックし、付与するアクセス許可レベルを選択します。

   ![](assets/new-share-permissions-dropdown.png)

   オブジェクトからの権限の削除については、[オブジェクトからの権限を削除](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

   次のオプションを使用できます。

   * **表示**：ユーザーはアイテムを確認したり共有したりできます。
   * **参加**：ユーザーは、更新の作成、情報の記録、軽微な編集、共有のほか、すべての表示権限を実行できます。
   * **管理：**&#x200B;ユーザーは、管理権限（アクセスレベルで付与）がなくても、オブジェクトのすべてにアクセスできます。また、すべての表示権限および参加権限も持っています。

     >[!NOTE]
     >
     >Workfront 管理者またはオブジェクト作成者は、これらのエンティティから権限を削除できます。

1. （オプション）オブジェクトに対する特定の権限を設定するために付与した権限レベルの横にある「詳細オプション」アイコンをクリックします。

   ![](assets/new-share-advanced-permissions-dropdown.png)

   表示、管理および参加の詳細設定オプションは、選択したオブジェクトに応じて異なります。\
   権限レベルの詳細については、を参照してください。 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. （オプション）システム内のすべてのユーザーがこのオブジェクトを使用できるようにするには、の下にあるドロップダウンメニューをクリックします **アクセスできるユーザー**&#x200B;をクリックし、ドロップダウンメニューでをクリックします **システム内の全員が表示できます**.

   ![](assets/new-share-everyone-access.png)

   すべてのユーザーは、設定した権限に基づいてオブジェクトを表示できます。

1. （オプションおよび条件付き）プロジェクトを共有する場合は、 **歯車** アイコン ![](assets/gear-icon-settings.png)で、の横にあるチェックボックスをオンにします。 **マイプロジェクトアクセステンプレートとして設定** 権限をテンプレートとして設定します。

   1 つのプロジェクトに対して権限を定義した後、次回プロジェクトをゼロから作成する際に、同じ権限が自動的に適用されます。

   >[!NOTE]
   >
   >プロジェクトアクセステンプレートは、アクセスレベルで Workfront 管理者が付与した共有のデフォルトよりも優先されます。\
   >アクセスレベルでプロジェクトの共有のデフォルトを指定する方法について詳しくは、[プロジェクトにアクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

   <!--
   >this note also appears in Understanding Project Permissions-->

   テンプレートを共有する際に、テンプレートから作成されるプロジェクトに対する権限を指定できます。詳しくは、[プロジェクトテンプレートを共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md)を参照してください。

1. （条件付き）外部ユーザーとオブジェクトを共有するには、 **リンクをコピー**&#x200B;その後、リンクを外部ユーザーに配布します。

   リンクを使用してすべてのユーザーがオブジェクトを表示できます。

   >[!CAUTION]
   >
   >機密情報を含んだオブジェクトを外部ユーザーと共有する場合は、注意することをお勧めします。Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

1. 「**保存**」をクリックします。

## ページからのドキュメント、ポートフォリオまたはプログラムの共有

1. 共有するオブジェクトに移動します。

   共有可能なオブジェクトについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. ポートフォリオとプログラムの場合：

   オブジェクト名の横にある「**共有**」ボタンをクリックします。

   ![](assets/new-share-button.png)

   または

   ドキュメント：

   「」をクリックします **詳細** アイコン ![](assets/more-icon.png) オブジェクト名の横にあるをクリックします。 **共有**.

   ![](assets/share-a-document-350x160.png)

1. が含まれる **&lt; オブジェクト名 > へのアクセス権の付与先** ボックスに、オブジェクトを共有するユーザー、チーム、役割、グループ、または会社の名前の入力を開始し、ドロップダウンリストに表示される名前をクリックします。

   ![](assets/list-share-add-people.png) {width=&quot;350&quot; }

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。



   >[!TIP]
   >
   >同様の名前を持つ複数のエンティティが存在する場合は、それらすべてがタイプの下に表示されます。エンティティの名前はアルファベット順に表示されます。ただし、エンティティタイプが表示される順序はランダムです。
   >

1. （オプション）オブジェクトへのアクセスを許可するユーザー、チーム、役割またはグループごとに、手順 3 を繰り返します。

1. ドロップダウンメニューをクリックし、付与する権限レベルを選択することで、手順 3 で追加した各ユーザー、チーム、役割、グループまたは会社に対する権限を指定します。

   オブジェクトからの権限の削除については、[オブジェクトからの権限を削除](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

   次のオプションを使用できます。

   * **表示**：ユーザーはアイテムを確認したり共有したりできます。
   * **管理：**&#x200B;ユーザーは、管理権限（アクセスレベルで付与）がなくても、オブジェクトのすべてにアクセスできます。また、すべての表示権限および参加権限も持っています。

     >[!NOTE]
     >
     >Workfront 管理者またはオブジェクト作成者は、これらのエンティティから権限を削除できます。

     ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

1. （任意）クリック **詳細設定** オブジェクトに特定の権限を設定します。

   表示、管理および参加の詳細設定オプションは、選択したオブジェクトに応じて異なります。\
   権限レベルについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. （オプション）システム内のすべてのユーザーがこのオブジェクトを使用できるようにするには、 **歯車** アイコン ![](assets/gear-icon-settings-with-dn-arrow.jpg)をクリックし、ドロップダウンメニューでをクリックします **システム全体で表示する**.

   すべてのユーザーは、設定した権限に基づいてオブジェクトを表示できます。

1. （オプション）オブジェクトをパブリックにするには、「**これを外部ユーザーに公開**」をクリックします。

   >[!TIP]
   >
   >このオプションは、一部のオブジェクトでは利用できません。

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png) {width=&quot;350&quot; }

1. （条件付き）オブジェクトを外部ユーザーに対して公開した場合は、「**リンクをコピー**」をクリックし、外部ユーザーにリンクを配布します。

   リンクを使用してすべてのユーザーがオブジェクトを表示できます。

   >[!CAUTION]
   >
   >機密情報を含んだオブジェクトを外部ユーザーと共有する場合は、注意することをお勧めします。Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

1. 「**保存**」をクリックします。

## リストからの単一オブジェクトまたは一括オブジェクトの共有

1. 共有するオブジェクトを含むリストに移動します。

   共有可能なオブジェクトについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. 共有するオブジェクトの横にあるチェックボックスをクリックし、 **共有アイコン** ![](assets/share-icon.png) ページの上部

   ![](assets/list-share-object-select.png) {width=&quot;350&quot; }

1. が含まれる **&lt; オブジェクト > アクセス** ウィンドウが表示されるので、 **の &lt; オブジェクト名 > アクセスを編集** ボックス オブジェクトを共有するユーザー、チーム、役割、グループ、または会社の名前を選択し、ドロップダウンリストに表示されたら名前をクリックします。

   ![](assets/list-share-add-people.png) {width=&quot;350&quot; }

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

   >[!TIP]
   >
   >同様の名前を持つ複数のエンティティが存在する場合は、それらすべてがタイプの下に表示されます。エンティティの名前はアルファベット順に表示されます。ただし、エンティティタイプが表示される順序はランダムです。
   >

1. （オプション） オブジェクトへのアクセス権を付与するユーザー、チーム、役割またはグループごとに手順 3 を繰り返します。

1. 手順 3 で追加した各ユーザー、チーム、役割、グループ、または会社に対するアクセス許可を指定します。それには、ユーザー名の右側にあるドロップダウン メニューをクリックし、付与するアクセス許可レベルを選択します。

   オブジェクトからの権限の削除については、[オブジェクトからの権限を削除](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

   ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

   次のオプションを使用できます。

   * **表示**：ユーザーはアイテムを確認したり共有したりできます。
   * **参加**：ユーザーは、更新の作成、情報の記録、軽微な編集、共有のほか、すべての表示権限を実行できます。

     >[!TIP]
     >
     >参加権限は、以下のオブジェクトに対してのみ付与できます。
     >
     >   * プロジェクト
     >   * タスク
     >   * イシュー
     >  

   * **管理：**&#x200B;ユーザーは、管理権限（アクセスレベルで付与）がなくても、オブジェクトのすべてにアクセスできます。また、すべての表示権限および参加権限も持っています。

     >[!NOTE]
     >
     >Workfront 管理者またはオブジェクト作成者は、これらのエンティティから権限を削除できます。

1. （任意）クリック **詳細設定** オブジェクトに特定の権限を設定します。

   表示、管理および参加の詳細設定オプションは、選択したオブジェクトに応じて異なります。\
   権限レベルについて詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. （オプション）このオブジェクトをシステム内のすべてのユーザーが使用できるようにするには、**歯車**&#x200B;アイコン ![](assets/gear-icon-settings-with-dn-arrow.jpg) をクリックし、ドロップダウンメニューで「**システム全体で表示できるようにする**」を選択します。

   設定した権限に基づいて、すべてのユーザーがオブジェクトを表示できます。

1. （オプションおよび条件付き）プロジェクトを共有する場合、**歯車**&#x200B;アイコン ![](assets/gear-icon-settings-with-dn-arrow.jpg)をクリックし、ドロップダウンメニューで「**マイプロジェクトアクセステンプレートに設定**」を選択して、権限をテンプレートとして設定します。

   1 つのプロジェクトに対して権限を定義した後、次回プロジェクトをゼロから作成する際に、同じ権限が自動的に適用されます。

   >[!NOTE]
   >
   >プロジェクトアクセステンプレートは、アクセスレベルで Workfront 管理者が付与した共有のデフォルトよりも優先されます。\
   >アクセスレベルでプロジェクトの共有のデフォルトを指定する方法について詳しくは、[プロジェクトにアクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

   <!--
   >this note also appears in Understanding Project Permissions-->

   テンプレートを共有する際に、テンプレートから作成されるプロジェクトに対する権限を指定できます。詳しくは、[プロジェクトテンプレートを共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md)を参照してください。

1. （オプション）オブジェクトを公開するには、 **これを外部ユーザーにパブリックにする**.

   >[!TIP]
   >
   >このオプションは、一部のオブジェクトでは利用できません。

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png) {width=&quot;350&quot; }

1. （条件付き）オブジェクトを外部ユーザーに公開した場合は、 **リンクをコピー**&#x200B;その後、リンクを外部ユーザーに配布します。

   リンクを使用してすべてのユーザーがオブジェクトを表示できます。

   >[!CAUTION]
   >
   >機密情報を含んだオブジェクトを外部ユーザーと共有する場合は、注意することをお勧めします。Workfront のユーザーや組織の一員でなくても、情報を表示できるようになるからです。

1. 「**保存**」をクリックします。
