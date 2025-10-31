---
product-area: projects;templates
navigation-topic: create-projects
title: テンプレートを使用したプロジェクトの作成
description: テンプレートをフレームワークとして使用して、Adobe Workfront でプロジェクトを作成できます。頻繁に繰り返されるプロジェクトがある場合、新しいプロジェクトでテンプレートを使用すると、同じプロジェクトを繰り返し作成する必要がなくなります。
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 80%

---

# テンプレートを使用したプロジェクトの作成

<!-- Audited: 10/2025 -->

テンプレートをフレームワークとして使用して、Adobe Workfront でプロジェクトを作成できます。頻繁に繰り返されるプロジェクトがある場合、新しいプロジェクトの一般タイムラインでテンプレートを使用すると、同じプロジェクトを繰り返し作成する必要がなくなります。

テンプレートを使用すると、繰り返し可能なプロセス、情報、およびプロジェクトに関連する設定を取り込むことができます。テンプレートに関連付けられた情報は、プロジェクトに転送されます。これには、タスク、割り当て、期間、ドキュメント、財務の詳細、リスク、およびカスタムフォームが含まれます。

>[!TIP]
>
>Workfront では、新しいプロジェクトのグループとステータスが次のように定義されます。
>
>* テンプレートから作成された新規プロジェクトのデフォルトステータスは、メインのプロジェクト環境設定エリアで Workfront 管理者が定義したステータス、またはグループのプロジェクト環境設定エリアでグループ管理者（または Workfront 管理者）が定義したステータスに対応します。プロジェクトの環境設定について詳しくは、[システム全体でのプロジェクトの環境設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)または[グループのプロジェクトの環境設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)を参照してください。
>
>* 新しいプロジェクトのグループは、テンプレートのグループです。テンプレートがグループに関連付けられていない場合、プロジェクトのグループは、プロジェクトを作成したユーザーのホームグループになります。
>
>* 新規プロジェクトで使用できるステータスは、プロジェクトのグループ（テンプレートのグループ、またはプロジェクトを作成するユーザーのホームグループ）のステータスと一致します。

テンプレートからプロジェクトを作成する場合は、次のオプションがあります。

