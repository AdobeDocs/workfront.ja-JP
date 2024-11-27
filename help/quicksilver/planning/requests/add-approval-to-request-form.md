---
title: リクエストフォームに承認を追加
description: Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 24%

---


<!--

---
title: Add an Approval to a Request Form
description: You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->

# リクエストフォームへの承認の追加

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。

この記事では、ワークスペースマネージャーがレコードタイプに関連付けられたリクエストフォームに承認を追加する方法について説明します。

Adobe Workfront Planning でのリクエストフォームの作成について詳しくは、[Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

レコードを作成するレコード・タイプにリクエストを発行する方法は、「レコードを作成するためのAdobe Workfront Planning リクエストの発行 [ を参照してください ](/help/quicksilver/planning/requests/submit-requests.md)。

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

## リクエストフォームへの承認の追加に関する考慮事項

* リクエストフォームには、1 人または複数の承認者を追加できます。 承認者として追加できるのはユーザーのみです。
* リクエストフォームに複数の承認者を追加する場合、Workfront Planning でレコードを作成する前に、すべての承認者がリクエストを承認する必要があります。
* リクエストフォームへの承認の追加はオプションです。 リクエストフォームが承認と関連付けられていない場合、リクエストの送信時にWorkfront Planning によって即座にレコードが作成されます。

## リクエストフォームへの承認の追加

1. [Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. **設定** をクリックします。

   **設定** 領域が表示されます。

   ![](assets/configuration-tab.png)
1. **承認者** フィールドで、ドロップダウンアイコンをクリックし、リストで 1 つまたは複数の名前を選択します

   または

   承認者の名前の入力を開始し、リストに表示されたら選択します。

   >[!TIP]
   >
   >    複数の承認者を追加する場合は、Workfront Planning でレコードを作成する前に、すべての承認者がリクエストを承認する必要があります。

1. （任意）これまでにリクエストフォームを共有したことがない場合は **** Publish} をクリックします

   または

   「**共有**」をクリックしてフォームを共有し、「**リンクをコピー**」をクリックします。
1. （任意）ユーザーが共有リンクを使用してリクエストを送信すると、Workfront Planning から承認者に承認通知とメールが送信されます。

   リクエストの承認について詳しくは、[ リクエストの承認 ](/help/quicksilver/planning/requests/approve-request.md) を参照してください。

