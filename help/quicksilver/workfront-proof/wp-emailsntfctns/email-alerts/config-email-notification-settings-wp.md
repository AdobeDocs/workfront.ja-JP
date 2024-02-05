---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: ' [!DNL Workfront Proof] でのメール通知設定の指定'
description: Workfrontの配達確認から生成される電子メール通知は、コメント、返信、決定など、配達確認に関する最近のアクティビティを共同作業者に通知します。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e80a3ede9ccf6ccf9ea7777aab35cc859f13a6ac
workflow-type: tm+mt
source-wordcount: '2058'
ht-degree: 89%

---

# [!DNL Workfront Proof] でのメール通知設定の指定

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

電子メール通知は、コメント、返信、決定など、配達確認に関する最近のアクティビティを共同作業者に通知します。

以下の領域で、レビュー担当者向けの電子メール通知を設定できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">製品</td> 
   <td>Workfront Proof Standalone</td> 
  </tr> 
</table>

レビュアーへのメール通知は、新しいプルーフページ、[!UICONTROL 新しいバージョン]ページで設定され、[!UICONTROL プルーフの詳細]ページの「[!UICONTROL ワークフロー]」セクションで管理できます。詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成を参照してください。

* 新しい配達確認ページ
* The [!UICONTROL 新しいバージョン] ページ
* The [!UICONTROL ワークフロー] のセクション [!UICONTROL 配達確認の詳細] ページに貼り付けます。

詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成を参照してください。


* [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成 [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)でプルーフを生成

* [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) でプルーフの詳細を管理を管理します。


また、各ユーザーは、共同作業者が自分の環境設定を持っている場合、またはアカウント管理者がアラートの頻度に関するレコメンデーションを持っている場合に、配達確認を共有したときに自動的に適用される独自の E メールアラート設定を設定できます。 これは、ユーザーの詳細ページで、プルーフのデフォルトとして設定できます。

また、各ユーザーは、配達確認が共有されたときに自動的に適用される、独自の E メールアラート設定を設定することもできます。 <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>これらの設定は、ユーザーがプルーフを作成し、これらの共同作業者を追加する際に提案されます。ただし、これらは提案のみなので、レビュープロセス中はいつでも調整でき、変更後のすべてのアクティビティに適用されます。プルーフのデフォルト設定は、プルーフレベルの設定で上書きされます。

[!UICONTROL 管理者]または[!UICONTROL 請求管理者]プロファイルを持つユーザーは、アカウント設定内からアカウント内の他のユーザーのプルーフのデフォルトを設定することもできます。

プロファイルについて詳しくは、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) のプルーフ権限プロファイルを参照してください。

