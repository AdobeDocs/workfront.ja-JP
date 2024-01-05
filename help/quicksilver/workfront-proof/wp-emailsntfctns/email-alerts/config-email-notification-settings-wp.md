---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: での電子メール通知の設定 [!DNL Workfront Proof]
description: Workfrontの配達確認から生成される電子メール通知は、コメント、返信、決定など、配達確認に関する最近のアクティビティを共同作業者に通知します。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e80a3ede9ccf6ccf9ea7777aab35cc859f13a6ac
workflow-type: tm+mt
source-wordcount: '2058'
ht-degree: 0%

---

# での電子メール通知の設定 [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

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

レビュー担当者向けの E メール通知を新しい配達確認ページで設定できます。 [!UICONTROL 新しいバージョン] ページに追加され、 [!UICONTROL ワークフロー] のセクション [!UICONTROL 配達確認の詳細] ページに貼り付けます。 詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* 新しい配達確認ページ
* The [!UICONTROL 新しいバージョン] ページ
* The [!UICONTROL ワークフロー] のセクション [!UICONTROL 配達確認の詳細] ページに貼り付けます。

詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [で配達確認の詳細を管理 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


また、各ユーザーは、共同作業者が自分の環境設定を持っている場合、またはアカウント管理者がアラートの頻度に関するレコメンデーションを持っている場合に、配達確認を共有したときに自動的に適用される独自の E メールアラート設定を設定できます。 これは、ユーザーの詳細ページで、配達確認のデフォルトとして設定できます。

また、各ユーザーは、配達確認が共有されたときに自動的に適用される、独自の E メールアラート設定を設定することもできます。 <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>これらの設定は、ユーザーが配達確認を作成し、これらの共同作業者を追加する際に提案されます。 ただし、これらは修正候補のみなので、レビュープロセス中はいつでも調整でき、変更後のすべてのアクティビティに適用されます。 配達確認のデフォルト設定は、配達確認レベルの設定で上書きされます。

次の条件を持つユーザー [!UICONTROL 管理者] または [!UICONTROL 請求管理者] また、プロファイルは、アカウント設定内から、アカウント内の他のユーザーに対する配達確認のデフォルトを設定することもできます。

プロファイルについて詳しくは、 [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [個人設定で配達確認のデフォルトを設定 ([!DNL Workfront Proof] ユーザーのみ )](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [受信者に対する E メールアラートの変更](#change-email-alerts-for-a-recipient)
* [ユーザーの配達確認のデフォルトを設定](#configure-proof-defaults-for-a-user)

## 個人設定で配達確認のデフォルトを設定 ([!DNL Workfront Proof] ユーザーのみ )

作成する配達確認の配達確認を設定できます。

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.

1. 次をクリック： **[!UICONTROL 校正の既定値]** タブをクリックします。
1. クリック **[!UICONTROL デフォルトの電子メール通知設定]** 拡張する
1. 次の 2 つの設定の右側にあるドロップダウンリストで、次の表で説明するオプションの 1 つを選択します。

   * **[!UICONTROL デフォルトの電子メールアラート]**：自分と共有されているすべての配達確認に影響します。 この設定は、配達確認レベルで上書きできます。
   * **[!UICONTROL 新しいゲストレビュー担当者向けのデフォルトの電子メールアラート]**：これまでアカウントに連絡先として存在しなかったレビュー担当者に影響します。

   >[!NOTE]
   >
   >次のオプションのいずれかを選択しない場合は、 [!DNL Workfront Proof] は、配達確認に関するアクティビティに関する日次概要を送信します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL すべてのアクティビティ ]</td> 
      <td>[!UICONTROL Workfront] は、新しいコメント、返信、決定など、配達確認に関するアクティビティが発生するたびに、レビュー担当者に電子メールを送信します。 <p>これは、アクティビティの発生を確認できるので、校正プロセスを管理するユーザーにとって最適なオプションです。 </p><p>ユーザーは、自分のアクティビティに関する電子メールアラートを受け取りません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL コメントに返信 ]</td> 
      <td>メールは、誰かが自分のコメントに明示的に返信した場合（自分のコメントに対する自分の返信を除く）にのみ、レビュー担当者に送信されます。 つまり、配達確認の担当者が新しいコメントを作成した場合、レビュー担当者には通知されません。<p>この設定は、配達確認に関する他のコメントが通知されないように、また、自分のコメントに対する返信のみが通知されるように、配達確認のクライアントに対して推奨されます。</p><p>この電子メールアラート設定を持つレビュー担当者は、他の新しいコメントについては通知されませんが、校正ビューアでは、配達確認に関するすべてのコメントを表示できます。</p><p>コメントについて詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">配達確認コメントを表示して返信します</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL の決定 ]</td> 
      <td>[!DNL Workfront] がレビュー担当者に電子メールを送信するのは、誰かが決定を下した場合のみです。<p>これは、承認プロセスを管理し、配達確認の進行状況を監視し、どのユーザーが決定したかを確認する必要がある人（プロジェクトマネージャーなど）に役立ちます。</p><p>決定を送信する際に電子メールの確認オプションを選択しない限り、自分の決定に関する通知は送信されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 最終決定 ]</td> 
      <td>[!DNL Workfront] 配達確認の最後の承認者が決定したら、電子メールを送信します。<p>この警告は多くの場合、実際のレビューディスカッションに参加する必要がないデザイナーが使用します。 最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対して対処できます。</p><p>このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーにも役立ちます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 時間別概要 ]</td> 
      <td>[!DNL Workfront] 1 時間ごとにレビュー担当者に電子メールを送信し、1 時間ごとに発生したすべてのコメント、返信、決定の概要を記録します。<p>この E メールは、過去 1 時間以内に自分自身のアクティビティが発生した場合にのみ送信されます。 </p><p>このアラートは、プロジェクトの概要を確認するのに適しています。</p><p>この概要の使用例としては、プロジェクトの概要を必要とする上級レビュー担当者が挙げられますが、配達確認のすべてのアクティビティをすぐに通知する必要はありません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 日別概要 ]</td> 
      <td>[!DNL Workfront] は、自分自身以外のアクティビティがある日にのみリストされるすべてのコメント、返信、決定を含む 1 つの電子メールを送信します。<p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。</p><p>このサマリの使用例の 1 つに、部門のリーダーがプロジェクトの全体的な進行状況を監視する場合があります。</p><p>詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">配達確認のコメントおよび決定に関する通知を管理</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 電子メールなし ]</td> 
      <td>[!DNL Workfront] は電子メールアラートを送信しません。<br>これは、参照用としてのみ配達確認に追加され、変更を通知する必要がない人に役立ちます。<p>システムのデフォルト値は [!UICONTROL 日別概要 ] です（[!UICONTROL 未設定 ] とも呼ばれます）。 自分または自分のレビュー担当者が他の変更を加えない場合、すべての配達確認にこの設定が適用されます。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 次のいずれかを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 配達確認の準備ができたら電子メールで確認する ]</td> 
      <td>配達確認の作成時に [!UICONTROL Proof maded] 電子メールを受け取るかどうかを指定します。 詳しくは、 <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[!UICONTROL Proof Made] 電子メール</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自分に送信される電子メールの形式 ] </td> 
      <td> <p>HTML形式の E メールとプレーンテキスト E メールのどちらかを選択します。 </p> <p><b>メモ</b></p>
      <p>校正の既定の設定は、配達確認レベルの設定で上書きされます。 ただし、[!UICONTROL アカウント ] の設定でアカウント全体に対して配達確認の電子メール通知が無効になっている場合、配達確認で [!UICONTROL 無効な電子メールアラート ] が選択されていなくても、共同作業者に電子メールアラートは送信されません。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. の下 **[!UICONTROL メッセージ設定]**、次のいずれかを変更します。

   | 配達確認テンプレート | 説明 |
   |---|---|
   | **[!UICONTROL 配達確認の件名テンプレート]** | 新しい配達確認ページ、新しいバージョンページ、メッセージページおよび通知ページに表示されます。 送信前に編集できます。 |
   | **[!UICONTROL 配達確認メッセージテンプレート]** | 新しい配達確認ページ、新しいバージョンページ、メッセージページおよび通知ページに表示されます。 送信前に編集できます。 |

