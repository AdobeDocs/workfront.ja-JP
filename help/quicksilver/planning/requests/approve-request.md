---
title: Adobe Workfront Planning で要求を承認する
description: Adobe Workfront Planning で、ユーザーが承認に関連付けられた要求フォームに要求を送信すると、承認者に承認保留中の承認に関する通知と電子メールが届きます。 Workfront Planning がオブジェクトを作成する前に、顧客がリクエストを承認する必要があります。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: e69209f449ba1643667135c3a0137b93c6171ef8
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 7%

---

# Adobe Workfront Planning でリクエストを承認する

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning で、ユーザーが承認に関連付けられた要求フォームに要求を送信すると、承認者に承認保留中の承認に関する通知と電子メールが届きます。 Workfront Planning がオブジェクトを作成する前に、顧客がリクエストを承認する必要があります。

この記事では、Workfront Planning に送信されたリクエストを Workspace Manager で承認してレコードを作成する方法について説明します。

次の記事も参照することをお勧めします。

* [Adobe Workfront Planning でのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)
* [レコードを作成するためのAdobe Workfront Planning 要求の発行](/help/quicksilver/planning/requests/submit-requests.md)
* [リクエストフォームへの承認の追加](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## リクエストの承認に関する考慮事項

* 送信されたリクエストは、Workfrontの「リクエスト」領域の「送信済み」セクションの「計画」タブに、次のいずれかのリクエストステータスで表示されます。

   * **レビュー保留中**：このステータスは、どの承認者もリクエストオブジェクトを開いていない場合に表示されます。
   * **レビュー中**：少なくとも 1 人の承認者がリクエストオブジェクトを開くと、**レビュー待ち** のステータスが **レビュー中** に変わります。 すべての承認者がリクエストを承認するまで、リクエストのステータスは **レビュー中** のままです。
   * **承認済み**：承認者が要求オブジェクトを承認すると、個々のステータスは **承認済み** になりますが、要求全体のステータスは、すべての承認者が決定するまで **レビュー中** のままです。 すべての承認者がリクエストを承認すると、リクエストのステータスは **承認済み** になります。
   * **完了**：すべての承認者が要求オブジェクトを承認すると、その状態は **完了** に変わります。または、要求に承認が必要なかった場合も同様です。
   * **却下**：承認者がリクエストオブジェクトを却下した場合、ステータスは **却下** になります。 レコードは作成されません。レコードを作成するには、新しいリクエストを送信する必要があります。

* <span class="preview"> リクエストフォームを送信することで作成されたレコードの承認者情報を、承認者情報および承認日フィールドに表示することができます。 詳しくは、[ フィールドの作成 ](/help/quicksilver/planning/fields/create-fields.md).</span> を参照してください。

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
<ul><li><p>任意のWorkfront パッケージ</p></li>
And
<li><p>任意の計画パッケージ</p></li></ul>
または
<ul><li><p>任意のワークフローパッケージ</p></li>
And
<li><p>任意の計画パッケージ</p></li></ul>
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## レコード作成リクエストの承認

ユーザーが承認に関連付けられたレコードタイプのリクエストフォームにリクエストを追加すると、リクエストが承認者に送信されます。

承認者は、承認待ちの要求に関する次の通知を受信します。

* アプリ内通知
* メール通知

>[!NOTE]
>
>組織のWorkfront インスタンスは、ユーザーがメールおよびアプリ内通知を受信できるように、Adobe統合エクスペリエンスにオンボーディングされている必要があります。

リクエストを承認するには：

1. 次のいずれかの操作を行います。

   * Workfront Planning へのアクセス権を持ち、少なくとも 1 つの作業領域を表示できる場合、画面の右上隅にある **メインメニュー**![ ドットのメインメニュー ](assets/dots-menu.png) または左上隅にある **メインメニュー**![ ラインのメインメニュー ](assets/lines-menu.png) をクリックし、**要求**/**送信済み**/**計画** をクリックし、**レビュー保留中** または **レビュー中** のステータスで要求をクリックします。

     >[!TIP]
     >
     >Workfront Planning へのアクセス権がない場合、またはワークスペースを表示するアクセス権がない場合は、メールまたはアプリ内通知を使用して承認するリクエストにのみアクセスできます。

   * 画面の右上隅にある「**通知**」領域アイコン ![ 統合シェルの通知領域アイコン ](assets/notifications-area-icon-unified-shell.png) をクリックし、承認待ちの要求に関する通知をクリックして要求を開きます。
   * 承認待ちのリクエストを通知するメール内のメール通知に移動し、「**リクエストを開く**」をクリックしてリクエストを開きます。<!--add the name of the button here, from the email-->

   リクエストページが読み取り専用モードで開きます。

   ![ レビューステータスの読み取り専用リクエストページ ](assets/read-only-reqeust-page-in-review-status.png)

1. （任意）リクエストの右上隅にある **承認** アイコン ![ 承認アイコン ](assets/approvals-icon.png) をクリックして、承認者を表示します。
1. 「**レビューして承認**」をクリックして、次のいずれかを選択します。

   * **承認**：リクエストを承認します。 すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプのレコードが直ちに作成されます。
   * **却下**：自分が唯一の承認者である場合でも、リクエストを却下します。 リクエストフォームに関連付けられたレコードタイプのレコードは作成されません。

   リクエストを送信したユーザーは、リクエストが承認または却下されると、メールとアプリ内通知を受け取ります。

   承認の決定に応じて、リクエストのステータスが次のように変わります。

   * **完了**：リクエストは承認されました。
   * **却下**：リクエストが却下されました。

   リクエストは、Workfrontの「リクエスト」領域にある「送信済み」セクションの「計画」タブに残ります。