* [個人設定でプルーフのデフォルトを設定する（[!DNL Workfront Proof] ユーザーのみ）](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [受信者向けのメールアラートを変更](#change-email-alerts-for-a-recipient)
* [ユーザーにプルーフのデフォルトを設定](#configure-proof-defaults-for-a-user)

## 個人設定でプルーフのデフォルトを設定する（[!DNL Workfront Proof] ユーザーのみ）

作成するプルーフのプルーフ設定を行うことができます。

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. **[!UICONTROL 設定]**／**[!UICONTROL 個人設定]**&#x200B;をクリックします。

1. 「**[!UICONTROL プルーフのデフォルト]**」タブをクリックします。
1. 「**[!UICONTROL デフォルトのメール通知設定]**」をクリックして、展開します。
1. 次の 2 つの設定の右側にあるドロップダウンリストで、次の表で説明するオプションの 1 つを選択します。

   * **[!UICONTROL デフォルトのメールアラート]**：自分と共有されているすべてのプルーフに影響します。この設定は、プルーフレベルで上書きできます。
   * **[!UICONTROL 新しいゲストレビュアー向けのデフォルトのメールアラート]**：これまでアカウントに連絡先として存在しなかったレビュアーに影響します。

   >[!NOTE]
   >
   >次のオプションのいずれかを選択しない場合は、[!DNL Workfront Proof] は、プルーフにおけるアクティビティに関する日次概要を送信します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront] は、新しいコメント、返信、決定など、プルーフにおけるアクティビティが発生するたびに、レビュアーにメールを送信します。 <p>これは、アクティビティの発生を確認できるので、プルーフプロセスを管理するユーザーにとって最適なオプションです。 </p><p>ユーザーは、自分のアクティビティに関するメール警告を受け取りません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Replies to my comments]</td> 
      <td>誰かがコメントに明示的に返信した場合にのみ、メールがレビュアーに送信されます（これには、自分のコメントに対する自分の返信は含まれません）。これは、プルーフ上の誰かが新しいコメントを作成しても、レビュアーには通知されないことを意味します。<p>この設定は、プルーフ上のクライアントに推奨されます。これにより、プルーフ上の他のコメントは通知されず、自分のコメントに対する返信のみが通知されます。</p><p>このメール通知設定を使用しているレビュアーには、他の新しいコメントは通知されませんが、プルーフビューアでプルーフ上のすべてのコメントを表示できます。</p><p>コメントについて詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">プルーフのコメントの表示と返信</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] は、誰かが決定を下した場合にのみレビュアーにメールを送信します。<p>これは、承認プロセスを管理するユーザー（プロジェクトマネージャーなど）で、プルーフの進行状況を監視し、どのユーザーが決定を下したかをモニターする必要がある場合に役立ちます。</p><p>決定を送信するときにメール確認オプションを選択しない限り、自分の決定は通知されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Final decision]</td> 
      <td>[!DNL Workfront] プルーフの最後の承認者が決定を下したときに、メールを送信します。<p>このアラートは、通常、実際のレビューの議論に参加する必要のない設計者によって使用されることがよくあります。最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対してアクションを実行できます。</p><p>また、このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーに対しても役立ちます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly Summary]</td> 
      <td>[!DNL Workfront] 1 時間以内に発生したすべてのコメント、返信および決定の概要を記載したメールを、1 時間ごとにレビュアーに送信します。<p>メールは、過去 1 時間以内に自分以外のアクティビティが発生した場合にのみ送信されます。 </p><p>このアラートは、プロジェクトの概要を確認するのに適しています。</p><p>この概要のユースケース例として、プロジェクトの概要を必要としながら、プルーフでのすべてのアクティビティについてすぐに通知される必要はない、シニアレビューアが挙げられます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Daily Summary]</td> 
      <td>[!DNL Workfront] 自分以外のアクティビティがある日にのみ、すべてのコメント、返信および決定を記載した 1 通のメールを送信します。<p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。</p><p>この概要のユースケースの例として、プロジェクトの全体的な進行状況の監視を担当する部門のリーダーが挙げられます。</p><p>詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">プルーフのコメントおよび決定に関する通知の管理</a>を参照してください。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] メールアラートを送信しません。<br>これは、参照用としてのみプルーフに追加され、変更の通知を必要としないユーザーに役立ちます。<p>システムのデフォルトは、[!UICONTROL Daily summary]（[!UICONTROL Not Set] とも表示される）です。自分または自分のレビューアが他の変更を加えない場合、すべてのプルーフにこの設定が適用されます。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 次のいずれかを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>プルーフの作成時に [!UICONTROL Proof made] メールを受け取るかどうかを指定します。詳しくは、<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[!UICONTROL Proof Made] メール</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自分に送信される電子メールの形式 ] </td> 
      <td> <p>HTML スタイルのメールとプレーンテキストのメールのどちらかを選択します。 </p> <p><b>メモ</b></p>
      <p>校正の既定の設定は、配達確認レベルの設定で上書きされます。 ただし、[!UICONTROL Account] 設定でアカウント全体のプルーフメール通知が無効になっている場合は、プルーフで [!UICONTROL Disabled email alert] が選択されていない場合でも、メールアラートが共同作業者に送信されません。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL メッセージ設定]**&#x200B;で、次のいずれかを変更します。

   | 配達確認テンプレート | 説明 |
   |---|---|
   | **[!UICONTROL プルーフ件名テンプレート]** | 新しいプルーフページ、新しいバージョンページ、メッセージページおよび通知ページに表示されます。送信前に編集できます。 |
   | **[!UICONTROL プルーフメッセージテンプレート]** | 新しいプルーフページ、新しいバージョンページ、メッセージページおよび通知ページに表示されます。送信前に編集できます。 |

## 受信者向けのメールアラートを変更

バッチアクションで特定の受信者向けのメールアラートを変更できます。

1. 左側のナビゲーションパネルで「**[!UICONTROL 連絡先]**」をクリックします。
1. 次をクリック： **[!UICONTROL その他]** メニュー ![](assets/more-button-small.png) 受信者に対して、「 **[!UICONTROL メンバーの詳細を表示]** 」と入力します。

1. 「**[!UICONTROL 共有項目]**」セクションを開きます。
1. メールアラートを変更する各項目の左側でチェックボックスを選択します。
1. 共有アイテムのリストの上にある「**[!UICONTROL その他]**」をクリックし、ドロップダウンメニューで「**[!UICONTROL メールアラートを変更]**」をクリックします。

1. メールアラートを変更して、「**[!UICONTROL 送信]**」をクリックします。

## ユーザーにプルーフのデフォルトを設定

[!DNL Workfront Proof] 管理者は、アカウント内のユーザーに対してプルーフのデフォルトを設定できます。

1. **[!UICONTROL 設定]**／**[!UICONTROL アカウント設定]**&#x200B;をクリックします。

1. 「**[!UICONTROL ユーザー]**」タブを開きます。
1. を開きます。 **[!UICONTROL その他]** メニュー ![More_button_small.png](assets/more-button-small.png) を使用して、ユーザー名の右側に表示されます。

