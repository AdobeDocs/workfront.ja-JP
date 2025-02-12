---
product-area: projects
navigation-topic: manage-issues
title: 問題の移動
description: イシューをプロジェクトとタスクの間で移動できます。
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 85%

---

# イシューを移動

<!--Audited: 12/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

次のオブジェクト間でイシューを移動できます。

* プロジェクトから別のプロジェクトへ
* タスクから同じプロジェクト内の別のタスク、または別のプロジェクト内の別のタスクへ
* タスクからプロジェクト、または別のプロジェクトへ
* プロジェクトから同じプロジェクト内のタスク、または別のプロジェクト内のタスクへ

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：</p> 
   <ul><li>投稿者以上</li>
   <li>プロジェクトの「イシュー」セクションでイシューを移動するには軽度以上</li></ul>
   <p>現在：</p>
   <ul>
   <li><p>リクエスト以上</p></li>
   <li><p>プロジェクトの「イシュー」セクションにイシューを移動するには、レビュー以上のライセンスが必要です。</p></li></ul>   
     </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトとタスクへのアクセス権またはそれ以上の権限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>イシューを追加機能を使用してイシューを移動する項目に対する参加権限。</td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## イシューの移動に関する考慮事項

ドキュメントを含むイシューや、リクエストキューに関連付けられているイシューを移動する際は、次の点を考慮してください。

* システム管理者またはグループ管理者は、設定領域の「ユーザーにログ時間を使用したタスクおよび問題の移動を許可」環境設定の設定方法に応じて、ログ時間を使用する問題の移動を防ぐことができます。 詳しくは、[システム全体のタスクおよびイシューの環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

* **イシューがリクエストキューに関連付けられている場合：**&#x200B;イシューを別のオブジェクトに移動し、そのイシューをリクエストキューに関連付けると、移動したイシューは最初のイシューの元になったキューに関連付けられなくなります。
* **イシューにドキュメントが添付されている場合：**&#x200B;イシューを別のオブジェクトに移動し、イシューにドキュメントが添付されている場合、そのドキュメント、バージョンおよびプルーフも新しいイシューに移動します。ドキュメントに関連付けられている承認は移動されません。
* **イシューがドキュメントまたはフォルダーにリンクされている場合：** Google Drive などのサードパーティのサービスにリンクされたドキュメントまたはフォルダーを含むイシューを移動すると、そのイシューと共にドキュメントへのリンクが移動します。

## リスト内のイシューを移動

イシューのリストまたはイシューレポートから 1 つまたは複数のイシューを移動できます。

1. 移動する 1 つまたは複数のイシューを含むプロジェクトに移動します。

   または

   イシューレポートに移動します。

1. プロジェクトに移動した場合は、左側のパネルで「**イシュー**」をクリックします。
1. 移動する 1 つまたは複数のイシューを選択し、イシューリストの上部にある&#x200B;**「その他」メニュー**&#x200B;をクリックし、「**指定の場所に移動**」をクリックします。

   ![ コピーしてリンクに移動 ](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. [ 単一の問題の移動 ](#move-a-single-issue) の節で説明しているように、手順 2 から問題の移動を続行します。

## 単一のイシューを移動 {#move-a-single-issue}

1 つのイシューを表示時に移動できます。

### 単一のイシューを移動

1. 移動するイシューに移動し、イシュー名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-icon.png) をクリックして、「**移動先**」をクリックします。

   ![ 問題レベルで移動 ](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   **イシューを移動**&#x200B;ボックスが表示されます。

   ![ イシューボックスを移動 ](assets/move-issue-box-nwe-350x280.png)

1. 「**宛先プロジェクトを選択**」セクションで、イシューの移動先のプロジェクトの名前を指定します。デフォルトでは、現在のプロジェクトの名前が表示されます。

   >[!TIP]
   >
   >リストには 100 個のプロジェクトのみが表示されます。

1. （条件付き）イシューをプロジェクトに移動するアクセス権がない場合は、「**アクセスをリクエスト**」をクリックします。
1. （条件付き）宛先プロジェクトのタスクの 1 つにイシューを追加するアクセス権がある場合は、アクセス権をリクエストせずに、引き続き選択した宛先プロジェクトにイシューを移動します。

   ![ イシューの移動とアクセスのリクエスト ](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Workfront 管理者がこれらのプロジェクトにイシューを追加できない場合、選択したプロジェクトが承認待ち、完了または無効の場合にも、同様のメッセージが表示されます。詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

1. （オプション）「**オプション**」セクションで、以下の表に示すいずれかの項目の選択を解除して、移動したイシューから削除します。デフォルトでは、すべてのオプションが選択されています。

   >[!IMPORTANT]
   >
   >オプションリストで項目の選択を解除すると、データが失われます。既存のイシューの情報は削除され、復元できません。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべて選択</td> 
      <td>このオプションの選択を解除すると、イシューを新しい場所に移動する際に、イシューのすべての情報を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">割り当て</td> 
      <td>イシューに割り当てられているユーザー、担当業務またはチームを削除します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進捗状況</td> 
      <td>イシューの完了率（存在する場合）を削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>ドキュメント</p></td> 
      <td> <p>ドキュメントのバージョン、リンクされたドキュメント、フォルダーなど、「ドキュメント」タブ内のすべての項目を削除します。

   <b>メモ</b>

   イシューでドキュメントを移動しないように選択した場合、ドキュメントは削除され、30 日間ごみ箱に入れられます。管理者はそれらのドキュメントを復元でき、移動したイシューで復元されます。

   イシューを移動した後に削除すると、復元されたドキュメントは、ドキュメントを復元した管理者のユーザーページのドキュメントエリアに配置されます。
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">権限</td> 
      <td>イシューの共有先エンティティを削除します。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>イシューの「更新」セクションからコメントを削除します。</td> 
     </tr> 
    </tbody> 
   </table>


1. （オプション）「**タスクを選択**」セクションで、イシューを移動するタスクを選択します。
1. 「**イシューを移動**」、またはリストで複数のイシューを選択した場合は「**複数のイシューを移動**」をクリックします。

   移動されたイシューが、指定したプロジェクトに追加されます。




