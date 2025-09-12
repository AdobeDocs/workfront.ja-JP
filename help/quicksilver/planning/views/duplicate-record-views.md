---
title: レコードビューを複製
description: 複数のバージョンのビューを保持し、バージョン間でわずかな変更を加える場合、Adobe Workfront Planning でビューを複製できます。 この記事では、ビューを複製する方法について説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 35%

---

# レコードビューを複製

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

複数のバージョンのビューを保持し、バージョン間でわずかな変更を加える場合、Adobe Workfront Planning でビューを複製できます。

ビューを複製すると、既存のビューと同一のコピーが作成されます。

元のビューの共有権限は、複製されたビューには移行されません。

ビューの複製は、Workfront Planning のすべてのタイプのビューで同じです。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。 

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
   <td>   <p>ビューに対する権限を管理</p>  
   <p>ビュー設定を一時的に変更したり、複製したりするためのビューへのアクセス許可を表示します。</p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++   

## レコードビューを複製

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプ ページが開きます。
デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 複製するビューのタブにポインタを合わせ、ビュー名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックしてから、「**複製**」をクリックします。

   ![ レコード ビューで詳細メニューを表示 ](assets/view-more-menu-with-duplicate-option.png)

   <!--at preview release, replace the step above with this one: 
    1. Depending on which environment you use, do the following: 
    * In the Production environment, hover over one the of the view's names in the view tab, then click **More** ![More menu](assets/more-menu.png) to the left of the view name, then click **Duplicate**. 
    * <span class="preview">In the Preview environment, click the dropdown icon ![Dropdown icon](assets/drop-down-icon.png) next to the current view name, hover over the name of a view, click **More**, then **Duplicate**.</span>-->
   ビューが複製され、新しいビューの名前が次のパターンに従います。`Original view's name (Copy)`新しいビュータブは、すべてのビュータブの最後に表示されます。
