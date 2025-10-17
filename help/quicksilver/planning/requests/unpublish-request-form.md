---
title: Adobe Workfront Planning でのリクエストフォームの非公開
description: リクエストフォームが不要になった場合や、関係がなくなった場合は、非公開にすることができます。 非公開にすると、フォームに対するすべてのユーザーの権限が削除されます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: df0686038adb1278339e872e122a311884cb6d29
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 15%

---

# Adobe Workfront Planning でのリクエストフォームの非公開


<!--take Preview and Production references at Production time-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

リクエストフォームが不要になった場合や、関係がなくなった場合は、非公開にすることができます。 非公開にすると、フォームに対するすべてのユーザーの権限が削除されます。

また、より少ないユーザーのグループがリクエストフォームを使用できるようにする場合は、リクエストフォームを共有するエンティティを変更することもできます。

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
<p>任意のWorkfront パッケージと任意の Planning パッケージ</p>
または
<p>任意のワークフローパッケージと任意の Planning パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限とレコードタイプの管理 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## リクエストフォームの共有の変更

社外のユーザーを含むすべてのユーザーとの間で、に対する要求を公開する場合、フォームが関連付けられているワークスペースを表示または管理する特定のユーザーに対して、このアクセスを制限することを検討できる場合があります。

リクエストフォームの共有を変更するには：

{{step1-to-planning}}

1. フォームを共有するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側にある **その他** メニュー ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックし、**リクエストフォームの管理** をクリックします。

   レコードタイプに関連付けられたすべてのリクエストフォームがテーブル表示に表示されます。
1. リクエストフォームの名前にポインタを合わせ、名前の右側にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックしてから、**共有** をクリックします。
1. 次のいずれかを選択して、共有の選択肢を更新します。

   * ワークスペースに対する表示またはそれ以上のアクセス権を持つすべてのユーザー
   * ワークスペースに対する参加またはそれ以上のアクセス権を持つすべてのユーザー
   * リンクを知っているすべてのユーザー

   詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。
1. （任意）リクエストフォームの共有を変更し、新しいリンクを使用して新しいユーザーグループに共有する場合は、「**リンクをコピー**」をクリックします。

## レコードタイプのリクエストフォームを非公開にする

リクエストフォームが無関係になり、誰にもアクセスされないようにするには、そのリクエストフォームを非公開にします。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側にある **その他** メニュー ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックし、**リクエストフォームの管理** をクリックします。

   レコードタイプに関連付けられたすべてのリクエストフォームがテーブル表示に表示されます。
1. リクエストフォームの名前にポインタを合わせ、名前の右側にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックしてから、「**非公開**」をクリックします。

または

リクエストフォームの名前をクリックして開き、リクエストフォームの右上隅にある「**非公開**」をクリックします。

![&#x200B; ハイライト表示された「非公開」ボタン &#x200B;](assets/unpublish-button-highlighted.png)

フォームが非公開になったことを知らせる確認が画面の下部に表示されます。

**非公開** リンクまたはボタンが **公開** に変わります。

1. （条件付き）フォームを開いた後に非公開にした場合は、「**保存**」をクリックします。

   ユーザーは、リンクから、またはWorkfrontの「リクエスト」領域のリクエストキューからリクエストフォームにアクセスできなくなりました。

   リクエストフォームを使用して以前に追加したレコードは、レコードタイプページに残ります。

   以前に追加されたリクエストは、Workfrontの「計画」タブの「リクエスト」領域に残ります。
