---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: 「個人設定」の指定
description: ' [!DNL Adobe Workfront]  プロファイルには、自分に関する情報（名前、メールアドレス、住所、電話番号、役職など）が含まれます。また、 [!DNL Workfront]  および社内の他のユーザーとのインタラクションに関する情報も含まれます。'
author: Nolan
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: a750d2707699e1d4783d950807138a74baf78715
workflow-type: tm+mt
source-wordcount: '3311'
ht-degree: 80%

---

# 「個人設定」の指定

<!-- Audited: 01/2024 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

[!DNL Adobe Workfront] プロファイルには、自分に関する情報（名前、メールアドレス、住所、電話番号、役職など）が含まれます。また、[!DNL Workfront] および社内の他のユーザーとのインタラクションに関する情報（例えば、通知設定、[!DNL Workfront] で表示するタブ、担当業務、管理者、グループとチームのメンバーシップなど）も含まれます。

この情報のほとんどは、[!DNL Workfront] アカウントの作成時に [!DNL Workfront] 管理者によって既に設定されています。

[!DNL Workfront] でのアクセスレベルに応じて[!UICONTROL 個人設定]領域を設定することにより、この情報の一部を編集できます。

## アクセスレベルに応じた[!UICONTROL 個人設定]エリアの編集

アクセスレベルに応じて、[!UICONTROL 個人設定]エリアで編集できるセクションが異なります。

編集可能なセクションに含まれるフィールドでも、アクセスレベルでの他の設定の内容によっては、編集できないことがあります。[!UICONTROL 個人設定]の一部のフィールドの編集に追加で必要なアクセス権について詳しくは、[[!UICONTROL 個人設定]エリアの設定](#configuring-the-my-settings-area)を参照してください。

現在のアクセスレベルを確認するには、[!DNL Workfront] 管理者にお問い合わせください。

次の表は、アクセスレベルに応じて[!UICONTROL 個人設定]エリアのどのセクションが表示または編集可能であるかを示しています。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!UICONTROL My Settings]エリア</strong> </th> 
   <th><strong>表示または編集可能</strong> </th> 
   <th><strong>[!UICONTROL System Administrator]</strong> </th> 
   <th><strong>[!UICONTROL Standard] または [!UICONTROL Planner]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Light] または [!UICONTROL Reviewer]</strong> </th> 
   <th><strong>[!UICONTROL コントリビューター ] または [!UICONTROL リクエスト元 ]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL Personal Info]</td> 
   <td> <p>表示</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td> <p>編集可能</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Preferences]</td> 
   <td> <p>表示</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>編集可能</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Notifications]</td> 
   <td> <p>表示</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>編集可能</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Access]</td> 
   <td>表示</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編集可能</td> 
   <td> ✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Organization]</td> 
   <td>表示</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編集可能</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Resource Planning]</td> 
   <td>表示</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編集可能</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Custom Forms]</td> 
   <td>表示</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>編集可能</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Comment]</td> 
   <td>表示</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>編集可能</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 個人設定]エリアの設定

{{step1-click-profile-pic}}

1. 次をクリック： **[!UICONTROL その他]** 名前の横のメニュー ![その他のメニュー](assets/more-icon.png)を選択し、次に **[!UICONTROL 編集]**.

