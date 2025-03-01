---
title: ユーザーに完全な管理アクセスを付与する
description: ユーザーに Workfront への完全な管理アクセス権を付与できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 92%

---

# ユーザーへの完全な管理アクセス権の付与

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>このページで説明する手順は、Admin Console にまだ登録されていない組織にのみ適用されます。組織が Adobe Admin Console に登録されている場合は、Adobe Admin Console でこのアクションを実行してください。
>
>Adobe Admin Consoleで完全な管理者アクセス権を付与する手順については、[Adobe Admin Consoleでのユーザーの管理 ](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについては、[プラットフォームベースの管理上の違い（Adobe Workfront／Adobe ビジネスプラットフォーム）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

Adobe Workfront 管理者は、システム管理者のアクセスレベルを割り当てることによって別の Workfront 管理者を作成できます。このアクセスレベルのユーザーは、自分で作成しなかった項目を含め、Workfront 内のすべての項目に対する完全な管理者アクセス権を持ちます。

>[!NOTE]
>
>これは、システムの特定のエリアに管理者アクセス権をユーザーに付与するアクセスレベルを使用する場合とは異なります。詳しくは、以下を参照してください。
>
>* [特定のエリアに対する管理者アクセス権のユーザーへの付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* この記事の [Workfront 管理者のアクセスと管理権限を持つプランユーザーのアクセス](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights)
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。
+++

## 1 人のユーザーにシステム管理者の完全アクセス権を付与

{{step-1-to-users}}

1. 管理者権限を付与するユーザーの名前をクリックします。
1. ユーザー名の右 ![](assets/more-icon.png) にある **その他** メニューをクリックしてから、**編集** をクリックします。

   **担当者を編集** ボックスが表示されます。
1. 左側のパネルで「**アクセス**」をクリックします。
1. **アクセスレベル** ドロップダウンリストから、**システム管理者** アクセスレベルを選択します。

   システムで行われている変更によっては、このアクセスレベルの名前が変わる場合があります。

1. 「**変更を保存**」をクリックします。

   これで、ユーザーはシステムの完全なシステム管理者権限を持ちます。

## Workfront 管理者のアクセスと管理権限を持つプランユーザーのアクセス  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

次の 2 つの表に、Workfront System Administrator のアクセスレベルを持つユーザーのアクセス権と、一部の管理者権限を持つプランライセンスを持つユーザーのアクセス権の違いを示します。

Workfront の管理者は、誰が作成したかに関係なく、システム内のすべてのオブジェクトの表示、新しいオブジェクトの作成、既存のオブジェクトの変更または削除が可能です。システム内のすべてのオブジェクトに対する完全なアクセス権を持ちます。

1 つのエリアで機能を編集できるプランライセンスを持つユーザーは、そのエリアで機能に対する完全なアクセス権を持ちます。

>[!NOTE]
>
>プランライセンスを持つユーザーがグループ管理者として指定されている場合は、Workfront 管理者が実行できるアクションの一部を実行できます。管理グループ、サブグループ、およびそのグループとサブグループ内のユーザーに対してのみ、これらのアクションを実行できます。詳細情報については、[グループ管理者](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)を参照してください。

* [設定エリアへのアクセス](#access-to-the-setup-area)
* [オブジェクトへのアクセス](#access-to-objects)

### 設定エリアへのアクセス {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>エリア／オブジェクト</th> 
   <th>Workfront 管理者 </th> 
   <th>プランライセンスと一部の管理権限を持つユーザー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>プロジェクト環境設定：プロジェクト</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>プロジェクト環境設定：タスクとイシュー</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>プロジェクト環境設定：ステータス</td> 
   <td>フルアクセス</td> 
   <td> <p>アクセスなし</p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト環境設定：優先度</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>プロジェクト環境設定：重大度</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>プロジェクト環境設定：為替レート</td> 
   <td>フルアクセス</td> 
   <td>フルアクセス</td> 
  </tr> 
  <tr> 
   <td>プロセス：承認</td> 
   <td> <p>フルアクセス</p> </td> 
   <td>フルアクセス</td> 
  </tr> 
  <tr> 
   <td>プロセス：マイルストーンパス</td> 
   <td>フルアクセス</td> 
   <td>フルアクセス</td> 
  </tr> 
  <tr> 
   <td>カスタムフォーム</td> 
   <td>フルアクセス</td> 
   <td> <p>自分が作成したカスタムフォームや自分と共有されたカスタムフォームを管理できます。</p> <p>自分が作成したカスタムフォームや自分と共有されたカスタムフォームを、自分が管理または参加する権限を持つオブジェクトに添付できます。</p> </td> 
  </tr> 
  <tr> 
   <td>ごみ箱：最近削除された項目</td> 
   <td>フルアクセス</td> 
   <td> <p>グループ管理者であるユーザーは、自分が管理するグループに割り当てられたプロジェクトのほか、それらのプロジェクトに関連付けられたタスク、イシューまたはドキュメントを復元できます。</p> </td> 
  </tr> 
  <tr> 
   <td>ごみ箱：最近復元された項目</td> 
   <td>フルアクセス</td> 
   <td>グループ管理者であるユーザーは、最近復元した項目を表示できます。</td> 
  </tr> 
  <tr> 
   <td>担当業務</td> 
   <td>フルアクセス</td> 
   <td> <p>既存の担当業務を変更できますが、削除はできません。</p> <p>新しい担当業務を追加できます。</p> </td> 
  </tr> 
  <tr> 
   <td>チーム</td> 
   <td>フルアクセス</td> 
   <td> <p>チームを作成するアクセス権はありません。</p> <p>ユーザーの作成または編集時に、ユーザーに既存のチームを追加できます。</p> </td> 
  </tr> 
  <tr> 
   <td>グループ</td> 
   <td>フルアクセス</td> 
   <td> <p>グループを作成するアクセス権はありません。</p> <p>グループ管理者のみが、自分が管理するグループのグループメンバーシップ、サブグループおよびグループレベルのステータスを管理できます。 </p> </td> 
  </tr> 
  <tr> 
   <td>会社</td> 
   <td>フルアクセス</td> 
   <td>フルアクセス</td> 
  </tr> 
  <tr> 
   <td>別のユーザーとしてログイン</td> 
   <td>フルアクセス </td> 
   <td> <p>グループ管理アクセスがアクセスレベルで有効になっていて、グループ管理者として指定されている場合は、管理グループとサブグループのユーザーとしてログインできます。システム管理者としてログインすることはできません。<br>ユーザーのグループ管理アクセスを有効にする方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>スケジュール</td> 
   <td>フルアクセス</td> 
   <td> <p>スケジュール編集権限なし。</p> <p>ユーザーレベルで、既存のスケジュールを他のユーザーに追加する権限。 </p> </td> 
  </tr> 
  <tr> 
   <td>タイムシートと時間：タイムシートプロファイル</td> 
   <td>フルアクセス</td> 
   <td> <p>既存のタイムシートプロファイルをユーザーレベルでユーザーに割り当てる権限。</p> <p>グループ管理者であるユーザーは、管理するグループとそのサブグループのタイムシートプロファイルを作成できます。 </p> </td> 
  </tr> 
  <tr> 
   <td>タイムシートと時間：時間タイプ</td> 
   <td>フルアクセス</td> 
   <td> <p>ユーザーレベルで、ユーザーに時間タイプを割り当てる権限。</p> </td> 
  </tr> 
  <tr> 
   <td>タイムシートと時間：環境設定</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>メール：通知：イベント通知</td> 
   <td>すべてをアクティブ化／非アクティブ化</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>メール：通知：リマインダー通知</td> 
   <td>フルアクセス</td> 
   <td>フルアクセス</td> 
  </tr> 
  <tr> 
   <td>メール：通知：メールテンプレート</td> 
   <td>フルアクセス</td> 
   <td> <p>メールテンプレート編集権限なし。</p> <p>既存のメールテンプレートをリマインダー通知に追加する権限。</p> </td> 
  </tr> 
  <tr> 
   <td>メール：自動リマインダー</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>メール：招待状</td> 
   <td>フルアクセス</td> 
   <td> <p>メール招待状の編集権限なし。</p> <p>「ユーザー」タブからのみ未登録ユーザーに招待メールを再送信する権限。</p> </td> 
  </tr> 
  <tr> 
   <td>メール：設定</td> 
   <td>フルアクセス</td> 
   <td> <p>アクセスなし</p> </td> 
  </tr> 
  <tr> 
   <td>スコアカード</td> 
   <td>フルアクセス</td> 
   <td> <p>フルアクセス</p> </td> 
  </tr> 
  <tr> 
   <td>費用タイプ</td> 
   <td>フルアクセス</td> 
   <td> <p>アクセスなし</p> </td> 
  </tr> 
  <tr> 
   <td>リスクタイプ</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>アクセスレベル</td> 
   <td> <p>すべてのアクセスレベルを変更するフルアクセス。</p> <p>システム管理者と外部ユーザーのアクセスレベルは、デフォルトでは変更できません。</p> </td> 
   <td> <p>アクセスレベル編集権限なし。</p> <p>ユーザーレベルで、自分と同じかそれ以下の他のユーザーへのアクセスレベルを割り当てる権限。</p> </td> 
  </tr> 
  <tr> 
   <td>インターフェイス：レイアウトテンプレート</td> 
   <td>フルアクセス</td> 
   <td> <p>ユーザーレベルで、既存のレイアウトテンプレートを他のユーザーに割り当てる権限。 </p> <p>グループ管理者として指定されたユーザーは、管理するグループとサブグループのレイアウトテンプレートを作成できます。</p> </td> 
  </tr> 
  <tr> 
   <td>インターフェイス：フィードを更新</td> 
   <td>フルアクセス</td> 
   <td> <p>フィードを更新の変更権限無し。</p> <p>カスタムフォームの編集時に、フィードを更新でトラックするフィールドを追加する権限。</p> </td> 
  </tr> 
  <tr> 
   <td>インターフェイス：フィルター</td> 
   <td>フルアクセス</td> 
   <td> <p>設定エリアでフィルターを作成する権限なし。</p> <p>オブジェクトのリストで新しいフィルターを作成する権限。</p> </td> 
  </tr> 
  <tr> 
   <td>インターフェイス：ビュー</td> 
   <td>フルアクセス</td> 
   <td> <p>設定エリアでビューを作成する権限なし。</p> <p>オブジェクトのリストで新しいビューを作成する権限。</p> </td> 
  </tr> 
  <tr> 
   <td>インターフェイス：グループ化</td> 
   <td>フルアクセス</td> 
   <td> <p>設定エリアでグループ化を作成する権限なし。</p> <p>オブジェクトのリストでグループを新規作成する権限。</p> </td> 
  </tr> 
  <tr> 
   <td>インターフェイス：リストコントロール</td> 
   <td>フルアクセス</td> 
   <td> <p>アクセスなし</p> </td> 
  </tr> 
  <tr> 
   <td>ドキュメント：クラウドプロバイダー</td> 
   <td>フルアクセス</td> 
   <td> <p>クラウドプロバイダー設定権限なし。</p> <p>クラウドプロバイダーが Workfront と統合された後、「ドキュメント」タブからクラウドプロバイダーとの間でドキュメントをリンクする権限。</p> </td> 
  </tr> 
  <tr> 
   <td>ドキュメント：メタデータマッピング</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>ドキュメント：SharePoint 統合</td> 
   <td>フルアクセス</td> 
   <td> <p>SharePoint 統合の設定権限なし。</p> <p>SharePoint と Workfront の統合が設定された後、「ドキュメント」タブから SharePoint との間でドキュメントをリンクする権限。</p> </td> 
  </tr> 
  <tr> 
   <td>ドキュメント：カスタム統合</td> 
   <td>フルアクセス</td> 
   <td> <p>カスタム統合の設定権限なし。</p> <p>サードパーティプロバイダーが Workfront と統合された後、「ドキュメント」タブからサードパーティプロバイダーとの間でドキュメントをリンクする権限。</p> </td> 
  </tr> 
  <tr> 
   <td>システム：ブランディング</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>システム：顧客情報</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>システム：シングルサインオン（SSO）</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>システム：SSO ユーザーの更新</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>システム：キックスタート</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>システム：診断</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
  <tr> 
   <td>システム：環境設定</td> 
   <td>フルアクセス</td> 
   <td>アクセスなし</td> 
  </tr> 
 </tbody> 
</table>

### オブジェクトへのアクセス {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>エリア／オブジェクト</th> 
   <th>Workfront 管理者 </th> 
   <th>プランライセンスと一部の管理権限を持つユーザー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>カレンダー</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したカレンダーおよび自分と共有されているカレンダーの管理。</td> 
  </tr> 
  <tr> 
   <td>ダッシュボード</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したダッシュボードおよび自分と共有されているダッシュボードの管理。</td> 
  </tr> 
  <tr> 
   <td>ドキュメント</td> 
   <td>フルアクセス</td> 
   <td>自分がアップロードしたドキュメントおよび自分と共有されているドキュメントの管理。</td> 
  </tr> 
  <tr> 
   <td>イシュー</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したイシューおよび自分と共有されているイシューの管理。</td> 
  </tr> 
  <tr> 
   <td>ポートフォリオ</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したポートフォリオおよび自分と共有されているポートフォリオの管理。 </td> 
  </tr> 
  <tr> 
   <td>プログラム</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したプログラムおよび自分と共有されているプログラムの管理。</td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したプロジェクトおよび自分と共有されているプロジェクトの管理。</td> 
  </tr> 
  <tr> 
   <td>レポート</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したレポートおよび自分と共有されているレポートの管理。システムレポートの表示、コピー、編集。</td> 
  </tr> 
  <tr> 
   <td>タスク</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したタスクおよび自分と共有されているタスクの管理。</td> 
  </tr> 
  <tr> 
   <td>テンプレート</td> 
   <td>フルアクセス</td> 
   <td>自分が作成したテンプレートおよび自分と共有されているテンプレートの管理。</td> 
  </tr> 
  <tr> 
   <td>タイムシート</td> 
   <td>フルアクセス</td> 
   <td>フルアクセス</td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>フルアクセス</td> 
   <td> <p>制限付きアクセス</p> <p>自分がグループ管理者になっていないグループのユーザーや、公開されていないグループには、グループを割り当てることはできません。</p> <p>自分のアクセスレベルよりも高いアクセスレベルをユーザーに割り当てることはできません。</p> <p>グループ管理アクセス権がアクセスレベルで有効になっており、グループのグループ管理者として指定されている場合は、管理しているグループおよびそのサブグループのユーザーのパスワードをリセットしたり、それらのユーザーとしてログインしたりできます。システム管理者のパスワードをリセットしたり、システム管理者としてログインしたりすることはできません。<br>ユーザーへのグループ管理アクセス権の有効化について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>
