---
title: CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、CSV または Excel ファイルから情報をインポートすることで、組織のライフサイクルで必要な作業項目を示すカスタムレコードタイプを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 32%

---

# CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、CSV または Excel ファイルから情報をインポートすることで、組織のライフサイクルで必要な作業項目を示すカスタムレコードタイプを作成できます。

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
<p>任意のWorkfrontと任意の Planning パッケージ</p>
または
<p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
 
</tbody> 
</table>-->


## Excel または CSV ファイルを使用したレコードタイプの読み込みに関する考慮事項

* Excel ファイルの各シートがレコードタイプになります。 シートの名前がレコードタイプの名前になります。
* シートが 1 つだけの場合、または CSV ファイルを読み込む場合、ファイルの名前がレコードタイプの名前になります。
* 各シートの列ヘッダーは、各レコードタイプに関連付けられたフィールドになります。
* フィールドは、それぞれのレコードタイプについて一意です。
* 各シートの各行は、各レコードタイプに関連付けられた一意のレコードになります。
* Excel ファイルの各シートの上限は次のとおりです：
   * 25,000 行
   * 500 列
* ファイルのサイズは 5 MB 以下にしてください。
* 空のシートはサポートされていません。
* 次のタイプのフィールドはサポートされておらず、インポートシートのフィールドにマッピングできません。

   * Workfront、AEM Assets オブジェクトタイプまたはGenStudio ブランドへの接続フィールド。
   * 接続された Planning レコード、Workfront、AEM Assets オブジェクト、GenStudio ブランドのフィールドを検索します。
   * 数式フィールド
   * 作成日、作成者
   * 最終変更日、最終変更者
   * 承認日、承認者
   * ユーザー

Excel または CSV ファイルを使用してレコードタイプを読み込むには：

{{step1-to-planning}}

1. レコードタイプを作成するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。
1. 「**レコードタイプを追加**」をクリックします。
1. **ファイルからアップロード** をクリックします。
1. コンピューターに以前に保存した Excel または CSV ファイルをドラッグ&amp;ドロップするか、「**CSV または Excel ファイルを選択**」をクリックして参照してから選択します。
1. **プレビューと編集** をクリックします。

   **プレビューと編集** ボックスが表示され、次の情報が表示されます。

   * 左パネルに、シートまたは将来のレコードタイプの名前が表示されます。Workfront Planning により、新しいレコードタイプごとにデフォルトでアイコンとカラーが選択されます。
   * 最初のシートまたはレコードタイプが選択され、関連付けられたフィールド名が列ヘッダーとして表示されます。各フィールドのタイプは、デフォルトで選択されています。
   * 各行は新しいレコードを表します。「プレビューと編集」ボックスには、最初の 10 レコードのみが表示されます。

   ![ プレビューと編集ボックス ](assets/preview-and-edit-box.png)

1. （オプション）左パネルの各シート名をクリックすると、シートに含まれる情報を確認できます。

   >[!NOTE]
   >
   >空のシートはサポートされておらず、淡色の表示になります。

1. （オプション）左側のパネルから読み込まないシートの選択を解除します。

   ![ 読み込むシートを選択ドロップダウン（未選択 ](assets/select-sheets-to-import-drop-down-with-unselected.png)

   選択を解除したシートは、グレーの背景で表示されます。

1. （オプション）列ヘッダーの右側にある下向き矢印をクリックして、「**フィールド**」タブで次のいずれかの操作を行います。

   ![ レコードタイプマッピングのインポートボックスの「フィールド」タブ ](assets/field-tab-on-record-type-import-mapping-box.png)

   * いずれかのフィールドの名前を変更する
   * **フィールドタイプ** を変更する
   * フィールド **説明** を更新

1. （オプション）「**接続**」タブをクリックして、列内の情報を他のレコードタイプの接続されたフィールドにマッピングします。

   ![ レコードタイプの読み込みマッピングボックスの「接続」タブ ](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >マッピングできるのは、Workfront Planning に接続されたレコードのフィールドのみです。 Workfront、AEM Assets、GenStudio Brands のいずれかの接続からフィールドにマッピングすることはできません。 詳しくは、この記事の「[Excel または CSV ファイルを使用したレコードタイプの読み込みに関する考慮事項 ](#considerations-about-importing-record-types-using-an-excel-or-csv-file) の節を参照してください。

1. （任意）フィールドに関する情報を更新したら、「**保存**」をクリックします。

1. ファイルを読み込む準備が整ったら「**読み込み**」をクリックします。

   次の情報が Workfront Planning にインポートされます。

   * 新しいレコードタイプ
   * 各レコードタイプに関連付けられた新しいフィールド
   * 各レコードタイプに関連付けられた新しいレコード

   レコードタイプページのフィールドとレコードの管理を開始できます。

   Workfront Planning およびワークスペースへのアクセス権を持つすべてのユーザーは、インポートされたレコードタイプとその情報を表示および編集できるようになりました。