1. ドロップダウンメニューで「**[!UICONTROL ユーザーの詳細を表示]**」をクリックします。
1. **[!UICONTROL 設定]**&#x200B;で、「**[!UICONTROL デフォルトのメールアラート設定]**」をクリックして展開します。

1. 次の 2 つの設定の右側にあるドロップダウンリストで、次の表で説明するオプションの 1 つを選択します。

   * **[!UICONTROL デフォルトのメールアラート]**：自分と共有されているすべてのプルーフに影響します。この設定は、プルーフレベルで上書きできます。
   * **[!UICONTROL 新しいゲストレビュアー向けのデフォルトのメールアラート]**：これまでアカウントに連絡先として存在しなかったレビュアーに影響します。

   >[!NOTE]
   >
   >ユーザーに対して次のオプションの 1 つを選択しない場合、[!DNL Workfront Proof] はプルーフのアクティビティに関する日別の概要をユーザーに送信します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] 新しいコメント、返信、決定などのプルーフに関するアクティビティが発生するたびに、レビュアーにメールを送信します。 <p>これは、アクティビティの発生を確認できるので、プルーフプロセスを管理するユーザーにとって最適なオプションです。 </p><p>ユーザーは、自分のアクティビティに関するメール警告を受け取りません。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Replies to my comments]</td>
      <td>誰かがコメントに明示的に返信した場合にのみ、メールがレビュアーに送信されます（これには、自分のコメントに対する自分の返信は含まれません）。これは、プルーフ上の誰かが新しいコメントを作成しても、レビュアーには通知されないことを意味します。<p>この設定は、プルーフ上のクライアントに推奨されます。これにより、プルーフ上の他のコメントは通知されず、自分のコメントに対する返信のみが通知されます。</p><p>このメール通知設定を使用しているレビュアーには、他の新しいコメントは通知されませんが、プルーフビューアでプルーフ上のすべてのコメントを表示できます。</p><p>コメントについて詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">プルーフのコメントの表示と返信</a>を参照してください。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] は、誰かが決定を下した場合にのみレビュアーにメールを送信します。<p>これは、承認プロセスを管理するユーザー（プロジェクトマネージャーなど）で、プルーフの進行状況を監視し、どのユーザーが決定を下したかをモニターする必要がある場合に役立ちます。</p><p>決定を送信するときにメール確認オプションを選択しない限り、自分の決定は通知されません。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Final decision]</td>
      <td>[!DNL Workfront] プルーフの最後の承認者が決定を下したときに、メールを送信します。<p>このアラートは、通常、実際のレビューの議論に参加する必要のない設計者によって使用されることがよくあります。最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対してアクションを実行できます。</p><p>また、このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーに対しても役立ちます。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Hourly Summary]</td>
      <td>[!DNL Workfront] 1 時間以内に発生したすべてのコメント、返信および決定の概要を記載したメールを、1 時間ごとにレビュアーに送信します。<p>メールは、過去 1 時間以内に自分以外のアクティビティが発生した場合にのみ送信されます。 </p><p>このアラートは、プロジェクトの概要を確認するのに適しています。</p><p>この概要のユースケース例として、プロジェクトの概要を必要としながら、プルーフでのすべてのアクティビティについてすぐに通知される必要はない、シニアレビューアが挙げられます。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Daily Summary]</td>
      <td>[!DNL Workfront] 自分以外のアクティビティがある日にのみ、すべてのコメント、返信および決定を記載した 1 通のメールを送信します。<p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。</p><p>この概要のユースケースの例として、プロジェクトの全体的な進行状況の監視を担当する部門のリーダーが挙げられます。</p><p>詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">プルーフのコメントおよび決定に関する通知の管理</a>を参照してください。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] メールアラートを送信しません。<br>これは、参照用としてのみプルーフに追加され、変更の通知を必要としないユーザーに役立ちます。<p>システムのデフォルトは、[!UICONTROL Daily summary]（[!UICONTROL Not Set] とも表示される）です。自分または自分のレビューアが他の変更を加えない場合、すべてのプルーフにこの設定が適用されます。</p></td>
     </tr>
    </tbody>
   </table>

1. 残りの&#x200B;**[!UICONTROL デフォルトのメールアラート設定]**&#x200B;で、次のいずれかを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>プルーフの作成時に [!UICONTROL Proof made] メールを受け取るかどうかを指定します。詳しくは、<a href="https://support.workfront.com/hc/en-us/article">[!UICONTROL Proof Made] メール</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自分に送信される電子メールの形式 ] </td> 
      <td> <p>HTML スタイルのメールとプレーンテキストのメールのどちらかを選択します。 </p> <p><b>メモ</b></p> <p>校正の既定の設定は、配達確認レベルの設定で上書きされます。 ただし、[!UICONTROL Account] 設定でアカウント全体のプルーフメール通知が無効になっている場合は、プルーフで [!UICONTROL Disabled email alert] が選択されていない場合でも、メールアラートが共同作業者に送信されません。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
