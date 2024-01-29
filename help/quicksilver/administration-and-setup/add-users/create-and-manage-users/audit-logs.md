---
title: 監査ログ
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront管理者は、監査ログを使用して、過去 90 日間にシステムでトリガーされたユーザーの変更を追跡できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '1464'
ht-degree: 3%

---

# 監査ログ

<!--Audited: 01/2024-->

Adobe Workfront管理者は、以下に説明する監査ログを使用して、過去 90 日間にシステムでトリガーされたユーザーの変更を追跡できます。

これらの監査ログに表示する内容を表示およびフィルタリングする手順については、 [監査ログの表示と書き出し](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## 監査ログに記載されている情報

次のフィールドは、すべての監査ログエントリに記録されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">日付および時刻</td> 
   <td>アクションが発生した日時。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ログタイプ</td> 
   <td>監査ログのタイプ（アクセスレベル、カスタムフォームなど）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザー名</td> 
   <td> <p>アクションを実行したユーザーの名前。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクション</td> 
   <td> ユーザーが実行するアクション（変更、作成、削除など）。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト</td> 
   <td> アクションの結果として影響を受けるオブジェクトの名前。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">詳細</td> 
   <td>アクションに関する追加の詳細。 テキストの上にマウスを置くと、すべてのメッセージが表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP アドレス</td> 
   <td> <p>アクションの実行時にアクションを実行したユーザーの IP アドレス。</p> <p>一部のシステム操作では、IP アドレスを使用できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 監査ログのタイプと、それらをトリガーするアクション

* [アクセスレベル](#access-level)
* [会社情報](#company)
* [条件](#condition)
* [カスタムフィールド](#custom-field)
* [カスタムフォーム](#custom-forms)
* [カスタムセクション](#custom-section)
* [為替レート](#exchange-rate)
* [グループ](#group)
* [ジョブの役割](#job-roles)
* [ログイン試行](#login-attempt)
* [優先度](#priority)
* [プロジェクトの環境設定](#project-preference)
* [重大度](#severity)
* [ステータス](#status)
* [タスクと問題の環境設定](#tasks-issues-preferences)
* [ユーザー](#user)

### アクセスレベル {#access-level}

ユーザーが次のいずれかの操作を行うと、アクセスレベルログエントリが生成されます。

* アクセスレベルを作成します
* アクセスレベルを削除します
* アクセスレベルを変更します。

   * ライセンスの種類を変更します
   * プロジェクト、タスク、タスク、タスク、Portfolio、プログラム、レポート、ドキュメント、ユーザー、またはテンプレートに対する権限を変更します

     >[!NOTE]
     >
     >財務データに対する権限の変更、または表示と編集のアクセス・タイプ内には、何も記録されません。
     >
     >例えば、ユーザーがプランナーのアクセス・タイプを「表示」から「編集」に変更した場合、「設定の微調整」ドロップダウン・メニューに含まれる情報は表示されません。

### 会社 {#company}

ユーザーが次のいずれかの操作を行うと、会社の監査ログエントリが生成されます。

* 会社を作成
* 会社の変更：

   * 名前を変更
   * メンバーを追加または削除します
   * [ グループ ] フィールドの値を追加、編集、または削除します
   * ジョブロールの会社の請求率を追加または編集します
   * ジョブロールの会社請求率を削除します
   * 組織の主な会社として設定します
   * カスタムフォームを添付または削除します

* 会社を削除します

ステータスについて詳しくは、 [ステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 状況 {#condition}

ユーザーが次のいずれかの操作を実行すると、条件監査ログエントリが生成されます。

* 条件を作成します
* 条件を変更します。

   * 名前を変更
   * 色を変更します
   * デフォルトとして設定します
   * 条件の説明を変更または削除します
   * 条件の表示/非表示を切り替えます

* 条件を削除します

ジョブの役割の設定について詳しくは、 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### カスタムフィールド {#custom-field}

ユーザーが次のいずれかの操作を行うと、カスタムフィールド監査ログエントリが生成されます。

* カスタムフィールドを作成します
* カスタムフィールドを変更します。

   * 名前、ラベル、手順、または形式を変更します
   * 表示タイプを変更します

     これは、1 行、段落、ドロップダウン、チェックボックス、ラジオボタンのいずれかのタイプのフィールドの場合にのみ使用できます。

   * フィールドサイズを変更します

     これは、1 行、段落、書式設定されたテキストのいずれかのタイプのフィールドである場合にのみ使用できます

   * フィールド選択の追加、削除、非表示を切り替えます。
   * フィールド選択のラベルまたは値を編集します
   * フィールドの選択を選択するか、既定で選択しないかを設定します
   * 複数選択または 1 つの選択を許可するドロップダウンフィールドを設定します
   * 時刻を表示する、または表示しない日付フィールドを設定します
   * ハイパーリンクを編集したり、説明テキストフィールドの値を変更したりします

* カスタムフィールドを削除します
* カスタムフィールドを共有

### カスタムフォーム {#custom-forms}

ユーザーが次のいずれかの操作を実行すると、カスタムForms監査ログエントリが生成されます。

* カスタムフォームを作成します
* カスタムフォームを変更します。

   * 名前または説明を変更します
   * 「アクティブ」を有効または無効にします
   * フィールドまたはセクションを追加または削除します
   * カスタムセクションの場合、[ 追加設定 ] の設定を変更します。
   * フィールドを必須または不要に変更
   * カスタムフィールドの計算を変更します
   * 「説明のカーソルを合わせたテキスト」の計算フィールドに関連付けられた数式を表示または非表示にします
   * 以前の計算の更新を有効または無効にします
   * スキップロジックまたは表示ロジックを追加または変更します

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* カスタムフォームを削除します
* カスタムフォームを共有

### カスタムセクション {#custom-section}

ユーザーがカスタムフォームで次のいずれかの操作を実行すると、カスタムセクション監査ログエントリが生成されます。

* カスタムセクションを作成します
* カスタムセクションの名前または説明を変更します
* カスタムセクションを削除します

カスタムフォームのカスタムセクションについて詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### 為替レート {#exchange-rate}

ユーザーが次のいずれかの操作を行うと、システムは為替レート監査ログエントリを生成します。

* 為替レートを作成します
* 為替レートを変更します。

   * 通貨を追加します
   * 通貨のレートを変更します
   * システム全体のすべてのプロジェクトとレポートで、通貨をベース（デフォルト）通貨として設定します

* 為替レートを削除します

為替レートの設定の詳細は、 [為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### グループ {#group}

ユーザーが次のいずれかの操作を実行すると、システムはグループ監査ログエントリを生成します。

* グループを作成します
* グループを削除します
* グループの変更：

   * ユーザーを追加または削除します
   * サブグループを追加または削除

### 担当業務 {#job-roles}

ユーザーが次のいずれかの操作を行うと、ジョブの役割監査ログエントリが生成されます。

* ジョブロールを作成します
* ジョブの役割を変更します。

   * 名前を変更
   * 説明を追加、変更、または削除します
   * 時間あたりのコスト（コスト/時間）を追加、変更、または削除します。
   * 請求率（請求/人）を追加、変更、または削除します。

* ジョブの役割を削除します

ジョブの役割の設定について詳しくは、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### ログイン試行 {#login-attempt}

ユーザーが次のいずれかの操作を行うと、システムは Login Attempt 監査ログエントリを生成します。

* （ブラウザーおよびモバイルアプリで）Workfrontでのログイン、ログアウト、またはログインの試行に失敗する
* 任意のWorkfront統合 (Slack用のWorkfront、Salesforce 用のWorkfrontなど ) でのログイン、ログアウト、またはログインの試行に失敗します。
* Workfront API へのログインとログアウト

Workfront管理者が「Log In As」機能を使用した場合、ログイン試行ログに記録されません。

>[!NOTE]
>
>組織がAdobe Admin Consoleにオンボーディングされている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

### 優先度 {#priority}

ユーザーが次のいずれかの操作を行うと、優先順位監査ログエントリが生成されます。

* 優先度を作成
* 優先度を変更します。

   * 名前を変更
   * 色を変更します
   * デフォルトとして設定します
   * 優先度の説明を追加、変更、または削除します
   * 優先度を表示または非表示にします

* 優先度を削除します

優先度の設定について詳しくは、 [優先度の作成とカスタマイズ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### プロジェクト環境設定 {#project-preference}

ユーザーが次のいずれかの操作を行うと、プロジェクト環境設定監査ログエントリが生成されます。

* カスタム四半期を作成します
* プロジェクト環境設定を変更します。

   * ロックまたはロック解除
   * 設定の 1 つを変更
   * 有効、無効、または編集
   * タイムラインの計算を編集します

* カスタム四半期を削除します

プロジェクトの環境設定の詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### 重大度 {#severity}

ユーザーが次のいずれかの操作を行うと、重大度監査ログエントリが生成されます。

* 問題の重大度を作成します
* 問題の重大度を変更しました。

   * 名前を変更
   * 色を変更します
   * デフォルトとして設定します
   * 重大度の説明を変更または削除します
   * 重大度を表示または非表示にします

* 問題の重大度を削除します

ジョブの役割の設定について詳しくは、 [問題の重要度を作成またはカスタマイズ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### ステータス {#status}

ユーザーが次のいずれかの操作を行うと、ステータス監査ログエントリが生成されます。

* システムレベルまたはグループレベルでステータスを作成します
* システムレベルまたはグループレベルのステータスを変更します。

   * 名前を変更
   * デフォルトのステータスにします
   * ロックまたはロック解除
   * 非表示/非表示を切り替えます
   * 色または説明を変更します

* システムレベルまたはグループレベルのステータスを削除します

ステータスについて詳しくは、 [ステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### タスクと問題の設定 {#tasks-issues-preferences}

ユーザーが次のいずれかの方法で Tasks &amp; Issues 環境設定を変更すると、Tasks &amp; Issues Preferences 監査ログエントリが生成されます。

* プリファレンスをロックまたはロック解除する
* 環境設定の設定を変更します。
* タスク、問題、または要求のアクセス設定を変更します

タスクと問題の環境設定について詳しくは、 [システム全体のタスクと問題の環境設定を構成する](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### ユーザー {#user}

ユーザーが次のいずれかの操作を行うと、システムはユーザー監査ログエントリを生成します。

* ユーザーを作成

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >組織がAdobe Admin Consoleにオンボーディングされている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

* ユーザーを削除します
* ユーザーのアクセスレベル、会社、チーム、またはグループを変更します
* ユーザーをアクティベート
* ユーザーを非アクティブ化します
