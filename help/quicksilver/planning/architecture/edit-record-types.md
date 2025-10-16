---
title: レコードタイプを編集
description: 保存後にレコードタイプを編集できます。レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 27%

---


# レコードタイプの編集

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

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
<p>接続可能レコード・タイプを使用可能にする手順は、次のとおりです。 </p>
<ul> 
<li><p>任意のWorkfront パッケージと任意の Planning パッケージ</p></li>
<p>または</p>
<li><p>ワークフローおよび計画のPrimeとUltimate パッケージ</p></li></ul>

<p>グローバルレコードタイプを有効にするには：</p>

<ul> 
<li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
<p>または</p>
<li><p>ワークフローおよび計画のPrimeとUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
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
</table> -->

## レコードタイプの編集

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックしてから、**編集** をクリックします
     <!--<span class="preview">or **Settings**</span>-->
または
   * <span class="preview"> レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**編集**<!--<span class="preview">or **Settings**</span>. </span>--> をクリックします

   <!--<span class="preview">![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)</span>-->

1. **レコードタイプを編集** ボックスで、「**外観** タブがデフォルトで開きます。<!--update screen shot below at preview-->

   ![&#x200B; レコードタイプを編集ボックスの「外観」タブ &#x200B;](assets/edit-record-type-box-appearance-tab.png)

   「**外観**」タブで次の情報を更新します。

   * 必要に応じて、レコードタイプ名を編集します。<!--did they add a field label for this?-->
   * **説明**：詳しい情報を含むレコードタイプの説明を編集または追加します。
   * レコードタイプに関連付けられたアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードタイプを識別するための色を選択します。これは、レコードタイプアイコンの色です。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。


1. （オプションおよび条件付き）システム管理者の場合は、「**詳細設定**」をクリックして、「**クロスワークスペース機能**」セクションで次の情報を更新します。<!--the info here is duplicated in the Create record types article-->
   * **他のワークスペースでこのレコードタイプへの接続を許可** 設定を有効にする：これにより、ワークスペースマネージャーは他のワークスペースからこのレコードタイプに接続できます。\
     このレコードタイプを接続できるワークスペースを指定できます。 すべてのワークスペースで使用できるようにすることも、読み込み先となる特定のワークスペースを指定することもできます。
詳しくは、[&#x200B; レコードタイプに対するクロスワークスペース機能の設定 &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。


   ![&#x200B; 「詳細設定」タブの「レコードタイプを作成」ボックス &#x200B;](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release global record types; the preview tags might need to be edited, too:
    1. <span class="preview">(Optional and conditional) If you are a system administrator, update the information in the **Cross-workspace settings** tab.</span>
    <span class="preview">For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).</span>
    ***********Add screenshot***********
    -->

1. 「**保存**」をクリックします。

   ワークスペースのレコードタイプカードの右上隅に、接続アイコン ![&#x200B; 他のワークスペースから接続アイコン &#x200B;](assets/connect-from-other-workspaces-icon.png) が表示され、レコードが他のワークスペースからアクセスできるようになったことを示します。

   <!--replace the blurb above after "Save" with this: <span class="preview">If you configured the cross-workspace capabilities for the record, the **connectable record type** icon ![Connectable record type icon](assets/connect-from-other-workspaces-icon.png) and the **global record type** icon ![Global record type icon](assets/global-icon.png) also display on the card. </span>-->

1. （オプション）ワークスペース領域からレコードタイプカードをクリックしてレコードタイプのページを開き、ヘッダーでレコードタイプの名前を変更します。

1. （オプション）別のレコードの種類を編集するには、レコードの種類のページで、レコードの種類名の右側にある下向き矢印を展開し、レコードの種類を検索してから、一覧に表示されるときにその種類を選択します。

   ![&#x200B; 検索ボックス付きレコードタイプページのレコードタイプドロップダウン &#x200B;](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