## 受信者に対する E メールアラートの変更

バッチアクションで特定の受信者に関する E メールアラートを変更できます。

1. クリック **[!UICONTROL 連絡先]** （左側のナビゲーションパネル）
1. 次をクリック： **[!UICONTROL その他]** メニュー ![](assets/more-button-small.png) 受信者に対して、「 **[!UICONTROL メンバーの詳細を表示]** 」と入力します。

1. を開きます。 **[!UICONTROL 共有項目]** 」セクションに入力します。
1. 電子メールアラートを変更する各項目の左側にあるチェックボックスを選択します。
1. クリック **[!UICONTROL その他]** 共有アイテムのリストの上に移動し、 **[!UICONTROL メールアラートの変更]** 」と入力します。

1. メールアラートを変更し、「 **[!UICONTROL 送信]**.

## ユーザーの配達確認のデフォルトを設定

次の場合、 [!DNL Workfront Proof] 管理者に問い合わせる場合は、アカウント内のユーザーに対して配達確認のデフォルトを設定できます。

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL アカウント設定]**.

1. を開きます。 **[!UICONTROL ユーザー]** タブをクリックします。
1. を開きます。 **[!UICONTROL その他]** メニュー ![More_button_small.png](assets/more-button-small.png) を使用して、ユーザー名の右側に表示されます。

1. クリック **[!UICONTROL ユーザーの詳細を表示]** 」と入力します。
1. の下 **[!UICONTROL 設定]**&#x200B;をクリックし、 **[!UICONTROL デフォルトのメールアラート設定]** 拡張する