* 「プロジェクト」エリアでのテンプレートからのプロジェクトの作成
* テンプレートレベルでのテンプレートからのプロジェクトの作成
* 既存のプロジェクトにテンプレートを添付

  詳しくは、[プロジェクトへのテンプレートの添付](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

* 「グループ」エリアでのテンプレートからのプロジェクトの作成

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
   <td role="rowheader">Workfront ライセンス</td> 
   <td> <p>標準</p>
        <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトおよびテンプレートへのアクセス権の編集</p>
   <p>使用するテンプレートにPortfolioとプログラムが含まれている場合、ポートフォリオとプログラムへのアクセスを編集します</p>  
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートに対する権限の表示</p> 
  <p>使用するテンプレートにPortfolioとプログラムが含まれている場合、プロジェクトを作成するには、ポートフォリオとプログラムに対する管理権限が必要です </p> 
   <p>プロジェクトを作成すると、そのプロジェクトに対する管理権限が自動的に付与されます。</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects and to Templates</p>
   
   <p>edit access to Portfolios and Programs, if the template you use contains a Portfolio and a Program</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> 
  <p>If the template you use contains a Portfolio and a Program, you must have Manage permissions to the portfolio and program to create the project </p> 
   <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>-->

## 「プロジェクト」エリアでのテンプレートからのプロジェクトの作成

プロジェクトは、「メインメニュー」の「プロジェクト」エリアや、ポートフォリオまたはプログラムの「プロジェクト」エリアから作成できます。

>[!NOTE]
>
>システム管理者またはグループ管理者は、レイアウトテンプレートを使用してインターフェイスを変更する場合があります。この場合、次の手順で参照されるセクションとエリアの名前の一部が、Workfront のインスタンスでは異なる可能性があります。

1. 次のいずれかの操作を行います。

   * 左上隅の **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) またはAdobe Workfrontの右上隅の **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックし（使用可能な場合）、「**プロジェクト**」をクリックして「**新規プロジェクト**」を展開します。
   * ポートフォリオに移動し、「**新規プロジェクト**」を展開します。

     >[!TIP]
     >
     >ポートフォリオのテンプレートを使用してプロジェクトを作成すると、新しいプロジェクトの「ポートフォリオ」フィールドが更新され、プロジェクトの作成元として選択したポートフォリオが表示されます。これにより、テンプレートの「ポートフォリオ」フィールドが指定されている場合、それが上書きされます。

   * プログラムに移動し、「**新規プロジェクト**」を展開します。

     >[!TIP]
     >
     >プログラムのテンプレートを使用してプロジェクトを作成すると、新しいプロジェクトの「プログラム」フィールドが更新され、プロジェクトの作成元として選択したプログラムが表示されます。テンプレートの「ポートフォリオ」フィールドが更新され、プロジェクトの作成元として選択したプログラムのポートフォリオが表示されます。これにより、テンプレートの「プログラム」フィールドと「ポートフォリオ」フィールドが指定されている場合、それらが上書きされます。

   * グループ管理者の場合は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。詳しくは、[グループのプロジェクトの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

     >[!TIP]
     >
     >グループのテンプレートを使用してプロジェクトを作成する場合、新しいプロジェクトの「グループ」フィールドには、テンプレートの「グループ」フィールドが指定されていない場合にのみ、そのプロジェクトの作成元のグループが表示されます。テンプレートの「グループ」フィールドを指定した場合、新しいプロジェクトの「グループ」フィールドはテンプレートの「グループ」フィールドになります。

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![新規プロジェクトのオプション](assets/new-project-dropdown.png)

1. **お気に入りのテンプレート**&#x200B;リストでテンプレート名をクリックします。

   ![お気に入りのテンプレートを選択](assets/new-project-from-template-dropdown-with-template-favorites.png)

   または

   次の操作を実行します。

   1. **テンプレートから新規プロジェクト** をクリックします。
   1. **テンプレートの検索**&#x200B;フィールドで、テンプレートの名前を入力し、リストに表示されたらクリックして選択します。
   1. 右側でテンプレートの詳細を確認します。

      テンプレートの詳細には、以下の情報が含まれています。

      * テンプレートの期間
      * テンプレート所有者
      * 上位 3 つのタスク名を含む上位レベルのタスクの数
      * テンプレート内のすべてのタスクの数
      * テンプレートのカスタムフォームの名前

   1. （任意）左側のペインのテンプレート名の上にマウスポインターを置き、**お気に入り****アイコン**![ お気に入りアイコン ](assets/favorites-icon-small.png) をクリックして、後で使用するためにお気に入りとしてマークします。

      または

      **お気に入りのテンプレート**&#x200B;リストを展開し、ドロップダウンリストからテンプレートを選択します。

      >[!TIP]
      >
      >お気に入りに登録できる Workfront の項目は最大 40 個です。これには、テンプレートやその他の項目が含まれます。

   1. テンプレートを選択したら、「**テンプレートを使用**」をクリックします。

      ![テンプレートの詳細](assets/new-project-from-template-small-box-with-template-details-panel.png)

      <!--no longer available, after unshimming - Oct 2025:
      >[!NOTE]
      >
      >If you have the Milestone View applied to the list of projects, click the name of a template in the **New from Template section**.
      >
      >
      >![Milestone view of creating a project from a template](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >
      -->

   **新規プロジェクト**&#x200B;ボックスが開きます。

   ![新規プロジェクトボックス](assets/new-project-from-template-box.png)

1. （条件付き）テンプレートにフィールドが既に入力されている場合、そのフィールドは **新しいプロジェクト** ボックスに事前入力されます。

   プロジェクトに合わせて、事前入力された値を編集します。

   詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。
1. **プロジェクトを作成** をクリックします。

   前の手順で変更しなかった場合、テンプレートで定義したすべての詳細は、新しく作成されたプロジェクトに自動的に関連付けられます。

## テンプレート領域でテンプレートからプロジェクトを作成

プロジェクト領域から始める代わりに、テンプレートからプロジェクトを作成するできます。

{{step1-to-templates}}

1. 使用するテンプレートの名前をクリックします。
1. ヘッダーのテンプレート名の右側にある **その他** メニュー ![ その他アイコン ](assets/more-icon.png) をクリックし、**プロジェクトを作成** をクリックします。

   ![テンプレートからプロジェクトを作成](assets/project-sharing-on-template.png)

   **新規プロジェクト** ボックスが開きます。

1. プロジェクトの名前を入力します。 Workfrontは、このテンプレートの名前を使用して新しいプロジェクトに名前を付けます。

1. 「**新規プロジェクト**」ボックスの各セクションを確認し、必要な変更を加えます。

   ![新規プロジェクトボックス](assets/new-project-from-template-box.png)

   テンプレートに既にフィールドが入力されている場合、そのフィールドは&#x200B;**新規プロジェクト**&#x200B;ボックスで事前に入力されています。事前入力された値を編集して、プロジェクトに合わせることができます。

   詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

1. **プロジェクトを作成** をクリックします。

   前の手順で変更しなかった場合、テンプレートで定義したすべての詳細は、新しく作成されたプロジェクトに自動的に関連付けられます。
