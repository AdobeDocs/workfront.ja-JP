---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: ' [!DNL Workfront]  for Outlook の権限レベル'
description: ' [!DNL Workfront for Outlook]  アドインには、メールボックスの読み取り / 書き込みアクセス権が必要です。 [!DNL Workfront for Outlook]  統合では、ユーザーが添付ファイル付きのメールからリクエストを送信した際に、Outlook Exchange サーバーから添付ファイルをダウンロードして  [!DNL Workfront] にアップロードする機能があるため、最も高いレベルの権限が必要です。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 79%

---

# [!DNL Workfront for Outlook] の権限レベル

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**


[!DNL Workfront for Outlook] には、[!DNL Outlook] アドインで許可されている 4 つの中で最も高いレベルの権限が必要です。

[!DNL Outlook] アドインでの権限について詳しくは、[!DNL Microsoft] ドキュメントの[ [!DNL Outlook]  アドインに関するプライバシー、アクセス許可、セキュリティ](https://docs.microsoft.com//office/dev/add-ins/outlook/privacy-and-security)を参照してください。

[!DNL Workfront for Outlook] アドインには、最も高い権限範囲であるメールボックスの読み取り / 書き込みアクセス権（`ReadWriteMailbox`）が必要です。
[!DNL Workfront for Outlook] 統合では、ユーザーが添付ファイル付きのメールからリクエストを送信した際に、[!DNL Outlook] Exchange サーバーから添付ファイルをダウンロードして [!DNL Workfront] にアップロードする機能があるため、最も高いレベルの権限が必要です。そのために、[!DNL Workfront for Outlook] では [!DNL Office] アドイン JavaScript API の `mailbox.getCallbackTokenAsync()` 関数を使用してトークンを取得し、そのトークンを使用して Exchange サーバーからメールの添付ファイルをダウンロードします。その関数を使用できる権限は、`ReadWriteMailbox` のみです。詳しくは、Microsoft ドキュメントの [Outlook アドインに関するプライバシー、アクセス許可、セキュリティ](https://docs.microsoft.com//office/dev/add-ins/outlook/privacy-and-security)を参照してください。

[!DNL Workfront for Outlook] アドインには、`ReadWriteItem` 権限も必要です（`ReadWriteMailbox` に含まれています）。これはメールの本文の読み取り、およびメールのメタデータの読み取り / 更新に使用されます。

* メール本文の読み取り：

  [!DNL Workfront for Outlook] は、ユーザーがリクエストを送信したとき、または [!DNL Adobe Workfront] オブジェクトへの更新としてメール本文を送信したときに、メールの本文を読み取ります。
* メールのメタデータの読み取り / 更新：

  [!DNL Workfront for Outlook] は、ユーザーがメールからリクエストを送信したときに、メールヘッダーを更新します。これは、送信された [!DNL Adobe Workfront] オブジェクトの情報を格納するために行われ、ユーザーがその後、同じメールのアドインを開くと、そのメールでの以前のアクションに関する情報が表示されます。

[!DNL Workfront for Outlook] は、ユーザーがアドオン内でアクションを実行した場合のみ、ユーザーのメールボックスにアクセスします。バックグラウンド機能はありません。Workfront for Outlook は、次のシナリオでのみ、ユーザーのメールボックスにアクセスします。

* ユーザーが [!DNL Workfront for Outlook] から、リクエストの送信、タスクの作成、または更新としてのメールの送信を行う（アドインを開き、アクションを選択する）
   * [!DNL Workfront for Outlook] はメールの本文を読み取り、アドイン内のフォームに入力します。
   * [!DNL Workfront for Outlook] はメールのメタデータを読み取り、同じメールのアドインでの以前の操作に関する情報を表示します。
* ユーザーが [!DNL Workfront for Outlook] から、リクエストの送信、タスクの作成、または更新としてのメールの送信を行う（アドインで「[!UICONTROL 送信]」ボタンをクリックする）
   * [!DNL Workfront for Outlook] はメールの本文を読み取り、リクエストの説明またはコメントとして Workfront に送信します。
   * [!DNL Workfront for Outlook] はメールのメタデータを更新して、送信されたリクエストや更新されたオブジェクトに関する情報を格納します。
   * [!DNL Workfront for Outlook] は Exchange サーバーからメールの添付ファイルをダウンロードして、送信されたリクエスト、作成されたタスク、または更新されたオブジェクトにアップロードします。
