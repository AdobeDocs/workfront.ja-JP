---
title: レイアウトテンプレートを使用した概要パネルのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートを使用すると、ユーザーが概要でタスクまたはイシューをクリックしたときに表示される内容を設定できます。 以下の手順を使用して行う各設定は、概要パネルに影響します。 ただし、これらのカスタマイズは「ドキュメントの概要」パネルには適用されません。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 8880891c0f5fd8fecad6c2f58136d36a943105ae
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 53%

---

# レイアウトテンプレートを使用した概要パネルのカスタマイズ

<!--Audited: 11/2024-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


レイアウトテンプレートを使用すると、ユーザーがタスクまたは問題をクリックしたときに概要パネルに表示される内容を設定できます。 以下の手順を使用して行う各設定は、概要パネルに影響します。 ただし、これらのカスタマイズは「ドキュメントの概要」パネルには適用されません。

以下を設定できます。

* 「詳細」でタスクまたはイシューに対して表示されるフィールドおよび順序
* 選択したタスクまたはイシューに対して、更新、ログに記録された時間、添付されたドキュメント、タイムスタンプを表示するかどうか

ユーザーに割り当てられているプロジェクトの承認、ドキュメントの承認、ドキュメントのバージョンの承認をクリックする際に、「ホーム」に表示されるフィールドをカスタマイズすることもできます。

「概要」パネルについて詳しくは、[概要について](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートの作成と管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td><p>新規：標準</p>
  <p> 現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レイアウトテンプレートを使用した概要パネルのカスタマイズ

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。

1. **ユーザーに表示する内容をカスタマイズ** の下の下向き矢印 ![](assets/dropdown-arrow.png) をクリックし、**概要パネル** をクリックします。

1. 下に表示されるリストで、概要パネルをカスタマイズするオブジェクトタイプをクリックします。

   次の表に、各オブジェクトに対してカスタマイズできる内容を示します

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">タスク</td> 
      <td> <p>タスクのリストでは、この設定は、ユーザーがタスクを選択して「概要を開く」アイコンを <img src="assets/summary-panel-icon.png"> リックするとページの右側に表示される概要パネルに影響します。</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">イシュー</td> 
      <td><p>イシューのリストでこの設定は、ユーザーがイシューを選択して概要を開くアイコン <img src="assets/summary-panel-icon.png"> をクリックした際に、ページの右側に表示される「概要」パネルに反映されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">プロジェクト</td> 
      <td><ul><li><p>「ホーム」でこの設定は、ユーザーが自分に割り当てられたプロジェクト承認をクリックした際に、承認の右側のエリアに反映されます。</p>
      <p><b> 重要：</b> </p><p>これは非推奨（廃止予定）の機能です。 この領域に加える変更は、Workfrontによって削除された機能に関連しています。 このオプションは、後のメンテナンス更新でWorkfrontから削除されます。</p></li>
      <li><span class="preview"><p>この領域はプレビュー環境から削除されました。</p></li></span></ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメント</td> 
      <td>
     <ul><li><p>「ホーム」でこの設定は、ユーザーが自分に割り当てられたドキュメントの承認をクリックした際に、承認の右側のエリアに反映されます。</p>
      <p><b> 重要：</b> </p><p> これは非推奨（廃止予定）の機能です。 この領域に加える変更は、Workfrontによって削除された機能に関連しています。 このオプションは、後のメンテナンス更新でWorkfrontから削除されます。</p></li>
      <li><span class="preview"><p>この領域はプレビュー環境から削除されました。</p></li></span></ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドキュメントバージョン</td> 
      <td><ul><li><p>「ホーム」でこの設定は、ユーザーが特定のバージョンのドキュメントの自分に割り当てられた承認をクリックした際に、承認の右側のエリアに反映されます。</p>
      <p><p><b>重要：</b></p> これは非推奨（廃止予定）の機能です。 この領域に加える変更は、Workfrontによって削除された機能に関連しています。 このオプションは、後のメンテナンス更新でWorkfrontから削除されます。</p></li>
      <li><span class="preview"><p>この領域はプレビュー環境から削除されました。</p></li></span></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >タスクが未割り当ての場合、レイアウトテンプレートに割り当てられたユーザーには、「概要」にフィールドのカスタマイズが表示されません。

1. （条件付き）前の手順で「タスク」または「イシュー」をクリックした場合は、カスタマイズするタスクまたはイシューのカテゴリを選択します。

   <span class="preview">![](assets/choose-cat-cstmz-nwe-adobe-branding.png)</span>

1. （条件付き） **プライマリアクションを設定** ボタン ドロップダウンメニューが表示された場合（左側のリストで **タスク** または **イシュー** を選択した場合）、ユーザーがタスクまたはイシューを表示したときに概要パネルで使用できるプライマリアクション（**完了** または **ステータス**）をクリックします。

   <span class="preview">![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)</span>

1. 選択したオブジェクトタイプでフィールドを追加 ![](assets/add-item-plus-in-circle-blue.png) 非表示 ![](assets/close-or-hide---x.png) にします。

   <span class="preview">![](assets/lt-home-add-hide-fields-adobe-branding.png)</span>

1. 手順 3～6 を繰り返し、他のオブジェクトタイプの概要パネルをカスタマイズします。
1. 左下隅付近の **グローバル設定** をクリックし、概要のAdobe Workfront オブジェクトに関連する次のオプションのいずれかを有効または無効にします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">作業の更新を表示</td> 
      <td>選択したタスクまたは問題に対して行われた更新を概要パネルに表示します。 これには、システム更新とユーザーによる更新の両方が含まれます。ユーザーは、システムの更新をフィルターして除外できます（<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">作業を更新</a>の<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">システムアップデートを有効化または無効化</a>の節を参照）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業に対する時間を記録する</td> 
      <td>タスクまたはイシューが選択されている場合に「作業に対する時間を記録する」オプションを表示し、ホームエリアと概要エリアから作業アイテムに対する時間を直接記録できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業に関連付けられたドキュメントを表示</td> 
      <td>タスクまたは問題が選択されると、概要パネルにドキュメント領域が表示され、タスクまたは問題に添付されたすべてのドキュメントが一覧表示されます。 ユーザーは、ドキュメントをクリックして、プレビューウィンドウに表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムスタンプを非表示</td> 
      <td>概要パネル内の次の日付フィールドのタイムスタンプを非表示にします。
       <ul>
        <li>予定完了日</li>
        <li>コミット日</li>
        <li>送信日</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。
