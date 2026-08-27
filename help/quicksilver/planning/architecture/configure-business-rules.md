---
title: レコードタイプのビジネスルールの設定
description: そのタイプのレコードをAdobe Workfront Planningでどのように管理するかを定義するレコードタイプのビジネスルールを設定できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 914f1f8a25aa5b9e1045d2f940ed15061301c21b
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 12%

---


# レコードタイプのビジネスルールの設定

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

そのタイプのレコードをAdobe Workfront Planningでどのように管理するかを定義するレコードタイプのビジネスルールを設定できます。

## アクセス要件

+++ 展開してアクセス要件を表示し、この記事の手順を実行します。  

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
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>計画標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## ビジネスルールを設定する際の考慮事項

* 定義した条件に応じて、レコードを編集または削除できるタイミングのルールを設定できます。

  例えば、特定のフィールドに値を指定するための条件を作成できます。 これらのフィールドに値がない場合、ユーザーはそのレコードを編集または削除できません。
* プライマリワークスペースまたはセカンダリワークスペースのグローバルレコードタイプにビジネスルールを追加することはできません。
* レコードの作成時にルールを設定することはできません。 レコードタイプに対する管理権限を持つすべてのユーザーがレコードを作成できます。
* 次の以外のすべてのフィールドタイプを参照するビジネスルールの条件を作成できます。
  * 数式フィールド
  * ルックアップフィールド
  * 参照フィールド

## ビジネスルールの設定

1. レコードタイプに移動します。
1. レコードタイプ名の右側にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、「ビジネスルール」をクリックします。



