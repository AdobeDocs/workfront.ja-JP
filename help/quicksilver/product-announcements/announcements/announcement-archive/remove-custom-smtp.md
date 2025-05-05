---
content-type: reference
navigation-topic: announcements
title: カスタム SMTP を送信メールオプションとして削除する
description: 20.3 リリース（2020年8月を目標とする）で、Adobe Workfront は、Workfront のアップデートおよび通知に関するメール配信の信頼性を大幅に向上させる新しいメールシステムに移行します。その結果、お客様は、Workfront プラットフォームから目的の受信者にメールをリレーするために、独自の SMTP メールサーバーを使用できなくなります。すべてのメールは、Workfront メールサーバーから直接送信されます。
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 98%

---

# カスタム SMTP を送信メールオプションとして削除する

20.3 リリース（2020年8月を目標とする）で、Adobe Workfront は、Workfront のアップデートおよび通知に関するメール配信の信頼性を大幅に向上させる新しいメールシステムに移行します。その結果、お客様は、Workfront プラットフォームから目的の受信者にメールをリレーするために、独自の SMTP メールサーバーを使用できなくなります。すべてのメールは、Workfront メールサーバーから直接送信されます。

この機能にアクセスするには、システム管理者としてログインし、設定／メール／設定の順に移動します。この機能を強調表示したスクリーンショットを次に示します。

![ メールサーバーの設定 ](assets/email-server-settings-350x226.png)

このスクリーンショットで強調表示されている設定は、20.3 リリースで「Workfront メールサーバー」オプションを使用するように自動的に切り替わります。

カスタム SMTP メールサーバーを設定済みの場合は、**IT チームに連絡して**、notifications@my.workfront.com からのメールがシステムへの受信メールとしてブロックされないようにすることを強くお勧めします。また、トラフィックとメールの送信元の IP アドレスについて詳しくは、ファイアウォールの設定を参照してください。

その他のご質問やご不明な点は、[Workfront サポートチーム](https://experienceleague.adobe.com/ja?support-tab=home#support)にお問い合わせください。
