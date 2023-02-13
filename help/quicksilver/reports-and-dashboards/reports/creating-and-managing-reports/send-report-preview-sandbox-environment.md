---
product-area: reporting
navigation-topic: create-and-manage-reports
title: プレビューサンドボックス環境でのレポートの送信
description: このページの情報は、プレビューおよびカスタム更新サンドボックス環境でのみ使用できる機能について説明します。 この機能は、実稼動環境では使用できません。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# プレビューサンドボックス環境でのレポートの送信

このページの情報は、プレビューおよびカスタム更新サンドボックス環境でのみ使用できる機能について説明します。 この機能は、実稼動環境では使用できません。

任意のAdobe Workfrontテスト環境で「レポート配信」オプションを設定できます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

テスト環境は、実稼動環境にできるだけ近く機能するように設計されていますが、一部の機能は実稼動環境とは異なります。

テスト環境でレポートのスケジュールを設定することはできますが、レポートの配信方法は実稼動環境での配信方法とは異なります。

実稼動環境での配信レポートのスケジュールについて詳しくは、 [レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

レポートのスケジュール場所に応じて、配信機能は、プレビューサンドボックスとカスタム更新サンドボックスで異なります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プレビュー環境でのレポートのスケジュール設定

* [プレビュー環境でのレポートのスケジュール設定](#schedule-reports-in-the-preview-environment)

### プレビュー環境でのレポートのスケジュール設定

配信されたレポートがプレビュー環境で生成されるかどうかは、 **このテスト環境からメールを受信** が有効かどうか。

サンドボックス環境からの E メールの有効化について詳しくは、 [プレビューサンドボックス環境からの E メールの配信を有効にする](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

プレビュー環境での配信レポートのスケジュール設定は、実稼動環境でのレポートのスケジュール設定と同じです。 レポートの配信スケジュールについて詳しくは、 [レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

プレビュー環境でレポートの配信スケジュールを設定する場合、次のシナリオが考えられます。

* 条件 **このテスト環境からメールを受信** レポートを受信するユーザーに対しては、が無効になっている場合、配信用のレポートをスケジュールする際にファイルは生成されません。
* 条件 **このテスト環境からメールを受信** を有効にすると、レポートを受け取るユーザーに対して、配信用のレポートをスケジュールする際に生成されるファイルが、ユーザーの「ドキュメント」タブに追加されます。

## カスタム更新サンドボックス環境でレポートをスケジュールする

配信されたレポートがカスタム更新サンドボックスで生成されるかどうかは、[ このテスト環境からのメール受信 ] 設定が有効になっているかどうかによって異なります。

プレビュー環境からの E メールの有効化について詳しくは、「 [電子メール通知設定を表示および変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) 記事内 [独自のイベント通知をアクティブ化または非アクティブ化する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

カスタム更新サンドボックス環境で配信するレポートのスケジュール設定は、実稼動環境でレポートをスケジュールする場合と同じです。 レポートの配信スケジュールについて詳しくは、 [レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

カスタム更新サンドボックス環境でレポートの配信スケジュールを設定する場合、次のシナリオが考えられます。

* レポートを受信するユーザーに対して「このテスト環境から電子メールを受信」が無効になっている場合、レポートの配信スケジュールを設定する際にファイルが生成されません。
* 「このテスト環境からの電子メールの受信」がレポートの受信者に対して有効になっている場合、レポートはユーザーに関連付けられた電子メールアドレスに添付ファイルとして電子メールで送信されます。

## 外部ユーザーへの通知方法

外部ユーザーは、Workfrontのテスト環境から送信されたレポートを受け取らず、電子メール通知も受け取りません。

外部ユーザーは、実稼動環境から配信された場合にのみ、電子メールでレポートを受け取ります。
