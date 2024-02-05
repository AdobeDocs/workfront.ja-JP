---
title: 監査ログ
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront 管理者は、監査ログを使用して、過去 90 日間にシステムでトリガーされたユーザーの変更を追跡できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '1464'
ht-degree: 95%

---

# 監査ログ

<!--Audited: 01/2024-->

Adobe Workfront 管理者は、以下に説明する監査ログを使用して、過去 90 日間にシステムでトリガーされたユーザーの変更を追跡できます。

これらの監査ログに表示する内容を表示およびフィルタリングする手順については、[監査ログの表示と書き出し](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)を参照してください。

## 監査ログに記録される情報

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
   <td>アクションに関するその他の詳細。テキストの上にマウスを置くと、すべてのメッセージが表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP アドレス</td> 
   <td> <p>アクションを実行したユーザーの IP アドレス。</p> <p>一部のシステム操作では、IP アドレスを使用できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 監査ログのタイプと、それらをトリガーするアクション

* [アクセスレベル](#access-level)
* [会社](#company)
* [状況](#condition)
* [カスタムフィールド](#custom-field)
* [カスタムフォーム](#custom-forms)
* [カスタムセクション](#custom-section)
* [為替レート](#exchange-rate)
* [グループ](#group)
* [担当業務](#job-roles)
* [ログイン試行](#login-attempt)
* [優先度](#priority)
* [プロジェクトの環境設定](#project-preference)
* [重大度](#severity)
* [ステータス](#status)
* [タスクと問題の設定](#tasks-issues-preferences)
* [ユーザー](#user)

### アクセスレベル {#access-level}

ユーザーが次のいずれかのアクションを実行すると、アクセスレベルログエントリが生成されます。

* アクセスレベルの作成
* アクセスレベルの削除
* アクセスレベルの変更

   * ライセンスタイプの変更
   * プロジェクト、タスク、イシュー、ポートフォリオ、プログラム、レポート、ドキュメント、ユーザー、またはテンプレートに対する権限の変更

     >[!NOTE]
     >
     >財務データに対する権限の変更、または表示と編集のアクセスタイプ内での権限の変更は記録されません。
     >
     >例えば、ユーザーがプランナーのアクセス・タイプを「表示」から「編集」に変更した場合、「設定の微調整」ドロップダウン・メニューに含まれる情報は表示されません。

### 会社 {#company}

ユーザーが次のいずれかの操作を行うと、会社の監査ログエントリが生成されます。

* 会社の作成
* 会社の変更

   * 名前の変更
   * メンバーの追加または削除
   * [グループ] フィールドの値の追加、編集、または削除
   * 担当業務に対する会社請求率の追加または編集
   * 担当業務に対する会社請求率の削除
   * 組織のプライマリ会社として設定
   * カスタムフォームの添付または削除

* 会社の削除

ステータスの詳細については、[ステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)を参照してください。

### 状況 {#condition}

ユーザーが次のいずれかのアクションを実行すると、条件監査ログエントリが生成されます。

* 条件の作成
* 条件の変更

   * 名前の変更
   * カラーの変更
   * デフォルトとして設定
   * 条件の説明の変更または削除
   * 条件の表示または非表示

* 条件の削除

担当業務の設定について詳しくは、[カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)を参照してください。

### カスタムフィールド {#custom-field}

ユーザーが次のいずれかの操作を行うと、カスタムフィールド監査ログエントリが生成されます。

* カスタムフィールドの作成
* カスタムフィールドの変更

   * 名前、ラベル、手順、または形式の変更
   * 表示タイプの変更

     これは、1 つの行、段落、ドロップダウン、チェックボックス、ラジオボタンのいずれかのタイプのフィールドの場合にのみ使用できます

   * フィールドサイズの変更

     これは、1 つの行、段落、書式設定されたテキストのいずれかのタイプのフィールドである場合にのみ使用できます

   * フィールド選択の追加、削除、または非表示
   * フィールド選択のラベルまたは値の編集
   * 選択する、またはデフォルトで選択しないフィールド選択の設定
   * 複数選択または単一の選択を許可するドロップダウンフィールドの設定
   * 時刻を表示する、または表示しない日付フィールドの設定
   * ハイパーリンクの編集、または説明テキストフィールドの値の変更

* カスタムフィールドの削除
* カスタムフィールドの共有

### カスタムフォーム {#custom-forms}

ユーザーが次のいずれかのアクションを実行すると、カスタムフォーム監査ログエントリが生成されます。

* カスタムフォームの作成
* カスタムフォームの変更

   * 名前または説明の変更
   * [アクティブ] の有効化または無効化
   * フィールドまたはセクションの追加または削除
   * カスタムセクションでの [追加設定] の設定の変更
   * フィールドの必須または不要への変更
   * カスタムフィールドの計算の変更
   * 「説明のカーソルを合わせたテキスト」の計算フィールドに関連付けられた数式を表示または非表示にする
   * 以前の計算の更新を有効または無効にする
   * スキップロジックまたは表示ロジックを追加または変更する

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* カスタムフォームの削除
* カスタムフォームの共有

### カスタムセクション {#custom-section}

ユーザーがカスタムフォームで次のいずれかの操作を実行すると、カスタムセクション監査ログエントリが生成されます。

* カスタムセクションの作成
* カスタムセクションの名前または説明を変更
* カスタムセクションの削除

カスタムフォームのカスタムセクションについて詳しくは、[カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

### 為替レート {#exchange-rate}

ユーザーが次のいずれかの操作を行うと、システムは為替レート監査ログエントリを生成します。

* 為替レートの作成
* 為替レートを変更します。

   * 通貨の追加
   * 通貨のレートの変更
   * システム全体のすべてのプロジェクトとレポートで、通貨をベース（デフォルト）通貨として設定

* 為替レートの削除

為替レートの設定について詳しくは、[為替レートの設定](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。

### グループ {#group}

ユーザーが次のいずれかの操作を実行すると、システムはグループ監査ログエントリを生成します。

* グループの作成
* グループの削除
* グループを変更します。

   * ユーザーの追加または削除
   * サブグループの追加または削除

### 担当業務 {#job-roles}

ユーザーが次のいずれかの操作を行うと、担当業務監査ログエントリが生成されます。

* 担当業務の作成
* 担当業務の変更：

   * 名前の変更
   * 説明の追加、変更または削除
   * 時間あたりのコスト（コスト/時間）を追加、変更、または削除します。
   * 請求レート（請求/人）を追加、変更、または削除します。

* 担当業務の削除

担当業務の設定について詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

### ログイン試行 {#login-attempt}

ユーザーが次のいずれかの操作を行うと、システムはログイン試行監査ログエントリを生成します。

* （ブラウザーおよびモバイルアプリで）Workfront でのログイン、ログアウト、またはログインの試行に失敗する
* 任意の Workfront 統合（Slack 用のWorkfront、Salesforce 用の Workfrontなど）でのログイン、ログアウト、またはログインの試行に失敗する
* Workfront API へのログインとログアウト

Workfront 管理者が別のユーザーとしてログインする機能を使用した場合は、ログイン試行ログに記録されません。

>[!NOTE]
>
>組織が Adobe Admin Console にオンボーディングされている場合は、これは使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

### 優先度 {#priority}

ユーザーが次のいずれかの操作を行うと、優先度で監査ログエントリが生成されます。

* 優先度を作成
* 優先度を変更します。

   * 名前の変更
   * カラーの変更
   * デフォルトとして設定
   * 優先度の説明の追加、変更または削除
   * 優先度の表示または非表示

* 優先度の削除

優先度の設定について詳しくは、[優先度の作成とカスタマイズ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)を参照してください。

### プロジェクト環境設定 {#project-preference}

ユーザーが次のいずれかのアクションを実行すると、プロジェクト環境設定監査ログエントリが生成されます。

* カスタム四半期の作成
* プロジェクト環境設定の変更：

   * ロックまたはロック解除
   * 設定の 1 つを変更
   * 有効化、無効化または編集
   * タイムライン計算の編集

* カスタム四半期の削除

プロジェクト環境設定について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

### 重大度 {#severity}

ユーザーが次のいずれかのアクションを実行すると、重大度監査ログエントリが生成されます。

* イシューの重大度の作成
* イシューの重大度の変更：

   * 名前の変更
   * カラーの変更
   * デフォルトとして設定
   * 重大度の説明の変更または削除
   * 重大度の表示または非表示

* イシューの重大度の削除

担当業務の設定について詳しくは、[イシューの重要度を作成またはカスタマイズ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md)を参照してください。

### ステータス {#status}

ユーザーが次のいずれかのアクションを実行すると、ステータス監査ログエントリが生成されます。

* システムレベルまたはグループレベルでステータスを作成
* システムレベルまたはグループレベルでステータスを変更：

   * 名前の変更
   * デフォルトのステータスとして設定
   * ロックまたはロック解除
   * 表示または非表示
   * 色または説明の変更

* システムレベルまたはグループレベルでステータスを削除

ステータスについて詳しくは、[ステータスの概要](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)を参照してください。

### タスクと問題の設定 {#tasks-issues-preferences}

ユーザーが次のいずれかの方法でタスクとイシューの設定を変更すると、タスクとイシューの環境設定監査ログエントリが生成されます。

* 環境設定のロックまたはロック解除
* 環境設定の変更
* タスク、イシューまたはリクエストのアクセス設定の変更

タスクとイシューの環境設定について詳しくは、[システム全体のタスクとイシューの環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

### ユーザー {#user}

ユーザーが次のいずれかのアクションを実行すると、ユーザー監査ログエントリが生成されます。

* ユーザーの作成

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >組織が Adobe Admin Console にオンボーディングされている場合は、これは使用できません。詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

* ユーザーの削除
* ユーザーのアクセスレベル、会社、チーム、またはグループの変更
* ユーザーのアクティベート
* ユーザーのディアクティベート
