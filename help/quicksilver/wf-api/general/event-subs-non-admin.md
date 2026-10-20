---
content-type: api
navigation-topic: general-api
title: 管理者以外のユーザーとしてのイベント購読の管理
description: Workfront アクセスで許可されている場合は、権限とシステム設定で許可されている範囲内のイベントサブスクリプションを作成、表示、削除できます。
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%
---

# 管理者以外のユーザーとしてのイベント購読の管理

Workfront アクセスで許可されている場合は、設定領域からイベントサブスクリプションを作成、表示、削除できます。 ただし、アクセスは、自分の役割と組織のシステム設定によって許可されているサブスクリプションとアクションに限定されます。

この機能は、Workfront管理者と同じように、すべてのユーザーが利用できるわけではありません。 必要なアクセス権を持つユーザーは、付与された範囲内でのみイベントのサブスクリプションを管理できます。

例えば、権限では、定義された作業セットに対して、特定のオブジェクトタイプ、イベントタイプ、またはサブスクリプションのみを管理できます。 アクセスと設定で許可されているスコープ以外のイベントのサブスクリプションを管理することはできません。

管理者が管理する設定については、[Workfrontでのイベントサブスクリプションの設定](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)を参照してください。

イベント購読APIについて詳しくは、[&#x200B; イベント購読API](/help/quicksilver/wf-api/general/event-subs-api.md)を参照してください。

>[!NOTE]
>
>ユーザーは、権限と組織のシステム設定で許可された範囲内でのみ、イベントのサブスクリプションを管理できます。 アクセスは、管理者アクセスと自動的に同等ではありません。

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
    <p>アクセスは、権限と組織のシステム設定で許可されているサブスクリプションとアクションに制限されます。</p>
   </td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イベントサブスクリプションの操作

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、**システム**&#x200B;をクリックし、**イベントのサブスクリプション**&#x200B;をクリックします。
1. 利用可能なサブスクリプションを確認します。
1. 承認済みスコープ内のサブスクリプションのみを作成、表示、または削除します。

必要なオプションが表示されない場合、またはサブスクリプションを作成または管理できない場合は、Workfront管理者に連絡して、アクセス権がロール、権限、システム設定によって制限されているかどうかを確認してください。

## 関連する記事

* [Workfrontでのイベントサブスクリプションの設定](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [Event Subscription API](/help/quicksilver/wf-api/general/event-subs-api.md)
