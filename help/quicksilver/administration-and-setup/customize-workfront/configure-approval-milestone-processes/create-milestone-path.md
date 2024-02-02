---
title: マイルストーンパスを作成
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfront 管理者は、システム内の任意のプロジェクトに適用できるマイルストーンパスを作成します。このエリアでマイルストーンパスに加えた変更は、Workfront システム全体に影響を与えます。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: ht
source-wordcount: '520'
ht-degree: 100%

---

# マイルストーンパスを作成

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Adobe Workfront 管理者は、システム内の任意のプロジェクトに適用できるマイルストーンパスを作成します。このエリアでマイルストーンパスに加えた変更は、Workfront システム全体に影響を与えます。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## マイルストーンとマイルストーンパス

プロジェクト内の主要タスクを、事前に定義されたマイルストーンに関連付けることができます。この機能を使用すると、管理者や他の関係者に対し、プロジェクトの進行状況などに関する概要を提供できます。

事前に定義されたすべてのマイルストーンの合計は、マイルストーンパスと呼ばれます。

マイルストーンパスを作成する最初の手順は、マイルストーンの手順の内容を識別し、マイルストーンを確立することです。マイルストーンパスは複数のプロジェクトに関連付けることができるので、マイルストーンの手順は、任意のプロジェクトの一般的なフェーズまたはステージである必要があります。

マイルストーンパスをプロジェクトに関連付け、マイルストーンをタスクに関連付ける方法に関して詳しくは、[タスクへのマイルストーンの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)を参照してください。

## マイルストーンパスを作成

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**設定** ![](assets/gear-icon-settings.png)」の順にクリックします。

1. **プロセス**／**マイルストーンパス**&#x200B;をクリックします。
1. **新しいマイルストーンパス**&#x200B;をクリックします。
1. **基本情報**&#x200B;エリアに以下の情報を指定します。

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

1. 以下の情報を&#x200B;**マイルストーン**&#x200B;エリアに指定します。

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

1. 「**マイルストーンを追加**」をクリックし、必要に応じて、パスが完了するまでマイルストーンを追加し続けます。
1. 「**マイルストーンパスを作成**」をクリックして変更を保存します。

   マイルストーンパスをプロジェクトに関連付ける準備が整いました。

   マイルストーンパスをプロジェクトに関連付ける方法と、マイルストーンをタスクに関連付ける方法に関して詳しくは、[タスクへのマイルストーンの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)を参照してください。
