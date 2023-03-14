---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 作業を更新
description: Adobe Workfrontオブジェクト（プロジェクト、タスクまたはイシュー）に更新を追加して、オブジェクトの進行状況を伝えることができます。 オブジェクトを割り当てられた、またはサブスクライブしたユーザーは、更新を表示できます。 また、ユーザーにタグを付けて、更新に注意を向けることもできます。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '1774'
ht-degree: 1%

---

# 作業を更新

<!-- Drafted for commenting experience: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for a limited number of objects.</span> -->

Adobe Workfrontオブジェクト（プロジェクト、タスクまたはイシュー）に更新を追加して、オブジェクトの進行状況を伝えることができます。 オブジェクトを割り当てられた、またはサブスクライブしたユーザーは、更新を表示できます。 また、ユーザーにタグを付けて、更新に注意を向けることもできます。

Workfrontの次の領域で、オブジェクトに更新を追加できます。

* Workfrontオブジェクトの「更新」セクションで、
* 「ホーム」領域から（タスクおよび問題について）
* オブジェクトのリスト内の Summary パネルから（タスクと問題に関して）
* タイムシートから（タスクとタスクの場合）

## アクセス要件

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>問題およびドキュメントの要求以上その他のすべてのオブジェクトを確認するか、それ以上の値を設定します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>更新先のオブジェクトのアクセスを表示または編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 作業項目に更新を追加する

<!--drafted for the commenting experience - change the NOTE at the top of this paragraph with every new release to other objects

Adding an update to a work item differs depending on what environment and what object you choose. 

### Add an update to a work item in the Production environment

>[!NOTE]
>
>The following functionality is available for all objects except for goals, in the Production and Preview environments. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md)

-->

1. 更新を行う作業項目（プロジェクト、タスク、タスクなど）に移動します。
1. 次をクリック： **更新** 」セクションに入力します。
1. クリック **新しい更新を開始し、** 次に、更新を入力します。

1. （オプション）リッチテキストの書式設定を更新に追加するには、 **リッチテキスト** ツールバーを使用します。

   | **属性** | **ツールバーボタン** | **Mac Shortcut Keys** | **PC ショートカットキー** |
   |---|---|---|---|
   | 太字 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜体 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl + I |
   | 下線 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | ハイパーリンク | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl+K |
   | 箇条書き | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 番号付きリスト | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | ブロック引用 | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   テキストの書式設定を停止するには、 **リッチテキスト** ツールバー。

   >[!NOTE]
   >
   >* また、ユーザーが受け取った更新内容を含む電子メール通知にも、フォーマットが表示されます。
   >* E メールの更新に適用したリッチテキスト書式は、「更新」タブで表示した場合、更新に表示されません。
   >* 組織が Internet Explorer でWorkfrontを使用している場合、更新に貼り付けた書式付きテキストはリッチテキストの書式が失われ、プレーンテキストとして表示されます。 リッチテキストツールバーの属性を使用して、テキストの書式を変更できます。
   >* リッチテキストの書式設定は、[ タイムシート ] 領域で行われた更新や、レポート内の [ メモ ] および [ 最終条件 ] オブジェクトで表示された更新には使用できません。


1. （オプション）以前の更新のテキストや他のソースのテキストを含め、独自の更新と区別する場合は、ブロック引用としてマークできます。 次をクリック： **ブロック見積もり** アイコン ![](assets/block-quote-small.png) 引用するテキストを入力します。 引用されたテキストは、垂直の灰色の線でマークされて表示されます。 次をクリック： **ブロック見積もり** 通常の書式に戻るにはアイコンを再度使用します。

   ![](assets/block-quote-marked-350x144.png)

1. （オプション）更新に絵文字を追加します。

   >[!NOTE]
   >
   >* Workfrontでは、 ：などの句読点の顔文字は絵文字に置き換えられません。
   >* 絵文字は、[ タイムシート ] 領域で行われた更新、またはレポートで表示された [ 注記 ] および [ 最終条件 ] オブジェクトでは使用できません。
   >* Workfrontの絵文字機能では Unicode 文字を使用するので、は Unicode コードポイントをサポートするブラウザーとオペレーティングシステムでのみ表示されます。 お使いのプラットフォーム、ブラウザー、またはオペレーティングシステムのバージョンが異なるユーザーは、同じ絵文字にアクセスできない場合があります。
   >* サポートされていない絵文字は、黒または白のボックスで表されます。
   >* Windows 7 では、黒と白の絵文字のみがサポートされています。
   >* 電子メールでおこなった更新に適用される絵文字は、「更新」領域に表示されると、更新に表示されません。


