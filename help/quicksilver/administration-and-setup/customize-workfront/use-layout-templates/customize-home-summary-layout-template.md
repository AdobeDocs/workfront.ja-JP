---
title: レイアウトテンプレートを使用してホームと概要をカスタマイズする
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートを使用して、ホームおよびサマリでタスクやイシューをクリックしたときにユーザーに表示する内容を設定できます。 以下の手順を使用して行った各設定は、同じ方法でホーム領域と Summary パネルに影響します。 これらのカスタマイズは、ドキュメントの概要パネルには適用されません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 2%

---

# レイアウトテンプレートを使用してホームと概要をカスタマイズする

レイアウトテンプレートを使用して、ホームおよびサマリでタスクやイシューをクリックしたときにユーザーに表示する内容を設定できます。 以下の手順を使用して行った各設定は、同じ方法でホーム領域と Summary パネルに影響します。 これらのカスタマイズは、ドキュメントの概要パネルには適用されません。

以下を設定できます。

* 「詳細」領域でタスクまたはイシューに対して表示されるフィールドと順序
* 選択したタスクまたはイシューの更新、ログに記録された時間、添付されたドキュメント、タイムスタンプを表示するかどうか

ユーザーが割り当てられているプロジェクトの承認、ドキュメントの承認、ドキュメントのバージョンの承認をクリックしたときに、ホーム領域に表示されるフィールドをカスタマイズすることもできます。

ホーム領域については、 [ホーム領域を使用](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). 概要パネルについて詳しくは、 [概要の概要](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

グループのレイアウトテンプレートについて詳しくは、 [グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## レイアウトテンプレートを使用してホームと概要をカスタマイズする

1. レイアウトテンプレートの使用を開始する ( [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 下向き矢印をクリックします。 ![](assets/dropdown-arrow.png) under **ユーザーに表示する内容をカスタマイズ**&#x200B;を選択し、「 **ホームと概要**.

1. 左側に表示されるリストで、オブジェクトタイプ (**タスク**, **問題**, **プロジェクト**, **ドキュメント**&#x200B;または **ドキュメントのバージョン**) をクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">タスク</td> 
      <td> <p>ホームでは、この設定を行うと、ユーザーがタスクをクリックしたときにタスクの右側の領域が変わります。 また、タスクのリストでは、ユーザーがタスクを選択して [ 概要を開く ] アイコンをクリックすると、ページの右側に表示される概要パネルに影響します <img src="assets/summary-panel-icon.png">.</p> <p>例えば、ユーザーがホームでタスクを選択する際に「詳細」領域に表示されるフィールドを指定できます。</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>また、サマリーでタスクを選択した場合は、次のようになります。</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">問題</td> 
      <td> <p>ホームでは、この設定は、ユーザーが問題をクリックしたときに問題の右側の領域に影響します。</p> <p>問題の一覧では、この設定は、ユーザーが問題を選択して [ 概要を開く ] アイコンをクリックしたときにページの右側に表示される [ 概要 ] パネルに影響します <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクト</td> 
      <td>ホームでは、ユーザーが割り当てられたプロジェクト承認をクリックすると、この設定の影響を受けるのは承認の右側の領域です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td>ホームでは、ユーザーが割り当てられているドキュメントの承認をクリックすると、この設定の影響を受けるのは承認の右側の領域です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント バージョン</td> 
      <td>ホームでは、ユーザーが特定のバージョンのドキュメントに割り当てられている承認をクリックすると、この設定の影響を受けるのは承認の右側の領域です。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >タスクの割り当てが解除されている場合、レイアウトテンプレートに割り当てられたユーザーには、概要にフィールドのカスタマイズが表示されません。

1. （条件付き）前の手順で [ タスク ] または [ タスク ] をクリックした場合は、カスタマイズするタスクまたはタスクのカテゴリを選択します。

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. （条件付き） **「プライマリアクションを設定」ボタン** ドロップダウンメニューが表示されます ( **タスク** または **問題** 左側のリストで )、プライマリアクション (**完了** または **ステータス**) を選択します。

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. 追加 ![](assets/add-item-plus-in-circle-blue.png) または非表示 ![](assets/close-or-hide---x.png) 選択したオブジェクトタイプのフィールド。

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. 手順 3 ～ 6 を繰り返して、他のオブジェクトタイプのホーム領域と [ 概要 ] パネルをカスタマイズします。
1. クリック **グローバル設定**&#x200B;をクリックし、左下隅付近にある、「ホーム」と「概要」のAdobe Workfrontオブジェクトに関連する次のオプションを有効または無効にします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">作業の更新を表示する</td> 
      <td>選択したタスクまたは問題に対して行われた更新を [ ホーム ] または [ 概要 ] に表示します。 これには、ユーザーによるシステム更新と更新の両方が含まれます。 ユーザーは、システムの更新をフィルターして除外できます。詳しくは、 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">システム更新を有効または無効にする</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業に対する時間を記録する</td> 
      <td>タスクまたは問題が選択されている場合に [ 作業時間に対するログ ] オプションを表示し、[ ホーム ] 領域と [ 概要 ] 領域から作業項目に対する時間を直接記録できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業に関連付けられたドキュメントを表示</td> 
      <td>タスクまたはタスクが選択されたとき、[ ホーム ] と [ サマリ ] に [ ドキュメント ] 領域が表示され、タスクまたはタスクに添付されたドキュメントが一覧表示されます。 ユーザーは、ドキュメントをクリックして、プレビューウィンドウに表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムスタンプを非表示</td> 
      <td>ホームおよび概要の次の日付フィールドのタイムスタンプを非表示にします。
       <ul>
        <li>予定完了日</li>
        <li>コミット日</li>
        <li><p>送信日</p></li>
       </ul><p><b>注意</b>:このオプションを有効にすると、期限を過ぎた作業項目は、時間ではなく、日付に基づいてホームワークリストの遅延グループに移動されます。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、 **保存**.

レイアウトテンプレートについて詳しくは、 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
