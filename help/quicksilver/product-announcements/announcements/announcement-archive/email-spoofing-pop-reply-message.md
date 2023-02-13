---
content-type: reference
navigation-topic: announcements
title: メールのスプーフィングと POP 返信の削除
description: 20.3 リリース（2020 年 8 月をターゲット）での、Adobe Workfrontの電子メールの送受信方法に 2 つの変更を加えています。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# メールスプーフィングと POP 返信

20.3 リリース（2020 年 8 月をターゲット）での、Adobe Workfrontの電子メールの送受信方法に 2 つの変更を加えています。

## Workfrontからの送信メール

E メールの配信を成功に導くために、スパムとしてタグ付けされる E メールのスプーフィングを排除します（E メールスプーフィングを参照）。 Workfrontからのすべての電子メールは、自動アラートとユーザー間通信の両方を含め、notifications@my.workfront.comから送信されます。 Joan Harris からの電子メールの例は、電子メールの送信元領域で次のように表示されます。

![](assets/noreply.png)

*IT チームに連絡することを強くお勧めします* notifications@my.workfront.comからの電子メールがシステムへの受信メールをブロックされないようにするため。 また、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) を参照してください。

## 通知への受信メール返信（POP 返信）

特定の電子メール通知を使用すると、ユーザーは電子メールで返信し、その返信をWorkfrontにコメントの返信としてコピーできます (Workfrontシステム内 )。 Workfrontのシステム管理者は、従来、これらの返信を受け取るために独自の POP 電子メールサーバーを提供するか、組み込みのWorkfront返信システムを使用するかを選択できました。 20.3 リリースでは、カスタム POP 電子メールサーバーの選択が削除されます。 カスタムサーバーを使用するように設定されているすべてのアカウントは、ネイティブのWorkfront電子メール返信システムを使用するように自動的に移行されます。 システム管理者やその他のWorkfrontユーザーに対して必要なアクションはありません。

Workfront Proof システムから直接送信される E メールは変更されません。 あなたは過去と同じようにそのメールを引き続き受け取ります。

その他のご質問やご不明な点は、 [Workfront Support Team](https://one.workfront.com/s/support?language=en_US).