1. アクセスレベルに応じて、次のセクションを更新できます。

   * [個人情報](#personal-info)
   * [環境設定](#preferences)
   * [通知](#notifications)
   * [アクセス](#access)
   * [組織](#organization)
   * [リソース計画](#resource-planning)
   * [カスタムフォーム](#custom-form)
   * [コメント](#comment)

1. 「**[!UICONTROL 保存]**」をクリックします。

### [!UICONTROL 個人情報]

このセクションには、次のサブセクションがあります。

* [基本情報](#basic-info)
* [業務内容](#job-info)
* [連絡情報](#contact-info)

#### [!UICONTROL 基本情報]

この情報は、[!DNL Workfront] 管理者によって既に設定されているはずです。このサブセクションのフィールドはすべて必須フィールドです。

このサブセクションでは、次のいずれかを変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL First Name]</strong></td> 
   <td>名前（名）を更新します。必須フィールドです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Last Name]</strong></td> 
   <td>名前（姓）を更新します。必須フィールドです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Email Address]</strong></td> 
   <td> メールアドレスを更新します。必須フィールドです。メールアドレスは、[!DNL Workfront] のユーザー名となります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Reset password]</strong></td> 
   <td>このセクションでパスワードをリセットします。パスワードのリセットについて詳しくは、<a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">パスワードのリセット</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）&lt;SSO Configuration&gt; [!UICONTROL Username]</strong></td> 
   <td> [!DNL Workfront] 管理者が [!DNL Workfront] との SSO 統合を有効にした場合、SSO ユーザー名がこのフィールドに表示されます。[!DNL Workfront] インスタンスに対して有効にされた SSO 設定のタイプは、このフィールドに表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）[!UICONTROL Only Allow &lt;SSO Configuration&gt; Authentication]</strong></td> 
   <td> <p> [!DNL Workfront] 管理者が [!DNL Workfront] との SSO 統合を有効にして SSO 用にユーザーを更新した場合、このフィールドはデフォルトで選択されます。[!DNL Workfront] インスタンスに対して有効にされた SSO 設定のタイプは、このフィールドに表示されます。</p> <p>このフィールドを選択した場合、SSO 資格情報で [!DNL Workfront] にログインすることが必要です。選択を解除すると、[!DNL Workfront] 資格情報で [!DNL Workfront] にログインできるようになります。</p> <p>SSO ソリューションで [!DNL Workfront] の設定について詳しくは、<a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">[!DNL Adobe Workfront]</a> でのシングルサインオンを参照してください。SSO のユーザーの更新について詳しくは、<a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">シングルサインオンのユーザーの更新</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 業務内容]

このサブセクションでは、次のいずれかを変更できます。

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Title]</strong></td>
        <td>タイトルを指定します。これは担当業務とは異なります。タイトルは、リソーススケジュール設定の一部ではありませんが、担当業務はその一部です。タイトルは、[!DNL Workfront] インターフェイスでユーザーの名前とアバターが表示される場所に表示されます。ユーザープロファイルを表示するためのアクセス権を持つすべてのユーザーに表示されます。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Talk to Me About]</strong></td>
        <td>このフィールドに職業上の関心を指定します。</td>
    </tr>
</table>

#### [!UICONTROL 連絡情報]

このサブセクションでは、次のいずれかを変更できます。

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Phone Number]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Extension]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Mobile Number]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Address]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL State]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Postal Code]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Country]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Profile Picture]</strong></td>
        <td>プロファイル画像がアバターになり、[!DNL Workfront] システムを通じて名前が表示される場所に表示されます。</td>
    </tr>
</table>

### [!UICONTROL 環境設定]

このセクションの [!DNL Workfront] インターフェイスで表示する内容を指定します。

>[!NOTE]
>
>を持つユーザー [!UICONTROL 寄稿者] または [!UICONTROL 要求者] ライセンスには、他にパネルに追加できる項目はありません [!UICONTROL メインメニュー]( [!UICONTROL リクエスト] 領域。 A [!DNL Workfront] 管理者は、 [!UICONTROL 寄稿者] または [!UICONTROL 要求者] 内の他のすべての領域を含むレイアウトテンプレートのライセンス [!UICONTROL メインメニュー]. その後、ユーザープロファイルを編集することで、[!UICONTROL メインメニュー]で表示する領域を選択できます。

このサブセクションでは、次のいずれかを変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Time Zone]</strong> </td> 
   <td><p>タイムゾーンを指定します。これは、送信するメールメッセージに表示される時間を制御します。</p>
       <p>タイムゾーンは、PTO カレンダーレポートに表示される内容にも影響します。</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Email Locale]</strong> </td> 
   <td>ここで目的の言語を指定します。これは、送信メールメッセージで使用される言語、日付、数値の形式を制御します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Show percent completepercent complete on update status]</strong> </td> 
   <td>従来のコメントエクスペリエンスを使用する際に、タスクの更新領域内に完了率のバーを表示する場合は、このオプションを選択します。 詳しくは、 <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">新しいコメントエクスペリエンス</a>.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Send work assigned to myself to my Working On tab]</strong> </td> 
   <td>このフィールドを選択して、自分に直接割り当てている作業を「[!UICONTROL Work Requests]」タブではなく「[!UICONTROL Working On]」タブで表示します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）Automatically generate proofs when uploading documents</strong></td> 
   <td>ドキュメントが [!DNL Workfront] に読み込まれた直後にプルーフの生成を開始するには、このフィールドを選択します。このフィールドはデフォルトで無効になっており、Workfront 管理者のみが更新できます。<br>このフィールドは、Workfront の Workfront Proof コンポーネントを購入し、プルーフユーザーとして有効になっている場合にのみ表示されます。Workfront Proof について詳しくは、<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Adobe Workfront 内でのプルーフの管理</a>を参照してください。
   <p><b>メモ：</b>リクエストにアップロードされたドキュメントは、プルーフを自動生成しません。 </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 通知]

