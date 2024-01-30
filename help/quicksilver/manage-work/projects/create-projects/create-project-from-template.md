---
product-area: projects;templates
navigation-topic: create-projects
title: テンプレートを使用したプロジェクトの作成
description: テンプレートをフレームワークとして使用し、Adobe Workfrontでプロジェクトを作成できます。 頻繁に繰り返されるプロジェクトがある場合、新しいプロジェクトの一般的なタイムラインでテンプレートを使用すると、同じプロジェクトを繰り返し作成する必要がなくなります。
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
source-git-commit: 9447310f0d4cf4504ee6d690116fb62f718fe23d
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# テンプレートを使用したプロジェクトの作成

<!-- Audited: 01/2024 -->

テンプレートをフレームワークとして使用し、Adobe Workfrontでプロジェクトを作成できます。 頻繁に繰り返されるプロジェクトがある場合、新しいプロジェクトの一般的なタイムラインでテンプレートを使用すると、同じプロジェクトを繰り返し作成する必要がなくなります。

テンプレートを使用すると、繰り返し可能なプロセス、情報、およびプロジェクトに関連する設定を取り込むことができます。 テンプレートに関連付けられた情報は、プロジェクトに転送されます。 これには、タスク、割り当て、期間、ドキュメント、財務の詳細、リスク、およびカスタムフォームが含まれます。

>[!TIP]
>
>Workfrontでは、新しいプロジェクトのグループとステータスを次のように定義します。
>
>* テンプレートから作成される新しいプロジェクトのデフォルトのステータスは、主な「プロジェクトの環境設定」領域でWorkfront管理者が定義したステータス、またはグループの「プロジェクトの環境設定」領域でグループ管理者 ( またはWorkfront管理者 ) が定義したステータスに対応します。 プロジェクトの環境設定の詳細については、「 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) または [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).
>
>* 新しいプロジェクトのグループは、テンプレートのグループです。 テンプレートがグループに関連付けられていない場合、プロジェクトのグループは、プロジェクトを作成するユーザーのホームグループになります。
>
>* 新しいプロジェクトで使用できるステータスは、プロジェクトのグループのステータス（テンプレートのグループ、またはプロジェクトを作成するユーザーのホームグループ）に一致します。

テンプレートからプロジェクトを作成するには、次のオプションがあります。

