---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 配達確認の新しいバージョンの作成
description: 複数のバージョンや作品の改訂をまたいでフィードバックを管理することは、大きな課題となります。 Workfrontでは、配達確認の複数のバージョンを作成および比較できるので、このプロセスが簡単になります。
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# 配達確認の新しいバージョンの作成

複数のバージョンや作品の改訂をまたいでフィードバックを管理することは、大きな課題となります。 Workfrontでは、配達確認の複数のバージョンを作成および比較できるので、このプロセスが簡単になります。

配達確認の新しいバージョンを作成する際は、次の情報を考慮します。

* ユーザーに、あるバージョンを表示する権限を与えることができますが、別のバージョンを表示する権限を与えることはできません。 反対に、ユーザーと新しいバージョンを共有した場合、戻って以前のバージョンへのアクセス権を明示的に付与しない限り、そのユーザーは以前のバージョンを表示できません。
* 配達確認の新しいバージョンを作成するには、配達確認の編集権限が必要です。

   詳しくは、 [Workfront Proof での配達確認の役割の管理](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) および [Workfront Proof の配達確認権限プロファイル](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 配達確認の編集権限を持つユーザーの詳細を取得します。

   配達確認のバージョンの共有について詳しくは、  [Workfrontの配達確認での配達確認の共有](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Adobe Workfront内で配達確認を作成した場合は、その配達確認用に新しく作成したバージョンもWorkfront内で作成する必要があります。 Workfront内で作成された配達確認の場合、Workfrontの配達確認内で新しいバージョンの配達確認を作成することはできません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：選択またはプレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャ以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## Workfrontでの配達確認の新しいバージョンの作成

Workfrontで新しい配達確認バージョンをアップロードするには、いくつかの方法があります。 デフォルトの配達確認設定は、選択した方法に応じて、以前のバージョンから引き継ぐ場合と引き継がない場合があります。

* **ドキュメントのアップロード時に配達確認を自動生成**:デフォルトの配達確認設定は引き継がれません。 ユーザープロファイルでこの設定を有効にしている場合、新しいバージョンをドラッグ&amp;ドロップしても、デフォルトの配達確認設定は有効になりません。
* **配達確認を作成/シンプル**:デフォルトの配達確認設定は引き継がれません。 新しい配達確認バージョンを作成するときに「シンプル」を選択した場合、デフォルトの配達確認設定は以前のバージョンから引き継がれません。
* **新規追加/バージョン/配達確認**:デフォルトの配達確認設定は、以前のバージョンから引き継がれます。
* **配達確認を作成/詳細**:デフォルトの配達確認設定は、以前のバージョンから引き継がれます。

   <table>
  <tbody>
  <tr>
  <td>ドキュメントのアップロード中に自動的にプルーフを作成する</td>
  <td>デフォルトの配達確認設定は引き継がれません。 ユーザープロファイルでこの設定を有効にしている場合、新しいバージョンをドラッグ&amp;ドロップしても、デフォルトの配達確認設定は有効になりません。</td>
  </tr>
  <tr>
  <td>配達確認を作成/シンプル</td>
  <td>デフォルトの配達確認設定は引き継がれません。 新しい配達確認バージョンを作成するときに「シンプル」を選択した場合、デフォルトの配達確認設定は以前のバージョンから引き継がれません。</td>
  </tr>
  <tr>
  <td>新規追加/バージョン/配達確認</td>
  <td>デフォルトの配達確認設定は、以前のバージョンから引き継がれます。</td>
  </tr>
  <tr>
  <td>配達確認を作成/詳細</td>
  <td>デフォルトの配達確認設定は、以前のバージョンから引き継がれます。</td>
  </tr>
  </tbody>
  </table>




配達確認の新しいバージョンを作成するには：

1. 配達確認を含むドキュメントのリストを開きます。
1. コンピューターのファイルシステムから、新しいファイルを配達確認の上にドラッグ&amp;ドロップします。

   または

   配達確認が表示される行を選択し、「 **新規追加** > **バージョン**&#x200B;次に、配達確認の新しいバージョンの追加に使用するオプションをクリックします。

   ![](assets/add-new-version-350x185.png)

## 校正ビューアからの配達確認の新しいバージョンの作成 (Workfront Proof のみ )

スタンドアロンのWorkfront Proof を使用している場合は、単一のファイルまたは Web キャプチャを含む新しいバージョンの配達確認を作成できます。 

>[!NOTE]
>
>アカウントがエンタープライズプラン上にあり、複数のファイルや Web キャプチャをアップロードした場合、それらは自動的に 1 つの新しいバージョンに結合されます。 詳しくは、 [複数ページの配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) を参照してください。

Workfront Proof で新しいバージョンの配達確認を作成するには：

1. 配達確認を開きます。
1. 次をクリック： **バージョン** 左上隅のドロップダウンメニューで、 **+新しいバージョン** をクリックします。

   の **の新しい配達確認バージョン** 表示されるページで、以前のバージョンのすべてのレビュー担当者（役割や電子メール通知の設定を含む）を確認できます。 既存のレビュー担当者の役割や通知を簡単に編集したり、このページの新しいバージョンから既存のレビュー担当者を削除したりできます。

1. の下 **ファイルを追加**、コンピューターからドラッグ&amp;ドロップするか、「 **参照** をクリックし、必要なファイルを選択します。 次の項目を入力できます。 **配達確認名** バージョンの場合は、このボックスを空白のままにして、同じファイル名の末尾にバージョン番号を追加します。

   または

   URL を入力して、配達確認の新しいバージョンとして Web ページを取り込みます。

   >[!NOTE]
   >
   >ドラッグ&amp;ドロップは、HTML5 を完全にサポートするブラウザーでのみ使用できます。 これには、Internet Explorer 7 ～ 9 および Safari が含まれません。

1. の下 **ワークフロー**、次のいずれかの変更を行って、このバージョンの配達確認のレビュー担当者を指定します。

   以前のバージョンのレビュー担当者は、追加したレビュー担当者に置き換えられます。

   * を **所有者** のバージョンを、アカウント内の別のユーザーに割り当てます。\
      所有者権限について詳しくは、 [Workfront Proof の配達確認権限プロファイル](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * の使用 **連絡先名または電子メールアドレスを入力して受信者ボックスを追加**、バージョンにレビュー担当者を追加します。 次の項目を指定できます。 **配達確認の役割** および **E メールアラート** 各受信者のタイプ。

      配達確認へのグループの追加について詳しくは、  [配達確認へのグループの追加](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). 役割について詳しくは、 [Workfront Proof での配達確認の役割の管理](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      >[!NOTE]
      >
      >配達確認の作成者または所有者が [配達確認が E メールを送信しました](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) （個人設定で）デフォルトで無効になっている場合、新しい配達確認ページの「 E メールで人に通知」ボックスがオンになっていても、作成済みの配達確認または新しい配達確認の電子メールは受信されません。 電子メール通知について詳しくは、 [Workfront Proof での電子メール通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). 関連トピック [配達確認が E メールを送信しました](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) および [新しい配達確認 E メール](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * バージョンの配達確認の期限を設定します。
   * レビュー担当者の名前の上にマウスポインターを置くと、以前のバージョンでおこなった決定が表示されます。

1. の下 **電子メール通知**、次のいずれかの操作を行います。

   * 新しいバージョンをレビュー担当者に通知するかどうかを指定します。\
      選択した内容が、配達確認の詳細ページの「アクティビティ」セクションに記録されます。 詳しくは、 [Workfront配達確認で配達確認の詳細を管理](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * カスタム件名とメッセージを追加します。

1. 内 **組織** セクションで、次のいずれかの操作を行います。 

   * 配達確認に 1 つ以上のタグを適用します。 詳しくは、 [Workfront Proof でのタグの作成と管理](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
      タグは、以前のバージョンの配達確認からも継承されます。 新しいバージョンに新しいタグを追加すると、以前のバージョンもタグ付けされます。

   * フォルダーにバージョンを追加します。 詳しくは、 [Workfront Proof でのフォルダーの管理](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) を参照してください。 このフォルダーは、配達確認の以前のバージョンからコピーされます。 別のフォルダーを選択すると、配達確認全体（すべてのバージョン）が移動されます。

   * 請求管理者および管理者は、「設定」タブのアカウント全体で、フォルダーフィールドを必須フィールドに設定できます。 詳細は、を参照してください。

1. 「配達確認の設定」で、次のいずれかの変更をおこないます。

   * 配達確認にログインする必要があります
   * 配達確認に電子署名が必要（エンタープライズプランのみ）
   * すべての決定がおこなわれたら配達確認をロックする
   * 元のファイルのダウンロードを許可またはブロック
   * 公開共有設定を含む、配達確認の公開共有
   * 配達確認の購読\
      このセクションでの選択は、配達確認の詳細ページに表示されます（一部のフィールドは編集可能）。 詳しくは、 [Workfront配達確認で配達確認の詳細を管理](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## 新しいバージョンのメッセージについて

以前のバージョンの配達確認にカスタムの件名/メッセージが含まれていた場合は、デフォルトで新しいバージョンページに表示されます。 次の操作が可能です。

* 件名とメッセージを編集します。
* 「電子メールで人に通知」ボックスの選択を解除します。つまり、レビュー対象の新しいバージョンがあることをレビュー担当者に通知する電子メールがレビュー担当者に送信されません。

   >[!NOTE]
    個人設定に保存されるデフォルトのカスタム件名/メッセージの影響は受けません。

デフォルトの件名とメッセージが個人設定に保存されている場合、これは、新しいバージョンページにデフォルトで表示されるメッセージに影響します。

* 標準の E メールを使用して、以前のバージョンの配達確認の E メールでレビュー担当者に通知する場合（例：カスタムの件名やメッセージがない場合）、デフォルトのカスタムの件名やメッセージ（個人設定）が新しいバージョンページに表示されます。 その後、カスタムの件名とメッセージを編集するか、「電子メールで担当者に通知」ボックスの選択を解除できます（レビュー対象の新しいバージョンがあることをレビュー担当者に通知する電子メールは送信されません）。
* 以前のバージョンの配達確認に対して E メールでレビュー担当者に通知しない場合（標準 E メールやカスタム E メールがない場合など）、新しいバージョンページにはデフォルトでメッセージが含まれません。 新しいバージョンをレビュー担当者に通知するには、「メッセージを送信」リンクをクリックします。このリンクには、（個人の設定に従って）デフォルトのカスタム件名/メッセージが表示されます。 必要に応じて、カスタム件名とメッセージを編集できます。

個人設定にデフォルトの件名とメッセージが保存されていない場合、新しいバージョンページに次の情報が表示されます。

* 標準の E メールを使用して、配達確認の前のバージョンのレビュー担当者に E メールで通知する場合（例えば、カスタムの件名やメッセージがない場合）、新しいバージョンページでは、「E メールで人に通知」オプションがデフォルトで選択されます。 カスタムメッセージを追加するには、リンクをクリックします。
* 以前のバージョンの配達確認に対して E メールでレビュー担当者に通知しない場合（標準 E メールやカスタム E メールがない場合など）、新しいバージョンページにはデフォルトでメッセージが含まれません。 新しいバージョンをレビュー担当者に通知するには、「メッセージを送信」リンクをクリックします。 その後、「カスタムメッセージを追加」リンクをクリックして、カスタム件名とメッセージを追加できます。
