---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals での情報のフィルタリング
description: 自分または他のユーザーが Adobe Workfront Goals に追加した目標を表示できます。目標の作成について詳しくは、「Adobe Workfront Goals での目標の作成」を参照してください。目標を表示する際に、Workfront Goals で情報をフィルタリングして、重要な目標のみを表示できます。
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: ht
source-wordcount: '1342'
ht-degree: 100%

---

# Adobe Workfront Goals での情報のフィルタリング

自分または他のユーザーが Adobe Workfront Goals に追加した目標を表示できます。目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。目標を表示する際に、Workfront Goals で情報をフィルタリングして、重要な目標のみを表示できます。

## アクセス要件

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> <p>詳しくは、<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>Goals に対する表示以上のアクセス権</p> <p><b>メモ</b>

<p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront Goals へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標の表示以上の権限</p> 
     <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの Workfront Goals 領域を含んだレイアウトテンプレート。

## Workfront Goals のフィルターの概要

>[!NOTE]
>
>適切な目標を効率的に見つけて焦点を当てるには、Workfront Goals のフィルターを使用することをお勧めします。これにより、重要な目標の管理を開始する前に、正しい情報を表示できます。デフォルトでは、Workfront Goals にはシステム内のすべての目標が表示されます。

Workfront の Goals エリアの次のセクションで目標を見つけてフィルタリングできます。

* 目標リスト
* グラフ
* 目標の整合性

Goals エリアのセクションについて詳しくは、[Adobe Workfront Goals セクションの概要](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)を参照してください。

>[!IMPORTANT]
>
>あるセクションに対してフィルターを設定すると、Workfront Goals の別のセクションに移動してもそのフィルターは保持されます。

Workfront Goals でフィルターを使用する際は、次の点を考慮してください。

* フィルターは、保存せずに作成して適用することも、保存して後で再利用することもできます。

  次のシナリオが存在します。

   * フィルターを保存すると、Workfront Goals にログインするたびにデフォルトのフィルターになります。
   * 保存せずにフィルターを適用した場合は、ページを更新すると元のリストに戻すことができます。

* 作成したフィルターは表示と適用のみ可能です。他のユーザーが作成したフィルターは、そのユーザーにのみ表示されます。
* 作成したフィルターを他のユーザーと共有することはできません。

## Workfront Goals でのクイックフィルターの適用

目標のリストでクイックフィルターを使用すると、重要なアイテムだけを見つけることができます。クイックフィルターは保存できず、永続的ではありません。ページを更新すると、Workfront はクイックフィルターの結果をクリアします。

詳しくは、[クイックフィルターをリストに適用する](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)を参照してください。

## Workfront Goals でのフィルターの作成と適用

フィルターの作成手順は、Workfront Goals のどのセクションでも同じです。

一からフィルターを作成することも、組み込みのフィルターのいずれかを編集することもできます。

1. Workfront Goals に移動します。

   Workfront Goals へのアクセスについて詳しくは、[Adobe Workfront Goals へのアクセスと目標のオープン](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)を参照してください。

   デフォルトでは「目標リスト」セクションが表示されます。

1. リストの右上隅にある「**フィルター**」をクリックします。

   ![](assets/filter-icon-and-label.png)

   デフォルトでは、Workfront はシステム内のすべての目標を表示する「**すべて**」のフィルターを適用します。

   >[!TIP]
   >
   >「すべて」のフィルターを編集または削除することはできません。

