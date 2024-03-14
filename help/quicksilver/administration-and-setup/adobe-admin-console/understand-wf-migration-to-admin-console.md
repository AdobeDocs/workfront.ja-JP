---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Adobe Admin ConsoleへのWorkfrontの移行について
description: Workfront製品およびAdobe Admin Consoleへのユーザーの移行について
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 0a638b143d2de4b8ff2948e701ee90acbd1ab857
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Adobe Admin ConsoleへのWorkfrontの移行について

Adobeは、Adobe Workfrontユーザーの管理方法を変え、ユーザーや組織の生産性を高めています。 この変更の一環として、Adobeは、WorkfrontインスタンスとユーザーをAdobe Admin Consoleに移行中です。 これは移行が必要で、レポート、承認パス、コンテンツ、アセットには影響しません。 ユーザーアクセスの管理方法やユーザーのログイン方法に影響を与えます。

Adobe Admin Consoleを使用して組織全体のAdobe使用権限を管理する方法については、 [Adobe Admin Consoleでのユーザー管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## 変更点

移行の一環として、ユーザー管理は、次の管理者の役割を持つWorkfrontアプリケーション内からAdobe Admin Consoleに移行します。

* **システム管理者** は、すべての管理者の権限を持つスーパーユーザーです。 すべての管理者ロールを割り当て、すべての製品に対して組織全体のユーザーを管理します。

* **製品プロファイル管理者 (Workfrontシステム管理者 )** 組織内のどのユーザーがWorkfrontにアクセスできるかを管理します。

* **ユーザーはAdobeID でログインします。** Adobeが既存のAdobeをAdobe Admin Consoleに移行すると、ユーザーは新しいユーザー ID(Adobe IDまたはAdobeFederated ID(SSO)) を使用してWorkfrontインスタンスにログインします。

* **その他のすべての機能の管理方法に変更はありません** 機能、ユーザーの役割、ワークスペース、機能および動作の管理を含め、Workfrontアプリケーション自体内で使用できます。

## 移行ジャーニーのタイムライン

Adobeは、最初にWorkfrontインスタンスをAdobe Admin Consoleに移行してから、検証済みの電子メールアドレスを持つ既存のすべてのユーザーを移行します。 システム管理者またはWorkfront製品プロファイル管理者 (Workfront System 管理者 ) の場合、移行プロセスをガイドする電子メールが届きます。 以下に、期待できるタイムラインを示します。

### WorkfrontからAdobe Admin Consoleへの移行の完了

Adobe Admin ConsoleへのWorkfrontの移行が完了すると、システム管理者に電子メールが送信されます。 現時点では、システム管理者が必要な手順をいくつか実行する必要がある場合があります。 **ユーザー移行の開始前**&#x200B;を使用して、Workfrontユーザーへの影響を最小限に抑えます。

* **Workfrontユーザーが現在 SSO でログインしている場合**&#x200B;を設定している場合、ユーザーが SSO を使用してログインを続行できるように、Adobe Admin Consoleで SSO を設定する必要があります。 Workfrontユーザーが現在 SSO を使用していないが、Adobe Admin Consoleで設定したい場合は、移行ジャーニーのこの時点で設定できます。
* **Adobe Admin Consoleで他のAdobe製品を既に管理している場合**&#x200B;の場合、Adobeは、ユーザーを既存のコンソールに自動的に移行する同意を求める場合があります。 次をクリック： **はじめに** ボタンをクリックして同意ページに移動します。
* **以前にリクエスト元のライセンスタイプを削除した場合**&#x200B;を探すと、システムに追加されます。 このライセンスの種類にはユーザーが割り当てられませんが、WorkfrontとAdobe Admin Consoleの間の同期に必要です。 リクエスト元のライセンスの種類に関して、お客様からのアクションは不要です。

現時点では、ユーザー管理に変更はありません。 Workfront管理者はWorkfrontで引き続きユーザーを管理し、ユーザーの移行が完了するまで、Workfront ID または SSO を使用してログインし続けます。

### ユーザー移行のスケジュール設定

前の節で説明した前提条件をAdobeが完了すると、システムは、前述の前提条件が完了してから 30 日間、自動的にユーザー移行のスケジュールを設定し、Workfront製品プロファイル管理者 (Workfrontシステム管理者 ) に連絡して管理します。

Workfront製品プロファイル管理者 (Workfrontシステム管理者 ) は、次の操作をおこないます。

* スケジュールされたユーザー移行開始日（前提条件が完了してから約 30 日後）と共に電子メールを受信します
* 指定されたWorkfront管理者コンソールにアクセスし、移行日を変更することができます。

  >[!NOTE]
  >
  >移行が複雑なので、日付の変更はスケジュールされた日付から 30 日以内に制限されます。 後日が必要な場合は、サポートにお問い合わせください。

* ユーザー移行開始日の 1 日前にリマインダーの電子メールを受け取る

### 移行日のユーザー準備

Workfront製品プロファイル管理者 (Workfront System Administrator) は、すべてのユーザーが移行に関する準備を 1 日おこなうように責任を負います。

* AdobeID への今後の移行に備えて、以下の情報をユーザーに通知します。

   * ユーザーが移行すると、Workfrontへのログイン方法の変更をAdobeから通知する電子メールが送信されます。 AdobeID を使用したログインの招待を受け入れるよう、既存のAdobe IDでサインインするか、同じ電子メールアドレスを使用して新しいログインを設定して、初めて招待されます。

### 移行日に期待される事項

* **ユーザーの移行は、お客様がホストするWorkfront Datacenter の午前 0 時に開始されます。**

* **Adobeは、最初にWorkfront管理者を自動的に移行します。** Workfront管理者がAdobeID に移行されると、Adobe製品プロファイル管理者 (Workfrontシステム管理者 ) の役割が割り当てられます。 移行前にユーザーが持っていた既存の役割には影響しません。

  >[!NOTE]
  >
  >ユーザーの移行中に、製品へのアクセス権が失われることはありません。 ユーザーの移行中にログインした場合、影響はありません。 ただし、次回ログインする際には、AdobeID を使用する必要があります。



* **ユーザーが移行されると、Workfrontへのログイン方法の変更をAdobeに通知する電子メールがユーザーに届きます。** AdobeID を使用したログインの招待を受け入れるよう、既存のAdobe IDでサインインするか、同じ電子メールアドレスを使用して新しいAdobe IDを設定して、初めて招待されます。

  Adobe IDを使用してWorkfrontにログインする方法について詳しくは、 [Adobe Experience Cloudにログイン](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### ユーザー移行完了

Adobeは、すべての管理者とユーザーが移行された後、電子メールですべてのシステム管理者と製品プロファイル管理者 (Workfrontシステム管理者 ) に通知します。 現時点では、そのインスタンスのすべてのWorkfrontユーザーは、AdobeID を使用してWorkfrontにログインします。 Workfrontシステム管理者と製品プロファイル管理者 (Workfrontシステム管理者 ) は、Adobe Admin Console内でユーザーアクセスを管理できます。 管理者コンソール内でディレクトリ同期の形式を使用していない場合、Workfrontアプリケーション内で引き続きWorkfrontへのアクセスを管理できます。

## サポートを受ける

質問や懸念事項については、記事に記載されている手順に従ってください。 [カスタマーサポートに連絡](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




