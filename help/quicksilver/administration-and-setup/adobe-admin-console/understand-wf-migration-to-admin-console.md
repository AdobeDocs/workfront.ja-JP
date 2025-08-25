---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Adobe Admin Console への Workfront の移行について
description: この記事では、一般的な用語で組織をAdobe Admin Consoleに移行するプロセスを説明します。これにより、Workfront管理者は移行の見通しを把握できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 94%

---

# Adobe Admin Console への Workfront の移行について

アドビは、Adobe Workfront ユーザーの管理方法を変更し、ユーザーや組織の生産性を高めます。この変更の一環として、アドビは、Workfront のインスタンスとユーザーを Adobe Admin Console に移行中です。これは必要な移行であり、レポート、承認パス、コンテンツ、アセットには影響しません。ユーザーアクセスの管理方法やユーザーのログイン方法に影響を与えます。

この記事では、一般的な用語で組織をAdobe Admin Consoleに移行するプロセスを説明します。これにより、Workfront管理者は移行の見通しを把握できます。

Adobe Admin Console を使用して組織全体の Adobe 使用権限を管理する方法については、[Adobe Admin Console でのユーザー管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください。

## 変わること

移行の一環として、ユーザー管理が Workfront アプリケーション内から Adobe Admin Console に移行し、次の管理者の役割を持つようになります。

* **システム管理者**&#x200B;は、すべての管理権限を持つスーパーユーザーです。すべての管理者の役割を割り当て、すべての製品に対する組織全体のユーザーを管理します。

* **製品プロファイル管理者（Workfront システム管理者）**&#x200B;は、組織内のどのユーザーが Workfront にアクセスできるかを管理します。

* **ユーザーは Adobe ID でログインします。** アドビが既存のユーザーを Adobe Admin Console に移行すると、ユーザーは新しいユーザー ID（Adobe ID または Adobe Federated ID（SSO））を使用して Workfront インスタンスにログインします。

* 機能、ユーザーの役割、ワークスペース、機能、動作の管理を含む、Workfront アプリケーション自体の&#x200B;**他のすべての機能の管理方法に変更はありません**。

## 移行ジャーニーのタイムライン

アドビは、最初に Workfront インスタンスを Adobe Admin Console に移行してから、検証済みのメールアドレスを持つ既存のユーザーをすべて移行します。システム管理者または Workfront 製品プロファイル管理者（Workfront システム管理者）には、移行プロセスを案内するメールが届きます。以下はそのタイムラインです。

### Workfront から Adobe Admin Console への移行の完了

Workfront から Adobe Admin Console への移行が完了すると、システム管理者にメールが届きます。この時点で、**ユーザー移行を開始する前に**、システム管理者はいくつかの必要な手順を実施して、Workfront ユーザーへの影響を最小限に抑える必要があります。

* **現在 Workfront ユーザーが SSO でログインしている場合**、Adobe Admin Consoleで SSO を設定して、ユーザーが引き続き SSO でログインできるようにする必要があります。現在 Workfront ユーザーは SSO を使用していないが、Adobe Admin Consoleでは SSO を設定する場合は、移行ジャーニーのこの時点で設定できます。
* **Adobe Admin Console で他のアドビ製品を既に管理している場合**、アドビはユーザーを既存の Console に自動的に移行する同意を求める場合があります。同意ページには、メールにある「**開始**」ボタンをクリックすると移動できます。
* **以前に依頼者ライセンスタイプを削除したことがある場合**&#x200B;は、システムに追加されます。このライセンスタイプに割り当てられるユーザーはいませんが、Workfron tと Adobe Admin Console の間の同期に必要となります。依頼者ライセンスタイプについては、ユーザーによるアクションは不要です。

現時点ではユーザー管理に変更はありません。Workfront 管理者は Workfront で引き続きユーザーを管理し、ユーザーは移行が完了するまで、Workfront ID または SSO を使用してログインし続けます。

### ユーザー移行スケジュール

前の節で説明した前提条件をシステム管理者が完了すると、アドビはこれらの前提条件が完了してから 30 日後にユーザー移行を自動的にスケジュールし、Workfront 製品プロファイル管理者（Workfront システム管理者）とやり取りしてユーザー移行を管理します。

Workfront 製品プロファイル管理者（Workfront システム管理者）は：

* メールでユーザー移行開始日（前提条件が完了してから約 30 日後）のスケジュールを受信します。
* 指定された Workfront 管理者コンソールにアクセスし、移行日を変更することができます。

  >[!NOTE]
  >
  >移行が複雑なので、日付の変更はスケジュールされた日付から 30 日以内に制限されます。さらに先の日程に変更する必要がある場合は、サポートにお問い合わせください。

* ユーザー移行開始日の 1 日前にリマインダーのメールを受け取ります。

### 移行日に向けたユーザーの準備

Workfront 製品プロファイル管理者（Workfront システム管理者）は、すべてのユーザーが移行に備えられるようにする必要があります。

* 次の情報を共有することで、Adobe ID への今後の移行に対する準備を整えます。

   * ユーザーが移行すると、Workfront へのログイン方法の変更を通知するメールが届きます。ユーザーは、既存の Adobe ID でログインするか、同じメールアドレスを使用して新しい Adobe ID を設定することで、初めて Adobe ID を使用してログインするための招待を受け入れるように求められます。

### 移行日に期待される事項

* **ユーザー移行は、お客様がホスディングしている Workfront データセンターの午前 0 時に開始されます。**

* **アドビは、最初に Workfront 管理者を自動的に移行します。** Workfront 管理者は Adobe ID に移行されると、Adobe 製品プロファイル管理者（Workfront システム管理者）の役割が割り当てられます。移行前にユーザーが持っていた既存の役割には影響しません。

  >[!NOTE]
  >
  >ユーザーの移行中に、製品へのアクセス権が失われることはありません。ユーザー移行中にユーザーがログインしている場合も、影響はありません。ただし、次回ログインする際には、Adobe ID を使用する必要があります。



* **ユーザーが移行されると、Workfront へのログイン方法の変更を通知するメールがアドビからユーザーに届きます。**&#x200B;ユーザーは、既存の Adobe ID でサインインするか、同じメールアドレスを使用して新しい Adobe ID を設定することで、初めて Adobe ID を使用してサインインするための招待を受け入れるように求められます。

  Adobe ID で Workfront にログインする方法について詳しくは、[Adobe Experience Cloud にログイン](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud)を参照してください。

### ユーザー移行完了

アドビは、すべての管理者とユーザーが移行された後、すべてのシステム管理者と製品プロファイル管理者（Workfront システム管理者）にメールで通知します。この時点では、そのインスタンスのすべての Workfront ユーザーは、Adobe ID を使用して Workfront にログインしています。Workfront システム管理者と製品プロファイル管理者（Workfront システム管理者）は、Adobe Admin Console でユーザーアクセスを管理できます。管理者コンソール内でディレクトリ同期の形式を使用していない場合、Workfront アプリケーション内で引き続き Workfront へのアクセスを管理できます。

## サポートを受ける

ご質問やご不明な点は、[カスタマーサポートに連絡](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)の記事に記載されている手順に従ってください。




