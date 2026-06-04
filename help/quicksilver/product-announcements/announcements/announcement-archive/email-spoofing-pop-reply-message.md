---
content-type: reference
navigation-topic: announcements
title: メールのスプーフィングと POP 返信の削除
description: 20.3 リリース（2020年8月をターゲット）での、Adobe Workfront のメールの送受信方法に 2 つの変更を加えています。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
TQID: https://experienceleague.adobe.com/eOFRSbJicMbYHqq74-O9VW0c73RDQmAC-OIkLX-FKFw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 319
ht-degree: 85%

---

# メールスプーフィングと POP 返信

20.3 リリース（2020年8月をターゲット）での、Adobe Workfront のメールの送受信方法に 2 つの変更を加えています。

## Workfront からの送信メール

メールの配信を成功に導くために、スパムとしてタグ付けされるメールのスプーフィングを排除します（メールスプーフィングを参照）。 Workfrontからのすべての電子メールは、自動アラートとユーザー間のコミュニケーションの両方を含め、`notifications@my.workfront.com`から送信されます。 Joan Harris からのメールの例は、メールの送信元エリアで次のように表示されます。

![電子メールの例](assets/noreply.png)

*IT チーム*&#x200B;に連絡して、`notifications@my.workfront.com`からの電子メールがシステムへの電子メール受信でブロックされないようにすることを強くお勧めします。 また、トラフィックとメールの送信元の IP アドレスの詳細については、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## 通知への受信メール返信（POP 返信）

特定のメール通知では、ユーザーがメールで返信し、その返信を Workfront システムのコメント返信として Workfront にコピーすることができます。 Workfront のシステム管理者は、従来、これらの返信を受け取るために独自の POP メールサーバーを指定するか、ビルトインの Workfront 返信システムを使用するかを選択できました。 20.3 リリースでは、カスタム POP メールサーバーの選択が削除されます。 カスタムサーバーを使用するように設定されているすべてのアカウントは、ネイティブの Workfront メール返信システムを使用するように自動的に移行されます。 システム管理者やその他の Workfront ユーザーに対して必要なアクションはありません。

Workfront Proof システムから直接送信されるメールは変更されません。 これらのメールは、これまでと同様に引き続き受信します。

その他のご質問やご不明な点は、[Workfront サポートチーム](https://experienceleague.adobe.com/?support-tab=home&lang=ja#support)にお問い合わせください。
