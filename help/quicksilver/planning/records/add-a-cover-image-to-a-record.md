---
title: レコードへのカバー画像の追加
description: レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 22%

---


# レコードへのカバー画像の追加

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードの編集時に、Adobe Workfront Planning のレコード・ページに表紙を追加することで、レコードをパーソナライズできます。

レコードの編集方法については、「[ レコードの編集 ](/help/quicksilver/planning/records/edit-records.md)」を参照してください。

レコードの作成と編集を開始する前に、レコードタイプを作成する必要があります。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

## アクセス要件

+++ 展開してアクセス要件を表示します…

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
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
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
   <td>   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> への投稿権限または上位権限  </p>  
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

   テーブルビューで、最初の列の **詳細を開く** アイコン ![ 詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックします。

   レコードのプレビューがビューで開きます。

   ![ 詳細プレビューボックス ](assets/details-box.png)


1. （オプション）レコードプレビューの右上隅にある **新しいタブで開く** アイコン ![ 新しいタブで開く ](assets/open-details-in-a-new-tab-icon.png) アイコン <!--check the icon; they are changing it--> 新しいタブでレコードのページを開く）をクリックします。

   レコードページが開きます。

   ![ 詳細ページ ](assets/details-page.png)

1. レコードのプレビューまたは詳細ページで、レコード名の上のスペースにマウスポインターを置いて、「**カバーを追加**」をクリックします。

   または

   既存のカバー画像にポインタを合わせ、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**アップロード** をクリックしてください。 <!--check the casing here; I logged a bug for this-->
**レコードカバー** ボックスが **アップロード** タブで開きます。

   ![ アップロード用のレコードカバーボックス ](assets/record-cover-box-for-upload.png)

1. **画像を参照** をクリックし、コンピューター上の画像を参照して選択して追加します。

1. （任意）保存前に画像を削除するには、**新しい画像をアップロード** アイコン ![ 新しい画像をアップロード アイコン ](assets/upload-new-image-icon.png) をクリックして、新しい画像をアップロードします。

1. （オプション）「**ギャラリー**」タブをクリックして、画像ギャラリー内の画像をクリックします。 画像ギャラリーは変更できません。

   ![ ギャラリー用カバーボックスの記録 ](assets/record-cover-box-for-gallery.png)

1. **画像を使用** をクリックします。

   画像はレコードのプレビューページまたは詳細ページの上部にアップロードされ、変更は自動的に保存されます。

   ![ 表紙付きレコードページ ](assets/record-page-with-cover-image.png)

1. （オプション）画像の上にマウスポインターを置き、カバー画像の右下隅にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、次のいずれかの操作を行います。

   * カバー画像を置き換える場合は **アップロード** をクリックし、手順 6 を繰り返して新しい画像をアップロードして保存します。
   * **再配置** をクリックし、**再配置** ツール ![ 再配置ツールアイコン ](assets/reposition-tool-icon.png) を使用してカバー画像を中央に配置し、完了したら **保存** をクリックします。
   * **削除** をクリックして、カバー画像を削除します。

   Workfront では、変更を自動的に保存します。
