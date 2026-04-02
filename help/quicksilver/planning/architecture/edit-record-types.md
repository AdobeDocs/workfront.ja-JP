---
title: レコードタイプの編集
description: 保存後にレコードタイプを編集できます。レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 10d2bcf3f2d349418a8a04e96873bc5c2d3af4a1
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 27%

---


# レコードタイプの編集

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。自分または他のユーザーが作成したレコードタイプの外観を編集できます。Workfront Planning レコードタイプの作成について詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

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
<p>任意のWorkfrontおよびプランニングパッケージ</p>
<p>任意のWorkfrontおよびプランニングパッケージ</p>
<p><b>メモ</b></p>
<p>接続可能なレコードタイプを設定するには： </p>
<ul> 
<li><p>任意のWorkfront パッケージと任意のPlanning パッケージ</p></li>
または
<li><p>任意のワークフローとプランニング PrimeまたはUltimate パッケージ</p></li></ul>


<p>グローバルレコードタイプを設定するには：</p>

<ul> 
<li><p>任意のWorkfront パッケージとPlanning Plus パッケージ</p></li>
または
<li><p>任意のワークフローとプランニング PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p>

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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

<!--
Old:
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table>
-->

## レコードタイプの編集

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにカーソルを合わせ、レコードタイプカードの右上隅にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**編集**&#x200B;または&#x200B;**設定**をクリックします
または
   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**編集**&#x200B;または&#x200B;**設定**&#x200B;をクリックします。

   ![設定を含むレコードタイプカードのその他のメニューオプション ](assets/more-menu-options-from-record-type-card-with-settings-link.png)

1. **レコードタイプを編集** ボックスで、**アピアランス** タブがデフォルトで開きます。

   ![ レコードタイプボックスのアピアランスを編集タブ ](assets/edit-record-type-box-appearance-tab.png)

   「**アピアランス**」タブの次の情報を更新します。

   * 必要に応じて、レコードタイプ名を編集します。<!--did they add a field label for this?-->
   * **説明**: レコードタイプの説明を、その詳細を含めて編集または追加します。
   * レコードタイプに関連付けられているアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードタイプを識別するための色を選択します。これは、レコードタイプアイコンの色です。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。

1. （オプションおよび条件付き）システム管理者の場合は、「**クロスワークスペース設定**」タブをクリックし、レコードタイプのクロスワークスペース機能に関する情報を更新します。

   詳細については、[ レコードタイプのクロスワークスペース機能の設定](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)を参照してください。

   ![ クロスワークスペース設定タブを含むレコードタイプボックスを編集](assets/edit-record-type-box-advanced-settings-tab.png)

1. 「**保存**」をクリックします。

   このレコードを他のワークスペースから接続することを選択した場合、**接続可能なレコード** アイコン ![他のスペースから接続アイコン ](assets/connect-from-other-workspaces-icon.png)がレコードカードに表示されます。

   このレコードを他のワークスペースに追加することを許可するように選択した場合、**グローバルレコード** アイコン ![ グローバルレコードタイプアイコン ](assets/global-icon.png)がレコードカードに表示されます。

1. （オプション）ワークスペース領域のレコードタイプカードをクリックしてレコードタイプのページを開き、ヘッダーのレコードタイプの名前を変更します。

1. （オプション）別のレコードタイプを編集するには、レコードタイプページから、レコードタイプ名の右側にある下向き矢印を展開し、レコードタイプを検索して、リストに表示されたら選択します。

   ![検索ボックスを含むレコードタイプページのレコードタイプ ドロップダウン ](assets/record-type-drop-down-on-record-type-page-with-search-box.png)

   >[!TIP]
   >
   ><span class="preview">次のキーボードの組み合わせを使用して、任意のWorkfront Planning ページからグローバル検索ボックスを開き、レコードタイプ :</span>を検索できます
   >
   >* Windows<span class="preview">の</span>CTRL+K
   >* Mac<span class="preview">⌘の</span>+K
   >
   >![ グローバル検索ボックス ](assets/global-search-box.png)
