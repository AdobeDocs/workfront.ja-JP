---
title: クロスワークスペースのレコードタイプを追加
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、既存のレコードタイプを別のワークスペースからインポートできます。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 19%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# ワークスペース間のレコードタイプを追加

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

ワークスペースマネージャーは、既存のレコードタイプを別のワークスペースに読み込んだり追加したりできます。

ワークスペースマネージャーがレコードタイプを他のワークスペースに読み込む前に、レコードタイプを一元的なものとして指定する必要があります。

ワークスペース間の設定を定義する際に、レコードタイプを作成または編集する際に、レコードタイプを一元的として指定できます。

詳しくは、[ レコードタイプのクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

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
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++   

## 一元化されたレコードタイプの概要

別のワークスペースから既存のレコードタイプを追加する際の考慮事項

* 別のワークスペースに追加するように設定されたレコードタイプがない場合、レコードタイプの作成時に、別のワークスペースからインポートするオプションは表示されません。<!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* 別のワークスペースからレコードタイプを追加すると、既存のレコードタイプから次の情報も追加されます。

   * フィールド
   * レコード
   * レコード接続

* フィールドを含むレコードタイプは、元のワークスペースでのみ編集できます。 追加されたワークスペースから編集することはできません。

## 既存のレコードタイプからレコードタイプを作成する

1. [ レコードタイプの作成 ](/help/quicksilver/planning/architecture/create-record-types.md) の説明に従ってレコードタイプの作成を開始し、「**既存を追加**」をクリックします。<!--check this - the option might have been renamed in the UI-->

   ![ 別のワークスペースから読み込むオプションを持つレコードタイプを追加するためのモーダル ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. 「**続行**」をクリックします。
1. **レコードタイプを選択** ボックスで、既存のワークスペースから追加するレコードタイプのカードをクリックし、**追加** をクリックします。

   レコードタイプが選択したワークスペースに追加され、次の処理が行われます。

   * **ワークスペース間レコードタイプ** アイコン ![ ワークスペース間接続アイコン ](assets/global-icon.png) が、読み込まれたレコードタイプのカードに追加されます。
   * 読み取り専用 **Workspace** フィールドが、読み込まれたレコードタイプに追加されます。 フィールドには、各レコードが作成されたワークスペースが表示されます。

     >[!NOTE]
     >
     >* 読み込んだレコードタイプやそのフィールドは編集できません。 レコードタイプとそのフィールドは、元のワークスペースから編集できます。

1. （オプション）読み込まれたレコードタイプのカードまたはページ上のレコードタイプの名前の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックしてから、**削除** をクリックします。
1. （条件付き）表示されたフィールドに **削除** と入力し、「**完全に削除**」をクリックします。

   読み込んだレコードタイプが、選択したワークスペースから削除されます。 元のレコードタイプとそのフィールドは、元のワークスペースに残ります。

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



