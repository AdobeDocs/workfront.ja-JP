---
title: レコードページのエクスポート
description: Adobe Workfront Planning からMicrosoft Word ファイルにレコードのプレビューまたは詳細ページをエクスポートできます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: 10fec10e1bb885ac20e1ef9526cfa8a59086d874
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 14%

---

# レコードの詳細のエクスポート

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->


Workfront アカウントを持っていない他のユーザーとのより効率的な共同作業を行うには、レコードの詳細ページをMicrosoft Word ファイルに書き出して共有できます。

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
   <td> <p>ライト以上</p>
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
   <td>   <p>ワークスペースおよびレコードタイプに対する表示以上の権限 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## レコードの詳細の書き出しに関する考慮事項：

* レコードの詳細を次のファイル形式で書き出すことができます。

   * .docx Word
   * .pdf

* 書き出すことができるのは、レコードのページまたはプレビュー領域の「詳細」タブのみです。

* 書き出されたファイルには、サムネールやカバー画像を含むレコードページのレイアウトが保持されます。

## レコードの詳細のエクスポート

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、カードにレコードタイプが表示されます。

1. レコードタイプのカードをクリックします。
レコードタイプのページが開き、そのタイプのすべてのレコードが表示されます。

1. 任意のビューで、レコードの名前をクリックします。

   レコードのプレビューボックスが開きます。

1. （オプション） **新しいタブで開く** アイコン ![ 詳細を新しいタブアイコンで開く ](assets/open-details-in-a-new-tab-icon.png) をクリックして、レコードのページを開きます。

1. 「**詳細**」タブを選択します。 「詳細」タブは、デフォルトで開きます。

1. プレビューまたはレコードのページで、**書き出し** メニュー ![ レコードの詳細ページの書き出しアイコン ](assets/export-icon-in-record-details-page.png) をクリックし、次のいずれかをクリックします。

   * **Microsoft Word**
   * **Adobe PDF**

   Word （.docx）またはPDF ファイルがダウンロードされ、コンピューターに保存されます。

   書き出されるファイルの名前は、レコードのプライマリフィールドです。

   ![ 書き出された word ファイル ](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    ページに表示されず、レコードの詳細領域の「詳細を表示」をクリックした後にのみ表示される追加情報は、書き出されたPDF ファイルには表示されません。 ページに表示される情報のみが書き出されたファイルに表示されます。


1. （オプション）ダウンロードしたファイルに移動して、ファイルを開いて編集するか（Word ファイルの場合）、他のユーザーと共有します。

