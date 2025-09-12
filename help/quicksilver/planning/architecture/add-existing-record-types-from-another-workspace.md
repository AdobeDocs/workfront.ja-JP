---
title: 別のWorkspaceからの既存のレコードタイプの追加
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、別のワークスペースで作成された既存のレコードタイプを追加できます。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 11%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 別のワークスペースからの既存のレコードタイプの追加

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

ワークスペース管理者は、ワークスペースにあるレコードタイプを、Adobe Workfront Planning で管理するワークスペースに追加できます。

ワークスペースマネージャーがレコードタイプを既存のレコードタイプとして他のワークスペースに追加する前に、まずレコードタイプを一元的なものとして指定する必要があります。

ワークスペース間の設定を定義する際に、レコードタイプを作成または編集する際に、レコードタイプを一元的として指定できます。

詳しくは、[ レコードタイプのクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

一元化されたレコードタイプからワークスペースにレコードを追加する前に、[ ワークスペース間のレコードタイプの概要 ](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) を参照してください。

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
<ul><li><p>任意のWorkfront パッケージ</p></li>
And
<li><p>Planning Plus パッケージ</p></li></ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

## 既存のレコードタイプからレコードタイプを作成する

1. [ レコードタイプの作成 ](/help/quicksilver/planning/architecture/create-record-types.md) の説明に従ってレコードタイプの作成を開始し、「**既存を追加**」をクリックします。<!--check this - the option might have been renamed in the UI-->

   ![ 別のワークスペースから追加するオプションを使用してレコードタイプを追加するモーダル ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. 「**続行**」をクリックします。
1. **レコードタイプを選択** ボックスで、既存のワークスペースから追加するレコードタイプのカードをクリックし、**追加** をクリックします。

   レコードタイプが、選択したワークスペースに追加されます。

   >[!TIP]
   >
   >別のワークスペースに追加するように設定されたレコードタイプがない場合、レコードタイプの作成時に、別のワークスペースから追加するオプションは表示されません。

   次のことが発生します。

   * 既存の一元化されたレコードタイプから、次の情報も追加されます。

      * すべての元のフィールド
      * すべてのレコード接続
   * 他のワークスペースから追加されたレコードを表示できるのは、そのワークスペースに対して少なくとも表示権限を持っている場合のみです。
   * **一元的レコードタイプ** アイコン ![ 一元的レコードタイプアイコン ](assets/global-icon.png) が、新しいレコードタイプのカードに追加されます。
   * 読み取り専用 **Workspace** フィールドが新規レコードタイプのテーブルビューに追加されます。 フィールドには、各レコードが作成されたワークスペースが表示されます。

     >[!NOTE]
     >
     >* 新しいレコードタイプの外観、詳細設定、元のフィールドは編集できません。 レコードタイプとすべての元のフィールドおよび設定は、元のワークスペースからのみ編集できます。

1. （オプション）をクリックして、新しく追加したレコードタイプをワークスペース内の任意のセクションにドラッグ&amp;ドロップします。

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

1. （省略可能）新しいレコードの種類のカードの **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックするか、ページ上のレコードの種類の名前の右側をクリックして、[**削除**] をクリックします。
1. （条件付き）表示されたフィールドに **削除** と入力し、「**完全に削除**」をクリックします。

   次のことが発生します。

   * 一元化されたレコードタイプから作成されたレコードタイプは、選択したワークスペースから削除されます。
   * 元のレコードタイプとそのフィールドは、元のワークスペースに残ります。
   * レコードタイプは、追加された他のすべてのワークスペースに残ります。
   * 現在のワークスペースからレコードタイプに追加されたレコードが削除されます。 一元化されたレコードタイプが追加された追加のワークスペースから追加された他のすべてのレコードは、保持されます。





