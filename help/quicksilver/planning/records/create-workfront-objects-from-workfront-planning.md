---
title: Workfront Planning からのWorkfrontオブジェクトの作成
description: Workfront オブジェクトタイプは、Workfront Planning 内の他のレコードから関連付ける際に作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 10%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront オブジェクトをレコードに関連付ける際に、Workfront Planning からデータモデルを作成する

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview"> このページでハイライト表示されている情報は、まだ一般公開されていない機能を指しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Workfront Planning からAdobe Workfrontオブジェクトを作成するには、次の方法があります：

* Workfront オブジェクトを Planning レコードから接続する場合

  ここでは、Workfront Planning からWorkfrontオブジェクトを作成し、Planning レコードから接続する方法について説明します。
* <span class="preview"> レコードのページから自動化を使用する場合。</span>

  <span class="preview"> 自動化を使用したWorkfront オブジェクトの作成については、[Adobe Workfront Planning レコードの自動化を使用したオブジェクトの作成 ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。</span>

Workfront計画レコードを次のWorkfrontオブジェクト・タイプと関連付けると、Workfront計画から次のタイプのWorkfrontオブジェクトを作成できます。

* プロジェクト
* ポートフォリオ
* <span class="preview">プログラム</span>

>[!IMPORTANT]
>
>* レコードから接続する場合、Workfrontで作成できるのは、プロジェクト、ポートフォリオおよび <span class="preview"> プログラム </span> のみです。
>
>* Workfront Planning のレコードからグループや会社を関連付ける場合は、それらのグループや会社を作成できません。
>

Workfront Planning の次の領域の接続フィールドから、プロジェクト、ポートフォリオ、<span class="preview"> およびプログラムを接続で </span> ます：

* レコードタイプのテーブル表示
* レコードの詳細ページまたはプレビューボックス
* レコードの「接続」タブ

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
   <p>レコードを関連付ける際に作成するオブジェクトタイプ（プロジェクト、プログラム、ポートフォリオ）のWorkfrontでのアクセス権を編集します。 </p>  
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

* Workfront プロジェクト、ポートフォリオまたは <span class="preview"> プログラム </span> に接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* レコード。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* この記事の [ アクセス要件 ](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

## Workfront Planning のレコードにプロジェクトを結び付けながらプロジェクトを作成します

他のレコードから接続する際にプロジェクトを作成するには：

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront プロジェクトの接続を開始します。

1. （条件付き） <span class="preview"> クリック **プロジェクトを追加**</span>
または
プロジェクトの名前の入力を開始し、見つからない場合は **プロジェクトを追加** をクリックします。

   別のレコードの「接続されたレコード」フィールドからプロジェクトを追加しようとして、見つからない場合は、名前を追加してから、「**プロジェクトを追加**」をクリックします。 「追加」ボタンの後に、入力したプロジェクト名が続きます。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![ 接続フィールドから接続する際にプロジェクトを追加 ](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview"> 「**プロジェクトを作成** ボックスが開きます。</span>

1. <span class="preview"> （任意） **プロジェクト名** を更新します。 デフォルトでは、プロジェクトの名前は、レコードから接続する際に検索項目として追加した名前に基づいて付けられます。</span>
1. <span class="preview"> （任意） **プロジェクトテンプレート** を選択します。 テンプレートを選択しない場合、Workfrontはタスクを含まない空のプロジェクトを作成します。</span>
1. <span class="preview">**作成** をクリックします。</span>
1. <span class="preview"> （条件付き）テンプレートからプロジェクトを作成することを選択した場合は、記事 [ テンプレートを使用したプロジェクトの作成 ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) の記事の手順に従って、プロジェクトの追加を完了します。</span>

   新しいプロジェクトが作成され、選択したレコードの接続されたフィールドに追加されます。

1. （任意） Workfront Planning から新しいプロジェクトの名前をクリックして、Workfrontでプロジェクトのページを開き、プロジェクトをさらに更新します。

## ポートフォリオをWorkfront Planning のレコードに接続する際のポートフォリオの作成

計画レコードから接続するポートフォリオを作成する手順は、次のとおりです。

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. （条件付き） <span class="preview"> クリック **ポートフォリオを追加**</span>

   または

   ポートフォリオ名の入力を開始し、見つからない場合は **ポートフォリオを追加** をクリックします。—> 別のレコードの「接続済みレコード」フィールドから追加しようとしたときにポートフォリオが見つからない場合は、名前を追加して、「**ポートフォリオを追加**」をクリックします。 「追加」ボタンの後には、入力したポートフォリオ名も続きます。

   ![ 接続フィールドから接続する際にポートフォリオを追加 ](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   ポートフォリオが作成され、選択したレコードの接続フィールドに追加されます。

1. （任意）Workfront プランニングから新しいポートフォリオの名前をクリックして、Workfrontでポートフォリオのページを開き、ポートフォリオをさらに更新します。

<div class="preview">

## Workfront Planning のレコードにプログラムを関連付ける際に、プログラムを作成します

Planning レコードから接続するプログラムを作成するには、次の手順に従います。

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."-->

1. 「**プログラムを追加**」をクリックします

   または

   プログラム名の入力を開始し、見つからない場合は **プログラムを追加** をクリックします。 「追加」ボタンの後に、入力したプログラム名が続きます。

   ![ 接続フィールドから接続する際にWorkfront プログラムを追加する ](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   **プログラムを作成** ボックスが開きます。

1. **プログラム名** を更新します。 必須フィールドです。
1. ドロップダウンから **Portfolio** を選択するか、ポートフォリオの名前の入力を開始し、リストに表示されたら選択します。 必須フィールドです。
1. 「**作成**」をクリックします。

   プログラムが作成され、選択したレコードの接続フィールドに追加されます。

1. （オプション）Workfront Planning から新しいプログラムの名前をクリックして、Workfrontでプログラムのページを開き、さらに更新を行います。

</div>

