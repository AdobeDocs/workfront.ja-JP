---
title: レコードタイプを削除
description: 関係がなくなったレコードタイプは削除できます。レコードタイプを削除すると、レコード、フィールド、ビューなど、レコードタイプに関連付けられているすべての情報も削除されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 50%

---


# レコードタイプの削除

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

関係がなくなったレコードタイプは削除できます。

ただし、レコードタイプを削除すると、そのレコードタイプに関連付けられているすべての情報も削除されます。詳しくは、この記事で[レコードタイプを削除する際の考慮事項](#considerations-when-deleting-record-types)の節を参照してください。

レコードタイプについて詳しくは、[ レコードタイプの概要 ](/help/quicksilver/planning/architecture/overview-of-record-types.md) を参照してください。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> に対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p></td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## レコードタイプを削除する際の考慮事項

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 自分が管理権限を持つワークスペースからは、レコードタイプのみを削除できます。
* レコードタイプを削除すると、それに関連付けられている次の情報が削除されます。

   * そのタイプのすべてのレコード。
   * そのレコードタイプに関連付けられているすべてのフィールド。
   * そのレコードタイプのすべてのビュー（フィルター、グループ化、並べ替え条件を含む）。
* そのレコードタイプは、ワークスペースにアクセスするすべてのユーザーから削除されます。
* 削除したレコードタイプやその情報は復元できません。
* 削除するレコードタイプに関連付けられているフィールドとレコードを別のレコードタイプで再作成してから削除することをお勧めします。

## レコードタイプの削除

{{step1-to-planning}}

1. レコードタイプを削除するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。

   ワークスペースが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプカードにポインタを合わせ、「**詳細**」メニューをクリックしてから **削除** をクリックします。
   * 削除するレコードの種類のカードをクリックし、レコードの種類ページで、レコードの種類名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、[**削除**] をクリックします。

   ![ レコードタイプを完全に削除する確認 ](assets/permanently-delete-record-type-confirmation.png)

1. 確認ボックスに **削除** と入力し、「**完全に削除**」をクリックします。 これは、大文字と小文字を区別しません。

   選択したレコードタイプは、フィールド、関連レコード、ビューと共に削除され、復元できません。
