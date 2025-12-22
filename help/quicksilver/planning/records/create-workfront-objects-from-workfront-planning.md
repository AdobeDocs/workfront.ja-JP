---
title: Workfront オブジェクトをレコードに関連付ける際に、Workfront Planning からデータモデルを作成する
description: Workfront オブジェクトタイプは、Workfront Planning 内の他のレコードから関連付ける際に作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 6%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront オブジェクトをレコードに関連付ける際に、Workfront Planning からデータモデルを作成する

<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Workfront Planning からAdobe Workfrontオブジェクトを作成するには、次の方法があります：

* Workfront オブジェクトを Planning レコードから接続する場合

  ここでは、Workfront Planning からWorkfrontオブジェクトを作成し、Planning レコードから接続する方法について説明します。
* レコードのページから自動化を使用する場合。

  オートメーションを使用したWorkfrontオブジェクトの作成については、[Adobe Workfront計画レコードのオートメーションを使用したオブジェクトの作成 &#x200B;](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。

>[!IMPORTANT]
>
>Workfront Planning から次のWorkfrontオブジェクトを Planning レコードに接続すると、それらのオブジェクトを作成できます。
>
>* プロジェクト
>* ポートフォリオ
>* プログラム
>
>次のWorkfrontオブジェクトを Planning レコードに接続できますが、接続プロセスでは作成できません。
>
>* グループ
>* 会社
>

Workfront オブジェクトをWorkfront Planning レコードに接続して作成する場合は、次の点に注意してください。

* Workfront Planning の次の領域の「接続」フィールドから、Workfront プロジェクト、ポートフォリオ、プログラム、グループおよび会社を接続できます。

   * レコードタイプのテーブル表示
   * レコードの詳細ページまたはプレビューボックス
   * レコードの「接続」タブ

* Workfront Planning の次の領域からプロジェクトを作成できます：

   * レコードタイプのテーブル表示
   * 接続フィールドのレコードの「詳細」領域
   * レコードの接続済みレコードページ

* ポートフォリオとプログラムは、Workfront Planning の次の領域から作成できます。

   * レコードタイプのテーブル表示
   * 接続フィールドのレコードの「詳細」領域

Planning レコードとWorkfrontオブジェクトの接続の詳細は、[&#x200B; レコードの接続 &#x200B;](/help/quicksilver/planning/records/connect-records.md) を参照してください。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontと任意の Planning パッケージ</p> <p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td>

<tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>作成するオブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム）のWorkfrontでオブジェクトを作成アクセス権を使用してアクセスを編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードを追加するワークスペースとレコードタイプに対する投稿以上の権限。 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
   </td> 
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++ 

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## Workfront オブジェクトをWorkfront Planning のレコードに関連付ける際の、オブジェクト作成の前提条件

既存のレコードから接続して新しいプロジェクトまたはポートフォリオを追加するには、次のものが必要です。

* Workfront プロジェクト、ポートフォリオまたはプログラムに接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* Workfront オブジェクトに接続されたレコードタイプのレコード。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* この記事の [&#x200B; アクセス要件 &#x200B;](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

## Workfront Planning のレコードにプロジェクトを結び付けながらプロジェクトを作成します

Workfront Planning の次の領域で、プロジェクトをWorkfront Planning のレコードに関連付けながらプロジェクトを作成できます：

* 接続フィールドのレコードタイプのテーブルビューまたはレコードの詳細エリア
* レコードの「詳細」領域にある、レコードの「接続済みレコード」ページ

### レコードの「詳細」エリアまたはレコードタイプのテーブル表示からプロジェクトを作成する

他のレコードから接続する際にプロジェクトを作成するには：

1. [&#x200B; レコードの接続 &#x200B;](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront プロジェクトの接続を開始します。

1. （条件付き） **プロジェクトを追加** をクリック
または
プロジェクトの名前の入力を開始し、見つからない場合は **プロジェクトを追加** をクリックします。 「追加」ボタンの後に、入力したプロジェクト名が続きます。

   ![&#x200B; 接続フィールドから接続する際にプロジェクトを追加 &#x200B;](assets/add-project-when-connecting-it-from-connection-field.png)

   **プロジェクトを作成** ボックスが開きます。

1. （任意） **プロジェクト名** を更新します。 デフォルトでは、プロジェクトの名前は、レコードから接続する際に検索項目として追加した名前に基づいて付けられます。
1. （任意）「**プロジェクトテンプレート**」を選択します。 テンプレートを選択しない場合、Workfrontはタスクを含まない空のプロジェクトを作成します。
1. 「**作成**」をクリックします。
1. （条件付き）テンプレートからプロジェクトを作成することを選択した場合は、記事 [&#x200B; テンプレートを使用したプロジェクトの作成 &#x200B;](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) の手順に従って、プロジェクトの追加を完了します。

   新しいプロジェクトが作成され、選択したレコードの接続されたフィールドに追加されます。

1. （任意） Workfront Planning から新しいプロジェクトの名前をクリックして、Workfrontでプロジェクトのページを開き、プロジェクトをさらに更新します。

### レコードの接続されたレコードページからのプロジェクトの作成

1. テーブル表示で、プロジェクトのオブジェクトタイプをWorkfrontの Planning レコードタイプに関連付けます。

   詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

1. 任意のビューでレコードの名前をクリックします。 「詳細」 プレビューボックスが開きます。

1. プロジェクトの **接続されたレコードのページ** を追加します。

   詳しくは、[&#x200B; 接続されたレコードページのレコードへの追加 &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) を参照してください。

   接続されたレコード ページがテーブル ビューに表示されます。 接続されたプロジェクトがテーブルに表示されます。

   ![&#x200B; 接続されたレコードページのプロジェクト テーブルビュー &#x200B;](assets/projects-connected-records-page-table.png)

1. プロジェクト テーブルで **新規行** をクリックして、プロジェクトを追加します。

   この領域で追加できるのは空のプロジェクトのみです。 テンプレートを使用してプロジェクトを追加することはできません。
1. （オプション）テーブル表示でプロジェクトの名前をクリックして、Workfrontでプロジェクトを開き、詳細を追加します。

## ポートフォリオをWorkfront Planning のレコードに接続する際のポートフォリオの作成

ポートフォリオは、レコードタイプのテーブル表示またはレコードの詳細ページから作成できます。

計画レコードから接続するポートフォリオを作成する手順は、次のとおりです。

1. [&#x200B; レコードの接続 &#x200B;](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

1. （条件付き） **ポートフォリオを追加** をクリック

   または

   ポートフォリオ名の入力を開始し、見つからない場合は **ポートフォリオを追加** をクリックします。 「追加」ボタンの後に、入力したポートフォリオ名が表示されます。

   ![&#x200B; 接続フィールドから接続する際にポートフォリオを追加 &#x200B;](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   ポートフォリオが作成され、選択したレコードの接続フィールドに追加されます。

1. （任意）Workfront プランニングから新しいポートフォリオの名前をクリックして、Workfrontでポートフォリオのページを開き、ポートフォリオをさらに更新します。

## Workfront Planning のレコードにプログラムを関連付ける際に、プログラムを作成します

プログラムは、レコードタイプのテーブル表示またはレコードの詳細ページから作成できます。

Planning レコードから接続するプログラムを作成するには、次の手順に従います。

1. [&#x200B; レコードの接続 &#x200B;](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

1. 「**プログラムを追加**」をクリックします

   または

   プログラム名の入力を開始し、見つからない場合は **プログラムを追加** をクリックします。 「追加」ボタンの後に、入力したプログラム名が続きます。

   ![&#x200B; 接続フィールドから接続する際にWorkfront プログラムを追加する &#x200B;](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   **プログラムを作成** ボックスが開きます。

1. **プログラム名** を更新します。 必須フィールドです。
1. ドロップダウンから **Portfolio** を選択するか、ポートフォリオの名前の入力を開始し、リストに表示されたら選択します。 必須フィールドです。
1. 「**作成**」をクリックします。

   プログラムが作成され、選択したレコードの接続フィールドに追加されます。

1. （オプション）Workfront Planning から新しいプログラムの名前をクリックして、Workfrontでプログラムのページを開き、さらに更新を行います。

