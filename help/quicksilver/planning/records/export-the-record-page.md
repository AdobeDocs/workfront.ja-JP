---
title: レコードページのエクスポート
description: レコードのプレビューまたは詳細ページを Word にエクスポートできます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 29%

---

# レコードの詳細のエクスポート

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、[2023年第 4 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)を参照してください。</span>


Workfront アカウントを持っていない他のユーザーとのより効率的な共同作業を行うために、レコードの詳細をファイルに書き出して共有できます。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

Workfront Planning にアクセスするには、次のものが必要です：

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
   <td role="rowheader"><p>Adobe Workfront計画*</p></td> 
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
   <td> <p>標準</p>
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
   <td>   <p>ワークスペースに対する表示またはそれ以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## レコードの詳細の書き出しに関する考慮事項：

* レコードの詳細を次のファイル形式で書き出すことができます。

   * .docx Word
   * <span class="preview">.pdf</span>

* レコードのページの「詳細」タブを書き出すことができます。 「接続」タブは書き出せません。

* 書き出されたファイルには、サムネールやカバー画像を含むレコードページのレイアウトが保持されます。

## レコードの詳細のエクスポート

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、カードにレコードタイプが表示されます。

1. レコードタイプのカードをクリックします。
レコードタイプのページが開き、そのタイプのすべてのレコードが表示されます。

1. 任意のビューで、レコードの名前をクリックします。

   レコードのプレビューボックスが開きます。

1. （オプション） **新しいタブで開く** アイコン ![](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを開きます。

1. 「**詳細**」タブを選択します。 「詳細」タブは、デフォルトで開きます。

1. プレビューまたはレコードのページ ![](assets/export-icon-in-record-details-page.png) ある **エクスポート** アイコンをクリックし、次のいずれかをクリックします。

   * **Microsoft Word**
   * <span class="preview">**Adobe PDF**</span>

   Word （.docx） <span class="preview"> またはPDF</span> ファイルがダウンロードされ、コンピューターに保存されます。

   書き出されるファイルの名前は、レコードのプライマリフィールドです。

   ![](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    ページに表示されず、「詳細」タブで「詳細を表示」をクリックした後にのみ表示される追加情報は、エクスポートされたPDFファイルには表示されません。 ページに表示される情報のみが書き出されたファイルに表示されます。


1. （オプション）ダウンロードしたファイルに移動して、ファイルを開いて編集するか（Word ファイルの場合）、他のユーザーと共有します。