1. （オプション）追加の情報ソースに URL リンクを追加するには：

   1. リンクを挿入する更新内をクリックします。
   1. の **リッチテキスト** ツールバーで、 **ハイパーリンク** アイコン ![](assets/link-icon.png)

   1. 内 **リンクを作成** 下に表示されるボックス **URL**、リンク先のソースの URL を入力または貼り付けます。

   1. の下 **表示するテキスト**、リンクテキストを入力または貼り付けます。
   1. 「**保存**」をクリックします。



1. （オプション）更新に画像を添付するには、 **画像** アイコン ![](assets/addimageicon-35x32.png) お使いのコンピューター上の画像を参照します。\
   または\
   画像を更新領域にドラッグします。

   >[!NOTE]
   >
   >* 画像アイコンを表示するには、Workfrontの管理者が画像の追加を有効にする必要があります。
   >* 画像ファイルの最大サイズは 7 MB です。 サポートされる画像ファイルタイプは、.jpg、.gif および.png です。
   >* 画像は、オブジェクトの「更新」タブからのみアクセスでき、「ドキュメント」タブでは使用できません。
   >* 画像とテキストを含まない更新を送信できます。


1. （オプション）次の項目のいずれかを指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>通知 </strong></td> 
      <td>更新の通知が必要なユーザーを特定します。 オブジェクトに割り当てられた、またはサブスクライブされたユーザーは、更新がおこなわれると、自動的に通知を受け取ります。<br><p>更新に他のユーザーを含める方法について詳しくは、 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>コミット日</strong></td> 
      <td>日付選択で、作業項目を完了するためにコミットする日付を選択します。 コミット日の詳細は、 <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">コミット日の概要</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状況</strong></td> 
      <td>タスクまたはタスクの新しい条件を選択します。 条件の選択について詳しくは、 <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">タスクおよび問題の条件を更新</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ステータス</strong></td> 
      <td>現在のステータスの横にある矢印をクリックし、ドロップダウンメニューから目的のステータスを選択します。 ステータスの設定について詳しくは、 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">タスクステータスを更新</a>.<p>作業項目のステータスを更新しても、プロジェクトのステータスは自動的には変更されません。 プロジェクトの設定に応じて、プロジェクトのステータスを個別に更新する必要が生じる場合があります。 様々なプロジェクト更新タイプの詳細については、 <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択 </a>.</p><p><b>メモ</b>

   作業項目のステータスが「承認待ち」の場合は、ステータスを変更できません。</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>完了バー</strong></td> 
      <td>（タスクでのみ使用可能）進行状況バーを目的の割合にスライドして、完了した作業の割合を示します。 完了バーをダブルクリックして、完了率を入力することもできます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>社外秘</strong></td> 
      <td> <p>このオプションを無効にすると、会社外のユーザーがこの更新を表示する権限を持たなくなります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **更新** をクリックして、Workfrontオブジェクトに更新を追加します。

   >[!NOTE]
   >
   >クリック後 7 秒間、小さなポップアップウィンドウが表示されます **更新**&#x200B;を使用すると、更新を取り消し、更新が投稿される前に編集ウィンドウに戻ることができます。 取り消しポップアップを閉じたり、ポップアップが表示されなくなるのを待ったり、ページから移動したりすると、更新が投稿されます。
   >
   >Workfront管理者がアクセスレベルで「ユーザーによるコメントの削除を許可しない」設定を選択した場合、コメントを取り消すことはできません。 詳しくは、 [カスタムアクセスレベルの作成と変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. 更新に返信するには、 [更新情報に返信](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

<!--
### Add an update to a work item in the Preview environment

>[!NOTE]
>
> In the Preview environment, the following functionality is available only for issues, after opting in the Beta program for the new commenting experience.
> 
> In the Production environment, the following functionality is available for goals. You must have an additional license to access Workfront Goals. For information about commenting on goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md). 

1. Locate the object you want to add comments to, then click its name to open the object's page.
1. Click  **Updates** in the left panel. 
1. Activate the **Beta** toggle in the upper-right corner of the Updates area. This switches the Updates area to the new commenting experience. 
1. Click the **Comments** tab in the upper-left corner of the Updates area.
1. Start entering a comment in the **New comment** box. 
   
   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >Navigating away from the Updates section before you finish typing and submitting a comment keeps the comment on the page in draft mode even after you log off and log back on. Drafted comments are only visible to the user entering them.

1. (Optional) In the **Tag people or teams** area, start typing the name or the email of a user, or a team that you would like to include in this comment, then select it when it displays in the list. 
1. (Optional) To add rich text formatting to your update, use any attributes on the **Rich Text** toolbar as you type.

   | **Attribute** |**Toolbar Button** |**Mac Shortcut Keys** |**PC Shortcut Keys** |
   |---|---|---|---|
   | Bold | ![mceclip10.png](assets/mceclip10.png)|⌘+b |Ctrl+B |
   | Italics | ![mceclip9.png](assets/mceclip9.png)|⌘+i |Ctrl+I |
   | Underline | ![mceclip8.png](assets/mceclip8.png)|⌘+u |Ctrl+U |
   | Hyperlink | ![mceclip7.png](assets/mceclip7.png)|⌘+K |Ctrl+K |
   | Bulleted List | ![mceclip6.png](assets/mceclip6.png)|⌘+Shift+8 |Ctrl+Shift+8 |
   | Numbered List | ![mceclip5.png](assets/mceclip5.png)|⌘+Shift+7 |Ctrl+Shift+7 |
   | Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |Ctrl+Shift+9 |

    To stop formatting text, deselect the attribute on the **Rich Text** toolbar.

   >[!NOTE]
   >
   >* Formatting also displays in any email notification users receive containing your update.
   >* Rich Text formatting applied to an update in an email does not display on the update when viewed in the Updates tab.  
   >* If your organization uses Workfront with Internet Explorer, any formatted text pasted into an update loses its Rich Text formatting and displays as plain text. You can reformat the text using the attributes on the Rich Text toolbar.
   >* Rich Text formatting is not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.

   ************ HIDE THIS ********* 1. (Optional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting.

   ********  HIDE THIS ******** 1. (Optional) Add any emojis to your update.

   >[!NOTE]
   >
   >* Workfront does not replace punctuation emoticons such as :) with emojis.
   >* Emojis are not available for updates made in the Timesheets area or for Note and Last Condition objects viewed in a report.
   >* The emoji feature in Workfront utilizes Unicode characters and, as such, displays only on browsers and operating systems that support Unicode code points. Users on a platform, browser, or operating system version different than yours might not have access to the same emojis.
   >* An unsupported emoji is represented by a black or white box.
   >* Windows 7 supports only black and white emojis.  
   >* Emojis that are applied to an update made via email do not display on the update when viewed in the Updates area.

1. (Optional) To add a URL link to additional information sources:

   1. Click in your update where you want to insert a link.
   1. On the **Rich Text** toolbar, click the **Hyperlink** icon. ![](assets/link-icon.png)  

   1. In the **Create Link** box that appears, under **URL**, type or paste the URL of the source to which you want to link.
   
   1. Under **Text to display**, type or paste the link text.
   1. Click **Save**.   
1. Click **Submit**. 
1. (Optional) Click **Reply** to reply to an existing comment, then follow the steps 5-7 above. (**************insure this stays accurate***********)
1. (Optional) Click the **Like** icon![](assets/like-icon.png) to like a comment that someone else added. The icon updates with the number of likes.
1. (Conditional and Optional) If you included additional people in your comment, click on the number of members included in the update to display a list of entities that the comment you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)
1. (Optional) Click the **System Activity** tab to view updates logged by the system. When a goal is updated, Workfront generates a note about that update that and displays it in the System Activity tab. Workfront also records a system update when a result, activity, or project is added to the goal or when it is updated. 

