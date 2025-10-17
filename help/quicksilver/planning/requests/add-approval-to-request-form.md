---
title: Adobe Workfront Planning の要求フォームへの承認の追加
description: Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: df0686038adb1278339e872e122a311884cb6d29
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 4%

---

# Adobe Workfront Planning でリクエストフォームに承認を追加する

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planning のリクエスト・フォームに承認プロセスを追加して、レコードを作成する前に、送信されたすべてのリクエストに対して承認を開始できます。

この記事では、ワークスペースマネージャーがレコードタイプに関連付けられたリクエストフォームに承認を追加する方法について説明します。

Adobe Workfront Planning でのリクエストフォームの作成について詳しくは、[Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

レコードを作成するレコード・タイプにリクエストを発行する方法は、「レコードを作成するためのAdobe Workfront Planning リクエストの発行 [&#x200B; を参照してください &#x200B;](/help/quicksilver/planning/requests/submit-requests.md)。

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

## リクエストフォームへの承認の追加に関する考慮事項

* リクエストフォームには、1 人または複数の承認者を追加できます。 承認者として追加できるのはユーザーのみです。
* リクエストフォームを送信して作成したレコードの承認情報を、「承認者」および「承認日」フィールドに表示できます。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。
* リクエストフォームに複数の承認者を追加する場合、Workfront Planning でレコードを作成する前に、すべての承認者がリクエストを承認する必要があります。
* すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプに対してレコードが作成されます。
* 少なくとも 1 人の承認者がリクエストを拒否し、他の全員がそのリクエストを承認した場合、Workfrontの「リクエスト」領域に対してリクエストが作成されますが、リクエストフォームに関連付けられたレコードタイプに対しては、レコードが作成されません。
* リクエストフォームへの承認の追加はオプションです。 リクエストフォームが承認と関連付けられていない場合、リクエストの送信時にWorkfront Planning によって即座にレコードが作成されます。

## リクエストフォームへの承認の追加

1. [Adobe Workfront Planning でのリクエストフォームの作成と管理 &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) の説明に従って、レコードタイプのリクエストフォームの作成を開始します。
1. **設定** をクリックします。

   **設定** 領域が表示されます。

   ![&#x200B; 「設定」タブ &#x200B;](assets/configuration-tab.png)
1. 「**承認者**」フィールドで、ドロップダウンアイコンをクリックし、リストで 1 人または複数のユーザーまたはチームを選択します

   または

   承認者として設定するユーザーまたはチームの名前の入力を開始し、リストに表示されたら選択します。

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
   >* チームが承認者として設定されている場合、チームからの決定は 1 つだけ必要です。


1. （任意）リクエストフォームを共有したことがない場合は、「**公開**」をクリックします

   または

   「**共有**」をクリックしてフォームを共有し、「**リンクをコピー**」をクリックします。
1. （任意）ユーザーが共有リンクを使用してリクエストを送信すると、Workfront Planning からアプリ内承認通知とメールが承認者に送信されます。

   >[!NOTE]
   >
   >   組織のWorkfront インスタンスは、ユーザーがメールおよびアプリ内通知を受信できるように、Adobe統合エクスペリエンスにオンボーディングされている必要があります。


   リクエストの承認について詳しくは、[&#x200B; リクエストの承認 &#x200B;](/help/quicksilver/planning/requests/approve-request.md) を参照してください。
