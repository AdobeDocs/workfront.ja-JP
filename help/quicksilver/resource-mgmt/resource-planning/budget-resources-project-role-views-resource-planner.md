---
product-area: resource-management
navigation-topic: resource-planning
title: プロジェクトビューや役割ビューを使用したリソースプランナーでのリソース予算の計上
description: プロジェクトビューや役割ビューを使用して、Adobe Workfront リソースプランナーでリソースの予算を計上できます。リソースプランナーのユーザービューを使用してリソースの予算を計上することはできません。
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: ht
source-wordcount: '2160'
ht-degree: 100%

---

# プロジェクトビューや役割ビューを使用したリソースプランナーでのリソース予算の計上

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

リソースプランナーの主な機能は、プロジェクトで完了する必要がある作業のリソースの予算を計上することです。

>[!IMPORTANT]
>
>リソースの予算を計上できるのは、**プロジェクト別に表示**&#x200B;ビューまたは&#x200B;**役割別に表示**&#x200B;ビューをリソースプランナーに適用した場合のみです。

リソースプランナーで情報の予算の計上を開始する前に、次の記事を参照してください。

* [リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Adobe Workfront でのリソース予算の計上に必要なアクセス権](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [リソースプランナーのプロジェクトビューと役割ビューの時間数、FTE およびコスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理への編集アクセス権（リソースプランナーで優先度や予算計上時間数を編集するためのアクセス権を含む）</p> <p>財務データへの編集アクセス権（リソースの予算をコスト別に計上するため）</p> <p>プロジェクトおよびユーザーへの編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、「<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>」を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>情報予算の計上対象となるプロジェクトの管理権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## リソースプランナーでのリソース予算の計上

* [プロジェクトビューでのリソース予算の計上](#budget-resources-in-the-project-view)
* [役割ビューでのリソース予算の計上](#budget-resources-in-the-role-view)
* [リソース予算の一括計上](#budget-resources-in-bulk)

### プロジェクトビューでのリソース予算の計上 {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**リソース**」をクリックします。
1. **計画担当者**&#x200B;がデフォルトで表示されます。
1. （条件付き）**プロジェクト別に表示**&#x200B;ビューを選択します。
1. プロジェクトと担当業務を展開して、プロジェクト、担当業務またはユーザーの割り振りを管理します。
1. ユーザーの予算配分を行うには、次のいずれかを行います。

   * **BDG** 列で、ユーザーの予算計上時間数、FTE またはコストを手動で指定します。

   * ユーザーの担当業務の&#x200B;**その他**&#x200B;メニューをクリックし、「**ユーザーの予定時間数を予算計上値として設定する**」をクリックします。\
     各ユーザーの予算計上時間数は、次の式を使用して計算されます。

     ```
     User Budgeted Hours = User Planned Hours
     ```

1. 担当業務の予算配分を行うには、次のいずれかを実行します。

   * **BDG** 列で、担当業務の予算計上時間数、FTE またはコストを手動で指定します。

     >[!NOTE]
     >
     >役割の予算計上時間数が、プロジェクトの予算計上時間数に追加されます。

   * （条件付き）ユーザーの予算計上時間数がある場合は、担当業務の&#x200B;**その他**&#x200B;メニューをクリックし、「**役割について予算計上したユーザーの時間数合計**」をクリックします。\
     役割ごとの予算計上時間数は、次の式を使用して計算されます。

     ```
     Role Budgeted Hours = SUM(User Budgeted Hours)
     ```

   * プロジェクトの&#x200B;**その他**&#x200B;メニューをクリックし、「**役割の予定時間数を予算計上値として設定する**」をクリックします。\
     役割ごとの予算計上時間数は、次の式を使用して計算されます。\
     *

     ```
     Role Budgeted Hours = Role Planned Hours
     ```

     >[!NOTE]
     >   
     >* 役割の予算計上時間数が、プロジェクトの予算計上時間数に追加されます。
     >* ユーザーは、「主要役割」と「その他の役割」（または「セカンダリの役割」）の両方に対して予算を計上できます。
     >* リソースプランナーで担当業務の利用可能時間数の値を表示するには、ユーザーの役割の **FTE 使用可能時間の割合**&#x200B;に 0% 以外の数値を指定する必要があります。**FTE 使用可能時間の割合**&#x200B;が 0% の役割にユーザーが関連付けられている場合、その担当業務の利用可能時間数の値は 0 になります。この場合、役割はマイナスの&#x200B;**純価**&#x200B;を示す可能性があります。\
     >担当業務の **FTE 使用可能時間の割合**&#x200B;について詳しくは、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の記事を参照してください。

   * **BDG** 列で、プロジェクトの予算計上時間数、FTE、またはコストを手動で指定します。プロジェクトの予算計上時間数が、プロジェクト内のそれぞれの役割に配分されます。次のシナリオが存在します。

      * 指定したプロジェクトの予算計上時間数がプロジェクトの予定時間数と等しい場合、役割の予算計上時間数は役割の予定時間数と一致します。
      * 指定したプロジェクトの予算計上時間数がプロジェクトの予定時間数と等しくない場合、役割の予算計上時間数は、それぞれの役割に必要な予定時間数の割合に従って配分されます。\
        例えば、プロジェクトに 20 時間分の予定時間があり、2 つの担当業務に配分されていて（コンサルタントが必要な予定時間数は 12 時間、エンジニアが必要な予定時間数は 8 時間）、さらにプロジェクトに 30 時間分の予算を計上する場合、コンサルタントは 18 時間分の予算計上時間を、エンジニアは 12 時間分の予算計上時間を受け取るように配分されます。

1. プロジェクトの予算配分を行うには、次のいずれかを実行します。

   * 手順 7 の説明に従って、プロジェクト内の役割の予算を計上します。\
     プロジェクトの予算計上時間は、次の式で計算されます。

     ```
     Project Budgeted Hours = SUM(Role Budgeted Hours)
     ```

   * **BDG** 列で、プロジェクトの予算計上時間数、FTE、またはコストを手動で指定します。\
     手順 7 で説明したとおり、役割の予算計上時間が更新されます。\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. 「**保存**」をクリックします。\
   リソースプランナーでリソースの予算を計上すると、リソースの予算計上時間とそれに関連するコストが、すべてのプロジェクトのビジネスケースにリストアップされます。\
   ビジネスケースの「リソース予算計上」領域の概要について詳しくは、[ビジネスケースの領域の概要](../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の記事にある「リソース予算計上」セクションを参照してください。

1. （オプション）ユーザービューを選択して、各ユーザーの利用可能時間数と予定時間数の間でユーザーの配分超過や低稼働率を確認します。予算計上時間数は、ユーザービューには表示されません。

   Workfront がユーザーの利用可能時間を計算する方法について詳しくは、[リソース管理の環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

### 役割ビューでのリソース予算計上 {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

リソースプランナーでリソースの予算を計上するには、プロジェクトの「リソース管理」、「財務データ」、「財務の管理」の権限に対する編集アクセス権が必要です。担当業務の下に表示される少なくとも 1 つのプロジェクトに対して表示アクセス権のみを持っている場合は、役割ビューで役割に対する予算配分を行うことはできません。管理権限を持つプロジェクトの予算配分は引き続き可能です。

リソース予算計上に必要なアクセス権について詳しくは、[Adobe Workfront でのリソース予算計上に必要なアクセス権](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)の記事を参照してください。

役割ビューのリソースプランナーで予算配分を行うには、次の操作を実行します。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**リソース**」をクリックします。
1. 「**計画担当者**」がデフォルトで表示されます。
1. （条件付き）**役割別に表示**&#x200B;ビューを選択します。
1. 担当業務とプロジェクトを展開して、プロジェクト、担当業務、またはユーザーの配分を管理します。
1. ユーザーの予算配分を行うには、次のいずれかを実行します。

   * **BDG** 列で、ユーザーの予算計上時間数、FTE またはコストを手動で指定します。
   * プロジェクトの「**その他**」メニューをクリックし、「**ユーザーの予定時間数を予算計上値として設定**」をクリックします。\
     各ユーザーの予算計上時間数は、次の式を使用して計算されます。

     ```
     User Budgeted Hours = User Planned Hours
     ```

1. 担当業務の予算配分を行うには、次のいずれかを実行します。

   * **BDG** 列で、担当業務の予算計上時間数、FTE またはコストを手動で指定します。\
     これにより、管理アクセス権のあるプロジェクトで、役割の予算計上時間数がプロジェクトの予算計上時間数に配分されます。

   * 担当業務の「**その他**」メニューをクリックし、「プロジェクトの予定時間数を予算計上値として設定」をクリックします。**役割の予算計上時間数は、次の式を使用して計算されます。\
     *

     ```
     Role Budgeted Hours = SUM(Project Budgeted Hours)
     ```

     *プロジェクトの予算計上時間数は、次の式を使用して計算されます。

     ```
     Project Budgeted Hours = Project Planned Hours
     ```

   * **BDG** 列で、担当業務の下にリストされているプロジェクトの予算時間数、FTE、またはコストを手動で指定します。\
     これにより、プロジェクトの予算計上時間数が役割に追加されます。

   >[!NOTE]
   >
   >ユーザーは、「主要役割」と「その他の役割」（または「セカンダリの役割」）の両方に対して予算を計上できます。リソースプランナーで担当業務の利用可能時間数の値を表示するには、ユーザーの役割の **FTE 使用可能時間の割合**&#x200B;に 0% 以外の数値を指定する必要があります。**FTE 使用可能時間の割合**&#x200B;が 0% の役割にユーザーが関連付けられている場合、その担当業務の利用可能時間数の値は 0 になります。この場合、役割はマイナスの **純価**&#x200B;を示す可能性があります。\
   >担当業務の **FTE 使用可能時間の割合**&#x200B;について詳しくは、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の記事を参照してください。

1. プロジェクトの予算配分を行うには、次のいずれかを実行します。

   * **BDG** 列で、プロジェクトの予算計上時間数、FTE、またはコストを手動で指定します。\
     これにより、プロジェクトがリストされている役割の予算計上時間も更新されます。

   * 担当業務の&#x200B;**その他**&#x200B;メニューをクリックし、「**プロジェクトの予定時間数を予算に設定**」を選択します。\
     プロジェクトの予算計上時間は、次の式で計算されます。

     ```
     Project Budgeted Hours = Project Planned Hours
     ```

     プロジェクトの予算計上時間は役割の予算計上時間に追加されます。

   * （条件付き）ユーザーの予算計上時間を立てている場合は、プロジェクトの&#x200B;**その他**&#x200B;メニューをクリックし、**プロジェクトのユーザーの合計予算計上時間** を選択します。\
     プロジェクトの予算計上時間は、次の式で計算されます。

     ```
     Project Budgeted Hours = SUM(User Budgeted Hours)
     ```

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. 「**保存**」をクリックします。\
   リソースプランナーでリソースの予算を計上すると、リソースの予算計上時間とそれに関連するコストが、すべてのプロジェクトのビジネスケースにリストアップされます。\
   ビジネスケースのリソース予算計上エリアについて詳しくは、記事[ビジネスケースの予算リソース](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

1. （オプション）**ユーザー別表示**&#x200B;ビューを選択して、各ユーザーの利用可能時間と予定時間数の間のユーザー割り当て超過または稼働率不足を確認します。予算計上時間は、ユーザー別表示ビューには表示されません。

### リソース予算の一括計上 {#budget-resources-in-bulk}

クイックリンクを使用すると、リソースの割り当ての予算を一括で設定できます。クイックリンクは、プロジェクトビューと役割ビューでのみ使用できます。

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>リソースの予算割り当てへのクイックリンクを使用すると、予算編成は画面に表示されている期間にのみ自動的に適用されます。プロジェクトのタイムラインが画面に表示されているタイムラインよりも長い期間にわたる場合は、左から右にスクロールし、クイックリンクを使用してリソースの予算を自動的に設定する必要があります。

リソースの予算を一括で設定するには、次の手順に従います。

1. 次の場所に移動します。\
   リソースプランナーへのアクセスに関して詳しくは、記事[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)の「リソースプランナーへのアクセス」の節を参照してください。\
   管理できるプロジェクトのリストがリストに表示されます。

1. （オプション）各プロジェクトを展開すると、それに関連付けられている担当業務のリストが表示されます。\
   または
1. （オプション）「**役割別に表示**」を選択し、各役割を展開して、それに関連付けられているプロジェクトのリストを表示します。
1. プロジェクトまたは職務の名前の上にポインタを合わせます。
1. プロジェクトまたは役割名の右端に表示される&#x200B;**その他**&#x200B;アイコン![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)をクリックします。

1. 利用可能なオプションの 1 つをクリックして、他のオブジェクトの予算計上時間数（BDG）を自動的に指定します。

   プロジェクトまたは役割のどちらで詳細アイコンをクリックしたかに応じて、一括予算作成のオプションが異なります。以下の表は、プロジェクトと役割で使用できるオプションを示しています。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>プロジェクトビュー</strong> </td> 
      <td><strong>役割を表示</strong> </td> 
     </tr> 
     <tr> 
      <td>プロジェクトオプション</td> 
      <td> 
       <ul> 
        <li><strong>役割の予定時間数を予算に設定する</strong>：役割の予算計上時間数を予定時間数と同じにするには、このオプションを選択します。役割の予算計上時間数の合計が、プロジェクトの予算計上時間数に表示されます。 </li> 
        <li><strong>予算作成日の調整</strong>：予算計上時間数を別の時間枠に移動するには、このオプションを選択します。<br>予算作成日の調整に関して詳しくは、<a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">リソースプランナーでの予算作成日の調整</a>を参照してください。</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>ユーザーの予定時間数を予算に設定する</strong>：ユーザーの予算計上時間数を予定時間数と同じにするには、このオプションを選択します。 </li> 
        <li><strong>プロジェクトのユーザー予算計上時間数の合計</strong>：すべてのユーザーの予算計上時間数を合計し、その合計をプロジェクトと役割の予算計上時間として表示するには、このオプションを選択します。ユーザーの予算を手動で設定した後、または最初に前のオプションを使用した後に、このオプションを使用することをお勧めします。 </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>役割のオプション</td> 
      <td> 
       <ul> 
        <li><strong>ユーザーの予定時間数を予算に設定する</strong>：ユーザーの予算計上時間数を予定時間数と同じにするには、このオプションを選択します。 </li> 
        <li><strong>役割に対するユーザー予算計上時間数の合計</strong>：ユーザーのすべての予算計上時間数を合計し、その合計を役割とプロジェクトの予算計上時間として表示するには、このオプションを選択します。ユーザーの予算を手動で設定した後、または最初に前のオプションを使用した後に、このオプションを使用することをお勧めします。 </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>プロジェクトの予定時間数を予算に設定する</strong>：プロジェクトの予算計上時間数をプロジェクトの予定時間数と同じにするには、このオプションを選択します。 </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >リソースプランナーで作業するための前提条件の一部が満たされていない場合、一部のオプションが表示されない場合があります。
   >
   >
   >リソースプランナーで正確な予算を立てるために満たす必要がある前提条件に関して詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)の記事の「リソースプランナーで作業するための前提条件」の節を参照してください。\
   >例えば、次のシナリオでは一部のオプションが表示されない場合があります。
   >
   >   
   >   
   >   * プロジェクトがリソースプールに関連付けられていない場合
   >   * プロジェクトに関連付けられたリソースプールにユーザーが含まれていない場合
   >   * プロジェクトに関連付けられたリソースプールに、担当業務が関連付けられていないユーザーが含まれる場合。
   >   
   >
