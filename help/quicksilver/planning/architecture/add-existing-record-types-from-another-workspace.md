---
title: 別のWorkspaceからの既存のレコードタイプの追加
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、別のワークスペースで作成された既存のレコードタイプを追加できます。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 8%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 別のワークスペースからの既存のレコードタイプの追加

{{planning-important-intro}}

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

ワークスペース管理者は、別のワークスペースにあるレコードタイプを、Adobe Workfront Planning で管理するワークスペースに追加できます。

ワークスペースマネージャは、まずレコードタイプをグローバルレコードタイプとして指定してから、既存のレコードタイプとして管理するワークスペースに追加する必要があります。 Workspace管理者は、レコードタイプのクロスワークスペース設定を定義することで、レコードタイプを作成または編集するときにグローバルとして指定できます。

詳しくは、[&#x200B; レコードタイプのクロスワークスペース機能の設定 &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

この記事では、既存のレコードタイプからレコードタイプを追加する方法と、不要になったレコードタイプを削除する方法について説明します。

グローバル レコード タイプからワークスペースにレコードを追加する前に、[&#x200B; ワークスペース間のレコード タイプの概要 &#x200B;](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) の記事も参照してください。


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
<p>And</p>
<li><p>接続可能なレコードタイプを作成する任意の Planning パッケージ</p></li>
<li><p>グローバル レコード タイプを作成するための Planning Plus パッケージ</p></li>
</ul>
または：
<ul><li><p>PrimeまたはUltimateのワークフローパッケージ</p> </li>
And
<li><p>Planning PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプに対する権限の管理 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

## 別のワークスペースから既存のレコードタイプを追加して作成する

>[!NOTE]
>
>少なくとも 1 つの他のワークスペースに、グローバルに指定されたレコードタイプが 1 つ以上あることを確認してください。

1. [&#x200B; レコードタイプの作成 &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) の説明に従ってレコードタイプの作成を開始し、「**既存を追加**」をクリックします。<!--check this - the option might have been renamed in the UI-->

   ![&#x200B; 別のワークスペースから追加するオプションを使用してレコードタイプを追加するモーダル &#x200B;](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >システム内の他のワークスペースに追加するように設定されたレコードタイプがない場合、「**既存のものを追加**」オプションは表示されません。

1. 「**続行**」をクリックします。
1. **レコードの種類を選択** ボックスで、既存のワークスペースから追加するレコードの種類のカードをクリックし、[**追加**] をクリックします。

   レコードタイプが選択したワークスペースに追加され、レコードタイプのカードに **グローバルレコードタイプ** アイコン ![](assets/global-icon.png) 表示されます。

   次のことが発生します。

   * 既存のグローバルレコードタイプから、次の情報も追加されます。

      * すべての元のフィールド
      * すべてのレコード接続
   * 同じグローバル レコード タイプを使用する他のワークスペースから追加されたレコードを表示できるのは、それらのワークスペースに対して少なくとも表示権限を持っている場合のみです。
   * 読み取り専用 **Workspace** フィールドが新規レコードタイプのテーブルビューに追加されます。 フィールドには、各レコードが作成されたワークスペースが表示されます。

     >[!NOTE]
     >
     >新しいレコードタイプの外観、追加の設定、元のフィールドは編集できません。 レコードタイプとすべての元のフィールドおよび設定は、元のワークスペースからのみ編集できます。

1. （オプション）をクリックして、新しく追加したレコードタイプをワークスペース内の任意のセクションにドラッグ&amp;ドロップします。

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;! – 自動化やリクエストフォームをセカンダリのグローバル RT に追加できるかどうかを Liliit でチェックする？? – ある場合は/これらの記事へのリンクを含むステップを追加する – >

## グローバルレコードタイプのセカンダリワークスペースからの削除

追加したレコードタイプは、不要になったら別のワークスペースから削除できます。 削除すると、セカンダリワークスペースからのみ削除されます。

グローバルレコードタイプをセカンダリワークスペースから削除すると、次の項目も削除されます。

* セカンダリワークスペースから追加されたレコード。
* セカンダリワークスペースから追加されたフィールド。

セカンダリ ワークスペースから削除されたグローバル レコード タイプはリカバリできません。

元のレコードタイプは、元のワークスペースと、それが追加された他のワークスペースに残ります。

セカンダリワークスペースからグローバルレコードタイプを削除するには：

1. セカンダリワークスペースのグローバルレコードタイプに移動します。

1. （オプション）レコードタイプのカードまたはページ上のレコードタイプの名前の右側にある **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックし、**削除** をクリックします。
1. （条件付き）表示されたフィールドに **削除** と入力し、「**完全に削除**」をクリックします。

   ![&#x200B; セカンダリ グローバル レコード タイプの削除の確認ボックス &#x200B;](assets/delete-secondary-global-record-type.png)

   次のことが発生します。

   * グローバル レコード タイプから作成されたレコード タイプは、選択したワークスペースから削除されます。
   * 元のレコードタイプとそのフィールドは、元のワークスペースに残ります。
   * レコードタイプは、追加された他のすべてのワークスペースに残ります。
   * 現在のワークスペースからレコードタイプに追加されたレコードとフィールドが削除されます。 グローバルレコードタイプが追加された追加のワークスペースから追加された他のすべてのレコードは、保持されます。 フィールドは、追加先のワークスペースに保持されます。





