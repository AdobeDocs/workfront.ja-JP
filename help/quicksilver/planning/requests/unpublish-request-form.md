---
title: Adobe Workfront Planning でのリクエストフォームの非公開
description: リクエストフォームが不要になった場合や、関係がなくなった場合は、非公開にすることができます。 非公開にすると、フォームに対するすべてのユーザーの権限が削除されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 28%

---


# Adobe Workfront Planning でのリクエストフォームの非公開


<!--take Preview and Production references at Production time-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

リクエストフォームが不要になった場合や、関係がなくなった場合は、非公開にすることができます。 非公開にすると、フォームに対するすべてのユーザーの権限が削除されます。

また、より少ないユーザーのグループがリクエストフォームを使用できるようにする場合は、リクエストフォームを共有するエンティティを変更することもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </td>

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
   <td>
   <p>標準</p>
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
   <td>
   <ul>
   <li><p>ワークスペースに対する権限の管理</p></li>
    <li><p>システム管理者は、自分が作成していないワークスペースを管理できます。 </p></li>
    </ul>
   <p>Workfront Planning オブジェクトの共有権限について詳しくは、
<a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a>を参照してください。 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストフォームの共有の変更

社外のユーザーを含むすべてのユーザーとの間で、に対する要求を公開する場合、フォームが関連付けられているワークスペースを表示または管理する特定のユーザーに対して、このアクセスを制限することを検討できる場合があります。

リクエストフォームの共有を変更するには：

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側 ![](assets/more-menu.png) ある **詳細** メニューをクリックし、「**リクエストフォームを更新**」をクリックします。
1. 画面の右上隅にある **共有** をクリックし、共有の選択を更新します。 詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。
1. （任意）リクエストフォームの共有を変更し、新しいリンクを使用して新しいユーザーグループに共有する場合は、「**リンクをコピー**」をクリックします。

## レコードタイプのリクエストフォームを非公開にする

リクエストフォームが無関係になり、誰にもアクセスされないようにするには、そのリクエストフォームを非公開にします。

{{step1-to-planning}}

1. レコードを追加するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。レコードタイプの作成については、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

   最後にアクセスしたビューで、レコードタイプのページが開きます。デフォルトでは、レコードタイプのページがテーブル表示で開きます。

1. ページヘッダーのレコードタイプ名の右側 ![](assets/more-menu.png) ある **詳細** メニューをクリックし、「**リクエストフォームを更新**」をクリックします。
1. 右上隅の **非公開** をクリックします。

   ![](assets/unpublish-button-highlighted.png)

   フォームが非公開になったことを知らせる確認が画面の下部に表示されます。

   **非公開** ボタンが **Publish** に変わります。

1. **保存**&#x200B;をクリックします。

   リンクからフォームにアクセスでき <!--or from the request queue in the Requests area of Workfront--> くなりました。

   リクエストフォームを使用して以前に追加したレコードは、レコードタイプページに残ります。

   <span class="preview"> 以前に追加されたリクエストは、Workfrontの「計画」タブの「リクエスト」領域に残ります。</span>