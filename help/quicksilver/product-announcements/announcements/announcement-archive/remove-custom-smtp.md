---
content-type: reference
navigation-topic: announcements
title: 送信メールオプションとしてのカスタム SMTP の削除
description: 20.3 リリース（2020 年 8 月を対象とする）で、Adobe Workfrontは、Workfrontのアップデートおよび通知に関する E メール配信の信頼性を大幅に向上させる新しい E メールシステムに移行します。 その結果、お客様は、Workfrontプラットフォームから目的の受信者に E メールをリレーするために、独自の SMTP E メールサーバーを使用できなくなります。 すべての電子メールは、Workfront Mail Server から直接送信されます。
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# 送信メールオプションとしてのカスタム SMTP の削除

20.3 リリース（2020 年 8 月を対象とする）で、Adobe Workfrontは、Workfrontのアップデートおよび通知に関する E メール配信の信頼性を大幅に向上させる新しい E メールシステムに移行します。 その結果、お客様は、Workfrontプラットフォームから目的の受信者に E メールをリレーするために、独自の SMTP E メールサーバーを使用できなくなります。 すべての電子メールは、Workfront Mail Server から直接送信されます。

この機能にアクセスするには、システム管理者としてログインし、「設定」>「電子メール」>「設定」の順に移動します。 次に、この機能をハイライトしたスクリーンショットを示します。

![](assets/email-server-settings-350x226.png)

このスクリーンショットでハイライト表示されている設定は、20.3 リリースでWorkfront Mail Server オプションを使用するように自動的に切り替わります。

カスタム SMTP メールサーバーを設定済みの場合、 **IT チームに連絡することを強くお勧めします** notifications@my.workfront.comからの電子メールがシステムへの受信メールをブロックされないようにするため。 また、トラフィックと電子メールの送信元 IP アドレスの詳細については、ファイアウォールの設定を参照してください。

その他のご質問やご不明な点は、 [Workfront Support Team](https://one.workfront.com/s/support?language=en_US).
