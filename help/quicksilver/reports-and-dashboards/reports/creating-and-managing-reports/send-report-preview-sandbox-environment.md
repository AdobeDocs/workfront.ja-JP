---
product-area: reporting
navigation-topic: create-and-manage-reports
title: The projects are imported as new initiatives.プレビューサンドボックス環境でのレポートの送信
description: このページでは、プレビューおよびカスタム更新サンドボックス環境でのみ使用できる機能について説明します。 この機能は実稼動環境では使用できません。
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 95%

---

# The projects are imported as new initiatives.プレビューサンドボックス環境でのレポートの送信

<!-- Audited: 11/2024 -->

このページでは、プレビューおよびカスタム更新サンドボックス環境でのみ使用できる機能について説明します。 この機能は実稼動環境では使用できません。

Adobe Workfront テスト環境で「レポート配信」オプションを設定できます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

テスト環境は、実稼動環境にできるだけ近く機能するように設計していますが、一部の機能は実稼動環境とは異なります。

テスト環境でレポートをスケジューリングできますが、レポートの配信方法は実稼動環境での配信方法とは異なります。

実稼動環境での配信レポートのスケジュールについて詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。

レポートをスケジューリングする場所に応じて、プレビューサンドボックスとカスタム更新サンドボックスで配信機能は異なります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
      <td> 
      <p>新規：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>プラン</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p></td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## プレビュー環境でレポートをスケジューリング

* [プレビュー環境でレポートをスケジューリング](#schedule-reports-in-the-preview-environment)

### プレビュー環境でレポートをスケジューリング

配信されたレポートがプレビュー環境で生成されるかどうかは、「**このテスト環境からEメールを受信する**」が有効になっているかどうかに依存します。

サンドボックス環境からのメールの有効化について詳しくは、[プレビューサンドボックス環境からのメール配信を有効にする](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)を参照してください。

![ 「サンドボックスからメールを受信」オプション ](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

プレビュー環境でのレポートの配信スケジュール設定は、実稼動環境でのレポートのスケジュール設定と同じです。レポートの配信スケジュールについて詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。

プレビュー環境でレポートの配信をスケジューリングする場合、次のシナリオが考えられます。

* レポートを受信するユーザーに対して「**このテスト環境からEメールを受信する**」が無効になっている場合、レポートの配信をスケジューリングする際にファイルは生成されません。
* レポートを受信するユーザーに対して「**このテスト環境からEメールを受信する**」を有効にすると、レポートの配信をスケジューリングする際に生成されたファイルがユーザーの「ドキュメント」タブに追加されます。

## カスタム更新サンドボックス環境でレポートをスケジューリング

配信されたレポートがカスタム更新サンドボックスで生成されるかどうかは、「このテスト環境からEメールを受信する」設定が有効になっているかどうかで異なります。

プレビュー環境からのメールを有効にする方法については、[自身のメール通知の変更](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)の記事の[メール通知設定を表示および変更](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view)の節を参照してください。

![ 「サンドボックスからメールを受信」オプション ](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

カスタム更新サンドボックス環境でのレポートの配信スケジュール設定は、実稼動環境でのレポートのスケジュール設定と同じです。レポートの配信スケジュールについて詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。

カスタム更新サンドボックス環境でレポートの配信をスケジューリングする場合、次のシナリオが考えられます。

* レポートを受信するユーザーに対して「このテスト環境からEメールを受信する」が無効になっている場合、レポートの配信をスケジューリングする際にファイルは生成されません。
* レポートを受信するユーザーに対して「このテスト環境からEメールを受信する」を有効にすると、レポートはユーザーに関連付けられたメールアドレスに添付ファイルとしてメールで送信されます。

## 外部ユーザーへの通知方法

外部ユーザーは、Workfront テスト環境から送信されたレポートを受信せず、メール通知も受信しません。

外部ユーザーは、実稼動環境から配信された場合にのみ、メールでレポートを受け取ります。
