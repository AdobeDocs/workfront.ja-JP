---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: の権限レベル [!DNL Workfront] （Outlook 用）
description: この [!DNL Workfront for Outlook] アドインには読み取り/書き込みメールボックスアクセスが必要です。 この [!DNL Workfront for Outlook] 統合には、Outlook exchange サーバーから電子メール添付ファイルをダウンロードし、次の場所にアップロードする機能があるので、最高レベルの権限が必要です。 [!DNL Workfront]：添付ファイルのある電子メールから要求を送信したとき。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# の権限レベル [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] には、 [!DNL Outlook] アドインです。

の権限の詳細 [!DNL Outlook] アドイン： [のプライバシー、権限、セキュリティ [!DNL Outlook] アドイン](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) 内 [!DNL Microsoft] ドキュメント。

この [!DNL Workfront for Outlook] アドインには読み取り/書き込みメールボックスアクセスが必要です (`ReadWriteMailbox`) に設定されます。これは、最も高い権限範囲です。
この [!DNL Workfront for Outlook] 統合には、電子メール添付ファイルを [!DNL Outlook] exchange サーバとの間で [!DNL Workfront]：添付ファイルのある電子メールから要求を送信したとき。 この機能を使用するには、 [!DNL Workfront for Outlook] 関数を使用 `mailbox.getCallbackTokenAsync()` から [!DNL Office] トークンを取得し、それを使用して Exchange サーバーから E メール添付ファイルをダウンロードするためのアドイン JavaScript API です。 その関数を使用できる権限は次のみです。 `ReadWriteMailbox`. 詳しくは、 [Outlook アドインのプライバシー、アクセス許可、セキュリティ](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) (Microsoftドキュメント ) を参照してください。

この [!DNL Workfront for Outlook] アドインにも必要です `ReadWriteItem` 権限（に含まれる） `ReadWriteMailbox`) です。電子メールの本文を読み取り、電子メールメタデータを読み取る/更新するために使用されます。

* メール本文を読み取る：

   [!DNL Workfront for Outlook] は、ユーザーがリクエストを送信したときに電子メール本文を読み取るか、電子メール本文を更新として [!DNL Adobe Workfront] オブジェクト。
* 電子メールメタデータの読み取り/更新：

   [!DNL Workfront for Outlook] ユーザーが電子メールから要求を送信すると、電子メールヘッダーを更新します。 これは、送信された [!DNL Adobe Workfront] オブジェクトに含まれるので、ユーザーが次に同じ電子メールのアドインを開くと、その電子メールに関する以前のアクションに関する情報が表示されます。

[!DNL Workfront for Outlook] ユーザーがアドオン内でアクションを実行した場合にのみ、ユーザーのメールボックスにアクセスします。 バックグラウンド機能はありません。 Workfront for Outlook は、次のシナリオでのみユーザーのメールボックスにアクセスします。

* ユーザーは、リクエストの送信、タスクの作成、または更新としての電子メールの送信を [!DNL Workfront for Outlook] （アドインを開き、アクションを選択する）
   * [!DNL Workfront for Outlook] は電子メールの本文を読み取り、アドイン内のフォームに入力します。
   * [!DNL Workfront for Outlook] は電子メールメタデータを読み取り、同じ電子メールでアドインでおこなわれた以前の操作に関する情報を表示します。
* ユーザーがリクエストを送信したとき、タスクを作成したとき、または電子メールを更新として送信したとき [!DNL Workfront for Outlook] ( [!UICONTROL 送信] 」ボタンをクリックします )。
   * [!DNL Workfront for Outlook] は電子メールの本文を読み取り、リクエストの説明またはコメントとしてWorkfrontに送信します。
   * [!DNL Workfront for Outlook] 電子メールメタデータを更新して、送信されたリクエストや更新されたオブジェクトに関する情報を保存します。
   * [!DNL Workfront for Outlook] exchange サーバーから電子メール添付ファイルをダウンロードして、送信された要求、作成されたタスク、または更新されたオブジェクトにアップロードします。
