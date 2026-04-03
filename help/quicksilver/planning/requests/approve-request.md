---
title: Adobe Workfront Planningでのリクエストの承認
description: Adobe Workfront Planningの承認に関連付けられたリクエストフォームにユーザーがリクエストを送信すると、承認者は保留中の承認に関する通知とメールを受け取ります。 Workfront Planningでオブジェクトを作成する前に、リクエストを承認する必要があります。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 8%

---

# Adobe Workfront Planning でのリクエストの承認

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfront Planningの承認に関連付けられたリクエストフォームにユーザーがリクエストを送信すると、承認者は保留中の承認に関する通知とメールを受け取ります。 Workfront Planningでオブジェクトを作成する前に、リクエストを承認する必要があります。

この記事では、Workspace ManagerがWorkfront Planningに送信されたリクエストを承認してレコードを作成する方法について説明します。

次の記事も参照することをお勧めします。

* [Adobe Workfront Planning でのリクエストフォームの作成と管理](/help/quicksilver/planning/requests/create-request-form.md)
* [Adobe Workfront Planning リクエストを送信して、レコードを作成](/help/quicksilver/planning/requests/submit-requests.md)
* [リクエストフォームへの承認の追加](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## リクエストの承認に関する考慮事項

* 送信されたリクエストは、次のいずれかのリクエストステータスを持つWorkfrontのリクエスト領域に表示されます。

   * **レビュー待ち**：このステータスは、承認者のいずれかがリクエストオブジェクトを開いていない場合に表示されます。
   * **レビュー中**：少なくとも1人の承認者がリクエストオブジェクトを開くと、**保留中のレビュー**&#x200B;のステータスが&#x200B;**レビュー中**&#x200B;に変更されます。 すべての承認者がリクエストを承認するまで、リクエストのステータスは&#x200B;**レビュー中**&#x200B;のままです。
   * **承認済み**：承認者がリクエストオブジェクトを承認すると、個々のステータスは&#x200B;**承認済み**&#x200B;になりますが、すべての承認者が決定を行うまで、全体的なリクエストオブジェクトのステータスは&#x200B;**レビュー中**&#x200B;のままです。 すべての承認者がリクエストを承認すると、リクエストのステータスは&#x200B;**Approved**&#x200B;になります。
   * **完了**：すべての承認者がリクエストオブジェクトを承認すると、そのステータスは&#x200B;**完了**&#x200B;に変更されます。または、リクエストに承認が必要なかった場合です。
   * **拒否**：いずれかの承認者が要求オブジェクトを拒否すると、ステータスは&#x200B;**拒否**&#x200B;になります。 レコードは作成されず、レコードを作成するには新しいリクエストを送信する必要があります。

* 「承認者」フィールドと「承認日」フィールドでリクエストフォームを送信して作成したレコードに承認情報を表示できます。 詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

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
<p>任意のWorkfront パッケージと任意のPlanning パッケージ</p>
または
<p>任意のワークフローパッケージと任意のプランニングパッケージ</p>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>任意</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースとレコードタイプ </a>に対する権限を管理 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

## レコードを作成するための計画要求の承認

承認に関連付けられているレコードタイプのリクエストフォームにユーザーがリクエストを追加すると、そのリクエストは承認者に送信されます。

承認者は、承認を保留しているリクエストに関する次の通知を受け取ります。

* アプリ内通知
* メール通知

通知からのリクエストの承認について詳しくは、次の記事を参照してください。

* [Adobe Workfront Planning のメール通知の管理](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)
* [Adobe Workfront Planning のアプリ内通知の管理](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)

>[!NOTE]
>
>組織のWorkfront インスタンスをAdobe Unified Experienceにオンボーディングして、ユーザーがメールやアプリ内の通知を受け取れるようにする必要があります。

リクエスト自体またはホームのMy Approvals ウィジェットからレコードを作成するリクエストを承認できます。

### 通知またはリクエスト領域から計画リクエストを承認します

1. 次のいずれかの操作を行って、リクエストを開きます。

   * 左上隅の&#x200B;**メインメニュー** ![行メインメニュー](assets/lines-menu.png)をクリックし、**リクエスト** > **新しいエクスペリエンスを使用**&#x200B;をクリックし、ステータスが&#x200B;**レビュー待ち**&#x200B;のリクエストをクリックします。

     >[!TIP]
     >
     >* Workfront Planningにアクセスできない場合、またはワークスペースを表示するアクセス権がない場合は、メールまたはアプリ内通知を使用して承認リクエストにのみアクセスできます。
     >* 従来のリクエストエクスペリエンスからPlanning リクエストにアクセスすることはできません。

   * 画面の右上隅にある&#x200B;**通知**&#x200B;領域アイコン ![統合シェル ](assets/notifications-area-icon-unified-shell.png)の通知領域アイコンをクリックし、承認待ちのリクエストに関する通知をクリックしてリクエストを開きます。
   * 承認待ちのリクエストについて通知するメールのメール通知に移動し、「**リクエストを開く**」をクリックしてリクエストを開きます。

   リクエストページが読み取り専用モードで開きます。

   ![ レビューステータスの読み取り専用リクエストページ ](assets/read-only-reqeust-page-in-review-status.png)
1. （オプション）リクエストの右上隅にある&#x200B;**承認** アイコン ![承認アイコン ](assets/approvals-icon.png)をクリックして、承認者を表示します。
1. 「**レビューして承認**」をクリックし、次のいずれかを選択します。

   * **承認**：これにより、リクエストが承認されます。 すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプのレコードがすぐに作成されます。
   * **拒否**：自分が唯一の承認者である場合でも、このリクエストは拒否されます。 リクエストフォームに関連付けられているレコードタイプのレコードは作成されません。

   リクエストを送信したユーザーは、リクエストが承認または拒否されたときに、メールとアプリ内通知を受け取ります。

   リクエストのステータスは、承認の決定に応じて、次のように変更されます。

   * **完了**：リクエストが承認されました。
   * **却下**：要求は拒否されました。

   リクエストは、Workfrontの&#x200B;**リクエスト**&#x200B;領域に残ります。

### ホームのマイ承認ウィジェットからリクエストを承認する

{{step1-to-home}}

1. **ホーム**&#x200B;の&#x200B;**マイ承認** ウィジェットに移動します。

   ![ ホームの自分の承認ウィジェット ](assets/my-approvals-widget-in-home.png)
1. 承認または却下する計画リクエストを探します。

1. （オプション）コメントを追加するには、**承認**&#x200B;または&#x200B;**却下**&#x200B;の横にあるドロップダウン矢印をクリックし、メモに入力して、**追加**&#x200B;をクリックします。

1. 次のいずれかをクリックします。

   * **承認**：これにより、リクエストが承認されます。 すべての承認者がリクエストを承認すると、リクエストフォームに関連付けられたレコードタイプのレコードがすぐに作成されます。
   * **拒否**：自分が唯一の承認者である場合でも、このリクエストは拒否されます。 リクエストフォームに関連付けられているレコードタイプのレコードは作成されません。

   リクエストを送信したユーザーは、リクエストが承認または拒否されたときに、メールとアプリ内通知を受け取ります。

   リクエストのステータスは、承認の決定に応じて、次のように変更されます。

   * **完了**：リクエストが承認されました。
   * **却下**：要求は拒否されました。

