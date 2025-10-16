---
title: レコードへのカバー画像の追加
description: レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 11%

---


# レコードへのカバー画像の追加

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。

レコードの編集方法については、「[&#x200B; レコードの編集 &#x200B;](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

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
<ul> 
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
または
<li><p>任意のワークフローおよび任意の計画パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
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
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## レコードページの表紙画像に関する考慮事項

表紙画像を追加して、レコードのページをパーソナライズできます。

次の点に注意してください。

* カバー画像は、1 つのレコードに固有で、同じタイプのすべてのレコードには適用されません。
* カバー画像として追加できるのは画像ファイルのみです。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 任意のビューのレコードプレビューまたはレコードページから、カバー画像を個々のレコードに追加できます。
* レコード ビューからカバー画像を追加することはできません。
* Workfrontは、レコードを作成するたびに、カバー画像を自動的にアップロードします。 この画像は後で変更できます。

## レコードへのカバー画像の追加

レコードのプレビューまたはページの上部にカバー画像を追加して、レコードをパーソナライズできます。

{{step1-to-planning}}

1. レコードをパーソナライズするワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。

   ワークスペースが開き、レコードタイプが表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. 任意の種類のビューから、レコードをクリックします

   または

   テーブルビューで、最初の列の **詳細を開く** アイコン ![&#x200B; 詳細を開くアイコン &#x200B;](assets/open-details-icon-in-table-name-field.png) をクリックします。

   レコードのプレビューがビューで開きます。

   ![&#x200B; 詳細プレビューボックス &#x200B;](assets/details-box.png)


1. （オプション）レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![&#x200B; 新しいタブで開く &#x200B;](assets/open-details-in-a-new-tab-icon.png) アイコン <!--check the icon; they are changing it--> 新しいタブでレコードのページを開く）をクリックします。

   レコードページが開きます。

   ![&#x200B; 詳細ページ &#x200B;](assets/details-page.png)

1. レコードのプレビューまたは詳細ページで、レコード名の上のスペースにマウスポインターを置いて、「**カバーを追加**」をクリックします。

   または

   既存のカバー画像にポインタを合わせ、**詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**アップロード** をクリックしてください。 <!--check the casing here; I logged a bug for this-->
**レコードカバー** ボックスが **アップロード** タブで開きます。

   ![&#x200B; アップロード用のレコードカバーボックス &#x200B;](assets/record-cover-box-for-upload.png)

1. **画像を参照** をクリックし、コンピューター上の画像を参照して選択して追加します。

1. （任意）保存前に画像を削除するには、**新しい画像をアップロード** アイコン ![&#x200B; 新しい画像をアップロード アイコン &#x200B;](assets/upload-new-image-icon.png) をクリックして、新しい画像をアップロードします。

1. （オプション）「**ギャラリー**」タブをクリックして、画像ギャラリー内の画像をクリックします。 画像ギャラリーは変更できません。

   ![&#x200B; ギャラリー用カバーボックスの記録 &#x200B;](assets/record-cover-box-for-gallery.png)

1. **画像を使用** をクリックします。

   画像はレコードのプレビューページまたは詳細ページの上部にアップロードされ、変更は自動的に保存されます。

   ![&#x200B; 表紙付きレコードページ &#x200B;](assets/record-page-with-cover-image.png)

1. （オプション）画像の上にマウスポインターを置き、カバー画像の右下隅にある **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、次のいずれかの操作を行います。

   * カバー画像を置き換える場合は **アップロード** をクリックし、手順 6 を繰り返して新しい画像をアップロードして保存します。
   * **再配置** をクリックし、**再配置** ツール ![&#x200B; 再配置ツールアイコン &#x200B;](assets/reposition-tool-icon.png) を使用してカバー画像を中央に配置し、完了したら **保存** をクリックします。
   * **削除** をクリックして、カバー画像を削除します。

   Workfront では、変更を自動的に保存します。
