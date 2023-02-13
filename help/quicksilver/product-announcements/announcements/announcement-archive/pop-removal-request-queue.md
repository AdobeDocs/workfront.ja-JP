---
content-type: reference
navigation-topic: announcements
title: 新しいAdobe Workfrontが管理するシステムで、リクエストキューの POP 電子メールを 21.1 に置き換えました。
description: リクエストキューの POP 電子メールオプションを、新しいAdobe Workfront管理システムに置き換えます。 引き続き電子メールでリクエストを送信できますが、代わりに、リクエストキュー領域で新しいWorkfrontが管理する電子メールアドレスを設定する必要があります。
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 新しいAdobe Workfrontが管理するシステムで、リクエストキューの POP 電子メールを 21.1 に置き換えました。

リクエストキューの POP 電子メールオプションを、新しいAdobe Workfront管理システムに置き換えます。 引き続き電子メールでリクエストを送信できますが、代わりに、リクエストキュー領域で新しいWorkfrontが管理する電子メールアドレスを設定する必要があります。

## POP 電子メールオプションを削除する理由

POP テクノロジーは、信頼性が低く、安全性の低い E メールオプションです。 また、特に POP E メールに関するお客様の問題も多く見られます。 Workfrontが管理するシステムに変更を加えると、より信頼性の高いエクスペリエンスが得られます。

## 実行する必要があるアクションは何ですか？

実稼動環境で POP E メールで設定したリクエストキューごとに新しい E メールアドレスを設定し、必要に応じて新しい E メールアドレスを配布する必要があります。 詳しくは、 [ユーザーが問題をリクエストキュープロジェクトに電子メールで送信できるようにします](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## 移行計画とは

2 月上旬の 21.1 リリースから、ユーザーを新しい *@intake.workfront.com* 作成する電子メールアドレス。 60 日間は、以前使用していた POP E メールが引き続き機能します。

## プレビューでテストするにはどうすればよいですか？

この変更をプレビューでテストするには、プレビュー環境で電子メールを有効にする必要があります。 そのためには、 [プレビューサンドボックス環境からの E メールの配信を有効にする](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>ここで設定した内容は、実稼動環境には引き継がれません。 機能が実稼動環境にリリースされた後、このプロセスを再度実行する必要があります。
