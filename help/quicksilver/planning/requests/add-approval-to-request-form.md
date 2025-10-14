---
title: Adobe Workfront Planning の要求フォームへの承認の追加
description: Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 83b3bd73fd30b5fba931e64783dee67485d98fe9
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 13%

---

# Adobe Workfront Planning でリクエストフォームに承認を追加する

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。

この記事では、ワークスペースマネージャーがレコードタイプに関連付けられたリクエストフォームに承認を追加する方法について説明します。

Adobe Workfront Planning でのリクエストフォームの作成について詳しくは、[Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

レコードを作成するレコード・タイプにリクエストを発行する方法は、「レコードを作成するためのAdobe Workfront Planning リクエストの発行 [&#x200B; を参照してください &#x200B;](/help/quicksilver/planning/requests/submit-requests.md)。

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
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </td>

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
   <li><p>ワークスペースに対する権限とレコードタイプの管理</p></li>
    <li><p>システム管理者は、自分が作成していないワークスペースを管理できます。 </p></li>
    </ul>
   <p>Workfront Planning オブジェクトの共有権限について詳しくは、
<a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning での共有権限の概要</a>を参照してください。 
  </td>
  </tr>

</tbody>
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストフォームへの承認の追加に関する考慮事項

* リクエストフォームには、1 人または複数の承認者を追加できます。 承認者として追加できるのはユーザーのみです。
* <span class="preview"> リクエストフォームを送信することで作成されたレコードの承認者情報を、承認者情報および承認日フィールドに表示することができます。 詳しくは、[&#x200B; フィールドの作成 &#x200B;](/help/quicksilver/planning/fields/create-fields.md).</span> を参照してください。
* リクエストフォームに複数の承認者を追加する場合、Workfront Planning でレコードを作成する前に、すべての承認者がリクエストを承認する必要があります。
* すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプに対してレコードが作成されます。
* 少なくとも 1 人の承認者がリクエストを拒否し、他の全員がそのリクエストを承認した場合、Workfrontの「リクエスト」領域に対してリクエストが作成されますが、リクエストフォームに関連付けられたレコードタイプに対しては、レコードが作成されません。
* リクエストフォームへの承認の追加はオプションです。 リクエストフォームが承認と関連付けられていない場合、リクエストの送信時にWorkfront Planning によって即座にレコードが作成されます。

## リクエストフォームへの承認の追加

1. [Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. **設定** をクリックします。

   **設定** 領域が表示されます。

   ![&#x200B; 「設定」タブ &#x200B;](assets/configuration-tab.png)
1. 「**承認者**」フィールドで、ドロップダウンアイコンをクリックし、リストで 1 人または複数のユーザー <span class="preview"> またはチーム </span> を選択します

   または

   承認者として設定するユーザー <span class="preview"> またはチーム </span> の名前の入力を開始し、リストに表示されたら選択します。

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* リクエストフォームには、1 人または複数の承認者を追加できます。
   >
   >* 複数の承認者を追加する場合は、Workfront Planning でレコードを作成する前に、すべての承認者がリクエストを承認する必要があります。
   >
   >* 少なくとも 1 人の承認者が要求を拒否した場合、要求は拒否され、レコードは作成されません。 リクエストは、Workfrontの「リクエスト」領域にある「送信済み」セクションの「計画」タブに残ります。
   >
   >* すべての承認者は、リクエストが承認または却下される前に決定を行う必要があります。
   >
   >* <span class="preview"> チームが承認者として設定されている場合、チームからの決定は 1 つだけ必要です。</span>


1. （任意）リクエストフォームを共有したことがない場合は、「**公開**」をクリックします

   または

   「**共有**」をクリックしてフォームを共有し、「**リンクをコピー**」をクリックします。
1. （任意）ユーザーが共有リンクを使用してリクエストを送信すると、Workfront Planning からアプリ内承認通知とメールが承認者に送信されます。

   >[!NOTE]
   >
   >   組織のWorkfront インスタンスは、ユーザーがメールおよびアプリ内通知を受信できるように、Adobe統合エクスペリエンスにオンボーディングされている必要があります。


   リクエストの承認について詳しくは、[&#x200B; リクエストの承認 &#x200B;](/help/quicksilver/planning/requests/approve-request.md) を参照してください。
