---
title: CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、CSV または Excel ファイルから情報をインポートすることで、組織のライフサイクルで必要な作業項目を示すカスタムレコードタイプを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 34%

---

# CSV または Excel ファイルから情報を読み込むことによるレコードタイプの作成

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、CSV または Excel ファイルから情報をインポートすることで、組織のライフサイクルで必要な作業項目を示すカスタムレコードタイプを作成できます。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


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

   * 接続フィールド（使用する環境による）

      * 実稼動環境では、計画レコードまたはWorkfrontおよびAEM Assets オブジェクトへの接続フィールドをマッピングできません

      * <span class="preview"> プレビュー環境では、接続フィールドを Planning レコードにマッピングしてインポートできます。 フィールドをWorkfrontとAEM Assetsにマッピングすることはできません。</span>

   * 接続された Planning レコードまたはWorkfrontおよびAEM Assetsオブジェクトからのフィールドの参照
   * 数式フィールド
   * 作成日、作成者
   * 最終変更日、最終変更者
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

1. （オプション）列ヘッダーの右側にある下向き矢印をクリックして、<span class="preview">**フィールド** タブ </span> で次のいずれかの操作を行います。

   <span class="preview">![ レコードタイプマッピングのインポートボックスの「フィールド」タブ ](assets/field-tab-on-record-type-import-mapping-box.png)</span>

   * いずれかのフィールドの名前を変更する
   * **フィールドタイプ** を変更する
   * フィールド **説明** を更新

1. <span class="preview"> （オプション）「**接続**」タブをクリックして、列内の情報を他のレコードタイプの接続されたフィールドにマッピングします。</span>

   <span class="preview">![ レコードタイプの読み込みマッピングボックスの「接続」タブ ](assets/connection-tab-on-record-type-import-mapping-box.png)</span>

   >[!TIP]
   >
   ><span class="preview"> マッピングできるのは、Workfront Planning に接続されたレコードのフィールドのみです。 WorkfrontまたはAEM Assets Connections からフィールドにマッピングすることはできません。 詳しくは、この記事の「[Excel または CSV ファイルを使用したレコードタイプの読み込みに関する考慮事項 ](#considerations-about-importing-record-types-using-an-excel-or-csv-file) の節を参照してください。</span>

1. （任意）フィールドに関する情報を更新したら、「**保存**」をクリックします。

1. ファイルを読み込む準備が整ったら「**読み込み**」をクリックします。

   次の情報が Workfront Planning にインポートされます。

   * 新しいレコードタイプ
   * 各レコードタイプに関連付けられた新しいフィールド
   * 各レコードタイプに関連付けられた新しいレコード

   レコードタイプページのフィールドとレコードの管理を開始できます。

   Workfront Planning およびワークスペースへのアクセス権を持つすべてのユーザーは、インポートされたレコードタイプとその情報を表示および編集できるようになりました。
