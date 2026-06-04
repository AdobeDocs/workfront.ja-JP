---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 自動リマインダーとリマインダー通知
description: この記事では、自動リマインダーとリマインダー通知の違いについて説明し、それぞれのシナリオを示します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 26c6fa2c-5c3a-4f53-bd7e-e49a623ff60d
TQID: https://experienceleague.adobe.com/hSVm-rgiBcbHaCwO1veCLEo-q6U5SWzt58qO6KqC84M
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 89%

---

# 自動リマインダーとリマインダーの通知

この記事では、自動リマインダーとリマインダー通知の違いについて説明し、それぞれのシナリオを示します。 すべての [!DNL Adobe Workfront] 通知について詳しくは、[[!DNL Adobe Workfront]  通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## 自動リマインダ

自動リマインダーに固有の特性は次のとおりです。

* オンにしたり編集したりできるのは [!DNL Workfront] 管理者のみです
* 期限、遅延、または予定完了日に近づいたすべてのタスクとイシューに対してトリガーされます
* 割り当て先、割り当て先のマネージャー、直属マネージャーのマネージャーにのみ送信可能です。
* メールテンプレートを添付することはできません。

シナリオ：システム全体のすべてのタスクとイシューに対してリマインダーをトリガーする場合は、自動リマインダー設定を構成します。 詳しくは、[自動リマインダーの設定](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md)を参照してください。

## リマインダー通知

次の特徴は、リマインダー通知に限られます。

* 管理者またはプランの標準ライセンスとリマインダー通知への管理アクセス権を持つユーザーが作成できます
* 手動でオブジェクトに関連付けることができます
* 添付されたオブジェクトに関する通知のみ可能です
* 所有者、作成者、承認者、割り当て先など、様々なオブジェクトの関係者に送信できます
* デフォルトのメール、または添付されたカスタマイズ済みのメールテンプレートを使用できます

シナリオ：プロジェクト、タイムシートのリマインダーを作成する場合、またはタスクとタスクのリマインダーをカスタマイズする場合は、リマインダー通知を設定します。 詳しくは、[リマインダー通知の設定](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md)を参照してください。
