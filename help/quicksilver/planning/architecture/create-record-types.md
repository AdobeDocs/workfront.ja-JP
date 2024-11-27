---
title: レコードタイプの作成
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、組織のライフサイクルで必要な作業アイテムを示すカスタムレコードタイプを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 64%

---


<!--this is linked to the UI in an empty workspace screen-->

# レコードタイプの作成

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、組織のライフサイクルで必要な作業に関連するアイテムを示すカスタムレコードタイプを作成できます。

レコードタイプについて詳しくは、[ レコードタイプの概要 ](/help/quicksilver/planning/architecture/overview-of-record-types.md) を参照してください。

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
   <td><p> 標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## レコードタイプの作成に関する考慮事項

* 以下の方法で、ワークスペースでレコードタイプを作成できます。

   * 自動：
      * テンプレートを使用してワークスペースを作成する場合。

        詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

      * <span class="preview">Excel または CSV ファイルを使用して読み込む場合。</span>

     >[!TIP]
     >
     ><span class="preview"> レコードタイプを Excel または CSV ファイルから読み込む場合、レコードやフィールドも読み込まれる場合があります。</span>

   * 手動：

      * 最初から。

        この記事では、レコードタイプをゼロから作成する方法について説明します。

* レコードタイプは、セクション内で、およびワークスペースのあるセクションから別のセクションに移動できます。あるワークスペースから別のワークスペースに移動することはできません。

## ワークスペーステンプレートを使用してレコードタイプを作成

Workfront Planning テンプレートを使用してワークスペースを作成すると、レコードタイプを自動的に作成できます。各テンプレートには、サンプルレコードタイプが含まれています。

テンプレートからワークスペースを作成する場合、レコードタイプは次のセクションにグループ化されます。

* 運用中のレコードタイプ
* 分類

運用レコードタイプおよび分類セクションの両方で、レコードタイプを手動で追加できます。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

各テンプレートに含まれているレコードタイプについては、[ワークスペーステンプレートのリスト](/help/quicksilver/planning/architecture/workspace-templates.md)を参照してください。

## レコードタイプを最初から作成

{{step1-to-planning}}

1. レコードタイプを作成するワークスペースをクリックし、

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。
1. （任意）「**セクションを追加**」をクリックし、新規セクションをワークスペースに追加します。
1. **レコードタイプを追加** をクリックし、<span class="preview">**新規**</span> をクリックします。

   レコードタイプを追加ボックスが開きます。
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 次の情報を更新します。

   * 「名称未設定のレコードタイプ」を、今後のレコードタイプの名前に置き換えます。<!--did they bring back the field label here and did they rename it to "Name"-->
   * **説明**：レコードタイプに関する詳細情報を追加します。
   * レコードタイプに関連付けられたアイコンの色と形状を選択します。 次の操作を実行します。
      * 新しいレコードタイプを識別する色を選択します。これは、レコードタイプアイコンの色です。灰色はデフォルトで選択されています。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。

1. 「**作成**」をクリックします。

   選択したセクションとワークスペースにレコードタイプカードが追加されます。
レコードタイプの説明がカードに表示されます。

   ![](assets/record-type-card-with-description.png)

1. （オプション）レコードタイプカードにポインタを合わせ、右上隅にある **詳細** アイコン ![](assets/more-menu.png) をクリックしてから、**編集** をクリックして、レコードタイプに関する情報を変更します。
1. （オプション）レコードタイプカードをクリックして、レコードタイプのページを開きます。

   ![](assets/operational-record-type-blank.png)

   デフォルトでは、レコードタイプページがテーブルビューに表示されます。テーブルの列は、新しいレコードタイプに関連付けられたフィールドです。各行は、追加する必要がある一意のレコードです。

   デフォルトでは、次のフィールドが、運用中のレコードタイプのテーブルビュー列に表示されます。

   * 名前
   * 説明
   * 開始日
   * 終了日
   * ステータス

1. （オプション）ページのヘッダーのレコードタイプ名を更新します。

   または

   レコードタイプ名の右側に ![](assets/more-menu.png) る **詳細** アイコンをクリックし、**編集** をクリックして名前を変更するか、情報を変更します。 詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

