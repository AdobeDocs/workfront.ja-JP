---
title: レコードタイプの設定領域の設定
description: レコードタイプを編集ボックスでレコードタイプを編集するだけでなく、設定ページでレコードタイプを編集することもできます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 4674d539-7a16-4d51-a564-e79dc9b4afca
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 11%

---

# レコードタイプの設定エリアの設定

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

レコードタイプがAdobe Workfront Planningに保存された後で、そのレコードタイプの追加設定を行うことができます。

レコードタイプに対して定義する機能に応じて、次のいずれかの操作を行って追加の設定を行うことができます。

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* 編集

  詳しくは、[ レコードタイプの編集](/help/quicksilver/planning/architecture/edit-record-types.md)を参照してください。

* レコードタイプの「設定」ページを設定します。

  この記事では、設定ページを設定してレコードタイプを編集する方法について説明します。

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
<p>任意のワークフローとプランニングパッケージ</p>

<p><b>メモ</b></p>

<p>接続可能なレコードタイプを設定するには：</p>

<ul> 
<li><p>任意のWorkfrontおよびプランニングパッケージ</p></li>
または
<li><p>任意のワークフローパッケージとPlanning PrimeまたはUltimate パッケージ</p></li></ul>

<p>グローバルレコードタイプを設定するには：</p>

<ul> 
<li><p>任意のWorkfront パッケージとPlanning Plus パッケージ</p></li>
または
<li><p>任意のワークフローパッケージとPlanning PrimeまたはUltimate パッケージ</p></li></ul>
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

## 設定ページでのレコードタイプ情報の設定

設定ページで情報を設定することで、レコードタイプのクロスワークスペース機能を定義できます。

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにカーソルを合わせ、レコードタイプカードの右上隅にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**設定**&#x200B;をクリックします

     ![ レコードタイプ カードのその他のメニューオプション ](assets/more-menu-options-from-record-type-card-with-settings-link.png)

     または

   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**設定**&#x200B;をクリックします。

   <!--update screen shot at prod??-->

   ![設定ページのワークスペース間の設定](assets/settings-page-cross-workspace-settings.png)

1. **クロスワークスペース設定** セクションがデフォルトで選択されています。
1. 次のいずれかの設定をオンまたはオフにします。

   * **このレコードタイプを他のワークスペース**&#x200B;に追加して、これがグローバルなレコードタイプであることを示します
   * **他のワークスペース**&#x200B;でこのレコードタイプへの接続を許可して、これが接続可能なレコードタイプであることを示します。

   設定はデフォルトでオフになっています。

   詳細については、[ レコードタイプのクロスワークスペース機能の設定](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)を参照してください
