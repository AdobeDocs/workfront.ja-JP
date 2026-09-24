---
title: プランニングリクエストの共有
description: Workfront計画リクエストは、送信後に他のユーザーと共有できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 4ee702aeded88e330ec456a0e6b5cf1813bfb64e
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 11%
---
# プランニングリクエストの共有

<!--add to TOC, and miniTOC-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 リリースからプレビューの後、高速リリースを有効にしたお客様は、同じ機能を毎月実稼動環境でも使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

プランニングリクエストが提出された後、それを見る人、作業できる人、各ユーザーまたはチームが取ることができるアクションを制御できます。 これにより、適切な担当者が適切なリクエストに集中し、それぞれの役割に適切なアクションのみを実行できるようになります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>プランニングパッケージを含む任意のWorkfrontまたはワークフロー</p> 
または
<p>スタンドアロン製品として購入した際のあらゆるWorkfrontプランニング</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計画ライセンス</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td> <p>ワークフローとPlanning パッケージの両方を持っている場合は、ワークフローとPlanning ライセンスタイプの両方をアクセスレベルに追加する必要があります</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>Workfront ユーザーの場合は、ワークスペースおよびレコードタイプに対する表示以上の権限</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## リクエストを共有する際の考慮事項

* リクエストに対してユーザーに次の権限を付与できます。

  * ビュー：ユーザーはリクエストのみを表示できます。
  * 貢献：ユーザーは、リクエストを表示、編集、およびコメントできます。
  * 管理：ユーザーはリクエストを表示、編集、コメント、削除できます。

* 管理者が別のデフォルトを設定していない限り、リクエスト者は、送信したリクエストに対する管理アクセス権を自動的に付与されます。

  詳しくは、[&#x200B; リクエストフォームの作成](/help/quicksilver/planning/requests/create-request-form.md)を参照してください。

* Workfront管理者は、すべてのリクエストにアクセスして管理できます。
* レコードタイプへの管理アクセス権を持つユーザーは、そのレコードタイプの受注フォームとそのフォームを通じて送信されたすべてのリクエストへの管理アクセス権を継承します。
* リクエストに対する権限を持つユーザーは、自分の権限レベルと同じ権限レベルまたは下位レベルのリクエストを共有できます。

  Contribute権限を持つユーザーは、他のユーザーにリクエストに対する管理権限を与えることはできません。

* 異なる人やチームが同じリクエストに対して異なるアクセスレベルを保持することができます。
* 権限は、複数のエンティティを通じて割り当てることができます。 ユーザーがリクエストに対するContribute権限を持っていても、そのグループまたはジョブロールに表示権限がある場合、Contributeという最高レベルの権限が保持されます。

## リクエストの共有

新しいリクエストエクスペリエンスを使用していることを確認します。

1. {{step1-to-requests}}
1. Planning リクエストを見つけてクリックして開きます。
1. 「**共有**」をクリックします。

   選択したリクエストの&#x200B;**共有** ボックスが開きます。

   ![&#x200B; リクエスト共有ボックス &#x200B;](assets/requests-sharing-box.png)

1. **このリクエストフィールドへのアクセス権を付与**&#x200B;で、ユーザー、チーム、役割、グループまたは会社の名前の入力を開始し、リストに表示されたらクリックします。

   アクティブなエンティティのみがリストに表示されます。
1. 各エンティティ名の右側にあるドロップダウンメニューから、次のいずれかの権限レベルを選択します。

   * 管理
   * 参加
   * 表示
1. （オプション）権限レベルごとに、詳細な権限アイコンをクリックし、**編集**、**コメント**、**共有**、**削除**&#x200B;など、詳細な権限を選択または選択解除します。

   ![&#x200B; リクエストに対する詳細な権限](assets/granular-permissions-on-requests.png)
1. 「**保存**」をクリックします。

   リクエストは、選択したエンティティと共有されます。


