---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF レコード
description: Workfront Proof は、notification@proofing.yourdomain.com などの Workfront Proof メールアドレスからレビュアーにメール通知を送信します。 受信者のメールサーバーがすべての Workfront Proof メール通知を信頼していることを確認するには、 [!DNL Workfront Proof]  アカウント（例：proofing.yourdomain.com）に接続されているカスタマイズされたドメインの  [!DNL Sender Policy]  フレームワーク（SPF）レコードを設定する必要があります。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
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
source-wordcount: 181
ht-degree: 100%

---

# Workfront Proof SPF レコード

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。 [!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

[!DNL Workfront Proof] は、notification@proofing.yourdomain.com などの [!DNL Workfront Proof] メールアドレスからレビュアーにメール通知を送信します。 受信者のメールサーバーがすべての [!DNL Workfront Proof] メール通知を信頼していることを確認するには、[!DNL Workfront Proof] アカウント（例：**proofing.yourdomain.com**）に接続されているカスタマイズされたドメインの[!UICONTROL 送信者ポリシーフレームワーク]（SPF）レコードを設定する必要があります。

SPF レコードを設定するには、プライマリドメインに使用する SPF レコードを含める必要があります。

1. 次の値を使用して、ドメインの **[!UICONTROL DNS TXT]** エントリを追加します。

   `v=spf1 a:mx.proofhq.com -all`

   メール管理者または IT 担当者がこの設定をお手伝いします。

   >[!TIP]
   >
   >[[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) にある無料のツールを使って、[!DNL Workfront] SPF レコードを確認することができます。