1. （オプション）「**+ 新規レコード**」をクリックして、選択したレコードタイプのレコードを追加します。詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
1. （オプション）テーブルの右上隅にある「**+**」アイコンをクリックして、レコードタイプにさらにフィールドを追加します。

   フィールドの作成について詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

1. （オプション）レコードタイプ名の左側にある左向き矢印をクリックして、選択したワークスペースに戻ります。

1. （オプション）ワークスペースでレコードタイプカードをクリックして保持し、目的の場所でレコードタイプをドラッグ＆ドロップするか、別のセクションに移動します。

   変更は自動的に保存されます。

   レコードの追加、レコードタイプの削除または編集、レコードタイプページでのビューの更新について詳しくは、次の記事を参照してください。

   * [レコードの作成](/help/quicksilver/planning/records/create-records.md)
   * [レコードタイプの削除](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [レコードタイプの編集](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [レコードビューの管理](/help/quicksilver/planning/views/manage-record-views.md)

<div class="preview">

## Excel または CSV ファイルをインポートしてレコードタイプを作成

Excel ファイルや CSV ファイルを使用してレコードタイプを読み込む際は、次の点を考慮してください。

* Excel ファイルの各シートがレコードタイプになります。 シートの名前がレコードタイプの名前になります。
* シートが 1 つだけの場合、または CSV ファイルを読み込む場合、ファイルの名前がレコードタイプの名前になります。
* 各シートの列ヘッダーは、各レコードタイプに関連付けられたフィールドになります。
* フィールドは、それぞれのレコードタイプについて一意です。
* 各シートの各行は、各レコードタイプに関連付けられた一意のレコードになります。
* Excel ファイルの各シートの上限は次のとおりです：
   * 10,000 行
   * 500 列
* Excel ファイルのサイズは 5 MB 以下にする必要があります。
* 空のシートはサポートされていません。

Excel または CSV ファイルを使用してレコードタイプを読み込むには：

{{step1-to-planning}}

1. レコードタイプを作成するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。
1. 「**レコードタイプを追加**」をクリックします。
1. **ファイルから** をクリックします。
1. コンピューターに保存済みの Excel ファイルまたは CSV ファイルをドラッグアンドドロップするか、「**CSV ファイルまたは Excel ファイルを選択**」をクリックして参照します。
1. **プレビューと編集** をクリックします。

   **プレビューと編集** ボックスが表示され、次の情報が表示されます。

   * 左パネルに、シートまたは将来のレコードタイプの名前が表示されます。Workfront Planning により、新しいレコードタイプごとにデフォルトでアイコンとカラーが選択されます。
   * 最初のシートまたはレコードタイプが選択され、関連付けられたフィールド名が列ヘッダーとして表示されます。各フィールドのタイプは、デフォルトで選択されています。
   * 各行は新しいレコードを表します。「プレビューと編集」ボックスには、最初の 10 レコードのみが表示されます。

   ![](assets/preview-and-edit-box.png)

1. （オプション）左パネルの各シート名をクリックすると、シートに含まれる情報を確認できます。

   >[!NOTE]
   >
   >空のシートはサポートされておらず、淡色の表示になります。

1. （オプション）左側のパネルから読み込まないシートの選択を解除します。

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   選択を解除したシートは、グレーの背景で表示されます。

1. （オプション）列ヘッダーの右側にある下向き矢印をクリックして、次のいずれかの操作を行います。

   * いずれかのフィールドの名前を変更する
   * **フィールドタイプ** を変更する
   * フィールド **説明** を更新

1. （任意）フィールドに関する情報を更新したら、「**保存**」をクリックします。

1. ファイルを読み込む準備が整ったら「**読み込み**」をクリックします。

   次の情報が Workfront Planning にインポートされます。

   * 新しいレコードタイプ
   * 各レコードタイプに関連付けられた新しいフィールド
   * 各レコードタイプに関連付けられた新しいレコード

   レコードタイプページのフィールドとレコードの管理を開始できます。

   読み込まれたレコードタイプとその情報をWorkfront Planning にアクセスできるユーザー全員が表示および編集できるようになりました。

</div>