1. 次のいずれかの操作を行います。

   * 次のいずれかの定義済みフィルターをクリックして、以下の所有者に対する目標のみを表示します。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>すべて</td> 
        <td> <p>誰が作成したか、どの期間であるか、または所有者が誰であるかに関係なく、システム内のすべての目標。これはデフォルトのフィルターで、編集できません。 </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>個人用</td> 
        <td>所有者の目標。</td> 
       </tr> 
       <tr> 
        <td>マイチーム</td> 
        <td> <p>いずれかのチームが所有者として選択された目標。 </p> <p><b>ヒント</b>

     ユーザーがどのチームにも割り当てられていない場合は、目標は表示されません。 </p> </td>
     </tr> 
       <tr> 
        <td>マイグループ</td> 
        <td>いずれかのグループが所有者として選択された目標。 </td> 
       </tr> 
       <tr> 
        <td>会社</td> 
        <td> <p>組織に関連付けられた目標。 </p> <p><b>ヒント</b>
        <p>Adobe Workfront Goals では、会社情報フィルターに、組織が所有者として選択されている目標が表示されます。 </p> <p>このフィールドを使用して会社を検索することはできません。デフォルトでは、Workfront インスタンスの所有者である組織のみが選択されます。 </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * フィルターの名前にポインタを合わせて、その名前の横にある&#x200B;**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックしてカスタマイズし、ユーザー、チーム、グループの特定の名前、または組織の名前を追加します。

   * 「**新規フィルター**」をクリックして新しいフィルターを作成し、次のオプションのいずれかを選択して、新しいフィルターをカスタマイズします。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">期間</td> 
        <td>ドロップダウンメニューで期間を選択します。複数の期間を選択できます。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">ステータス</td> 
        <td> <p>次のオプションから、ドロップダウンメニューでステータスを選択します。</p> 
         <ul> 
          <li> <p>アクティブ</p> </li> 
          <li> <p>ドラフト</p> </li> 
          <li> <p>非アクティブ</p> </li> 
          <li> <p>クローズ</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">進捗状況</td> 
        <td> <p>次のオプションから、ドロップダウンメニューで進捗状況を選択します。 </p> 
         <ul> 
          <li> <p>トラブル発生中</p> </li> 
          <li> <p>リスクあり</p> </li> 
          <li> <p>目標どおり</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">所有者</td> 
        <td> <p>所有者の名前を入力し、リストに表示されたら選択します。 </p> <p>ユーザー名、チーム名、グループ名または組織名を入力するか、事前定義済みのオプションから選択できます。 </p> <p>次の定義済みフィルターオプションは、常に、現在ログインしているユーザーを指します。 </p> 
         <ul> 
          <li> <p><strong>私</strong>：自分が所有者である目標を表示します。</p> </li> 
          <li> <p><strong>マイホームチーム</strong>および<strong>すべてのマイチーム</strong>：ホームチームまたはチームのいずれかが所有者に指定されている目標を表示します。 </p> <p>ヒント：どのチームにも割り当てられていない場合は、目標は表示されません。 </p> </li> 
          <li> <p><strong>マイホームグループ</strong>および <strong>すべてのマイグループ</strong>：自分のホームグループまたは任意のグループが所有者として指定されている目標を表示します。</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. （オプション）フィルターボックスの右下隅にある「**リセット**」をクリックして、選択したすべてのフィールドを消去し、最初からフィルターの作成を開始します。
1. （オプション）「**適用**」をクリックして、保存せずにフィルターを適用します。

   フィルターがフィルタービルダーの&#x200B;**未保存**&#x200B;エリアに&#x200B;**新規フィルター**&#x200B;として表示されます。

   未保存のフィルターの名前は変更できません。

   未保存のフィルターは、次回 Workfront からログアウトして再度ログインすると、目標エリアから削除されます。

   >[!TIP]
   >
   >一度に 1 つの未保存の新しいフィルターのみを使用できます。

1. 「**保存**」をクリックして後で使用するためにフィルターを保存し、「**フィルター名を追加**」フィールドにフィールドの名前を追加し、「**完了**」をクリックします。

   これにより、フィルターはフィルタービルダーの「**保存済み**」セクションに保存されます。このフィルターは今後使用できます。

   最後に保存および適用したフィルターは、次回 Workfront にログインするとデフォルトで表示されます

1. （オプション）**新規フィルター**&#x200B;の横にある&#x200B;**左矢印**&#x200B;をクリックしてフィルタービルダーを終了し、フィルターのリストに戻ります。
1. （オプション）カスタムフィルターの名前の上にポインタを合わせて、**その他**&#x200B;メニュー、「**削除**」、「**削除**」の順にクリックします。これにより、フィルターが削除され、復元できなくなります。

   >[!TIP]
   >
   >定義済みフィルターは削除できません。

1. フィルタービルダーの右上隅にある **X アイコン**&#x200B;をクリックして、フィルタービルダーを閉じます。

   現在適用されているフィルターの名前が、フィルターアイコンの右側の目標リストの右上隅に表示されます。

   目標のリストは、フィルター条件で絞り込まれます。

1. （オプションおよび条件付き）「目標の整合性」セクションで目標を表示して、フィルターした目標を表示する場合は「**表示する**」をクリックします。

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   フィルター名は、無視されていることを示すために黄色でアウトライン表示されます。

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. （オプションおよび条件付き）「**フィルターを再適用**」をクリックして、前の手順で表示した項目を除外し、フィルターを適用します。


