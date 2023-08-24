---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 作業を更新
description: Adobe Workfrontオブジェクト（プロジェクト、タスクまたはイシュー）に更新を追加して、オブジェクトの進行状況を伝えることができます。 オブジェクトを割り当てられた、またはサブスクライブしたユーザーは、更新を表示できます。 また、ユーザーにタグを付けて、更新に注意を向けることもできます。
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 709b36f4471e5576e45ed918783216a1f7f4abac
workflow-type: tm+mt
source-wordcount: '3521'
ht-degree: 1%

---

# 作業を更新



<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、すべての顧客のプレビュー環境でのみ使用できます。 実稼動環境では、毎月のリリース以降、高速リリースを有効にしたお客様も同じ機能を実稼動環境で使用できます。 </span>\
<span class="preview">高速リリースについて詳しくは、 [組織の高速リリースを有効または無効にします](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>

<span class="preview">現在のリリーススケジュールについて詳しくは、 [2023 年第 4 四半期リリースの概要](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>現在、Adobe Workfrontでのコメント作成エクスペリエンスの再設計中です。
>どの環境から、およびどのオブジェクトからコメントエクスペリエンスにアクセスしたかに応じて、「更新」セクションに異なる機能が表示される場合があります。
>
>新しいコメントエクスペリエンスとその可用性について詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>新しいコメントエクスペリエンスは、「更新」セクションでのみ使用でき、次の領域では使用できません。
>
> * ホーム
> * リスト内の概要パネル
> * タイムシートの [ 概要 ] パネル

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

## 作業の更新に関する考慮事項

* 「更新」セクションのAdobe Workfrontのほとんどのオブジェクトにコメントを追加できます。 更新セクションを表示するオブジェクトの詳細については、 [アップデートセクションの概要](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Workfrontと統合されている他のアプリケーションやWorkfrontモバイルアプリから、Workfrontオブジェクトにコメントを追加できます。

  Workfrontと統合されているすべてのアプリケーションに、Workfrontオブジェクトにコメントを追加する機能があるわけではありません。

  WorkfrontのオブジェクトからWorkfrontオブジェクトにアクセスする場合、アプリケーションの「更新」セクションで使用できる機能の一部が他のアプリケーションで使用できるわけではありません。 例えば、リッチテキスト機能や、コメントを会社の非公開にする場合は、サードパーティのアプリケーションからWorkfrontオブジェクトにコメントを追加する際に、使用できない可能性があります。

* オブジェクトにコメントを付ける際に、Workfrontオブジェクト（プロジェクト、タスクまたはイシュー）の進捗状況を伝えることができます。 オブジェクトを割り当てられた、またはサブスクライブしたユーザーは、更新に関する通知を受け取ることができます。 オブジェクトへの表示アクセス権を持つユーザーは誰でも、更新を表示できます。

* ユーザーにタグを付けて、更新に注意を向けることができます。 タグ付きユーザーには、アプリ内通知と更新に関する電子メールが送信されます。

  >[!TIP]
  >
  >   新しいコメントエクスペリエンスでは、コメントの所有者は自動的にタグ付けされます。 詳しくは、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
  <!--take the "in the new commenting experience" out when this is the only experience-->

* 表示可能なオブジェクトにコメントを追加したり、Workfrontまたはグループ管理者としてログインして、別のユーザーの代わりにコメントを追加したりできます。 詳しくは、 [別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

* Workfrontの次の領域で、プロジェクト、タスクおよびイシューに更新を追加できます。

   * Workfrontオブジェクトの「更新」セクションで、
   * 「ホーム」領域から（タスクおよび問題に関する）
   * オブジェクトの一覧の [ 概要 ] パネル、またはタイムシート（タスクと問題の場合）から

このページの情報では、Workfrontオブジェクトに対するコメントの作成方法と、プロジェクト、タスクおよび問題の更新方法について説明します。

目標のコメントについて詳しくは、 [Adobe Workfront目標で目標コメントを管理](../../workfront-goals/goal-management/manage-goal-comments.md). Workfront Goals にアクセスするには、追加のライセンスが必要です。

ボード領域でのカードのコメントについて詳しくは、 [ボードへのアドホックカードの追加](../../agile/get-started-with-boards/add-card-to-board.md).

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
   <td> <p>問題およびドキュメントに対する要求以上、その他のすべてのオブジェクトに対する確認以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>更新先のオブジェクトのアクセスを表示または編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクトの権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 作業項目に更新を追加する

作業項目に更新を追加する方法は、[ 更新 ] セクションのバージョンと選択したオブジェクトによって異なります。

### 現在の更新セクションの作業項目に更新を追加する

<!--on October 26, replace "current" with "legacy"-->

>[!NOTE]
>
>次の機能は、目標とカードを除くすべてのオブジェクトで使用できます。 Workfront Goals にアクセスするには、追加のライセンスが必要です。 目標のコメントについて詳しくは、 [Adobe Workfront目標で目標コメントを管理](../../workfront-goals/goal-management/manage-goal-comments.md).
>
>カードの「コメント」セクションと「システムアクティビティ」セクションを有効にすると、「ボード」領域でカードの更新を追加し、表示することができます。 詳しくは、 [ボードへのアドホックカードの追加](../../agile/get-started-with-boards/add-card-to-board.md).

1. 更新を行う作業項目（プロジェクト、タスク、タスクなど）に移動します。
1. 次をクリック： **更新** 」セクションに入力します。
1. クリック **新しい更新を開始し、** 次に、更新を入力します。
1. （オプション）リッチテキストを使用するか、更新に絵文字、リンク、画像を追加して、コンテンツを拡張します。 詳しくは、 [Workfrontの更新でのリッチテキストの使用](#use-rich-text-in-a-workfront-update) 」の節を参照してください。
1. （オプション）作業項目に関する次の情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>通知 </strong></td> 
      <td>更新の通知を受け取る必要があるユーザーを特定します。 オブジェクトに割り当てられた、またはサブスクライブされたユーザーは、更新がおこなわれると、自動的に通知を受け取ります。<br><p>更新に他のユーザーを含める方法について詳しくは、 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">更新時の他のユーザーへのタグ付け</a>.</p></td> 
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
      <td>現在のステータスの横にある矢印をクリックし、ドロップダウンメニューから目的のステータスを選択します。 ステータスの設定について詳しくは、 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">タスクステータスを更新</a>.<p>作業項目のステータスを更新しても、プロジェクトのステータスは自動的には変更されません。 プロジェクトの設定に応じて、プロジェクトのステータスを個別に更新できます。 様々なプロジェクト更新タイプの詳細については、 <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択 </a>.</p><p><b>メモ</b>

   作業項目のステータスが「承認待ち」の場合は、ステータスを変更できません。</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>完了バー</strong></td> 
      <td>（タスクでのみ使用可能）進行状況バーを目的の割合にスライドして、完了した作業の割合を示します。 完了バーをダブルクリックして、完了率を入力することもできます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>社外秘</strong></td> 
      <td> <p>このオプションを無効にすると、会社外のユーザーがこの更新を表示する権限を持たなくなります。</p> 
      <p><b>メモ</b></p>
      <p>このオプションは、ユーザーが会社に関連付けられている場合にのみ表示されます。</p>
      </td> 
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

### 新しいコメントエクスペリエンスを使用して作業項目に更新を追加する

新しいコメントエクスペリエンスで使用できる機能とオブジェクトについて詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. 更新するオブジェクトを探し、その名前をクリックしてオブジェクトのページを開きます。
1. クリック  **更新** をクリックします。

   The **コメント** 「 」タブがデフォルトで選択されています。
1. でコメントの入力を開始 **新しいコメント** ボックス。

   <span class="preview">![](assets/comment-box-empty-unshimmed.png)</span>

   >[!TIP]
   >
   >コメントを入力して送信する前に「更新」セクションから移動すると、ログオフしてログオンし直した後でも、ページ上のコメントがドラフトモードのままになります。 コメントに追加された画像も下書きに保存されます。 ドラフトは 7 日間保存され、その後は破棄され、復元できません。 下書きのコメントは、ユーザーが入力した場合にのみ表示されます。

1. （オプション）変更の取り消しまたはやり直しをおこなうには、次のショートカットキーを使用します。
   * Ctrl + Z( Macの場合は⌘+z)：変更を元に戻します。
   * Ctrl + Y( Macの場合は⌘+y)：変更をやり直します。
1. （オプション） **担当者またはチームのタグ付け** 領域に入力し、このコメントに含めるユーザーまたはチームの名前やメールを入力して、リストに表示されたら選択します。
1. （オプション）リッチテキストを使用するか、更新に絵文字、リンク、画像を追加して、コンテンツを拡張します。 詳しくは、 [Workfrontの更新でのリッチテキストの使用](#use-rich-text-in-a-workfront-update) 」の節を参照してください。

   >[!TIP]
   >
   >別のユーザーが、更新しようとしている同じ項目にコメントを送信すると、赤い線に「新規」インジケータが表示され、新しいコメントが通知されます。
   >
   >インジケーターは、コメントがアイテムに送信された後にのみ表示され、コメントがまだ構成されている場合は表示されません。
   >
   >「新規」インジケーターは、新しい更新を入力したユーザーと、現在更新を入力しているユーザーの両方が新しいコメント付けエクスペリエンスを使用している場合にのみ表示されます。
   ><span class="preview">![](assets/real-time-new-red-indicator-unified-commenting.png)</span>

1. クリック **送信** をクリックして、Workfrontオブジェクトに更新を追加します。
1. （オプション）コメントを編集するには、 **その他** メニュー ![](assets/more-menu.png)  <span class="preview">コメントの右上隅に</span>を選択し、次に **編集**.
1. コメント内の情報の編集、画像の追加や削除、タグ付きユーザーの削除をおこないます。
コメントは、送信後 15 件以内に編集できます。 コメントの入力時に表示される日付スタンプの左側に、「編集済み」のインジケーターが追加されます。

   <span class="preview">![](assets/edited-tag-on-comment-unified-commenting.png)</span>

   >[!TIP]
   >
   >* 元の更新を送信した場合にのみ、ユーザーに更新を通知する電子メールが生成されます。 更新を編集した後は、電子メールは生成されません。
   >* コメントの横の日付スタンプは、最後の編集の日付ではなく、元のコメントの日付です。
   >* 現在の年からのコメントでは、日付スタンプに年は表示されません。 タイムスタンプの上にマウスポインターを置くと、年を含む完全な日付が表示されます。

1. （オプション）「 **返信** 既存のコメントに返信するには、上記の手順 4～8 に従います。 <!--(**************insure this stays accurate***********)--> 更新への返信について詳しくは、 [更新情報に返信](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

   >[!TIP]
   >
   >   <span class="preview">既存の返信に返信を追加する場合は、 **返信を追加…** ボックスを使用するか、 **返信** 元のコメントに対して。 返信はスレッドの最後に追加されます。</span>


1. （条件付きおよびオプション）「更新」セクションの表示領域の外側に表示されるコメントを他のユーザーが追加した場合は、 **表示** 青の中に **新しいコメントバナー** をクリックして、これらのコメントを表示します。

   <span class="preview">![](assets/blue-new-comments-banner-with-view-button.png)</span>

   追加のコメントが画面の下部に表示されます。



   >[!NOTE]
   >
   >   「新しいコメント」インジケーターと「表示」ボタンは、新しい更新を入力したユーザーと、現在「更新」セクションを表示しているユーザーの両方が新しいコメントエクスペリエンスを使用している場合にのみ表示されます。


1. （オプション） **次に類似** アイコン![](assets/like-icon.png). アイコンは「いいね！」の数に応じて更新されます。
1. （条件付きおよびオプション）コメントに追加の担当者を含める場合は、更新に含まれるメンバーの数をクリックして、入力したコメントが共有されているエンティティのリストを表示します。

   <span class="preview">![](assets/members-icons-expanded-unshimmed.png)</span>

   >[!TIP]
   >
   >   <span class="preview">最初の 2 つのタグ付きエンティティの名前が、アバターの横に表示されます。 3 つ以上のエンティティがタグ付けされている場合は、最初のエンティティの名前と追加エンティティの数のみが表示されます。</span>

1. （オプション） **システムアクティビティ** タブをクリックして、システムによって記録された更新を表示します。 オブジェクトまたはその子オブジェクトが更新されると、Workfrontはその更新に関するメモを生成し、「システムアクティビティ」タブに表示します。

   詳しくは、 [アップデートセクションの概要](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >システム更新にコメントを追加することはできません。

## Workfrontの更新でのリッチテキストの使用{#use-rich-text-in-a-workfront-update}

<!--October 2023: remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>リッチテキストツールバーの一部のオプションは、新しいコメントエクスペリエンスでは使用できない場合があります。

リッチテキストを使用したり、絵文字、リンク、画像などの様々な項目を追加したりして、更新内容を強化できます。

1. 次に移動： **更新** Workfrontオブジェクトの領域に入力し、コメントの入力を開始します。
1. （オプション）リッチテキスト書式を更新に追加するには、 **リッチテキスト** ツールバーを使用します。

   ![](assets/rich-text-toolbar.png)

   <!--October 2023: the individual icons in the toolbar will need replacing-->

   | **属性** | **ツールバーボタン** | **Macショートカットキー** | **Windows のショートカットキー** |
   |---|---|---|---|
   | 太字 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜体 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl + I |
   | 下線 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | ハイパーリンク | ![mceclip7.png](assets/mceclip7.png) | <br>「リンクを作成」または「リンクを追加」ボックスを開くには、⌘+K を使用します。</br> <br>コメント化ベータ版のエクスペリエンスで、選択したテキストにリンクを貼り付けます (⌘+V)。</br> | <br>「リンクを作成」または「リンクを追加」ボックスを開くには、Ctrl+K を押します。</br> <br>コメントベータ版エクスペリエンスで、選択したテキストにリンクを貼り付けるには、Ctrl+V を使用します。</br> |
   | 箇条書き | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 番号付きリスト | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | ブロック引用 | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   テキストの書式設定を停止するには、 **リッチテキスト** ツールバー。

   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* また、ユーザーが受け取った更新内容を含む電子メール通知にも、フォーマットが表示されます。
   >* E メールの更新に適用したリッチテキスト書式は、「更新」タブで表示した場合、更新に表示されません。
   >* 組織が Internet Explorer でWorkfrontを使用している場合、更新に貼り付けた書式付きテキストはリッチテキストの書式が失われ、プレーンテキストとして表示されます。 リッチテキストツールバーの属性を使用して、テキストの書式を変更できます。
   >* リッチテキストの書式設定は、[ タイムシート ] 領域で行われた更新や、レポート内の [ メモ ] および [ 最終条件 ] オブジェクトで表示された更新には使用できません。

1. （オプション）以前の更新のテキストや他のソースのテキストを含め、独自の更新と区別する場合は、ブロック引用としてマークできます。 次をクリック： **ブロック見積もり** アイコン ![](assets/block-quote-small.png) 引用するテキストを入力します。 引用されたテキストは、垂直の灰色の線でマークされて表示されます。 次をクリック： **ブロック見積もり** 通常の書式に戻るにはアイコンを再度使用します。

   <span class="preview">![](assets/block-quote-marked-350x144.png)</span>

1. （オプション）更新に絵文字を追加します。

   >[!NOTE]
   >
   >* Workfrontでは、 ：などの句読点の顔文字は絵文字に置き換えられません。
   >* レポートに表示される「メモ」および「最終条件」オブジェクトでは、絵文字は使用できません。
   >* Workfrontの絵文字機能では Unicode 文字を使用するので、は Unicode コードポイントをサポートするブラウザーとオペレーティングシステムでのみ表示されます。 お使いのプラットフォーム、ブラウザー、またはオペレーティングシステムのバージョンが異なるユーザーは、同じ絵文字にアクセスできない場合があります。
   >* サポートされていない絵文字は、黒または白のボックスで表されます。
   >* Windows 7 では、黒と白の絵文字のみがサポートされています。
   >* 電子メールでおこなった更新に適用される絵文字は、「更新」領域に表示されると、更新に表示されません。

1. （オプション）追加の情報ソースに URL リンクを追加するには：

   1. リンクを挿入する更新内をクリックします。
   1. 次の日： **リッチテキスト** ツールバーで、 **ハイパーリンク** アイコン ![](assets/link-icon.png).

   1. Adobe Analytics の **リンクを作成** 表示されるボックス（下） **URL**、リンク先のソースの URL を入力または貼り付けます。

   1. の下 **表示するテキスト**、リンクテキストを入力または貼り付けます。
   1. 「**保存**」をクリックします。

1. （オプション）更新に画像を添付するには、使用する環境に応じて、次のいずれかの操作を実行します。

   * 次をクリック： **画像** アイコン ![](assets/addimageicon-35x32.png) 現在の更新エクスペリエンスを使用する場合は、コンピューター上の画像を参照するか、画像を更新領域にドラッグします。

   または

   次をクリック： **添付ファイルを追加** アイコン ![](assets/add-image-mountain-with-plus-icon.png) 新しいコメントエクスペリエンスを使用する場合は、コンピューター上の画像を参照します。 <!--**************** the tooltip of this icon might be renamed to "Add image")--> <!--in October 26 - leave this as the only icon instead of the OR option-->

   >[!NOTE]
   >
   >* 画像または添付ファイルを追加アイコンを表示するには、Workfront管理者が、Workfrontインターフェイス領域の「フィードの環境設定を更新」セクションで画像の追加を有効にする必要があります。 詳しくは、 [ユーザーの更新の環境設定を構成する](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
   >* 画像ファイルの最大サイズは 7 MB です。 サポートされる画像ファイルタイプは、.jpg、.gif および.png です。
   >* 画像は、オブジェクトの「更新」セクションからアクセスでき、「ドキュメント」領域でも使用できます。
   >* 画像とテキストを含まない更新を送信できます。
   >* 画像を含むコメントを削除する場合、選択したエクスペリエンスに応じて、次のシナリオが存在します。
   >
   >     * 現在のコメントエクスペリエンスでは、画像は「ドキュメント」領域に残りますが、「更新」セクションには表示されません。
   >     * 新しいコメントエクスペリエンスでは、画像は「更新」セクションおよび「ドキュメント」領域から削除されます。 コメントを編集して画像を削除すると、その画像もドキュメント領域から削除されます。
   >* コメントに添付された画像を「ドキュメント」領域から削除すると、その画像はコメントからも削除されます。

1. クリック **更新**  または **送信**（コメント機能ベータ版のエクスペリエンスを使用する場合）


## 更新情報をコピー

更新をコピーする方法はいくつかあります。 リンクをコピーした後、他のユーザーとリンクを共有して、更新に導くことができます。

更新のコピーは、使用するコメントエクスペリエンスに応じて異なります。

### 現在のコメントエクスペリエンスの更新をコピー

<!--October 26 - replace current with legacy-->

* [更新をコピー](#copy-the-update)
* [スレッドリンクをコピー](#copy-the-thread-link)
* [更新リンクをコピー](#copy-the-update-link)

#### 更新をコピー {#copy-the-update}

このオプションは、特定の更新からクリップボードにテキストをコピーします。

1. コピーする更新または返信に移動します。
1. 次をクリック： **その他** メニュー、次に「 **本文をコピー**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### スレッドリンクをコピー {#copy-the-thread-link}

このオプションは、スレッドを他のユーザーと共有できるように、完全なスレッドリンクをクリップボードにコピーします。

1. コピーする更新スレッドに移動します。

1. 次をクリック： **その他** メニュー、次に「 **スレッドリンクをコピー**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### 更新リンクをコピー {#copy-the-update-link}

このオプションは、特定の更新リンクをクリップボードにコピーします。 更新リンクを共有すると、リンクをたどるユーザーには、更新の周囲に境界線が表示されます。

1. コピーする更新または返信に移動します。
1. 次をクリック： **その他** 個々の更新の横にあるメニューで、 **更新リンクをコピー**.

   ![](assets/copy-update-link-old-ui.png)

### 新しいコメントエクスペリエンスでの更新のコピー

新しいコメントエクスペリエンスで使用できる機能とオブジェクトについて詳しくは、 [新しいコメントエクスペリエンス](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<!--when we remove and deprecate the legacy stream, add screen shots in the sections below- October 2023-->

* [リンクをコピー](#copy-link)
* [本文をコピー](#copy-body-text)

#### リンクをコピー

このオプションは、コメントまたはスレッドのリンクをクリップボードにコピーして、他のユーザーとコメントまたはスレッド全体を共有できるようにします。

1. リンクをコピーする更新に移動します。

1. 次をクリック： **その他** メニュー、次に「 **リンクをコピー**.

#### 本文をコピー

このオプションは、特定の更新からクリップボードにテキストをコピーします。

1. コピーする更新または返信に移動します。
1. 次をクリック： **その他** メニュー、次に「 **本文をコピー**.

## 更新または返信の削除

Workfront管理者がユーザーに提供するアクセス権によっては、オブジェクトの「更新」タブで追加した更新を削除できる場合があります。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 記事内 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

別のユーザーがおこなった更新を削除できるWorkfrontユーザー (Workfront管理者を含む ) はいません。 ただし、ユーザーのアクセスレベルでユーザーが自分の更新を削除できる場合、Workfront管理者はそのユーザーとしてログインし、加えた更新を削除できます。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) および [別のユーザーとしてログイン](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 削除する更新または返信に移動します。
1. 次をクリック： **その他** 削除する更新または返信の横のメニューから、 **削除**. <!--October 2023 - replace screen shot here-->

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 表示されるメッセージで、 **確認** または、 **削除**（コメント機能ベータ版のエクスペリエンスを使用する場合）

   >[!NOTE]
   >
   >画像が添付された更新を削除すると、コメントと画像の両方が削除されます。 詳しくは、 [Workfrontの更新でのリッチテキストの使用](#use-rich-text-in-a-workfront-update) 」の節を参照してください。

   削除したコメントに返信が関連付けられている場合は、コメントが削除されたユーザーの名前で削除されたことを示すメッセージが表示されます。

   <span class="preview">![](assets/removed-comment-indicator-new-experience.png)</span>

   コメントベータ版エクスペリエンスを使用する場合、削除されたコメントはWorkfrontから直ちに削除されます。 「更新」セクションを使用するユーザーは、別のユーザーがコメントをリアルタイムで削除しているのを確認します。

   <!--when we remove the beta, take out the first part of the sentence above about only when commenting in beta experience. Leave the rest though-->

<!--this is no longer needed - adding timesheet comments is just like adding comments to any other object now

## Add an update on a Timesheet

1. Go to a Timesheet on which you want to make an update.
1. Click the Timesheet to open it.
1. At the bottom of the Timesheet, click **Include a comment**.
1. In the box that displays at the bottom of the Timesheet, type an update.

   ![timesheet_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. (Conditional) To save your update without submitting the Timesheet for approval, click **Save for Later**.

   Or

   To save your update and submit the Timesheet for approval, click **Submit for Approval**.

   Or

   If your Timesheet is not set up with an approver, click **Save and Close Timesheet** to save your update.

-->

## システム更新を有効または無効にする

<!--October 2023: remove the whole section because this is no longer possible -->

<!--October 2023: when the new stream goes to all objects production, consider updating this article also, to say there is no System Activity tab to be disabled for objects anymore: help\quicksilver\administration-and-setup\set-up-workfront\system-tracked-update-feeds\system-tracked-update-feeds.md-->

>[!NOTE]
>
>新しいコメントエクスペリエンスを使用する際に、システムの更新を無効にすることはできません。
>この節の情報は、現在の更新セクションで利用できる機能のみを示しています。 <!--October 26: replace current with legacy-->
>ベータ版のシステム更新の詳細については、 [アップデートセクションの概要](../updating-work-items-and-viewing-updates/updates-tab-overview.md).


Workfrontオブジェクトの「更新」セクションには、次の 2 種類の情報が表示されます。

* **ユーザーの更新：** ユーザーの更新とは、自分とシステム内の他のユーザーが入力するコメントです。 <!--October 2023 - new screen shot -->

  ![](assets/user-update-cl-350x277.png)

* **システムの更新：** アセットの削除、バージョンの追加または削除、承認リクエストの添付または削除、およびオブジェクト上のドキュメントに対する編集または変更が記録されます。 <!--October 2023 - new screen shot -->

  ![](assets/system-updates-cl-350x277.png)

  ご使用のWorkfrontライセンスに応じて、システムのアップデートがデフォルトで有効になっている場合があります。 Workfrontの管理者は、システムの更新で何を追跡するかを決定できます。詳しくは、 [システムで追跡された更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). また、システムの更新やアクティビティを除外して、すべてのオブジェクトのユーザー更新のみを表示することもできます。

  次のオブジェクトには、システムで生成された更新はありません。

   * チーム
   * テンプレート
   * テンプレート タスク

システム更新を有効または無効にするには：

1. 次をクリック： **更新** タブをクリックします。
1. クリック **システムの更新を表示** スイッチを左（無効）または右（有効）にスライドさせます。

   ![](assets/show-system-updates-qs-350x55.png)

   このオプションは、Workfront全体のすべてのオブジェクトにわたって永続的で、Workfrontからログアウトした場合でも、選択した位置にとどまります。

   >[!TIP]
   >
   >   システムの更新を記録しないオブジェクトの [ 更新 ] 領域に [ システムの更新を表示 ] オプションはありません。

   <!--when Anna adds the new updates stream to ALL objects, she will remove the System Activity tab from the objects that don't record system updates - add another line to the TIP above to say: The System Activity tab is not available for objects that don't record system-generated updates.*************** OR: maybe make this part of the statement where we list which objects these are, above???  -->


