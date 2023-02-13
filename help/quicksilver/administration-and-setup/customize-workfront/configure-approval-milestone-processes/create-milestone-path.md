---
title: マイルストーンパスを作成
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfront管理者は、マイルストーンパスを作成し、それをシステム内の任意のプロジェクトに適用できます。 この領域でマイルストーンパスに加えた変更は、Workfrontシステム全体に影響を与えます。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

---

# マイルストーンパスを作成

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Adobe Workfront管理者は、マイルストーンパスを作成し、それをシステム内の任意のプロジェクトに適用できます。 この領域でマイルストーンパスに加えた変更は、Workfrontシステム全体に影響を与えます。

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
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## マイルストーンとマイルストーンのパス

プロジェクト内の主要タスクを事前に定義されたマイルストーンに関連付けることができます。 この機能を使用すると、管理者や他の関係者に対し、プロジェクトの進行状況に関する概要を提供できます。

事前に定義されたすべてのマイルストーンの合計は、マイルストーンパスと呼ばれます。

マイルストーンパスを構築する最初の手順は、マイルストーンステップの内容を識別し、マイルストーンを確立することです。 マイルストーンパスは複数のプロジェクトに関連付けることができるので、マイルストーンステップは、プロジェクトの一般的なフェーズまたはステージである必要があります。

マイルストーンパスをプロジェクトに関連付け、マイルストーンをタスクに関連付ける方法について詳しくは、 [タスクへのマイルストーンの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## マイルストーンパスを作成

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **プロセス** > **マイルストーンパス**.
1. クリック **新しいマイルストーンパス。**
1. 次の情報を **基本情報** 領域：

   <table style="table-layout:auto">
    <tr>
      <td>マイルストーンパス名</td>
       <td>マイルストーンパスの名前を入力します。</td>
    </tr>
    <tr>
      <td>説明</td>
      <td>マイルストーンパスを定義する説明を入力します。</td>
    </tr>
    <tr>
       <td>アクティブ</td>
      <td>マイルストーンパスを有効にする場合は、このチェックボックスを選択します。 他のユーザーは、プロジェクトの作成時や編集時に、このパスを見つけてプロジェクトに添付できます。 非アクティブなマイルストーンパスは、プロジェクトに添付できません。 これはデフォルトで有効になっています。</td>
    </tr>
    <tr>
      <td>グループ</td>
      <td>リストに表示されたグループを選択し、これらのグループのユーザーがこのマイルストーンパスを表示してプロジェクトに適用できるようにします。 マイルストーンパスに入るユーザーのホームグループは、デフォルトで選択されています。</td>
    </tr>
   </table>

1. 次の情報を **マイルストーン** 領域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>各マイルストーンのわかりやすい名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>マイルストーンの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>マイルストーンに関連付ける色を選択します。 </p> <p>色を選択しない場合は、マイルストーンパスで最後に使用された色が選択されます。 マイルストーンごとに一意の色を選択することをお勧めします。 色は、視覚的およびレポートの目的で使用されます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **マイルストーンの追加** 必要に応じて、パスが完了するまでマイルストーンを追加し続けます。
1. クリック **マイルストーンパスを作成** 変更を保存します。

   マイルストーンパスをプロジェクトに関連付ける準備が整いました。

   マイルストーンパスをプロジェクトに関連付ける方法と、マイルストーンをタスクに関連付ける方法の詳細については、 [タスクへのマイルストーンの関連付け](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