受信する通知を指定します [!DNL Workfront]. 通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL アクセス]

アクセスおよびそれに関連付けられている他のコンポーネントは、アカウントの設定時に [!DNL Workfront] 管理者によって設定されます。

[!DNL Workfront] 管理者のみが、このセクションのすべてのフィールドを表示して編集できます。

このサブセクションでは、次のいずれかを変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
   <td>このフィールドは、[!DNL Workfront] 管理者でもあるユーザーにのみ表示され、デフォルトでオンにする必要があります。これは、ユーザーがアクティブで、ログインできることを示します。 [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Access Level]</strong> </td> 
   <td>このフィールドは、[!UICONTROL Standard]、[!UICONTROL Plan]、または [!UICONTROL Workfront] 管理者のアクセスレベルのユーザーに対して表示され、次の場合にのみ編集可能です。 [!DNL Workfront] 管理者。[!DNL Workfront] 管理者は、このフィールドを変更する際に、アクセスレベルを低い値に変更しないように注意してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Layout Template]</strong> </td> 
   <td>このフィールドは、[!UICONTROL 標準 ]、[!UICONTROL プラン ] または [!UICONTROL [!DNL Workfront] administrator] アクセスレベルで、[!UICONTROL] でのみ編集可能 [!DNL Workfront] [!UICONTROL Standard] または [!UICONTROL Plan] ライセンスを持つ、管理者 ] または管理者ユーザー（管理者ユーザーアクセス権も持つユーザー） ここでレイアウトテンプレートを選択し、Workfront インターフェイスの外観とフィールドを更新します。管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>の<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">カスタムアクセスレベルを使用してユーザーを編集するためにユーザーのアクセス権を設定</a>を参照してください。<br>レイアウトテンプレートとお使いのインターフェイスへの影響について詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>を参照してください。</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）[!UICONTROL User can generate proofs (... out of ... proof licenses left)]</strong></td> 
   <td>このフィールドは、従来の [!DNL Workfront] プランを使用し、[!DNL Workfront Proof] コンポーネントを購入した場合にのみ使用できます。このオプションを選択すると、プルーフユーザーとして有効になります。購入したプルーフライセンスの合計数の中で、システムで使用されているプルーフライセンスの数も表示されます。このフィールドは、[!DNL Workfront] 管理者でもあるユーザーのみが表示および編集できます。[!DNL Workfront] でのプルーフのためのプランオプションについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">[!DNL Workfront]</a> のプルーフ機能へのアクセスを参照してください。</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）[!UICONTROL Permission Profile]</strong></td> 
   <td> <p>このフィールドには、[!DNL Workfront Proof] で持つアクセスレベルが表示されます。次の場合にのみ使用できます。</p> 
    <ul> 
     <li>レガシーを使用している [!DNL Workfront] プランおよび購入済み [!DNL Workfront Proof] コンポーネントを使用しているか、新しい [!DNL Workfront] プラン</li> 
     <li>プルーフユーザーとして有効になっています。</li> 
    </ul> <p>[!DNL Workfront] 管理者は、自分を除くすべてのユーザーのフィールドを編集できるので、すべてのユーザーは、自分のプロファイルでこのフィールドを表示のみとして表示できます。権限プロファイルについて詳しくは、<a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">プルーフ権限プロファイルの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 組織]