-->



## 更新情報をコピー

更新をコピーする方法はいくつかあります。 リンクをコピーした後、他のユーザーとリンクを共有して、更新に導くことができます。

* [更新をコピー](#copy-the-update)
* [スレッドリンクをコピー](#copy-the-thread-link)
* [更新リンクをコピー](#copy-the-update-link)

### 更新をコピー {#copy-the-update}

このオプションは、特定の更新からクリップボードにテキストをコピーします。

1. コピーする更新または返信に移動します。
1. 次をクリック： **詳細** メニュー、次に「 **本文をコピー**.

   ![「本文をコピー」を選択します。](assets/update-stream-copy-body-text-350x152.png)

### スレッドリンクをコピー {#copy-the-thread-link}

このオプションは、スレッドを他のユーザーと共有できるように、完全なスレッドリンクをクリップボードにコピーします。

1. コピーする更新スレッドに移動します。
1. 次をクリック： **詳細** メニュー、次に「 **スレッドリンクをコピー**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### 更新リンクをコピー {#copy-the-update-link}

このオプションは、特定の更新リンクをクリップボードにコピーします。 更新リンクを共有すると、リンクをたどるユーザーには、更新の周囲に境界線が表示されます。

1. コピーする更新または返信に移動します。
1. 次をクリック： **詳細** 個々の更新の横にあるメニューで、 **更新リンクをコピー**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## 更新または返信の削除

Workfront管理者がユーザーに提供するアクセス権によっては、オブジェクトの「更新」タブで追加した更新を削除できる場合があります。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 記事内 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

別のユーザーがおこなった更新を削除できるWorkfrontユーザー (Workfront管理者を含む ) はいません。 ただし、ユーザーのアクセスレベルでユーザーが自分の更新を削除できる場合、Workfront管理者はそのユーザーとしてログインし、加えた更新を削除できます。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) および [別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 削除する更新または返信に移動します。
1. 次をクリック： **詳細** 削除する更新または返信の横のメニューから、 **削除**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 表示されるメッセージで、 **確認**.

>[!NOTE]
>
>画像が添付された更新を削除すると、コメントと画像の両方が削除されます。

## タイムシートに更新を追加する

1. 更新するタイムシートに移動します。
1. [ タイムシート ] をクリックして開きます。
1. タイムシートの下部で、次をクリックします。 **コメントを含める**.
1. タイムシートの下部に表示されるボックスに、更新を入力します。

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. （条件付き）タイムシートを承認用に送信せずに更新を保存するには、 **後で使用するために保存**.

   または

   更新を保存し、タイムシートを承認用に送信するには、次をクリックします： **承認用に送信**.

   または

   タイムシートが承認者と共に設定されていない場合は、[ ] をクリックします。 **タイムシートを保存して閉じる** 更新を保存します。

## システム更新を有効または無効にする

Workfrontオブジェクトの「更新」セクションには、次の 2 種類の情報が表示されます。

* **ユーザーの更新：** ユーザーの更新とは、自分とシステム内の他のユーザーが入力するコメントです。

   ![](assets/user-update-cl-350x277.png)

* **システムの更新：** アセットの削除、バージョンの追加または削除、承認リクエストの添付または削除、およびオブジェクト上のドキュメントに対する編集または変更が記録されます。

   ![](assets/system-updates-cl-350x277.png)

ご使用のWorkfrontライセンスに応じて、システムのアップデートがデフォルトで有効になっている場合があります。 Workfrontの管理者は、システムの更新で何を追跡するかを決定できます。詳しくは、 [システムで追跡された更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). また、システムの更新やアクティビティを除外して、すべてのオブジェクトのユーザー更新のみを表示することもできます。

ユーザーとシステムの更新の違いについて詳しくは、 [システムで追跡された更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

システム更新を有効または無効にするには：

1. 次をクリック： **更新** タブをクリックします。
1. クリック **システム更新を表示** スイッチを左（無効）または右（有効）にスライドさせます。

   ![](assets/show-system-updates-qs-350x55.png)

   このオプションは、Workfront全体のすべてのオブジェクトにわたって永続的で、Workfrontからログアウトした場合でも、選択した位置にとどまります。

