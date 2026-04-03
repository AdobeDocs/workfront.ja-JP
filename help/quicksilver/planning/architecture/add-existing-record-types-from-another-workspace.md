---
title: 別のWorkspaceから既存のレコードタイプを追加する
description: レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。Workfront Planningでは、別のワークスペースで作成された既存のレコードタイプを追加できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 10%

---


# 別のワークスペースから既存のレコードタイプを追加

{{planning-important-intro}}

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

ワークスペース管理者は、別のワークスペースにあるレコードタイプを、Adobe Workfront Planningで管理するワークスペースに追加できます。

ワークスペースマネージャーは、既存のレコードタイプとして管理するワークスペースにレコードタイプを追加する前に、最初にレコードタイプをグローバルレコードタイプとして指定する必要があります。 Workspaceの管理者は、レコードタイプのクロスワークスペース設定を定義することで、レコードタイプを作成または編集する際にグローバルとして指定できます。

詳しくは、[ レコードタイプのクロスワークスペース機能の設定](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)を参照してください。

この記事では、既存のレコードタイプからレコードタイプを追加する方法について説明します。

グローバルレコードタイプからワークスペースにレコードを追加する前に、記事[ クロスワークスペースレコードタイプの概要](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)も参照してください。


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
<ul><li><p>任意のWorkfront パッケージとPlanning Plus パッケージ</p></li>
または
<li><p>任意のワークフローとプランニング PrimeまたはUltimate パッケージ</p></p></li></ul>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

<!--
Old:
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
</table>
-->

## 別のワークスペースから既存のレコードタイプを追加して、レコードタイプを作成する

>[!NOTE]
>
>他の少なくとも1つのプライマリワークスペースに、少なくとも1つのレコードタイプがグローバルに指定されていることを確認します。
>
>詳しくは、[ レコードタイプのクロスワークスペース機能の設定](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)を参照してください。

1. レコードタイプ（セカンダリワークスペース）を作成するワークスペースに移動します。
1. 記事[ レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)の説明に従ってレコードタイプの作成を開始し、**既存の**&#x200B;を追加をクリックします。<!--check this - the option might have been renamed in the UI-->

   ![別のワークスペースから追加するオプションを含むレコードタイプを追加するモーダル ](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >システム内の他のワークスペースに追加するように設定されたレコードタイプがない場合、「**既存の**&#x200B;を追加」オプションは表示されません。

1. 「**続行**」をクリックします。
1. **レコードタイプを選択** ボックスで、既存のワークスペースから追加するレコードタイプのカードをクリックし、**追加**&#x200B;をクリックします。

   <span class="preview"> レコードタイプが選択したセカンダリワークスペースに追加され、セカンダリワークスペースの&#x200B;**グローバルレコードタイプ** アイコン ![ グローバルレコードアイコン ](assets/global-icon-secondary-workspace.png)がレコードタイプのカードに表示されます。</span>
   <span class="preview"> グローバルなレコードタイプ アイコンには、セカンダリワークスペースのレコードタイプに表示される矢印が含まれており、既存のレコードタイプからレコードタイプが追加されたことを示します。</span>

   次のことが発生します。

   * 次の情報も、既存のグローバルレコードタイプから追加されます。

      * すべてのオリジナルフィールド
      * すべてのレコードの接続
   * セカンダリワークスペースからレコードタイプの元のワークスペースから追加されたレコードを表示することはできません。
   * 少なくともそのワークスペースに対する表示権限がある場合は、元のワークスペースでのみ、そのワークスペース内のレコードタイプの元のワークスペースから追加されたレコードを表示できます。
   * 読み取り専用の&#x200B;**Workspace** フィールドが、新しいレコードタイプのテーブルビューに追加されます。 このフィールドには、各レコードが作成されたワークスペースが表示されます。

     >[!NOTE]
     >
     >新しいレコードタイプの外観、追加設定、元のフィールドは編集できません。 レコードタイプとそのすべての元のフィールドと設定は、元のワークスペースからのみ編集できます。
     >

1. <span class="preview"> （オプション）セカンダリワークスペース ![のグローバルレコードタイプアイコン ](assets/global-icon-secondary-workspace.png) グローバルレコードアイコンにカーソルを合わせると、レコードタイプが追加された元のワークスペースの名前が表示されます。</span>
1. （オプション）をクリックし、新しく追加したレコードタイプをワークスペース内の任意のセクションにドラッグ&amp;ドロップします。
1. （オプション）新しいレコードタイプのカードまたはページのレコードタイプ名の右側にある&#x200B;**More** メニューをクリックし、次のいずれかをクリックします。

   * **共有**&#x200B;して、セカンダリワークスペースからレコードタイプを共有します。
   * **削除**&#x200B;して、セカンダリワークスペースからレコードタイプを削除します。 セカンダリワークスペースからレコードタイプを削除すると、セカンダリワークスペースから追加されたレコードも削除されます。

     セカンダリワークスペースから追加されたビューは削除されません。<!--checking with Lilit - not sure if this is by design??-->

   詳しくは、[ レコードタイプの削除](/help/quicksilver/planning/architecture/delete-record-types.md)の「グローバルレコードタイプの削除」の節を参照してください。

<!--
This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;! – 自動化を追加したり、セカンダリグローバル RT?？にフォームをリクエストしたりできるかどうかをLilitでチェックします – はい/はい場合は、これらの記事へのリンクを含むステップを追加します – >







