---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Workfrontでのイベントサブスクリプションの設定
description: Workfront管理者は、設定からイベントサブスクリプションを作成、表示、削除できます。 必要なアクセス権を持つユーザーは、権限とシステム設定で許可されている範囲内でイベントのサブスクリプションを管理することもできます。
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 8%
---

# Workfrontでのイベントサブスクリプションの設定

{{highlighted-preview-article-level}}

Adobe Workfront管理者は、設定領域からイベントサブスクリプションを作成、表示、削除できます。 イベントサブスクリプションは、指定されたイベントが発生したときに、Workfront イベント情報を外部エンドポイントに送信します。

Workfrontでイベントサブスクリプションを作成および削除することはできますが、既存のサブスクリプションを編集することはできません。 サブスクリプションを変更する必要がある場合は、サブスクリプションを削除して新しいサブスクリプションを作成します。

必要なアクセス権を持つユーザーは、Workfrontでイベントサブスクリプションを管理できる場合がありますが、その管理は、権限とシステム設定で許可されている範囲内でのみ行うことができます。 詳しくは、[管理者以外のユーザーとしてイベントサブスクリプションを管理](/help/quicksilver/wf-api/general/event-subs-non-admin.md)を参照してください。

イベントのサブスクリプションについて詳しくは、[&#x200B; イベントのサブスクリプション &#x200B;](/help/quicksilver/wf-api/api/event-subscriptions.md)の記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront パッケージ</td>
   <td>任意</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront プラン</td>
   <td>
    <p>標準</p>
    <p>プラン</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">アクセスレベル設定</td>
   <td>
    <p>イベント サブスクリプションを管理するには、適切なアクセス権が必要です。</p>
    <p>管理者以外のユーザーは、権限とシステム設定で許可されている範囲内でのみアクセスできます。</p>
   </td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イベントサブスクリプションの作成

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、**システム**&#x200B;をクリックし、**イベントのサブスクリプション**&#x200B;をクリックします。
1. 「**新規イベントサブスクリプション**」をクリックします。
1. 「**オブジェクト**」フィールドで、モニターするWorkfront オブジェクトを選択します。
1. 「**イベントタイプ**」フィールドで、オブジェクトの作成時、更新時、削除時、共有時にイベントサブスクリプションをトリガーするかどうかを選択します。
1. 「**Webhook URL**」フィールドに、イベントペイロードを受信するエンドポイントを入力します。
1. **認証トークン** フィールドに、エンドポイントへのリクエストの認証に使用するトークンを入力します。
1. Workfrontでペイロードを送信する前にエンコードする場合は、ペイロードをBase64として送信するオプションを有効にします。
1. 必要に応じて、1つ以上のフィルターを追加して、サブスクリプションをトリガーするイベントを制限します。 使用可能なフィルターは、選択したオブジェクトに基づいています。
1. 「**作成**」をクリックします。

エンドポイントの要件について詳しくは、[&#x200B; イベント サブスクリプション配信の要件](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md)を参照してください。

## イベント購読の表示

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、**システム**&#x200B;をクリックし、**イベントのサブスクリプション**&#x200B;をクリックします。

イベント購読ページから、環境に設定された購読を確認できます。 また、組織が持つサブスクリプションの合計数、およびアクティブ、無効、またはフリーズしているサブスクリプションの数を確認できます。

* **無効なサブスクリプション**：配信エラーが繰り返し発生したため、これらのサブスクリプションは自動的に無効になっています。
* **凍結されたサブスクリプション**：配信の問題により、これらのサブスクリプションは一時的に凍結されます。

## イベント購読を削除

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、**システム**&#x200B;をクリックし、**イベントのサブスクリプション**&#x200B;をクリックします。
1. 削除するイベントサブスクリプションを選択します。
1. 「**削除**」をクリックします。
