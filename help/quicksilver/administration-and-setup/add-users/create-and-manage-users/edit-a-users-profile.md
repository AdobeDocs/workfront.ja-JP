---
title: ユーザーのプロファイルの編集
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 管理者は、新規ユーザーを作成し、既存ユーザーのプロファイルを管理できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '3381'
ht-degree: 75%

---

# ユーザーのプロファイルの編集

{{highlighted-preview}}

>[!IMPORTANT]
>
>このページで説明する手順は、Admin Console にまだ登録されていない組織にのみ適用されます。組織が Adobe Admin Console に登録されている場合は、Adobe Admin Console でこのアクションを実行してください。
>
>Adobe Admin Console でユーザーのプロファイルを編集する手順については、[ユーザーの個別管理](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html)の記事の「ユーザーの詳細を編集」の節を参照するか、Adobe Admin Console 管理者にお問い合わせください。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront／Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

Adobe Workfront管理者は、ユーザーを作成し、既存のユーザーのプロファイルを管理できます。 ユーザーの作成については、[ユーザーの追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>新規：標準</p>
   または
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。 </p> </li> 
     <li> <p>The <b>ユーザー</b> に設定されたアクセスレベルの <b>編集</b> アクセス、 <b>作成</b> そして次の 2 つのうち少なくとも 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> ユーザー管理者（すべてのユーザー）</li>
     <li>ユーザー管理者（グループユーザー）</li></ul>
     <p>次の場合  <b>ユーザー管理者（グループユーザー）</b> が有効になっている場合、ユーザーを編集するには、そのユーザーがメンバーであるグループのグループ管理者である必要があります。</p> 
     <p>アクセスレベルでの<b>ユーザー</b>設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセスを許可</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## ユーザープロファイルを編集

{{step-1-to-users}}

1. ユーザーを選択し、 **編集** アイコン ![](assets/edit-icon.png).

   「ユーザーを編集」ボックスが表示されます。

1. Adobe Analytics の **ユーザーを編集** ボックスで、次の情報を変更し、 **変更を保存** いつでも

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">個人情報 </td> 
      <td> 
       <ul> 
        <li><p><b>名</b></p></li>
        <li><p><b>姓</b></p></li> 
        <li> <p><b>メールアドレス：</b>ユーザーのメールアドレスは、Workfront でのユーザー名でもあります。このフィールドでは大文字と小文字が区別され、一意である必要があります。ユーザーが、一意でないメールアドレスを 10 分以内に 3 回追加しようとすると、reCAPTCHA 応答が表示されます。</p> <p> を選択します。 <b>私はロボットではありません</b> を設定してから続行します。</p><p>メール許可リストを使用していて、リストにないメールドメインを入力した場合、ユーザーにはメール通知が届きません。許可リストに関して詳しくは、<a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">メール許可リストの設定</a>を参照してください。</p> </li> 
        <li> <p><b>パスワードのリセット</b>：このリンクをクリックすると、ユーザーのパスワードをリセットできます。別のユーザーのパスワードをリセットする前に、自分のパスワードを入力する必要があります。</p> <p>別のユーザーのパスワードをリセットするには、Workfront 管理者またはグループ管理者である必要があります。</p> <p><b>メモ</b>:  
          <ul> 
           <li> <p>グループ管理者の場合は、管理者として指定されたグループ内のユーザーに対してのみ、パスワードをリセットできます。 また、ユーザー管理（グループユーザー）権限をアクセスレベルで有効にする必要があります。</p> <p> <img src="assets/group-admin-user.png" > </p> <p>この設定は、デフォルトで無効になっています。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </li> 
           <li> <p>Workfront 管理者のパスワードはリセットできません。</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; ユーザー名</b>：Workfront 管理者が Workfrontとの SSO 統合を有効にしてある場合は、このフィールドに SSO ユーザー名が表示されます。Workfront インスタンスに対して有効になっている SSO 設定のタイプが、このフィールドに表示されます。 </li> 
        <li> <p><b>&lt;SSO Configuration&gt; 認証のみを許可</b>：Workfront 管理者が Workfront との SSO 統合を有効にし、SSO に対応するようにすべてのユーザーを更新してある場合、このフィールドはデフォルトで選択されています。Workfront インスタンスに対して有効になっている SSO 設定のタイプが、このフィールドに表示されます。</p> <p>このフィールドを選択した場合、ユーザーは SSO 資格情報を使用して Workfront にログインする必要があります。これをオフにすると、ユーザーは Workfront の資格情報で Workfront にログインできます。</p> <p>SSO ソリューションでの Workfront の設定について詳しくは、<a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront でのシングルサインオンの概要</a>を参照してください。</p> <p>SSO のユーザーのアップデートについて詳しくは、<a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">シングルサインオンのユーザーをアップデート</a>を参照してください。</p> 
        <p><b>メモ</b>：</p> 
        <p> グループ管理者は、 &lt;sso configuration=""&gt; フィールドは、自分が指定されたグループ内のユーザーに対してのみ使用できます。 また、ユーザー管理（グループユーザー）権限をアクセスレベルで有効にする必要があります。
        <p>グループ管理者で、ユーザー管理者（すべてのユーザー）権限をアクセスレベルで有効にしている場合は、すべてのユーザーの &lt;SSO Configuration&gt; フィールドを編集できます。</p> </li> 
        <li><b>ジョブ情報：</b> 役職 ( <b>タイトル</b> フィールド ) と、ユーザーが担当する ( <b>次について私にお問い合わせください：</b> フィールド ) に書き込まれます。</li> 
        <li><p><b>連絡先情報</b>：ユーザーの電話番号 ( <b>電話番号、内線</b>、および <b>モバイル番号</b> フィールド ) と住所 ( <b>住所、市区町村、都道府県、郵便番号、国</b> フィールド ) を参照してください。</p>
        <p>ユーザーが統合ユーザー管理（UUM）またはAdobe Identity Management システム（IMS）に対して有効になっている場合、「連絡先情報」セクションの「<b>国</b>」フィールドでは、国コードの値（US、GB、IN など）のみを使用できます。</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">環境設定 </td> 
      <td> 
       <ul> 
      <li> <p><b>タイムゾーン：</b>ユーザーのタイムゾーン。</p> <p>ユーザーが Workfront でタイムゾーンをまたいで共同作業できるようにスケジュールを使用する方法について詳しくは、<a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">タイムゾーンをまたいだ作業</a>を参照してください。</p> </li> 
       <li><b>メールのロケール</b>：ユーザーが希望するメールのロケール。これは、Workfrontからこのユーザーに送信される E メールの数値や日付の形式に影響します。</li>

   <li><b>このテスト環境からメールを受信</b>：現在ログインしている環境からメール通知を受け取る場合は、このオプションを選択します。
      <p><b>メモ</b></p>
      <p>このオプションは、プレビューおよびサンドボックス環境でのみ使用できます。メール通知は、実稼動環境でデフォルトで有効になっています。 </p>
      </li>

   <li><b>更新ステータスの完了率を表示</b>：従来のコメントエクスペリエンスを使用する場合に、このユーザーのタスクの更新領域内に完了率のバーを表示するには、このオプションを選択します。 詳しくは、 <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">新しいコメントエクスペリエンス</a>.</li> 
       <li><b>自分に割り当てた作業を [ 作業 ] タブに送信する</b>：ユーザーが割り当てたすべてのものをホーム領域の作業中リストに直接表示する場合は、このオプションを選択します。 デフォルトでは、ユーザーに割り当てられたすべての項目が、[ ホーム ] 領域の [ 開始準備完了 ] または [ 準備不可 ] リストに表示されます。</li> 
       <li><b>ドキュメントのアップロード時に配達確認を自動生成</b>：ユーザーがアップロードしたドキュメントで配達確認をすぐに生成する場合は、このオプションを選択します。 </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td> <p>新しいユーザーに対して有効にするメール通知を選択します。</p> <p>Workfront 管理者は、システムレベルおよびグループレベルのすべてのレイアウトテンプレートを表示できます。</p> <p>詳しくは、<a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">システムの全員に対するイベント通知の設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクセス</td> 
      <td> 
       <ul> 
      <li><b>アクティブ：</b>このボックスを選択して、ユーザーがアクティブであることを示します。アクティブなユーザーは Workfront のライセンスを使用しています。このボックスをクリアすると、ユーザーが非アクティブ化され、Workfrontにログインできなくなります。</li> 
       <li> <p><b>アクセスレベル：</b>これらのユーザーに割り当てるアクセスレベルを選択します。</p> 
       <p>ユーザーにアクセスレベルを割り当てる際に、自分のアクセスレベルと等しいかそれ以下のレベルを割り当てることができます。</p>
       <p>たとえば、アクセス・レベルが「計画」の場合は、管理者アクセス・レベルを割り当てることはできません。 ただし、Workfront管理者がアクセスレベルでデフォルト以外の権限を有効にしていて、独自のアクセスレベルでも無効になっている場合は、デフォルトで自分のアクセスレベルより低いアクセスレベルを割り当てることはできません。 </p>
       <p>たとえば、タスクを削除するアクセス権を持たない Plan ライセンスを持っている場合、Work ライセンスは Plan ライセンスよりも低いのに、削除タスクへのアクセス権を持つ Work ライセンスを割り当てることはできません。 詳しくは、  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>. </p> 
       <p>アクセスレベルについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Adobe Workfront へのアクセスの設定</a>を参照してください。</p>
       <p> <b>注意：</b></p> 
       <p> 組織で新しいアクセスモデル（標準/ライト/コントリビューター）を使用している場合、そのユーザーが月の決定制限に達している場合、標準またはライトユーザーをコントリビューターアクセスレベルに再割り当てすることはできません。 </p><p>新しいアクセスモデルについて詳しくは、<a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">新しいアクセスレベルの概要</a>を参照してください。 </p><p>決定制限について詳しくは、<a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">無償ユーザーに対する限定的なドキュメントおよびプルーフの決定の概要</a>を参照してください。</p></li> 
       <li> <p><b>レイアウトテンプレート</b>：ユーザー用のレイアウトテンプレートを選択します。このレイアウトテンプレートは、ユーザのホームグループ、ホームチーム、またはプライマリロールに割り当てられたレイアウトテンプレートよりも優先されます。 レイアウトテンプレートの割り当て優先度について詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>を参照してください。</p> <p><b>メモ</b>：  <p>次のリストでは、このフィールドで使用できるテンプレートのリストが、アクセス権に応じてどのように異なるかを説明します。</p> 
       <ul> 
       <li>Workfront 管理者は、システムレベルおよびグループレベルのすべてのレイアウトテンプレートを表示できます。</li> 
       <li>グループ管理者は、システムレベルのレイアウトテンプレートと、管理するグループに関連付けられているレイアウトテンプレートを表示できます。</li> 
       <li>プランライセンスとユーザー編集のアクセス権があるユーザーには、システムレベルのレイアウトテンプレートのみが表示されます。</li> 
       </ul> <p>グループレベルのレイアウトテンプレートについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>を参照してください。</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織 </td> 
      <td> 
       <ul> 
      <li><b>会社</b>：ユーザーの会社。ユーザーは、1 つの会社にのみ関連付けることができます。会社をユーザーに関連付ける前に、会社を作成する必要があります。アクティブな会社のみがリストに表示されます。会社の作成について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">会社の作成と編集</a>を参照してください。</li> 
      <li><b>レポート先：</b>ユーザーの会社を指定した場合は、このフィールドでユーザーの直属のマネージャーも指定できます。1 人のユーザーが管理者を 1 つだけ持つことができます。 ユーザーが最初に会社に関連付けられていない場合、このフィールドは表示されません。 </li> 
      <li><b>直属の部下：</b>ユーザーに会社を指定した場合は、そのユーザーの直属の部下も指定できます。1 人のユーザーが複数のダイレクトレポートを持つことができます。 ユーザーが最初に会社に関連付けられていない場合、このフィールドは表示されません。</li> 
      <li><b>ホームチーム</b>：ユーザーのホームチームを指定します。ホームチームは 1 つのみです。 ホームチームは、レイアウトテンプレートを割り当てる場合や、ユーザーに割り当てられたタスクや問題に対して「IT で作業」ボタンを定義する場合に重要です。 </li> 
      <li><b>その他のチーム</b>：ユーザーは複数のチームに属することができます。 ユーザーは、ホーム領域の任意のチームに割り当てられた作業項目を表示できます。 </li> 
      <li> <p><b>ホームグループ：</b>適切なグループを選択してユーザーを割り当てます。これにより、ユーザーはグループと共有されているオブジェクトにアクセスできます。 また、レイアウトテンプレートをユーザーのホームグループと共有することもできます。</p> <p>必須フィールドです。すべてのユーザーは、ホームグループに関連付ける必要があります。選択しない場合、グループは新しいユーザーのホームグループとして割り当てられます。</p> <p><b>メモ</b>：</p> 
      <p> 次のいずれかに該当する場合にのみ、グループをユーザーに割り当てることができます。</p>
      <ul><li>Workfront管理者である</li>
      <li>グループの管理者です</li>
      <li>グループはパブリックです。</li></ul> 
      <li> <p><b>その他のグループ</b>：ユーザーは複数のグループに属することができます。ユーザーにグループを割り当てることができるのは、Workfront管理者、グループの管理者、またはグループが公開されている場合のみです。</p> <p><b>重要</b>：</p> 
      <p>100 を超えるグループにユーザーを追加すると、Workfrontのどの領域でも、グループのリストを読み込む際にパフォーマンスの問題が発生する場合があります。</p> <p>公開グループについて詳しくは、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">グループの作成</a>を参照してください。</p> <p>グループについて詳しくは、<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>を参照してください。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リソース計画 </td> 
      <td> 
       <ul>
       <li>
       <b>作業時間</b>：ユーザーが実際の作業に使用できる（オーバーヘッドを含まない）フルタイム相当の（FTE）時間の割合を表します。「作業時間」は、1 までの小数で指定する必要があります。0 は指定できません。例えば、実際の作業可能時間が 20%の場合は 0.2 になります。

   フィールドのデフォルト値は 1 で、これはユーザーが FTE 時間全体を実際のプロジェクト関連の作業に費やすことを示します。

   この数値を使用して、プロジェクト関連の実際の作業に対するユーザーの作業可能時間が計算されます。

   Workfront でスケジュールを作成する方法について詳しくは、<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>を参照してください。

   スケジュールの例外とタイムオフも、ユーザーの処理能力に影響を与える可能性があります。

   Workfront では、設定エリアのリソース管理環境設定に応じて、ユーザーの空き時間を計算します。詳しくは、<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>を参照してください。

   <b>説明</b>

   [ 作業時間 ] の値を 1 に設定して、プロジェクト関連の作業でユーザーがフルタイムの同等の作業全体で使用できるようにします。
   </li> 
      <li> <b>無効化をスケジュール</b>：このユーザーを特定の日に特定の時間に非アクティブ化するようにスケジュールする場合は、このチェックボックスをオンにします。 </li> 
       <li><b>予定されている非アクティブ化日</b>：ユーザーが非アクティブ化された日時。 アクティブ化を解除するためのユーザーのスケジュール設定について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a>の<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">ユーザーのスケジュールの非アクティブ化</a>を参照してください。</li> 
       <li> <p><b>プライマリの役割</b>：ユーザーが Workfront で果たすことができる主要担当業務です。ユーザーが割り当てられているタスクとイシューも、このジョブの役割に割り当てられます。リソース管理には、担当業務が不可欠です。このフィールドは、管理者ユーザーアクセス権があるプランライセンスのユーザー、または Workfront 管理者のみが更新できます。管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> <p>リストには、アクティブな担当業務のみが表示されます。 </p> </li> 
       <li><b>プライマリの役割</b>を選択した場合、「<b>FTE 空き時間の割合</b>」フィールドが表示されます。この担当業務に割り当てるユーザーのスケジュールの時間の割合を指定します。主要役割における FTEの可用性の割合のデフォルト値は 100%です。 </li> 
       <li> <p><b>その他の役割</b>：ユーザーは Workfront で複数の担当業務を持つことができます。リソース管理には、担当業務が不可欠です。ユーザーが実行できる担当業務の数に制限はありません。ただし、リソース管理が複雑になりすぎる可能性があるため、1 人のユーザーにあまり多くの担当業務を割り当てないことをお勧めします。<p>リストには、アクティブな担当業務のみが表示されます。担当業務について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> <p>このフィールドは、管理者ユーザーアクセス権があるプランライセンスのユーザー、または Workfront 管理者のみが更新できます。<br>管理ユーザーアクセス権を持つユーザーの設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
       <li> <p>（条件付き）1 つまたは複数の<b>その他の役割</b>を選択した場合、それぞれの役割について「<b>FTE の空き時間の割合</b>」フィールドが表示されます。それぞれの担当業務に割り当てるユーザーのスケジュールの時間の割合を指定します。その他の役割における FTE の可用性の割合のデフォルト値は 0%です。</p> <p><b>メモ</b>：その他の役割の FTE の空き時間が 0％の場合、ユーザーがこれらの役割のタスクに割り当てられていない限り、リソースプランナーには表示されません。</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>メモ</b>： <p>すべての役割における <b>FTE の空き時間の割合</b>の合計を 100％にする必要があります。FTE の可用性の各割合では、リソースプランナーの各ユーザーの役割における空き時間が計算されます。ユーザーごとの各役割の空き時間は、それぞれのユーザーの空き時間に左右されます。</p> <p>ユーザーの空き時間は、Workfront 管理者がリソース管理環境設定で FTE を計算する際に選択した方法に応じて、Workfront によって計算されます。</p> <p>ユーザーの空き時間の計算について詳しくは、<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナーのユーザーと役割に対する時間と FTE の計算の概要</a>を参照してください。</p> <p>リソース管理の環境設定の指定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">リソース管理の環境設定の指定</a>を参照してください。</p> </p>
       <span class="preview"><p>（オプション）ユーザーの担当業務がプロジェクト中に変更された場合、有効日の担当業務割り当てが財務計算に使用されます。</p><p>クリック「<b>日付別の役割を定義</b>」をクリックし、<b>主要役割</b>および<b>その他の役割</b>を選択して、それぞれの役割の配分率を入力します。役割は、既存の役割と同じ（割合を変える）にすることも、新しい役割にすることもできます。これらの役割がアクティブになったら、<b>開始日</b>を選択します。未来の日付にすることができます。最新の役割がアクティブになったら、「<b>以前の役割を表示</b>」をクリックして、以前の非アクティブな役割を表示することができます。</p> </li></span>
       <li> <p><b>スケジュール</b>：スケジュールをユーザーに関連付けます。ユーザーのスケジュールは、ユーザーが割り当てられているタスクのタイムラインを計算します。</p> <p>スケジュールをユーザーに関連付ける前に、スケジュールを作成する必要があります。スケジュールの作成について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>を参照してください。</p> <p><b>メモ</b>：ユーザーに関連付けるスケジュールをユーザーのタイムゾーンと一致させることをお勧めします。</p> </li> 
       <li> <p><b>タイムシートプロファイル</b>：タイムシートプロファイルをユーザーに関連付けて、タイムシートプロファイルがユーザーのために自動的に生成されるようにします。</p> <p><b>メモ</b>：このフィールドで使用可能なプロファイルのリストは、アクセス権によって異なります。
       <ul>
       <li>Workfront 管理者は、すべてのシステムレベルおよびすべてのグループレベルのタイムシートプロファイルを表示することができます。</li>
       <li>グループ管理者は、システムレベルのタイムシートプロファイルと、自分が管理するグループに関連付けられたタイムシートプロファイルを確認できます。</li>
       <li>プランライセンスを持ち、ユーザーを編集するアクセス権を持つユーザーは、システムレベルのタイムシートプロファイルのみを表示できます。グループレベルのタイムシートプロファイルについて詳しくは、<a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">タイムシートプロファイルの作成、編集、割り当て</a>を参照してください。</li>
      </ul></p> </li> 
       <li><b>デフォルトの時間タイプ</b>：ユーザーのデフォルトの時間タイプを選択します。これは、ユーザーが時刻をログに記録する際にデフォルトで使用される時間タイプです。</li> 
       <li><b>利用可能な時間タイプ</b>：ユーザーが使用できる時間タイプを選択します。これらの時間タイプは、ユーザーが時間を記録できる Workfront のどこにでも表示されます。ユーザーは、プロジェクトレベルおよびユーザーレベルで有効になっている時間タイプのみを表示できます。ユーザーが使用できる時間タイプについて詳しくは、<a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">タイムシートの時間タイプと空き時間を定義</a>を参照してください。</li> 
       <li><b>時間の記録：</b>ユーザーが作業アイテムの時間を時間単位で記録するか、日単位で記録するかを選択します。詳しくは、<a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">時間を時間単位で記録するか日単位で記録するかを設定</a>を参照してください。</li>

   <li> <b>FTE</b>：これは、ユーザーのフルタイム換算です。Workfront ではこの数値を使用して、システムレベルの「リソース管理環境設定」が「規定のスケジュール」に設定されている場合にのみ、規定のスケジュールに基づいてユーザーの空き時間が計算されます。

   <p>FTE は、ユーザーが作業に費やせる時間を示します。これには、オーバーヘッドや、プロジェクト作業に費やされた時間が含まれます。例えば、ミーティングやトレーニングに費やした時間も FTE に含まれます。</p>

   FTE は 1 以下の小数にする必要があり、0 にはできません。例えば、FTE 値が 0.5 で、Workfront のデフォルトのスケジュールが 40 時間の場合、そのユーザーは週に 20 時間空いています。

   このフィールドのデフォルトは 1 です。

   スケジュールの例外、休暇および作業時間の値は、ユーザーの空き時間に影響を与える場合があります。

   Workfront では、設定エリアのリソース管理環境設定に応じて、ユーザーの空き時間を計算します。

   システムレベルのリソース管理環境設定がユーザーのスケジュールに設定されている場合、ここで指定した値は無視され、ユーザーはスケジュールで指定された内容に従って空いていると見なされます。

   詳しくは、<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理の環境設定</a>を参照してください。

   Workfront でスケジュールを作成する方法について詳しくは、<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>を参照してください。
   </li>

   <li><b>リソースプール</b>：ユーザーをリソースプールに関連付けます。詳しくは、<a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">リソースプールとユーザーの関連付け</a>を参照してください。</li>

   <li><b>コスト率</b>：ユーザーの 1 時間あたりのコストの量。
      <p>有効日のコスト率については、「<strong>レートを追加</strong>」をクリックします。期間のコスト率の値を入力し、必要に応じて開始日と終了日を割り当てます。コスト率 1 には開始日が設定されず、最後のコスト率には終了日が設定されません。</p><p>一部の日付は自動的に追加されます。例えば、コスト率 1 に終了日がなく、開始日が2023年5月1日のコスト率 2 を追加した場合、ギャップが生じないように、2023年4月30日の終了日がコスト率 1 に追加されます。</p></li>

   <li><b>請求レート</b>：ユーザーの 1 時間あたりの請求額。
      <p>有効日の請求レートについては、「<strong>レートを追加</strong>」をクリックします。期間の請求レートの値を入力し、必要に応じて開始日と終了日を割り当てます。請求レート 1 には開始日が設定されず、最後の請求レートには終了日が設定されません。</p> <p>一部の日付は自動的に追加されます。例えば、請求レート 1 に終了日がなく、開始日が 2023年5月1日の請求レート 2 を追加すると、ギャップが生じないように、請求レート 1 の終了日に 2023年4月30日が追加されます。</p><p> <img alt="ユーザーコストと請求レート" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td><p>既存のユーザーカスタムフォームをこのユーザーに関連付けます。カスタムフォームをユーザーに関連付けるには、カスタムフォームを作成する必要があります。アクティブなカスタムフォームのみがリストに表示されます。編集するアクセス権がないフィールドは、個々のカスタムフォームには表示されません。</p> <p>カスタムフォームの作成について詳しくは、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">コメント</td> 
      <td>ユーザーに送信するコメントと、ユーザープロファイルの更新エリアに入力します。</td> 
     </tr> 
    </tbody> 
   </table>
