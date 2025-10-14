---
title: テーブルビューからのレコードのエクスポート
description: テーブル表示のレコードとその情報を CSV ファイルまたは Excel ファイルに書き出すことができます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 10fec10e1bb885ac20e1ef9526cfa8a59086d874
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 11%

---

# テーブルビューからのレコードのエクスポート

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

レコードとその情報をテーブル表示からAdobe Workfront Planning の Excel または CSV ファイルにエクスポートできます。

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
   <td><p> ライト以上 </p>
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
   <td>   <p>ビューに対する表示以上の権限</p>  
   </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## テーブルビューからのレコードのエクスポート

テーブルビューをエクスポートする場合は、以下の点に注意してください。

* Excel ファイルに書き出された情報は、Workfront Planning のテーブルビューに適用されたフィルター、グループ化および並べ替えを保持します。 グループ化は、CSV ファイルには表示されません。

* サムネールとカスタム行カラーは、書き出されたファイルではサポートされません。

* Workfront インターフェイスで表示されたフィールドのみが書き出されます。 非表示のフィールドは書き出されません。

テーブル表示またはレコードタイプから情報をエクスポートするには：

1. レコードタイプのページに移動し、「テーブル表示」タブをクリックします。
1. 次のいずれかの操作を行います。

   * テーブルビュータブの名前にカーソルを合わせ、ビュー名の右側にある **その他** メニュー ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**エクスポート** をクリックしてください。

   ![&#x200B; ビューの詳細メニュー &#x200B;](assets/view-more-menu-with-duplicate-option.png)

   * **共有**/**現在のビューを書き出し** をクリックします。 このオプションは、テーブルビューを表示する場合にのみ使用できます。

   ![&#x200B; レコードタイプとビュー共有オプションを含む共有ボタン &#x200B;](assets/share-button-with-record-type-and-view-sharing-options.png)

1. 次のいずれかの形式を選択します。

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >画面に別のビューを表示している場合、テーブルビューから情報をエクスポートすることはできません。 「詳細」 メニューの「エクスポート」 オプションにアクセスするには、エクスポートするテーブルビューを表示する必要があります。

   ファイルがコンピューターにダウンロードされます。

1. （オプション）コンピューターのダウンロードフォルダーに移動し、ダウンロードしたファイルを見つけます。

   書き出されるファイルの名前は、次の形式に従います。

   `Name of the view - name of the record type`

   例えば、キャンペーン レコードタイプのテーブル ビューでは、`Table view - Campaigns` という名前のファイルを生成します。

   ファイルには次の情報が表示されます。

   * Excel ファイルでは、列ヘッダーが黒でハイライト表示されます
   * Workfront インターフェイスに表示されるすべてのフィールド（同じ条件で並べ替えおよびフィルタリングされます）
   * グループ化は Excel ファイルに保持されます

   書き出したファイルを他のユーザーと共有したり、任意の通信に添付したりできるようになりました。

</div>