この情報は通常、[!DNL Workfront] 管理者が [!DNL Workfront] アカウントを作成する際に設定します。また、このセクションでは、組織や組織の構造に関する情報を更新することもできます。次を持つユーザーのみ： [!UICONTROL 標準], [!UICONTROL プラン]または [!UICONTROL システム管理者] アクセスレベルでこのセクションを編集できます。

このサブセクションでは、次のいずれかを変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Company]</strong></td> 
   <td>ドロップダウンリストから、所属先の会社名を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）[!UICONTROL Reports To]</strong></td> 
   <td>プロファイルで <strong>[!UICONTROL Company]</strong> を選択した後、このフィールドでマネージャーの名前を指定できます。ここで指定できる名前は 1 名のみなので、直属のマネージャーの名前を指定することをお勧めします。名前を入力し、リストに表示されたらクリックして選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）[!UICONTROL Direct Reports]</strong></td> 
   <td>プロファイルで <strong>[!UICONTROL Company]</strong> を選択した後、このフィールドで直属の部下の名前を指定できます。ここでは、必要な数の直属の部下を指定できます。名前を入力し、リストに表示されたら、クリックして選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Team]</strong> </td> 
   <td> <p>ドロップダウンメニューから <strong>[!UICONTROL Home Team]</strong> を選択します。このフィールドは、[!UICONTROL Standard]、[!UICONTROL Plan]、または [!UICONTROL System Administrator] のアクセスレベルのユーザーに対して表示され、次の場合にのみ編集可能です。 [!DNL Workfront] [!UICONTROL Standard] または [!UICONTROL Plan] ライセンスを持つ管理者またはユーザーで、管理者ユーザーアクセス権も持っているもの。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>の<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">カスタムのアクセスレベルを使用して、ユーザーを編集するユーザーのアクセス権を設定</a>を参照してください。<br></p> <p>レイアウトテンプレートがチームに関連付けられている場合、<strong>ホームチーム</strong>は [!DNL Workfront] インターフェースのルックアンドフィールに影響する可能性があります。 </p> <p>チームについて詳しくは、 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">チームの概要</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Teams]</strong> </td> 
   <td> <p>複数のチームに所属できます。このフィールドに所属するチーム名を指定し、リストに表示されたら、クリックして選択します。チームが多すぎると、チームに割り当てられた作業について混乱が生じる可能性があります。チームについて詳しくは、<a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">チームの概要</a>を参照してください。</p> <p>このフィールドは、[!UICONTROL Standard]、[!UICONTROL Plan]、または [!UICONTROL System Administrator] のライセンスを持つユーザーに対して表示され、次の場合にのみ編集可能です。 [!DNL Workfront] [!UICONTROL Standard] または [!UICONTROL Plan] ライセンスを持つ管理者またはユーザーで、管理者ユーザーアクセス権も持っているもの。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>の<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">カスタムのアクセスレベルを使用して、ユーザーを編集するユーザーのアクセス権を設定</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Group]</strong> </td> 
   <td> <p>ドロップダウンメニューから <strong>[!UICONTROL Home Group]</strong> を選択します。</p> <p>メモ：これは必須フィールドです。グループに関連付けられていないユーザーを持つことはできません。<br></p> <p>このフィールドは、[!UICONTROL Standard]、[!UICONTROL Plan] または [!UICONTROL System Administrator] レベルのユーザーに表示されます。 を編集できるユーザーの詳細 <strong>[!UICONTROL ホームグループ ]</strong> フィールド：詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">ユーザーのプロファイルの編集</a>. お使いの <strong>[!UICONTROL ホームグループ ]</strong> は、すべてのプロジェクトのデフォルトグループで、デフォルトは <strong>[!UICONTROL ホームグループ ]</strong> 作成するすべての新規ユーザー用。 作成するカスタムフォームは、デフォルトで<strong>[!UICONTROL Home Group]</strong> と共有されます。</p> <p>グループについて詳しくは、<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Groups]</strong> </td> 
   <td> <p>複数のグループに所属できます。グループ名を入力して、このフィールドに所属する追加のグループを指定します。リストに表示されたら、クリックして選択します。このフィールドは、[!UICONTROL Standard]、[!UICONTROL Plan] または [!UICONTROL System Administrator] のアクセスレベルのユーザーに対して表示されます。 を編集できるユーザーの詳細 <strong>[!UICONTROL その他のグループ ]</strong> フィールド：詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">ユーザーのプロファイルの編集</a>.</p> <p>グループについて詳しくは、<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL リソース計画]

