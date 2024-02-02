---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF レコード
description: Workfront Proof は、notification@proofing.yourdomain.com などの Workfront Proof メールアドレスからレビュアーにメール通知を送信します。受信者のメールサーバーがすべての Workfront Proof メール通知を信頼していることを確認するには、 [!DNL Workfront Proof]  アカウント（例：proofing.yourdomain.com）に接続されているカスタマイズされたドメインの  [!DNL Sender Policy]  フレームワーク（SPF）レコードを設定する必要があります。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: ht
source-wordcount: '181'
ht-degree: 100%

---

# Workfront Proof SPF レコード

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

[!DNL Workfront Proof] は、notification@proofing.yourdomain.com などの [!DNL Workfront Proof] メールアドレスからレビュアーにメール通知を送信します。受信者のメールサーバーがすべての [!DNL Workfront Proof] メール通知を信頼していることを確認するには、[!DNL Workfront Proof] アカウント（例：**proofing.yourdomain.com**）に接続されているカスタマイズされたドメインの[!UICONTROL 送信者ポリシーフレームワーク]（SPF）レコードを設定する必要があります。

SPF レコードを設定するには、プライマリドメインに使用する SPF レコードを含める必要があります。

1. 次の値を使用して、ドメインの **[!UICONTROL DNS TXT]** エントリを追加します。

   `v=spf1 a:mx.proofhq.com -all`

   メール管理者または IT 担当者がこの設定をお手伝いします。

   >[!TIP]
   >
   >[[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) にある無料のツールを使って、[!DNL Workfront] SPF レコードを確認することができます。
