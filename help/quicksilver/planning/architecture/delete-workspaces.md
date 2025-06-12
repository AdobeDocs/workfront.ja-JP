---
title: ワークスペースの削除
description: 関係がなくなったワークスペースは削除できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 45%

---


# ワークスペースの削除

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

不要になったワークスペースは削除できます。

ワークスペースを削除する前に、そのワークスペースに関連付けられているレコードタイプ、レコード、フィールド、ビューの一部またはすべてを、別のワークスペースで再作成することをお勧めします。

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準 </p>
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
   <td>   <p>ワークスペースへの権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ワークスペースの削除に関する考慮事項

* ワークスペースを削除すると、すべてのレコードタイプ、レコード、そのフィールドおよびビューも削除されます。
* 削除したワークスペースとそれらに含まれる情報は復元できません。

## ワークスペースの削除

{{step1-to-planning}}

1. （条件付き）Workfront管理者の場合は、「**自分が参加しているワークスペース** **」をクリックして作成したワークスペースにアクセスしたり、「その他のワークスペース** をクリックして自分と共有されている他のワークスペースにアクセスしたりします。

1. （任意）「**すべて表示**」をクリックして、追加のワークスペースを表示します。 **すべてを表示** リンクは、ワークスペースカードが 3 行を超える場合にのみ表示されます。
1. （任意） ClicK **表示を減らす** を使用して、画面に表示するワークスペースの数を制限します。
1. ワークスペースを削除するには、次のいずれかの操作を行います。

   * ワークスペースカードにポインタを合わせ、カードの右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックします
または
   * ワークスペースカードをクリックしてワークスペースを開き、ワークスペース名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックします。
1. 「**削除**」をクリックします。

   ![ ワークスペースを完全に削除する確認 ](assets/permanently-delete-workspace-confirmation.png)

1. 表示されたスペースに「**削除**」と入力し、「**完全に削除**」をクリックします。 これは、大文字と小文字を区別しません。

   ワークスペースは削除され、復元できません。レコードタイプ、レコード、フィールドおよびそれらに関連付けられているビューも削除されます。<!--ensure this is right at or before GA-->
