---
title: レコードタイプの作成
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、組織のライフサイクルで必要な作業アイテムを示すカスタムレコードタイプを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 49%

---


<!--this is linked to the UI in an empty workspace screen-->

<!--keep the yellow for cross-workspace functionality till Jan 2026-->

# レコードタイプの作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、組織のライフサイクルで必要な作業に関連するアイテムを示すカスタムレコードタイプを作成できます。

レコードタイプについて詳しくは、[ レコードタイプの概要 ](/help/quicksilver/planning/architecture/overview-of-record-types.md) を参照してください。

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
<p>任意のWorkfrontおよび Planning パッケージ</p>
<p>任意のワークフローおよび計画パッケージ</p>
<p><b>メモ</b></p>
<p>接続可能なレコード・タイプを構成する手順は、次のとおりです。 </p>
<ul> 
<li><p>任意のWorkfront パッケージと任意の Planning パッケージ</p></li>
<p>または</p>
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>

<div class="preview">
<p>グローバルレコードタイプを設定するには：</p>

<ul> 
<li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
<p>または</p>
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p>

</div>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
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
</table> -->

## レコードタイプの作成に関する考慮事項

* 以下の方法で、ワークスペースでレコードタイプを作成できます。

   * 自動：
      * テンプレートを使用してワークスペースを作成する場合。

        詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

      * CSV または Excel ファイルを使用して読み込む場合。

        詳しくは、[CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成 ](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md) を参照してください。

     >[!TIP]
     >
     >レコードタイプを CSV または Excel ファイルから読み込む場合、レコードとフィールドを読み込むこともできます。

   * 手動：

      * 最初から。

        この記事では、レコードタイプをゼロから作成する方法について説明します。

     <!--
        * <span class="preview">By adding them from another workspace</span>
            <span class="preview">For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). </span>-->


* レコードタイプは、セクション内で、およびワークスペースのあるセクションから別のセクションに移動できます。あるワークスペースから別のワークスペースに移動することはできません。

## ワークスペーステンプレートを使用してレコードタイプを作成

Workfront Planning テンプレートを使用してワークスペースを作成すると、レコードタイプを自動的に作成できます。各テンプレートには、サンプルレコードタイプが含まれています。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

各テンプレートに含まれているレコードタイプについては、[ワークスペーステンプレートのリスト](/help/quicksilver/planning/architecture/workspace-templates.md)を参照してください。

テンプレートからワークスペースを作成する場合、レコードタイプは次のセクションにグループ化されます。

* 運用中のレコードタイプ
* 分類

運用中のレコードタイプおよび分類セクションの両方で、レコードタイプを手動で追加できます。 詳しくは、この記事の [ ゼロからレコードを作成する ](#create-a-record-type-from-scratch) の節を参照してください。

## レコードタイプを最初から作成

{{step1-to-planning}}

1. レコードタイプを作成するワークスペースをクリックし、

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。
1. （任意）「**セクションを追加**」をクリックし、新規セクションをワークスペースに追加します。
1. **レコードタイプを追加** をクリックし、次に **手動で追加** をクリックします。

   「レコードタイプを追加」ボックスが開きます。<!--update screen shot for preview-->

   ![ 外観のオプションを含むレコードタイプボックスを追加 ](assets/add-record-type-box-with-appearance-options.png)

1. 「**外観** タブの次の情報を更新します。

   * 「名称未設定のレコードタイプ」を、今後のレコードタイプの名前に置き換えます。<!--did they bring back the field label here and did they rename it to "Name"-->
   * **説明**：レコードタイプに関する詳細情報を追加します。
   * レコードタイプに関連付けられたアイコンの色と形状を選択します。 次の操作を実行します。
      * 新しいレコードタイプを識別する色を選択します。これは、レコードタイプアイコンの色です。灰色はデフォルトで選択されています。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。

1. （オプションおよび条件付き）システム管理者の場合は、**詳細設定**<span class="preview"> または **クロスワークスペース設定**</span> タブをクリックして、レコードタイプのクロスワークスペース機能に関する情報を更新します。

   詳しくは、[ レコードタイプのクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。<!--update screen shot at production - Jan 2026-->

   ![ 「詳細設定」タブの「レコードタイプを編集」ボックス ](assets/edit-record-type-box-advanced-settings-tab.png)

   詳しくは、[ レコードタイプに対するクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

1. 「**保存**」をクリックします。

   選択したセクションとワークスペースにレコードタイプカードが追加されます。
レコードタイプの説明がカードに表示されます。

   ![ 説明を記載したレコードタイプカード ](assets/record-type-card-with-description.png)

   このレコードを他のワークスペースから接続することを選択した場合、レコード カードに **接続可能なレコード** アイコン ![ 他のスペースから接続アイコン ](assets/connect-from-other-workspaces-icon.png) が表示されます。

   <span class="preview"> このレコードを他のワークスペースに追加することを許可するように選択した場合、レコードカードに **グローバルレコード** アイコン ![ グローバルレコードタイプアイコン ](assets/global-icon.png) が表示されます。</span>

1. （オプション）レコードタイプカードにポインタを合わせ、右上隅にある **詳細** アイコン ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**編集** または <span class="preview">**設定**</span> をクリックして、レコードタイプに関する情報を変更します。

   詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

1. （オプション）レコードタイプカードをクリックして、レコードタイプのページを開きます。

   ![ 運用レコードタイプが空白です ](assets/operational-record-type-blank.png)

   デフォルトでは、レコードタイプページがテーブルビューに表示されます。テーブルの列は、新しいレコードタイプに関連付けられたフィールドです。各行は、追加する必要がある一意のレコードです。

   デフォルトでは、次のフィールドが、運用中のレコードタイプのテーブルビュー列に表示されます。

   * 名前
   * 説明
   * 開始日
   * 終了日
   * ステータス

1. （オプション）ページのヘッダーのレコードタイプ名を更新します。

   または

   レコードタイプ名の右側にある **詳細** アイコン ![ 詳細メニュー ](assets/more-menu.png) をクリックし、**編集** をクリックして、名前を変更したり、情報を変更したりします。 詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

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

## CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成

CSV または Excel ファイルから情報を読み込む場合は、次の情報を読み込むことができます。

* レコードタイプ
* レコード
* レコードフィールド

詳しくは、[CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成 ](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md) を参照してください。

<!--

<div class="preview">

## Create record types by adding existing ones from another workspace 

You can add record types to a workspace by adding existing ones from another workspace. You can only add record types that have been configured as global record types. 

For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

</div>

-->