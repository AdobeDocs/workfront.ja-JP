---
title: アイデア創出スペースを他のユーザーと共有する
description: Adobe Workfront Planningでは、キャンペーンを開始する前にアイデアを立案するための機能が追加されました。 AIを活用して、アイデアを立案し、関係者と共同作業をおこなうことで、そのアイデアを記録的な速さで形にすることができます。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ff8ec4e7f5f9ffefcfc6eeea7e37443bcd1f55d2
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 7%
---

# アイデア創出スペースを他のユーザーと共有する

<!--add to TOC and miniTOC-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 これは、**アイデア創出スペース Beta** プログラムの一部としてのみ使用できます。</span>

<span class="preview">詳細については、[Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。</span>

{{planning-important-intro}}

<!--
Some of this information is also duplicated in the section for Ideation space permissions in the Access needed to use Ideation space article
-->

Workfront計画レコードの権限は、レコードのアイデア創出スペースに転送されます。

さらに、他のユーザーにアイデア創出スペースを使用するための権限を付与し、アイデアを追加することもできます。

次の点に注意してください。

* アイデアの作成者は、常に自分のアイデアに対する編集者の権限を持っています。

* ブリーフを作成して他のアプリケーションに書き出すには、アイデア創出スペースに対する編集者権限が必要です。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

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
<ul> 
<li><p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p></li>
または
<li><p>スタンドアロン製品として購入された場合の任意のプランニング・パッケージ</p></li></ul>
   </td> 
    <!--
    <tr> 
    <td role="rowheader"><p>Additional products</p></td> 
    <td><ul>
    <li><p>Adobe GenStudio for Performance Marketing</p></li>
    <li><p>Adobe Customer Journey Analytics</p></li>
    </ul>
    </td> 
    </tr> 
    -->
  <tr> 
   <td role="rowheader"><p>Adobe Workflow ライセンス</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> 
   <ul>
   <li><p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>   </li>
   <li><p>アクセスレベルの「アイデア創出スペースを無効にする」設定を選択解除する必要があります</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td> <p>レコードを追加するワークスペースおよびレコードタイプに対する権限を設定します </p>
      <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
      <p>Workfront オブジェクトに対する権限を表示して、ブリーフに追加する <!--not sure if this is available--></p>
      <p>ブリーフを作成するためのアイデア創出スペースの編集者権限</p>
   </td> 
  </tr>  
  <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/ja/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++  

## アイデア創出スペースの共有

1. プランニングレコードのアイデア創出スペースにアクセスします。

   詳しくは、次のいずれかの記事を参照してください。

   * [アイデア立案スペースの概要からプランニングレコードを作成](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
   * [アイデア創出スペースでブリーフを作成する](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

1. 右上隅の&#x200B;**共有**&#x200B;をクリックし、**ドキュメントを共有** ボックスの右上隅にある&#x200B;**設定** アイコン ![設定アイコン &#x200B;](assets/setting-icon.png)をクリックします。
1. 「誰がアクセス権を持っているか」リストで、次のいずれかを選択します。

   * **招待されたユーザーのみが**&#x200B;にアクセスできます

     個々のユーザーをアイデア創出スペースに追加し、権限レベルを付与する必要があります。
   * **会社の&lt;Workfront環境>の全員がコメントできます**

     ワークフローとプランニングライセンスをアクセスレベルに持つ組織内の全員が、アイデアに関する情報を見つけてコメントできます。
   * **リンクを知っているすべてのユーザーがコメントできます**

     アイデア出しリンクを共有したユーザーは、組織外のユーザーを含め、誰でもコメントできます。

1. 「**リンクをコピー**」をクリックして、アイデアのリンクを生成し、他のユーザーと共有します。 リンクがクリップボードに追加されます。
1. 設定ボックスの戻る矢印をクリックして、共有に戻ります。
1. （条件付き）特定のユーザーとアイデア創出スペースを共有することを選択した場合は、名前またはメールアドレスの入力を開始し、次のいずれかの権限レベルを選択します。

   | アイデア創出スペースの権限 | 機能 |
   |---|---|
   | **編集者** | アイデア創出スペースの編集、ダウンロード、共有が可能 |
   | **コメント** | アイデア創出スペースの表示とコメントを行えます |
   | **ビューアー** | アイデア創出スペースを表示できます |

1. （オプション）割り当てにメッセージを含め、**招待**&#x200B;をクリックします。

   招待されたユーザーには、権限の割り当てに関するメール通知が送信されます。

1. **X** アイコンをクリックして、**ドキュメントを共有** ボックスを閉じます。