1. 次の 2 つの設定の右側にあるドロップダウンリストで、次の表で説明するオプションの 1 つを選択します。

   * **[!UICONTROL デフォルトの電子メールアラート]**：自分と共有されているすべての配達確認に影響します。 この設定は、配達確認レベルで上書きできます。
   * **[!UICONTROL 新しいゲストレビュー担当者向けのデフォルトの電子メールアラート]**：これまでアカウントに連絡先として存在しなかったレビュー担当者に影響します。

   >[!NOTE]
   >
   >ユーザーに対して次のオプションの 1 つを選択しない場合、 [!DNL Workfront Proof] は、配達確認のアクティビティに関する日別の概要をユーザーに送信します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL すべてのアクティビティ ]</td>
      <td>[!DNL Workfront] 新しいコメント、返信、決定など、配達確認に関するアクティビティが発生するたびに、レビュー担当者に電子メールを送信します。 <p>これは、アクティビティの発生を確認できるので、校正プロセスを管理するユーザーにとって最適なオプションです。 </p><p>ユーザーは、自分のアクティビティに関する電子メールアラートを受け取りません。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL コメントに返信 ]</td>
      <td>メールは、誰かが自分のコメントに明示的に返信した場合（自分のコメントに対する自分の返信を除く）にのみ、レビュー担当者に送信されます。 つまり、配達確認の担当者が新しいコメントを作成した場合、レビュー担当者には通知されません。<p>この設定は、配達確認に関する他のコメントが通知されないように、また、自分のコメントに対する返信のみが通知されるように、配達確認のクライアントに対して推奨されます。</p><p>この電子メールアラート設定を持つレビュー担当者は、他の新しいコメントについては通知されませんが、校正ビューアでは、配達確認に関するすべてのコメントを表示できます。</p><p>コメントについて詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">配達確認コメントを表示して返信します</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL の決定 ]</td>
      <td>[!DNL Workfront] がレビュー担当者に電子メールを送信するのは、誰かが決定を下した場合のみです。<p>これは、承認プロセスを管理し、配達確認の進行状況を監視し、どのユーザーが決定したかを確認する必要がある人（プロジェクトマネージャーなど）に役立ちます。</p><p>決定を送信する際に電子メールの確認オプションを選択しない限り、自分の決定に関する通知は送信されません。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 最終決定 ]</td>
      <td>[!DNL Workfront] 配達確認の最後の承認者が決定したら、電子メールを送信します。<p>この警告は多くの場合、実際のレビューディスカッションに参加する必要がないデザイナーが使用します。 最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対して対処できます。</p><p>このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーにも役立ちます。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 時間別概要 ]</td>
      <td>[!DNL Workfront] 1 時間ごとにレビュー担当者に電子メールを送信し、1 時間ごとに発生したすべてのコメント、返信、決定の概要を記録します。<p>この E メールは、過去 1 時間以内に自分自身のアクティビティが発生した場合にのみ送信されます。 </p><p>このアラートは、プロジェクトの概要を確認するのに適しています。</p><p>この概要の使用例としては、プロジェクトの概要を必要とする上級レビュー担当者が挙げられますが、配達確認のすべてのアクティビティをすぐに通知する必要はありません。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 日別概要 ]</td>
      <td>[!DNL Workfront] は、自分自身以外のアクティビティがある日にのみリストされるすべてのコメント、返信、決定を含む 1 つの電子メールを送信します。<p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。</p><p>このサマリの使用例の 1 つに、部門のリーダーがプロジェクトの全体的な進行状況を監視する場合があります。</p><p>詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">配達確認のコメントおよび決定に関する通知を管理</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL 電子メールなし ]</td>
      <td>[!DNL Workfront] は電子メールアラートを送信しません。<br>これは、参照用としてのみ配達確認に追加され、変更を通知する必要がない人に役立ちます。<p>システムのデフォルト値は [!UICONTROL 日別概要 ] です（[!UICONTROL 未設定 ] とも呼ばれます）。 自分または自分のレビュー担当者が他の変更を加えない場合、すべての配達確認にこの設定が適用されます。</p></td>
     </tr>
    </tbody>
   </table>

1. 残りの **[!UICONTROL デフォルトのメールアラート設定]**、次のいずれかを変更します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 配達確認の準備ができたら電子メールで確認する ]</td> 
      <td>配達確認の作成時に [!UICONTROL Proof maded] 電子メールを受け取るかどうかを指定します。 詳しくは、 <a href="https://support.workfront.com/hc/en-us/article">[!UICONTROL Proof Made] 電子メール。</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自分に送信される電子メールの形式 ] </td> 
      <td> <p>HTML形式の E メールとプレーンテキスト E メールのどちらかを選択します。 </p> <p><b>メモ</b></p> <p>校正の既定の設定は、配達確認レベルの設定で上書きされます。 ただし、[!UICONTROL アカウント ] の設定でアカウント全体に対して配達確認の電子メール通知が無効になっている場合、配達確認で [!UICONTROL 無効な電子メールアラート ] が選択されていなくても、共同作業者に電子メールアラートは送信されません。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
