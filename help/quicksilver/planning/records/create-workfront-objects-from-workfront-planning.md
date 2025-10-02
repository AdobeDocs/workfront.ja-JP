---
title: Workfront オブジェクトをレコードに関連付ける際に、Workfront Planning からデータモデルを作成する
description: Workfront オブジェクトタイプは、Workfront Planning 内の他のレコードから関連付ける際に作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 5b9b1f397c76afa2e2ae550e0ce62a6038b8bd86
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 8%

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
* レコードのページから自動化を使用する場合。

  オートメーションを使用したWorkfrontオブジェクトの作成については、[Adobe Workfront計画レコードのオートメーションを使用したオブジェクトの作成 ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。

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
   * <span class="preview"> レコードの接続済みレコードページ（詳細領域） </span>

* ポートフォリオとプログラムは、Workfront Planning の次の領域から作成できます。

   * レコードタイプのテーブル表示
   * 接続フィールドのレコードの「詳細」領域

Planning レコードとWorkfrontオブジェクトの接続の詳細は、[ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
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
   <p>作成するオブジェクトタイプ（プロジェクト、ポートフォリオ、プログラム）のWorkfrontでオブジェクトを作成アクセス権を使用してアクセスを編集します。 </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>ワークスペースに対する権限と、レコードを追加するレコードタイプを管理します。 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
   <p>子オブジェクト（プロジェクト）を追加するためのWorkfront オブジェクト（ポートフォリオ）への権限を管理します。</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront オブジェクトをWorkfront Planning のレコードに関連付ける際の、オブジェクト作成の前提条件

既存のレコードから接続して新しいプロジェクトまたはポートフォリオを追加するには、次のものが必要です。

* Workfront プロジェクト、ポートフォリオまたはプログラムに接続されたレコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* Workfront オブジェクトに接続されたレコードタイプのレコード。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* この記事の [ アクセス要件 ](#access-requirements) の節で説明しているように、Workfront Planning およびWorkfrontでの正しいアクセス権と権限。

## Workfront Planning のレコードにプロジェクトを結び付けながらプロジェクトを作成します

Workfront Planning の次の領域で、プロジェクトをWorkfront Planning のレコードに関連付けながらプロジェクトを作成できます：

* 接続フィールドのレコードタイプのテーブルビューまたはレコードの詳細エリア
* <span class="preview"> レコード </span> ージの「詳細」領域にある、レコードの「接続済みレコード」ページ

### レコードの「詳細」エリアまたはレコードタイプのテーブル表示からプロジェクトを作成する

他のレコードから接続する際にプロジェクトを作成するには：

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront プロジェクトの接続を開始します。

1. （条件付き） **プロジェクトを追加** をクリック
または
プロジェクトの名前の入力を開始し、見つからない場合は **プロジェクトを追加** をクリックします。 「追加」ボタンの後に、入力したプロジェクト名が続きます。

   ![ 接続フィールドから接続する際にプロジェクトを追加 ](assets/add-project-when-connecting-it-from-connection-field.png)

   **プロジェクトを作成** ボックスが開きます。

1. （任意） **プロジェクト名** を更新します。 デフォルトでは、プロジェクトの名前は、レコードから接続する際に検索項目として追加した名前に基づいて付けられます。
1. （任意）「**プロジェクトテンプレート**」を選択します。 テンプレートを選択しない場合、Workfrontはタスクを含まない空のプロジェクトを作成します。
1. 「**作成**」をクリックします。
1. （条件付き）テンプレートからプロジェクトを作成することを選択した場合は、記事 [ テンプレートを使用したプロジェクトの作成 ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) の手順に従って、プロジェクトの追加を完了します。

   新しいプロジェクトが作成され、選択したレコードの接続されたフィールドに追加されます。

1. （任意） Workfront Planning から新しいプロジェクトの名前をクリックして、Workfrontでプロジェクトのページを開き、プロジェクトをさらに更新します。

<div class="preview">

### レコードの接続されたレコードページからのプロジェクトの作成

1. テーブル表示で、プロジェクトのオブジェクトタイプをWorkfrontの Planning レコードタイプに関連付けます。

   詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

1. 任意のビューでレコードの名前をクリックします。 「詳細」 プレビューボックスが開きます。

1. プロジェクトの **接続されたレコードのページ** を追加します。

   詳しくは、「レコードページレイアウトの管理 [ の「接続されたレコードページをレコードに追加する」の節を参照し ](/help/quicksilver/planning/records/manage-the-record-page.md) ください。

   接続されたレコード ページがテーブル ビューに表示されます。 接続されたプロジェクトがテーブルに表示されます。

   ![ 接続されたレコードページのプロジェクト テーブルビュー ](assets/projects-connected-records-page-table.png)

1. プロジェクト テーブルで **新規行** をクリックして、プロジェクトを追加します。

   この領域で追加できるのは空のプロジェクトのみです。 テンプレートを使用してプロジェクトを追加することはできません。
1. （オプション）テーブル表示でプロジェクトの名前をクリックして、Workfrontでプロジェクトを開き、詳細を追加します。

</div>

## ポートフォリオをWorkfront Planning のレコードに接続する際のポートフォリオの作成

ポートフォリオは、レコードタイプのテーブル表示またはレコードの詳細ページから作成できます。

計画レコードから接続するポートフォリオを作成する手順は、次のとおりです。

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

1. （条件付き） **ポートフォリオを追加** をクリック

   または

   ポートフォリオ名の入力を開始し、見つからない場合は **ポートフォリオを追加** をクリックします。 「追加」ボタンの後に、入力したポートフォリオ名が表示されます。

   ![ 接続フィールドから接続する際にポートフォリオを追加 ](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   ポートフォリオが作成され、選択したレコードの接続フィールドに追加されます。

1. （任意）Workfront プランニングから新しいポートフォリオの名前をクリックして、Workfrontでポートフォリオのページを開き、ポートフォリオをさらに更新します。

## Workfront Planning のレコードにプログラムを関連付ける際に、プログラムを作成します

プログラムは、レコードタイプのテーブル表示またはレコードの詳細ページから作成できます。

Planning レコードから接続するプログラムを作成するには、次の手順に従います。

1. [ レコードの接続 ](/help/quicksilver/planning/records/connect-records.md) の記事の説明に従って、レコードの詳細ページまたはレコードタイプのテーブルに移動し、Workfront Planning レコードとWorkfront ポートフォリオの接続を開始します。

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

