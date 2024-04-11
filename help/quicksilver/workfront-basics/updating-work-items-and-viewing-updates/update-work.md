---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 作業の更新
description: Adobe Workfront オブジェクト（プロジェクト、タスクまたはイシュー）に更新を追加して、オブジェクトの進行状況を伝えることができます。更新を表示できるのは、オブジェクトに割り当てられているまたは登録しているユーザーです。またユーザーにタグ付けして、更新に注意を向けさせることもできます。
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: c6575c832fa21a17a1d20fa7e92798d970ca0f50
workflow-type: tm+mt
source-wordcount: '2974'
ht-degree: 86%

---

# 作業の更新

<!-- Audited: 1/2024 -->

<!--info for April 11: take "legacy" and "new commenting" references out when we remove the legacy-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

<!--info for April 11: hide the "Important" box below-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span>
-->

Adobe Workfront オブジェクトに更新を追加して、オブジェクトの進行状況を伝えることができます。 Workfrontで更新を追加できるオブジェクトについて詳しくは、以下を参照してください。 [アップデートセクションの概要](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

この記事の情報では、プロジェクト、タスクおよび問題の情報をコメントして更新する方法について説明します。 更新を表示できるのは、オブジェクトに割り当てられているまたは登録しているユーザーです。またユーザーにタグ付けして、更新に注意を向けさせることもできます。

他のオブジェクトにコメントを追加することは、プロジェクト、タスク、イシューの更新と似ています。 カード、目標、イテレーションに対するコメントについて詳しくは、次の記事も参照してください。

* [Adobe Workfront Goals での目標コメントの管理](../../workfront-goals/goal-management/manage-goal-comments.md).

  Workfront Goals にアクセスするには、追加のライセンスが必要です。

* [ボードへのアドホックカードの追加](../../agile/get-started-with-boards/add-card-to-board.md)

* [反復コメントの管理](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md)



## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス</strong></td> 
   <td> 
   <p>現在：イシューとドキュメントについてはリクエスト以上、その他のすべてのオブジェクトについてはレビュー以上</p>
   <p>新規：イシューとドキュメントについてはコントリビューター以上、その他のすべてのオブジェクトについてはライト以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>更新先のオブジェクトに対する表示または編集アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトに対する表示アクセス権</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 作業の更新に関する考慮事項

* 「更新」セクションでは、Adobe Workfront のほとんどのオブジェクトにコメントを追加できます。「更新」セクションが表示される Workfront オブジェクトについて詳しくは、[「更新」セクションの概要](../updating-work-items-and-viewing-updates/updates-tab-overview.md)を参照してください。

* Workfront と統合されている他のアプリケーションや Workfront モバイルアプリから、Workfront オブジェクトにコメントを追加できます。

  Workfront と統合されているすべてのアプリケーションに、Workfront オブジェクトへのコメント追加機能があるわけではありません。

  アプリケーションから Workfront オブジェクトにアクセスする場合、Workfront のオブジェクトの「更新」セクションで使用できるすべての機能が他のアプリケーションでも使用できるわけではありません。例えば、サードパーティのアプリケーションから Workfront オブジェクトにコメントを追加する場合は、リッチテキスト機能を利用したりコメントを会社に非公開にしたりすることができない可能性があります。

* オブジェクトにコメントを付ける際に、Workfront オブジェクト（プロジェクト、タスクまたはイシュー）の進行状況を伝えることができます。オブジェクトに割り当てられているまたは登録しているユーザーは、更新に関する通知を受け取ることができます。オブジェクトへの表示アクセス権を持つユーザーは誰でも、更新を表示できます。

* ユーザーにタグ付けして、更新に注意を向けさせることができます。タグ付きユーザーには、更新に関するアプリ内通知とメールが届きます。

  >[!TIP]
  >
  >コメントの所有者は自動的にタグ付けされます。 詳しくは、[更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。


* 表示可能なオブジェクトにコメントを追加したり、Workfront 管理者またはグループ管理者としてログインして、別のユーザーの代わりにコメントを追加したりできます。詳しくは、[別のユーザーとしてのログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)を参照してください。

* Workfront の次のエリアから、プロジェクト、タスクおよびイシューに更新を追加できます。

   * Workfront オブジェクトから、「更新」セクションで（プロジェクト、タスク、および問題用）
   * ホームエリアから（タスクおよびイシューの場合）
   * 次の領域の概要パネルから（タスクおよび問題に対して）:

      * オブジェクトのリスト
      * タイムシート
      * ホーム
      * ワークロードバランサー

<!--info for April 11: hide the section below: add an update to a work item-->

<!--
## Add an update to a work item

Adding an update to a work item differs depending on what version of the Updates section you use.

You can add updates to the following objects: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--info for April 11: hide the section below completely:-->

<!--
### Add an update to a work item in the legacy Updates section

>[!IMPORTANT]
>
>The information on this page describes how you update projects, tasks, and issues.

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. (Conditional) If it is enabled, click the **New commenting** option in the upper-right corner of the Updates section to disable it and enable the legacy commenting experience.
1. Click **Start a new update,** then type your update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the [Use Rich Text in a Workfront update](#use-rich-text-in-a-workfront-update) section in this article.
1. (Optional) Update any of the following information about the work item:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who must be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> 
      <p><b>NOTE</b></p>
      <p>This option displays only when the user is associated with a Company.</p>
      <p>This option is not available in all areas where you can add updates from. For example, this is not available in third-party applications where you can add updates from. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update is posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
-->

<!--info for April 11: reword the title of this section to: "Add an update to a work item"; take out the step that says you need to enable the "New commenting" toggle (I think it is step 3??)-->

## 作業項目に更新を追加 <!--using the new commenting experience-->

1. 更新するオブジェクト（プロジェクト、タスク、イシュー）を見つけ、その名前をクリックしてそのオブジェクトのページを開きます。
1. クリック  **更新** 左側のパネルで次の操作を行います。
デフォルトでは、「**コメント**」タブが選択されています。

<!--
1. (Conditional) If the **New commenting** option is disabled, click to enable it. 

   This enables the new commenting experience. 

      >[!TIP]
      >
      ><span class="preview">The New commenting option has been removed in the Preview environment.</span>
-->

1. **新しいコメント**&#x200B;ボックスにコメントを入力します。

   ![「新しいコメント」ボックス](assets/comment-box-all-tabs.png)

   >[!TIP]
   >
   >コメント入力を完了して送信する前に更新セクションから移動すると、ログオフしてログオンし直した後でも、ページ上のコメントがドラフトモードのままになっています。コメントに追加された画像も下書きに保存されます。ドラフトは 7 日間保存され、その後は破棄され、復元できません。下書きのコメントは、入力したユーザーのみに表示されます。

1. （オプション）変更の取り消しまたはやり直しを行うには、以下のショートカットキーを使用します。
   * Ctrl + Z（Mac の場合は ⌘+z）で、変更を元に戻します
   * Ctrl + Y（Mac の場合は ⌘+y）で、変更をやり直します

1. （オプション）**担当者またはチームのタグ付け**&#x200B;エリアで、このコメントに含めるユーザーまたはチームの名前やメールを入力して、リストに表示されたら選択します。
1. （オプション）リッチテキストツールバーのオプションを使用すると、テキストの書式設定や、更新への絵文字、リンクまたは画像の追加を行って、コンテンツを拡充できます。詳しくは、[Workfront の更新でリッチテキストを使用](#use-rich-text-in-a-workfront-update)の節を参照してください。

   >[!TIP]
   >
   >更新中のアイテムに別のユーザーがコメントを送信した場合、「新規」インジケーターと赤い線が表示され、新しいコメントが通知されます。
   >
   >インジケーターは、コメントが項目に送信された後にのみ表示され、コメントがまだ構成されている場合は表示されません。
   >
   >「新規」インジケーターは、新しい更新を入力したユーザーと、現在更新を入力しているユーザーの両方が新しいコメント機能のエクスペリエンスを使用している場合にのみ表示されます。
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. 「**送信**」をクリックして、Workfront オブジェクトに更新を追加します。
1. （オプション）コメントを編集するには、コメントの右上隅にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックして、「**編集**」をクリックします。

   >[!IMPORTANT]
   >
   >コメントは送信後の 15 分間のみ編集できます。

1. コメント内の情報の編集、画像の追加や削除、タグ付きユーザーの削除を行います。コメントの入力時に表示される日付スタンプの左側に、「編集済み」インジケーターが追加されます。

   >[!TIP]
   >
   >当年からのコメントでは、日付スタンプに年は表示されません。タイムスタンプにポインタを合わせると、年を含む完全な日付が表示されます。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* 元の更新を送信した場合にのみ、ユーザーに更新を通知するメールが生成されます。更新を編集した後は、メールは生成されません。
   >* コメントの横の日付スタンプは、最後の編集の日付ではなく、元のコメントの日付です。
   >* 別のユーザーの代わりにコメントを追加する際（Workfront またはグループ管理者が別のユーザーとしてログインしている場合）、他のユーザーとしてログインしている場合は、コメントを編集できません。コメントを編集するには、そのユーザーとしてログアウトし、自分自身として再度ログインする必要があります。

1. （任意）クリック **返信** または、でコメントの入力を開始します **返信を追加…** 既存のコメントに返信するには、上記の手順 3～7 に従います。 <!--(**************insure this stays accurate***********)--> 更新への返信について詳しくは、[更新に返信](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md)を参照してください。

1. （条件付きおよびオプション）コメントを追加している間に、「更新」セクションの表示エリアの外側に表示されるコメントを他のユーザーが追加した場合は、画面下部の青い&#x200B;**新しいコメントバナー**&#x200B;内の「**表示**」をクリックして、これらのコメントを表示します。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   追加のコメントが画面の下部に表示されます。

   >[!NOTE]
   >
   >   「新しいコメント」インジケーターと「表示」ボタンは、新しい更新を入力したユーザーと、現在「更新」セクションを表示しているユーザーの両方が新しいコメント機能のエクスペリエンスを使用している場合にのみ表示されます。

1. （オプション）**いいね！**&#x200B;アイコン ![](assets/like-icon.png) をクリックします。アイコンは「いいね！」の数に応じて更新されます。
1. （条件付きおよびオプション）コメントに追加のユーザーを含める場合は、更新に含まれるメンバーの数をクリックして、入力したコメントが共有されているエンティティのリストを表示します。

   ![](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >最初の 2 つのタグ付きエンティティの名前が、アバターの横に表示されます。3 つ以上のエンティティがタグ付けされている場合は、最初のエンティティの名前と追加エンティティの数のみが表示されます。

1. （オプション）コミュニケーターの名前をクリックして、名前、役割、メールアドレスを情報ボックスに表示します。 情報ボックスでコミュニケーターの名前を再度クリックして、ユーザープロファイルを開きます。
1. （オプション）「**システムアクティビティ**」タブをクリックして、システムによって記録された更新を表示します。オブジェクトまたはその子のいずれかが更新されると、Workfront はその更新に関するメモを生成し、「システムアクティビティ」タブに表示します。

   詳しくは、[「更新」セクションの概要](../updating-work-items-and-viewing-updates/updates-tab-overview.md)を参照してください。

   >[!TIP]
   >
   >システムの更新にコメントを追加することはできません。 ただし、従来のコメントエクスペリエンスのシステムアクティビティレコードに対して行われた返信は、読み取り専用として「システムアクティビティ」タブに入力されます。

1. （任意） **すべて** tab キーを押すと、ユーザーコメントとシステムアクティビティコメントの両方が 1 か所で表示されます。 これは表示のみのタブです。

   >[!TIP]
   >
   >「すべて」タブでは、コメントに返信したり、既存のコメントに他のユーザーをタグ付けしたりすることはできません。「すべて」タブでコメントに返信するには、 **コメントで返信** をクリックして、「コメント」タブでコメントを開きます。

## Workfront の更新にリッチテキストを使用{#use-rich-text-in-a-workfront-update}

リッチテキストを使用したり、絵文字、リンク、画像などの様々な項目を追加したりして、更新内容を強化できます。

1. Workfront オブジェクトの&#x200B;**更新**&#x200B;エリアに移動し、コメントの入力を開始します。
1. （オプション）リッチテキスト書式を更新に追加するには、入力時に&#x200B;**リッチテキスト**&#x200B;ツールバーの属性を使用します。

   ![](assets/rich-text-toolbar.png)

   | **属性** | **ツールバーボタン** | **Mac ショートカットキー** | **Windows ショートカットキー** |
   |---|---|---|---|
   | 太字 | ![](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜体 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 下線 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | ハイパーリンク | ![mceclip7.png](assets/mceclip7.png) | <br>「リンクを追加」ボックスを開くには、⌘ + K を使用します</br> <br>選択したテキストにリンクを貼り付けるには、⌘ + V を使用します</br> | <br>「リンクを追加」ボックスを開くには、Ctrl + K を使用します</br> <br>選択したテキストにリンクを貼り付けるには、Ctrl + V を使用します</br> |
   | 箇条書き | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 番号付きリスト | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   <!--| Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |<br>Ctrl+Shift+9</br> <br>This is not available in the new commenting experience. </br> |-->

   <!--remove the last row when we remove legacy from the system-->

   テキストの書式設定を停止するには、**リッチテキスト**&#x200B;ツールバーで、属性を選択解除します。


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* 書式設定は、ユーザーが受信するメール通知（更新を含む）にも表示されます。
   >* メール内の更新に適用されたリッチテキスト形式は、「更新」タブで表示した場合には、更新に表示されません。
   >* 組織が Internet Explorer でWorkfront を使用している場合、更新に貼り付けた書式設定済のテキストからはリッチテキストの書式が失われ、プレーンテキストとして表示されます。リッチテキストツールバーの属性を使用して、テキストの書式を変更できます。
   >* リッチテキストの書式設定は、レポートで表示されるタイムシートエリアで行われた更新や、メモおよび最終状況オブジェクトの更新には使用できません。

<!--1. (Optional and conditional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting. This is not available in the new commenting experience.-->

<!--remove this picture below and the bullet above when we remove legacy-->

<!--![](assets/block-quote-marked-350x144.png)-->

1. （オプション）**絵文字**&#x200B;アイコン ![](assets/emoji-icon.png) をクリックして、更新に絵文字を追加します。

   >[!NOTE]
   >
   >* Workfront は、:) などの句読点絵文字を絵文字に置き換えません。
   >* レポートに表示されるメモおよび最終状況オブジェクトでは、絵文字は使用できません。
   >* Workfront の絵文字機能では Unicode 文字を使用するため、Unicode コードポイントをサポートするブラウザーとオペレーティングシステムでのみ表示されます。お使いのプラットフォーム、ブラウザー、またはオペレーティングシステムのバージョンが異なるユーザーは、同じ絵文字にアクセスできない場合があります。
   >* サポートされていない絵文字は、黒または白のボックスで表されます。
   >* Windows 7 では、黒と白の絵文字のみがサポートされています。
   >* メールを介して行われた更新に適用される絵文字は、更新エリアに表示されると、更新には表示されません。

1. （オプション）追加の情報ソースに URL リンクを追加するには、以下のように行います。

   1. リンクを挿入するアップデート内をクリックします。
   1. **リッチテキスト**&#x200B;ツールバーで、**ハイパーリンク**&#x200B;アイコン ![](assets/link-icon.png) をクリックします。

   1. **URL** の下に表示される&#x200B;**リンクを作成**&#x200B;ボックスに、リンク先のソースの URL を入力またはペーストします。

   1. **表示するテキスト**&#x200B;で、リンクテキストを入力またはペーストします。
   1. 「**保存**」をクリックします。

1. （オプション）更新に画像を添付するには、次のいずれかの操作を実行します。

   * コンピューター上に画像を保存し、新しいコメントエリアにドラッグ＆ドロップします。
   * コンピューターからスクリーンショットをコピーし、コメントに貼り付けます。<!-- This is not available in the legacy commenting experience.-->
   * **画像を追加**&#x200B;アイコン ![](assets/add-image-mountain-with-plus-icon.png) をクリックし、お使いのコンピューター上で画像を参照します。


   >[!NOTE]
   >
   >* 画像アイコンや、添付ファイルを追加アイコンを表示するには、Workfront 管理者が、画像の追加を Workfront インターフェイスエリアの「フィードの環境設定を更新」セクションで有効にする必要があります。詳しくは、[ユーザーの更新用に環境設定を指定](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)を参照してください。
   >* 画像ファイルの最大サイズは 7 MB です。サポートされる画像ファイルタイプは、.jpg、.gif および .png です。
   >* 画像はオブジェクトの「更新」セクションのほか、メインメニューのドキュメントエリアからもアクセスできます。
   >* 画像を貼り付けるには、新しいコメントを右クリックするか、Windows の場合は Ctrl + V（Mac の場合は ⌘ + V）キーを押します。
   >* 画像は含むがテキストを含まないアップデートを送信できます。
   >* 画像を含むコメントを削除すると、その画像は「更新」セクションと「ドキュメント」領域から削除されます。 コメントを編集して画像を削除すると、その画像もドキュメントエリアから削除されます。
   >* コメントに添付された画像をドキュメントエリアから削除すると、その画像はコメントからも削除されます。

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. （オプション）既存の更新で画像を表示するには、次のいずれかの操作を実行します。

   * 画像のサムネールで&#x200B;**プレビュー**&#x200B;アイコン ![](assets/previewimageicon-31x31.png) をクリックして、フルサイズの画像を新しいブラウザータブで開きます。
   * 画像のサムネールで&#x200B;**ダウンロード**&#x200B;アイコン ![](assets/downloadimageicon.png) をクリックして、画像をダウンロードします。

1. 「**送信**」をクリックして、コメントを追加します。

## 更新の検索

オブジェクトの「更新」セクションで、コメントや返信を検索できます。

1. オブジェクトの「**更新**」セクションに移動します。
1. 「**コメント**」タブの右上隅にある&#x200B;**検索**&#x200B;ボックスにキーワード<!--or a user's name -->を入力していきます。

   <!--Add this tip or note instead of the note below - when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   >[!NOTE]
   >
   >検索できるのは、コメントまたは返信のテキストに含まれている単語のみです。更新でタグ付けされたユーザーやチームの名前は検索できません。

   ![更新での検索](assets/updates-all-tabs-with-search-field.png)

   検索したキーワード<!--or user-->がハイライト表示され、その語を含んだコメントが「更新」セクションの上部に表示されます。

   Workfront は、画面に表示されるコメントの外側にある、オブジェクトの更新ストリーム全体を検索します。

1. 検索フィールドの「**x**」アイコンをクリックすると、検索結果を消去してすべてのコメントに戻ります。

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## 更新情報をコピー

更新をコピーする方法はいくつかあります。リンクをコピーした後、他のユーザーとリンクを共有して、ユーザーを更新に誘導することができます。

<!--Copying an update differs depending on which commenting experience you use.-->

<!--info for April 11: take the sentence above out and reword the section title below to: Copy an update-->

### 更新をコピー <!--in the new commenting experience-->

<!--For information about what features are available for the new commenting experience and for what objects, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).-->

次のいずれかの操作を行うと、既存のコメントから情報をコピーできます。

* [リンクをコピー](#copy-link)
* [本文をコピー](#copy-body-text)
* [引用返信](#quote-reply-1)

![](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### リンクをコピー

「リンクをコピー」オプションでは、コメントやスレッドリンクがクリップボードにコピーされて、コメントや完全なスレッドを他のユーザーと共有できるようになります。

1. リンクをコピーする更新に移動します。

1. **その他**&#x200B;メニュー、「**リンクをコピー**」の順にクリックします。

1. 前の手順でコピーしたリンクをメールまたは他のアプリケーションに貼り付けて、他の人と共有します。共有リンクをクリックすると、リンク元のコメントが開きます。

   >[!TIP]
   >
   >上位オブジェクトから子オブジェクト上の会話のリンクを共有すると、上位オブジェクトの更新エリアでスレッドが開きます。
   >
   >例えば、タスクのコメントのリンクをプロジェクトの更新エリアからコピーすると、プロジェクトページが開きます。

#### 本文をコピー

「本文をコピー」オプションは、特定の更新からのテキストをクリップボードにコピーします。

1. コピーする更新に移動、あるいは返信します。
1. **その他**&#x200B;メニュー、「**本文テキストをコピー**」の順にクリックします。

#### 引用返信

「引用返信」オプションは、元のコメントを新しい返信にブロック引用としてコピーします。

1. コピーする更新に移動、あるいは返信します。
1. **その他**&#x200B;メニューをクリックし、「**引用返信**」をクリックします。

   新しいコメントボックスが開き、引用された返信が新しいコメント内に含まれ、ブロック引用としてマークされます。

   ![](assets/block-quote-highlighted-mid-comment-before-submit.png)

   <!--ensure the screen shot above is correct - missing he block quote icon in rich text -->

1. 更新の追加を続行し、「**送信**」をクリックしてコメントを追加します。

<!--info for April 11: hide the entire section below - notice that there are several sub-sub sections below this main section - hide them all, all the way up to "Delete an update"-->

<!--
### Copy an update in the legacy commenting experience

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)
* [Quote Reply](#quote-reply)

   >[!TIP]
   >
   >When you copy and share the link of a conversation on a child object from a higher-ranking object, the link opens the thread in the child object's Updates area. 
   >
   >For example, if you copy the link of a task comment from the project's Updates area, the comment opens the task page.

#### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.

1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png) 

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/copy-update-link-old-ui.png)

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Quote Reply  

The Quote Reply option copies the original comment to a new reply as a block quote. 

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Quote Reply**.

   A new comment box opens and the quoted reply is included in the new comment and marked as a block quote.

1. Continue adding your update and click **Reply** to add the comment.
-->

## 更新または返信を削除

Workfront 管理者がユーザーに提供するアクセス権によっては、オブジェクトの「更新」タブで追加したアップデートを削除できる場合があります。詳しくは、[カスタムアクセスレベルを作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の記事にある[カスタムアクセスレベルを作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch)を参照してください。

Workfront ユーザー（Workfront 管理者を含む）は、別のユーザーが行った更新を削除できません。ただし、あるユーザーが自身の更新を削除できるアクセスレベルを有している場合、Workfront 管理者はそのユーザーとしてログインして、ユーザーが行った更新を削除できます。詳しくは、[カスタムアクセスレベルを作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch)および[別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)を参照してください。

1. 削除する更新または返信に移動します。
1. 削除する更新または返信の横にある&#x200B;**その他**&#x200B;メニューをクリックしてから、「**削除**」を選択します。<!--October 2023 - replace screen shot here-->

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 表示されるメッセージで、「**削除**」をクリックします。

   >[!NOTE]
   >
   >画像が添付された更新を削除すると、コメントと画像の両方が削除されます。詳しくは、[Workfront の更新でリッチテキストを使用](#use-rich-text-in-a-workfront-update)の節を参照してください。

   削除したコメントに返信が関連付けられている場合は、コメントが削除されたことが、削除したユーザーの名前とともに表示されます。

   ![](assets/removed-comment-indicator-new-experience.png)

   削除したコメントは、Workfront から直ちに消去されます。更新セクションを使用するユーザーには、他のユーザーによるコメントの削除が、リアルタイムで表示されます。


## システム更新の確認

Workfront オブジェクトの更新セクションには、以下の 2 種類の情報が表示されます。

* **ユーザーの更新：** ユーザーの更新は、自分およびシステム内の他のユーザーが入力するコメントです。 ユーザーの更新は、「更新」セクションの「コメント」タブと「すべて」タブに表示されます。

  ![](assets/user-update-cl-350x277.png)

* **システムの更新：** システムは、タスクまたは問題の削除、ドキュメントのバージョンの追加または削除、承認リクエストの添付または削除、およびオブジェクトに対して行われた編集や変更を記録に更新します。 システムの更新は、「システムアクティビティ」と「更新」セクションの「すべて」タブに表示されます。

  ![](assets/system-updates-cl-350x277.png)

  [システムで追跡された更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)で説明されているように、Workfront の管理者は、システム更新で何をトラックするかを決定できます。また、システムの更新やアクティビティを除外して、すべてのオブジェクトのユーザー更新のみを表示することもできます。

  次のオブジェクトには、システムで生成された更新はありません。

   * チーム
   * テンプレート
   * テンプレートタスク
   * アドホックカード

「更新」セクションのシステム更新の詳細については、を参照してください [更新セクションの概要](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->