リソース計画の情報は、作業割り当てのタイムライン、ログ時間、コストおよび現在のプロジェクトの収益に影響します。通常、このエリアは [!DNL Workfront] 管理者、プロジェクトマネージャーかリソースマネージャー、またはダイレクトマネージャによって設定されます。

このセクションでは、次のいずれかを使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Schedule Deactivation]</strong></td> 
   <td>一定期間後にアカウントを非アクティブ化するようにスケジュールする場合は、このチェックボックスをオンにします。表示される <p><strong>[!UICONTROL Scheduled Deactivation Date]</strong> で、アカウントが非アクティブ化される日付を指定します。ユーザーの非アクティブ化について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a>の<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation" class="MCXref xref">ユーザーの非アクティブ化のスケジュール</a>を参照してください。</p><p>[!UICONTROL Standard] または [!UICONTROL Plan] のライセンスをお持ちの場合や、 [!DNL Workfront] 管理者。 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Primary Role]</strong></td> 
   <td> <p>これは、Workfront で実行できる主な担当業務です。割り当てられているすべてのタスクやイシューも、デフォルトでこの担当業務に割り当てられます。リソース管理には、担当業務が不可欠です。担当業務について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> <p>このフィールドは、[!UICONTROL Standard] または [!UICONTROL Plan] のライセンスを管理者ユーザーがアクセスできる場合、または [!DNL Workfront] 管理者。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>の<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">カスタムアクセスレベルを使用してユーザーのアクセス権を設定することでユーザーを編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）[!UICONTROL Primary Role] を選択した場合は、[!UICONTROL Percentage of FTE Availability] フィールドが表示されます。</strong></td> 
   <td>この担当業務に割り当てる予定時間の割合を指定します。プライマリロールの [!UICONTROL FTE 可用性の割合 ] のデフォルト値は 100%です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Roles]</strong> </td> 
   <td> <p>[!DNL Workfront] では複数の担当業務を持つことができます。リソース管理には、担当業務が不可欠です。担当業務について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> <p>このフィールドは、[!UICONTROL Standard] または [!UICONTROL Plan] のライセンスを管理者ユーザーがアクセスできる場合、または [!DNL Workfront] 管理者。 管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>の<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">カスタムアクセスレベルを使用してユーザーのアクセスを設定することでユーザーを編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（条件付き）1 つ以上の他の役割を選択した場合、各役割に対して「[!UICONTROL Percentage of FTE Availability]」フィールドが表示されます。</strong></td> 
   <td> <p>各担当業務に割り当てる予定時間の割合を指定します。[!UICONTROL Other Roles] の [!UICONTROL Percentage of FTE Availability] のデフォルト値は 0% です。</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_dte_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>メモ：  
     <ul> 
      <li>[!UICONTROL Other Roles] の FTE 使用可能時間が 0％の場合、ユーザーがこれらの役割のタスクに割り当てられていない限り、[!UICONTROL Resource Planner] には表示されません。</li> 
      <li> <p>すべての役割の <strong>[!UICONTROL Percentages of FTE Availability]</strong> 合計は、100％になる必要があります。[!UICONTROL Percentage of FTE Availability] ごとに、[!UICONTROL Resource Planner] の各ユーザーの役割について [!UICONTROL Available Hours] が計算されます。 </p> <p>各ユーザーの役割の [!UICONTROL Available Hours] は、ユーザーの空き時間数によって異なります。ユーザーの空き時間数は、[!UICONTROL Resource Management Preferences] で FTE を計算するために [!DNL Workfront] 管理者によって選択されたメソッドで、[!DNL Workfront] により計算されます。ユーザーの空き時間の計算について詳しくは、<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナーのユーザーと役割に対する時間と FTE の計算の概要</a>を参照してください。リソース管理環境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理環境設定の指定</a>を参照してください。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>スケジュール</strong></td> 
   <td> <p>のみ [!DNL Workfront] [!UICONTROL Standard] または [!UICONTROL Plan] のライセンスを持つ管理者またはユーザーで、タイムシートと時間に対する管理者アクセス権を持っている場合は、このフィールドを更新できます。 タイムシートと時間の管理アクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>の「タイムシートと時間数」の節を参照してください。</p> <p>ドロップダウンメニューから正しいタイムシートを選択します。これにより、[!DNL Workfront] 管理者によって指定された設定に従って、タイムシートが自動的に生成されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Default Hour Type]</strong> </td> 
   <td>デフォルトの時間タイプを選択します。Workfront で時間を記録する際に、デフォルトでシステムが使用する時間タイプです。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Available Hour Types]</strong> </td> 
   <td>時間をログ記録する際に、選択できる時間タイプを選択します。このドロップダウンメニューの時間タイプは、[!DNL Workfront] 管理者によって設定されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Resource Pool]</strong> </td> 
   <td>所属するリソースプールを選択します。このフィールドは、レポートおよび情報提供の目的でのみ使用します。 リソースのスケジュール設定や計画には影響しません。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>ここで指定する数字は、システムレベルの [!UICONTROL Resource Management Preferences] が <strong>[!UICONTROL The Default Schedule]</strong> に設定されている場合にのみ、デフォルトスケジュールに基づいて空き時間を計算するために考慮されます。</p> <p>例えば、FTE 値が 0.5 で、[!UICONTROL Default Schedule]が 40 時間の場合、週に 20 時間働くことができます。</p> <p>システムレベルで[!UICONTROL Resource Management Preferences]を <strong>[!UICONTROL The User's Schedule]</strong>に設定すると、ここで指定した値は無視され、スケジュールに指定された値に従って作業できるようになります。この場合、[!UICONTROL Resource Planner]の FTE は次の式で計算されます。 </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>ユーザー FTE の計算について詳しくは、<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナのユーザーと役割に対する時間と FTE の計算の概要</a>を参照してください。</p> <p>[!DNL Workfront] でのスケジュール作成について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールの作成</a>を参照してください。</p> <p>リソース管理環境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理環境設定の指定</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Cost per Hour]</strong> </td> 
   <td>ユーザーの 1 時間あたりのコストの量を指定します。[!DNL Workfront] でのコストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。この情報を更新するには、自分のアクセスレベルの財務データにアクセスできるか、[!DNL Workfront] 管理者である必要があります。財務アクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Billing per Hour]</strong> </td> 
   <td>ユーザーの 1 時間あたりの請求額を指定します。請求と売上高のトラッキングについて詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a>を参照してください。この情報を更新するには、自分のアクセスレベルの財務データにアクセスできるか、[!DNL Workfront] 管理者である必要があります。財務アクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a>を参照してください。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL カスタムフォーム]

カスタムフォームをユーザープロファイルに関連付けることができます。これにより、ユーザーに関する追加情報を保存できます。追加情報を保存しないと、上記で説明した [!DNL Workfront] ネイティブフィールドに保存することができません。

カスタムフォームをユーザープロファイルに添付するには、次のアクセス権または権限が必要です。

* [!DNL Workfront] 管理者であること。
* あなたは [!UICONTROL 標準] または [!UICONTROL プラン] ライセンスユーザーとユーザーカスタムフォームが、グループの 1 つと共有されている。

すべてのユーザーが、自分のプロファイルに関連付けられたカスタムフォームを表示できます。

ユーザープロファイルにカスタムフォームを添付できるようにするには、[!DNL Workfront] 管理者がユーザーオブジェクトのカスタムフォームを設定する必要があります。カスタムフォームの作成について詳しくは、[カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

### [!UICONTROL コメント]

ユーザープロファイルに対するコメントを記録できます。ユーザープロファイルはプロファイルの [!UICONTROL 更新] タブをクリックします。

[!UICONTROL ユーザー]アイコンをクリックして、他の人をアップデートに含めることができます。

[!UICONTROL ロック]アイコンをクリックして、自分と同じ会社に属するユーザーに対してこの更新を非公開にできます。
