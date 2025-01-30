---
title: Workfront Planning からのWorkfrontオブジェクトの作成
description: Workfront オブジェクトタイプは、Workfront Planning 内の他のレコードから関連付ける際に作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 12%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront Planning からのWorkfrontオブジェクトの作成


<!-- remove preview and production at release time-->

<span class="preview"> このページでハイライト表示されている情報は、まだ一般公開されていない機能を指しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Workfront Planning から次のタイプのWorkfrontオブジェクトを作成できます。

* プロジェクト
* ポートフォリオ

Workfront計画レコードをプロジェクトまたはポートフォリオと関連付けると、Workfront計画からWorkfront プロジェクトおよびポートフォリオを作成できます。

>[!IMPORTANT]
>
>* レコードから接続する場合、Workfrontで作成できるのはプロジェクトとポートフォリオのみです。
>
>* Workfront Planning のレコードからプログラム、グループまたは会社を関連付ける場合、それらのプログラム、グループまたは会社を作成することはできません。
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

Planning レコードとWorkfrontオブジェクトの接続の詳細は、[ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) を参照してください。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 標準
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p> 
   <p>レコードをレコードに関連付ける際に、作成するオブジェクトタイプ（プロジェクトとポートフォリオ）のWorkfrontでのアクセス権を編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードの追加先となるワークスペースに対する権限を管理します。 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront管理者を含むすべてのユーザーには、メインメニューに計画エリアを含むレイアウトテンプレートを割り当てる必要があります </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront オブジェクトをWorkfront Planning のレコードに関連付ける際の、オブジェクト作成の前提条件

既存のレコードから接続して新しいプロジェクトまたはポートフォリオを追加するには、次のものが必要です。

* Workfront プロジェクトまたはポートフォリオに接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* レコード。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* この記事の [ アクセス要件 ](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

## Workfront Planning のレコードにプロジェクトを関連付ける際にプロジェクトを作成する

他のレコードから接続する際にプロジェクトを作成するには：

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront プロジェクトの接続を開始します。

   Workfront Planning の次の領域で、「接続」フィールドからプロジェクトを接続できます。

   * レコードタイプのテーブル表示
   * レコードの詳細ページまたはプレビューボックス

1. （条件付き）別のレコードの「接続されたレコード」フィールドから追加しようとしてプロジェクトが見つからない場合は、名前を追加して、「**+追加**」をクリックします。 「追加」ボタンの後に、入力したプロジェクト名が続きます。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click +Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview"> 「**プロジェクトを作成** ボックスが開きます。</span>

1. <span class="preview"> （任意） **プロジェクト名** を更新します。 デフォルトでは、プロジェクトの名前は、レコードから接続する際に検索項目として追加した名前に基づいて付けられます。</span>
1. <span class="preview"> （任意） **プロジェクトテンプレート** を選択します。 テンプレートを選択しない場合、Workfrontはタスクを含まない空のプロジェクトを作成します。</span>
1. <span class="preview">**作成** をクリックします。</span>
1. <span class="preview"> （条件付き）テンプレートからプロジェクトを作成することを選択した場合は、記事 [ テンプレートを使用したプロジェクトの作成 ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) の記事の手順に従って、プロジェクトの追加を完了します。</span>

   新しいプロジェクトが作成され、選択したレコードの接続されたフィールドに追加されます。

1. （任意） Workfront Planning から新しいプロジェクトの名前をクリックして、Workfrontでプロジェクトのページを開き、プロジェクトをさらに更新します。

## Workfront Planning のレコードにポートフォリオを接続する際にポートフォリオを作成する

他のレコードから接続する際にポートフォリオを作成するには：

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

   Workfront Planning の次の領域の「接続」フィールドからポートフォリオを接続できます。

   * レコードタイプのテーブル表示
   * レコードの詳細ページまたはプレビューボックス

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. （条件付き）別のレコードの接続済みレコードフィールドから追加しようとしたときにポートフォリオが見つからない場合は、名前を追加して、「**+ ポートフォリオを追加**」をクリックします。 「追加」ボタンの後には、入力したポートフォリオ名も続きます。

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   ポートフォリオが作成され、選択したレコードの接続フィールドに追加されます。

1. （任意）Workfront プランニングから新しいポートフォリオの名前をクリックして、Workfrontでポートフォリオのページを開き、ポートフォリオをさらに更新します。

<!--

<div class="preview">

## Create programs when connecting them with records from Workfront Planning

To create programs as you are connecting them from other records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    You can connect programs from a connection field in following areas of Workfront Planning:

    * The table view of a record type
    * The details page or preview box of a record

    ********at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."***********
    
1. (Conditional) If you cannot find a program when trying to add it from the connected record field of another record, add a name, then click **+ Add**. The Add button is followed by the program name you typed. 

    ![](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->