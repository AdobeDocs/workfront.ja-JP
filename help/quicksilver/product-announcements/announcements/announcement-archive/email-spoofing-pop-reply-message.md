---
content-type: reference
navigation-topic: announcements
title: メールのスプーフィングと POP 返信の削除
description: 20.3 リリース（2020年8月をターゲット）での、Adobe Workfront のメールの送受信方法に 2 つの変更を加えています。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: ht
source-wordcount: '314'
ht-degree: 100%

---

# メールスプーフィングと POP 返信

20.3 リリース（2020年8月をターゲット）での、Adobe Workfront のメールの送受信方法に 2 つの変更を加えています。

## Workfront からの送信メール

メールの配信を成功に導くために、スパムとしてタグ付けされるメールのスプーフィングを排除します（メールスプーフィングを参照）。Workfront からのすべてのメールは、自動アラートとユーザーとの間の通信の両方を含め、notifications@my.workfront.com から送信されます。Joan Harris からのメールの例は、メールの送信元エリアで次のように表示されます。

![](assets/noreply.png)

*IT チームに連絡して*、notifications@my.workfront.com からのメールがシステムへの受信メールとしてブロックされないようにすることを強くお勧めします。また、トラフィックとメールの送信元の IP アドレスの詳細については、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## 通知への受信メール返信（POP 返信）

特定のメール通知では、ユーザーがメールで返信し、その返信を Workfront システムのコメント返信として Workfront にコピーすることができます。Workfront のシステム管理者は、従来、これらの返信を受け取るために独自の POP メールサーバーを指定するか、組み込みの Workfront 返信システムを使用するかを選択できました。20.3 リリースでは、カスタム POP メールサーバーの選択が削除されます。カスタムサーバーを使用するように設定されているすべてのアカウントは、ネイティブの Workfront メール返信システムを使用するように自動的に移行されます。システム管理者やその他の Workfront ユーザーに対して必要なアクションはありません。

Workfront Proof システムから直接送信されるメールは変更されません。これらのメールは、これまでと同様に引き続き受信します。

その他のご質問やご不明な点は、[Workfront サポートチーム](https://one.workfront.com/s/support?language=ja_JP)にお問い合わせください。
