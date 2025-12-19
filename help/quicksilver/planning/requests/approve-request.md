---
title: Adobe Workfront Planning で要求を承認する
description: Adobe Workfront Planning で、ユーザーが承認に関連付けられた要求フォームに要求を送信すると、承認者に承認保留中の承認に関する通知と電子メールが届きます。 Workfront Planning がオブジェクトを作成する前に、顧客がリクエストを承認する必要があります。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '1103'
ht-degree: 7%

---

# Adobe Workfront Planning でリクエストを承認する

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning で、ユーザーが承認に関連付けられた要求フォームに要求を送信すると、承認者に承認保留中の承認に関する通知と電子メールが届きます。 Workfront Planning がオブジェクトを作成する前に、顧客がリクエストを承認する必要があります。

この記事では、Workfront Planning に送信されたリクエストを Workspace Manager で承認してレコードを作成する方法について説明します。

次の記事も参照することをお勧めします。

* [Adobe Workfront Planning でのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)
* [レコードを作成するためのAdobe Workfront Planning 要求の発行](/help/quicksilver/planning/requests/submit-requests.md)
* [リクエストフォームへの承認の追加](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## リクエストの承認に関する考慮事項

* 送信されたリクエストは、Workfrontの「リクエスト」領域に次のいずれかのリクエストステータスで表示されます。

   * **レビュー保留中**：このステータスは、どの承認者もリクエストオブジェクトを開いていない場合に表示されます。
   * **レビュー中**：少なくとも 1 人の承認者がリクエストオブジェクトを開くと、**レビュー待ち** のステータスが **レビュー中** に変わります。 すべての承認者がリクエストを承認するまで、リクエストのステータスは **レビュー中** のままです。
   * **承認済み**：承認者が要求オブジェクトを承認すると、個々のステータスは **承認済み** になりますが、要求全体のステータスは、すべての承認者が決定するまで **レビュー中** のままです。 すべての承認者がリクエストを承認すると、リクエストのステータスは **承認済み** になります。
   * **完了**：すべての承認者が要求オブジェクトを承認すると、その状態は **完了** に変わります。または、要求に承認が必要なかった場合も同様です。
   * **却下**：承認者がリクエストオブジェクトを却下した場合、ステータスは **却下** になります。 レコードは作成されません。レコードを作成するには、新しいリクエストを送信する必要があります。

* リクエストフォームを送信して作成したレコードの承認情報を、「承認者」および「承認日」フィールドに表示できます。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

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
   <td><p>任意</p> 
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

## レコード作成リクエストの承認

ユーザーが承認に関連付けられたレコードタイプのリクエストフォームにリクエストを追加すると、リクエストが承認者に送信されます。

承認者は、承認待ちの要求に関する次の通知を受信します。

* アプリ内通知
* メール通知

>[!NOTE]
>
>組織のWorkfront インスタンスは、ユーザーがメールおよびアプリ内通知を受信できるように、Adobe統合エクスペリエンスにオンボーディングされている必要があります。

作成レコードをリクエスト自体または <span class="preview"> ホームの自分の承認ウィジェット </span> からリクエストを承認できます。

* [Workfront Planning の要求からの要求を承認する](#approve-a-request-from-the-request-in-workfront-planning)
* [ホームの承認ウィジェットからのリクエストを承認](#approve-a-request-from-the-my-approvals-widget-in-home)

### Workfront Planning の要求からの要求を承認する

1. （条件付き）従来のWorkfrontのリクエストエクスペリエンスを使用している場合は、次のいずれかの操作を行ってリクエストを開きます。

   * Workfront Planning へのアクセス権を持ち、少なくとも 1 つの作業領域を表示できる場合、画面の右上隅にある **メインメニュー**![&#x200B; ドットのメインメニュー &#x200B;](assets/dots-menu.png) または左上隅にある **メインメニュー**![&#x200B; ラインのメインメニュー &#x200B;](assets/lines-menu.png) をクリックし、**要求**/**送信済み**/**計画** をクリックし、**レビュー保留中** または **レビュー中** のステータスで要求をクリックします。

     >[!TIP]
     >
     >Workfront Planning へのアクセス権がない場合、またはワークスペースを表示するアクセス権がない場合は、メールまたはアプリ内通知を使用して承認するリクエストにのみアクセスできます。

   * 画面の右上隅にある「**通知**」領域アイコン ![&#x200B; 統合シェルの通知領域アイコン &#x200B;](assets/notifications-area-icon-unified-shell.png) をクリックし、承認待ちの要求に関する通知をクリックして要求を開きます。
   * 承認待ちのリクエストを通知するメール内のメール通知に移動し、「**リクエストを開く**」をクリックしてリクエストを開きます。<!--add the name of the button here, from the email-->

   リクエストページが読み取り専用モードで開きます。

   ![&#x200B; レビューステータスの読み取り専用リクエストページ &#x200B;](assets/read-only-reqeust-page-in-review-status.png)
1. Workfrontで新しい要求操作を使用している場合、画面の右上隅にある **メインメニュー**![&#x200B; ドットメインメニュー &#x200B;](assets/dots-menu.png) をクリックするか、または左上隅にある **メインメニュー**![&#x200B; ラインメインメニュー &#x200B;](assets/lines-menu.png) をクリックします（使用可能な場合）。**要求** をクリックし、承認待ちの状態で **レビュー保留中** にする要求をクリックします。
1. （任意）リクエストの右上隅にある **承認** アイコン ![&#x200B; 承認アイコン &#x200B;](assets/approvals-icon.png) をクリックして、承認者を表示します。
1. 「**レビューして承認**」をクリックして、次のいずれかを選択します。

   * **承認**：リクエストを承認します。 すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプのレコードが直ちに作成されます。
   * **却下**：自分が唯一の承認者である場合でも、リクエストを却下します。 リクエストフォームに関連付けられたレコードタイプのレコードは作成されません。

   リクエストを送信したユーザーは、リクエストが承認または却下されると、メールとアプリ内通知を受け取ります。

   承認の決定に応じて、リクエストのステータスが次のように変わります。

   * **完了**：リクエストは承認されました。
   * **却下**：リクエストが却下されました。

   リクエストは、Workfrontのリクエスト エリアに残ります。

<div class="preview">

### ホームの承認ウィジェットからのリクエストを承認

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![&#x200B; メインメニュー &#x200B;](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL ホーム]**」の順にクリックします。

   または

   Adobe Workfrontの左上隅にある [!UICONTROL &#x200B; ホーム &#x200B;] アイコン ![&#x200B; ホームアイコン &#x200B;](/help/_includes/assets/home-icon-30x29.png) をクリックし、自分の承認ウィジェットを見つけます。

1. 承認または却下するオブジェクトを見つけます。

1. （オプション）コメントを追加するには、「承認」または「却下」の横のドロップダウン矢印をクリックし、メモを入力して「追加」をクリックします。

1. 以下のうちのいずれかを選択します。

   * **承認**：リクエストを承認します。 すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプのレコードが直ちに作成されます。
   * **却下**：自分が唯一の承認者である場合でも、リクエストを却下します。 リクエストフォームに関連付けられたレコードタイプのレコードは作成されません。

   リクエストを送信したユーザーは、リクエストが承認または却下されると、メールとアプリ内通知を受け取ります。

   承認の決定に応じて、リクエストのステータスが次のように変わります。

   * **完了**：リクエストは承認されました。
   * **却下**：リクエストが却下されました。

</div>
