---
title: 別のWorkspaceからの既存のレコードタイプの追加
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planning では、別のワークスペースで作成された既存のレコードタイプを追加できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 233051de458917fd3b40a675914552ccd7d2f474
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 9%

---


# 別のワークスペースからの既存のレコードタイプの追加

{{planning-important-intro}}

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

ワークスペース管理者は、別のワークスペースにあるレコードタイプを、Adobe Workfront Planning で管理するワークスペースに追加できます。

ワークスペースマネージャは、まずレコードタイプをグローバルレコードタイプとして指定してから、既存のレコードタイプとして管理するワークスペースに追加する必要があります。 Workspace管理者は、レコードタイプのクロスワークスペース設定を定義することで、レコードタイプを作成または編集するときにグローバルとして指定できます。

詳しくは、[ レコードタイプのクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

ここでは、既存のレコードタイプからレコードタイプを追加する方法について説明します。

グローバル レコード タイプからワークスペースにレコードを追加する前に、[ ワークスペース間のレコード タイプの概要 ](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md) の記事も参照してください。


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
<ul><li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
または
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## 別のワークスペースから既存のレコードタイプを追加して作成する

>[!NOTE]
>
>少なくとも 1 つの他のプライマリワークスペースに、グローバルに指定されたレコードタイプが 1 つ以上あることを確認してください。
>
>詳しくは、[ レコードタイプのクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

1. レコードタイプを作成するワークスペース（セカンダリワークスペース）に移動します。
1. [ レコードタイプの作成 ](/help/quicksilver/planning/architecture/create-record-types.md) の説明に従ってレコードタイプの作成を開始し、「**既存を追加**」をクリックします。<!--check this - the option might have been renamed in the UI-->

   ![ 別のワークスペースから追加するオプションを使用してレコードタイプを追加するモーダル ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >システム内の他のワークスペースに追加するように設定されたレコードタイプがない場合、「**既存のものを追加**」オプションは表示されません。

1. 「**続行**」をクリックします。
1. **レコードの種類を選択** ボックスで、既存のワークスペースから追加するレコードの種類のカードをクリックし、[**追加**] をクリックします。

   <span class="preview"> レコードタイプが選択したセカンダリワークスペースに追加され、レコードタイプのカードに **グローバルレコードタイプ** アイコン ![ セカンダリワークスペースのグローバルレコードアイコン ](assets/global-icon-secondary-workspace.png) が表示されます。</span>
   <span class="preview"> グローバルレコードタイプアイコンには、セカンダリワークスペースのレコードタイプで表示されたときに、そのレコードタイプが既存のレコードタイプから追加されたことを示す矢印が含まれています。</span>

   次のことが発生します。

   * 既存のグローバルレコードタイプから、次の情報も追加されます。

      * すべての元のフィールド
      * すべてのレコード接続
   * セカンダリワークスペースからレコードタイプの元のワークスペースから追加されたレコードは表示できません。
   * そのワークスペースに対して少なくとも表示権限がある場合、そのワークスペースのレコードタイプの元のワークスペースから追加されたレコードは、元のワークスペースでのみ表示できます。
   * 読み取り専用 **Workspace** フィールドが新規レコードタイプのテーブルビューに追加されます。 フィールドには、各レコードが作成されたワークスペースが表示されます。

     >[!NOTE]
     >
     >新しいレコードタイプの外観、追加の設定、元のフィールドは編集できません。 レコードタイプとすべての元のフィールドおよび設定は、元のワークスペースからのみ編集できます。
     >
1. <span class="preview"> （オプション）グローバルレコードタイプアイコン ![ セカンダリワークスペースのグローバルレコードアイコン ](assets/global-icon-secondary-workspace.png) にポインタを合わせると、レコードタイプが追加された元のワークスペースの名前が表示されます。</span>
1. （オプション）をクリックして、新しく追加したレコードタイプをワークスペース内の任意のセクションにドラッグ&amp;ドロップします。
1. （オプション）新しいレコードの種類のカードまたはページのレコードの種類名の右側にある **詳細** メニューをクリックして、次のいずれかをクリックします。

   * **共有**：セカンダリワークスペースからレコードタイプを共有します。
   * **削除**：セカンダリワークスペースからレコードタイプを削除します。 セカンダリワークスペースからレコードタイプを削除すると、セカンダリワークスペースから追加されたレコードも削除されます。

     セカンダリワークスペースから追加されたビューは削除されません。<!--checking with Lilit - not sure if this is by design??-->

   詳細については、「レコードの種類を削除する」の「グローバル レコードの種類を削除する [ を参照し ](/help/quicksilver/planning/architecture/delete-record-types.md) ください。

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;! – 自動化やリクエストフォームをセカンダリのグローバル RT に追加できるかどうかを Liliit でチェックする？? – ある場合は/これらの記事へのリンクを含むステップを追加する – >







