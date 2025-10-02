---
title: マイルストーン パスを作成する
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfront 管理者は、システム内の任意のプロジェクトに適用できるマイルストーンパスを作成します。このエリアでマイルストーンパスに加えた変更は、Workfront システム全体に影響を与えます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 5b9b1f397c76afa2e2ae550e0ce62a6038b8bd86
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 51%

---

# マイルストーンパスを作成

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

<div class="preview">

このページで強調表示されている情報は、まだ一般公開されていない機能を示しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 プレビューリリースから 1 週間後に、すべてのお客様の実稼動環境でも同じ機能が使用できるようになります。

詳しくは、[&#x200B; インターフェイスの最新化 &#x200B;](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md) を参照してください。

</div>

Adobe Workfront 管理者は、システム内の任意のプロジェクトに適用できるマイルストーンパスを作成します。このエリアでマイルストーンパスに加えた変更は、Workfront システム全体に影響を与えます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p>
   <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## マイルストーンとマイルストーンパス

プロジェクト内の主要タスクを、事前に定義されたマイルストーンに関連付けることができます。この機能を使用すると、管理者や他の関係者に対し、プロジェクトの進行状況などに関する概要を提供できます。

事前に定義されたすべてのマイルストーンの合計は、マイルストーンパスと呼ばれます。

マイルストーンパスを作成する最初の手順は、マイルストーンの手順の内容を識別し、マイルストーンを確立することです。マイルストーンパスは複数のプロジェクトに関連付けることができるので、マイルストーンの手順は、任意のプロジェクトの一般的なフェーズまたはステージである必要があります。

マイルストーンパスをプロジェクトに関連付け、マイルストーンをタスクに関連付ける方法に関して詳しくは、[タスクへのマイルストーンの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)を参照してください。

## マイルストーンパスを作成

{{step-1-to-setup}}

1. **プロセス**／**マイルストーンパス**&#x200B;をクリックします。
1. **新しいマイルストーンパス**&#x200B;をクリックします。

   <div class="preview">

   新規マイルストーンパス ボックスが開きます。

   ![&#x200B; 新規マイルストーンパスボックス &#x200B;](assets/new-milestone-path-box.png)

   </div>

1. 左側のパネルで **基本情報** をクリックします。

   次の情報を更新します。

   <table style="table-layout:auto">
    <tr>
      <td>マイルストーンパス名</td>
       <td>マイルストーンパスの名前を入力します。</td>
    </tr>
    <tr>
      <td>説明</td>
      <td>説明を入力して、マイルストーンパスを定義します。</td>
    </tr>
    <tr>
       <td>アクティブ</td>
      <td>マイルストーンパスをアクティブにする場合は、このチェックボックスを選択します。他のユーザーが、プロジェクトの作成時や編集時に、このパスを見つけてプロジェクトに添付できます。非アクティブなマイルストーンパスは、プロジェクトに添付できません。これはデフォルトで有効になっています。</td>
    </tr>
    <tr>
      <td>グループ</td>
      <td>リストに表示されたグループを選択し、これらのグループのユーザーがこのマイルストーンパスを表示してプロジェクトに適用できるようにします。マイルストーンパスに入るユーザーのホームグループは、デフォルトで選択されています。</td>
    </tr>
   </table>

1. 左側のパネルで **マイルストーン** をクリックします。
1.実稼動環境で、「**マイルストーンを追加**」をクリックして、パスにマイルストーンを追加します。
   <span class="preview"> プレビュー環境で **新しい行** をクリックして、パスにマイルストーンを追加します。</span>
1. 次の情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>それぞれのマイルストーンに、わかりやすい名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>マイルストーンの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>マイルストーンに関連付けるカラーを選択します。 </p> <p>カラーを選択しない場合は、マイルストーンパスで最後に使用されたカラーが選択されます。マイルストーンごとに一意のカラーを選択することをお勧めします。カラーは、視覚的およびレポートの目的で使用されます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （任意）各マイルストーンをドラッグ&amp;ドロップして並べ替えます。
1. 「**マイルストーンパスを作成**」をクリックして変更を保存します。

   マイルストーンパスをプロジェクトに関連付ける準備が整いました。

   マイルストーンパスをプロジェクトに関連付ける方法と、マイルストーンをタスクに関連付ける方法に関して詳しくは、[タスクへのマイルストーンの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)を参照してください。

1. （オプション） マイルストーンパス リストから 1 つのマイルストーンを選択し、**編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックしてマイルストーンパスを開き、その情報を編集します。
1. （オプション） **書き出し** アイコン ![&#x200B; 書き出しアイコン &#x200B;](assets/export-icon.png) をクリックし、次の形式から選択してマイルストーンパスリストをファイルに書き出します。

   * PDF
   * Excel
   * Excel（xlsx）
   * タブ区切り

1. （任意）マイルストーンリストで 1 つまたは複数のマイルストーンを選択し、**削除** アイコン ![&#x200B; 削除アイコン &#x200B;](assets/delete-icon.png) をクリックして削除します。
1. 「**はい、削除します**」をクリックします。

   マイルストーンは削除され、復元できません。 マイルストーンパスは、以前に関連付けられていたプロジェクトから削除され、すべてのマイルストーンが関連付けられたタスクから削除されます。

   削除したマイルストーンは復元できません。


## プロジェクトレポートでのマイルストーンパスの詳細の表示

マイルストーンパスの詳細は、プロジェクトレポートで表示できます。

プロジェクトレポートで詳細を表示するには、マイルストーンパスをプロジェクトに関連付ける必要があります。

マイルストーンパスのプロジェクトへの関連付けについて詳しくは、[&#x200B; プロジェクトの編集 &#x200B;](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) を参照してください。

{{step1-to-reports}}

1. **新しいレポート** をクリックし、**プロジェクト** をクリックします。
1. 「**列を追加**」をクリックします。
1. **この列に表示** 領域に **マイルストーンパス** と入力し始め、**マイルストーンパス名** をクリックして表示します。
1. （任意）「**フィルター**」をクリックして、レポートに次のフィルターを追加します。**プロジェクトマイルストーンのパス ID が空白ではありません**。

   フィルターを使用すると、マイルストーンパスに関連付けられているプロジェクトのみをレポートに表示できます。

1. 「**保存して閉じる**」をクリックします。
1. レポートの名前を追加し、「**適用**」をクリックします。

   プロジェクトレポートが表示されます。 各プロジェクトに関連付けられているマイルストーンパスは、レポートの最後の列に表示されます。
1. レポートの最後の列で、マイルストーンパスの名前をクリックします。

   マイルストーンパスの詳細が表示されます。

   ![&#x200B; プロジェクトレポートからのマイルストーンパスの詳細 &#x200B;](assets/milestone-details-from-project-report.png)

   マイルストーンパスの詳細ページには、次の情報が表示されます。

   * マイルストーンパス名、ID および説明
   * マイルストーン パス グループ
   * マイルストーン名、説明、カラーおよびカラーアイコン

1. （任意）「**戻る**」をクリックして、プロジェクトレポートに戻ります。