* 「プロジェクト」領域でテンプレートからプロジェクトを作成する
* テンプレートレベルでテンプレートからプロジェクトを作成する
* 既存のプロジェクトにテンプレートを添付する

  詳しくは、 [プロジェクトにテンプレートを添付する](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* 「グループ」領域でテンプレートからプロジェクトを作成します。

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfrontライセンス</td> 
   <td> <p>新規：標準</p>
        <p>または</p>
        <p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトおよびテンプレートへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>テンプレートに対する権限の表示</p> <p>プロジェクトを作成すると、そのプロジェクトに対する管理権限が自動的に付与されます。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 「プロジェクト」領域でテンプレートからプロジェクトを作成する

プロジェクトは、メインメニューの「プロジェクト」領域、またはポートフォリオやプログラムの「プロジェクト」領域から作成できます。

1. 次のいずれかの操作を行います。

   * 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックします。 クリック **プロジェクト**&#x200B;を展開し、を展開します。 **新規プロジェクト**.
   * ポートフォリオに移動し、を展開します。 **新規プロジェクト**.

     >[!TIP]
     >
     >ポートフォリオのPortfolioを使用してプロジェクトを作成すると、新しいプロジェクトのテンプレートフィールドが更新され、プロジェクトの作成元として選択したポートフォリオが表示されます。 指定されている場合は、Portfolioのテンプレートフィールドが上書きされます。

   * プログラムに移動し、を展開します。 **新規プロジェクト**.

     >[!TIP]
     >
     >プログラムからテンプレートを使用してプロジェクトを作成すると、新しいプロジェクトの「プログラム」フィールドが更新され、プロジェクトの作成元として選択したプログラムが表示されます。 テンプレートの「Portfolio」フィールドが更新され、プロジェクトの作成元として選択したプログラムのポートフォリオが表示されます。 指定されている場合は、テンプレートの「プログラム」フィールドと「Portfolio」フィールドが上書きされます。

   * グループ管理者は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。 詳しくは、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >グループのテンプレートを使用してプロジェクトを作成する場合、新しいプロジェクトの「グループ」フィールドには、テンプレートの「グループ」フィールドが指定されていない場合にのみ、そのプロジェクトの作成元のグループが表示されます。 テンプレートの「グループ」フィールドを指定した場合、新しいプロジェクトの「グループ」フィールドはテンプレートの「グループ」フィールドになります。

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![新しいプロジェクトオプション](assets/new-project-dropdown.png)

1. テンプレートの名前をクリックします。 **お気に入りのテンプレート** リスト。

   ![お気に入りのテンプレートを選択](assets/new-project-from-template-dropdown-with-template-favorites.png)

   または

   次の操作を実行します。

   1. 選択 **テンプレートからの新規プロジェクト**.
   1. Adobe Analytics の **テンプレートを検索** 「 」フィールドで、テンプレートの名前の入力を開始し、リストに表示されたらクリックします。
   1. 右側でテンプレートの詳細を確認します。

      テンプレートの詳細には、以下が含まれます。

      * テンプレートの期間
      * テンプレート所有者
      * 上位 3 つのタスクの名前を含む最上位タスクの数
      * テンプレート内のすべてのタスクの数
      * テンプレートのカスタムフォームの名前

   1. （オプション）左側のウィンドウでテンプレート名の上にマウスポインターを置き、 **お気に入力** **アイコン** ![](assets/favorites-icon-small.png) 将来の使用のお気に入りとしてマークする

      または

      を展開します。 **お気に入りのテンプレート** リストを開き、ドロップダウンリストからテンプレートを選択します。

      >[!TIP]
      >
      >お気に入りに登録できるWorkfront項目は 40 個までです。 これには、テンプレートやその他の項目が含まれます。

   1. クリック **テンプレートを使用** をクリックします。

      ![テンプレートの詳細](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >プロジェクトの一覧にマイルストーンビューを適用している場合は、 **「テンプレートから新規作成」セクション**.
      >
      >
      >![テンプレートからプロジェクトを作成するためのマイルストーン表示](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   The **新規プロジェクト** ボックスが開きます。

   ![新規プロジェクトボックス](assets/new-project-from-template-box.png)

1. テンプレートに既にフィールドが入力されている場合、そのフィールドは **新規プロジェクト** ボックス。 事前入力された値を編集して、プロジェクトに合わせて調整できます。 詳しくは、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).
1. クリック **プロジェクトを作成**.

   前の手順で変更しなかった場合、テンプレートで定義したすべての詳細は、新しく作成されたプロジェクトに自動的に関連付けられます。

## 「テンプレート」領域で、テンプレートからプロジェクトを作成します。

「プロジェクト」領域で開始する代わりに、テンプレートを使用してテンプレートからプロジェクトを作成できます。

{{step1-to-templates}}

1. 使用するテンプレートの名前をクリックします。
1. 次をクリック： **その他** メニュー ![](assets/more-icon.png)を選択し、次に **プロジェクトを作成**.

   ![テンプレートからプロジェクトを作成](assets/project-sharing-on-template.png)

   The **新規プロジェクト** ボックスが開きます。

1. プロジェクトの名前を入力し、各セクションを確認して必要な変更を行います。

   ![新規プロジェクトボックス](assets/new-project-from-template-box.png)

   テンプレートに既にフィールドが入力されている場合、そのフィールドは **新規プロジェクト** ボックス。 事前入力された値を編集して、プロジェクトに合わせて調整できます。 詳しくは、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

1. クリック **プロジェクトを作成**.

   前の手順で変更しなかった場合、テンプレートで定義したすべての詳細は、新しく作成されたプロジェクトに自動的に関連付けられます。
