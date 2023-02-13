---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF レコード
description: Workfrontの配達確認は、notification@proofing.yourdomain.comなどのWorkfront配達確認用 E メールアドレスからレビュー担当者に E メール通知を送信します。 受信者のメールサーバーがすべてのWorkfront配達確認の E メール通知を信頼できるようにするには、 [!DNL Sender Policy] に接続されたカスタマイズドメインのフレームワーク (SPF) レコード [!DNL Workfront Proof] アカウント（proofing.yourdomain.com など）を使用します。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Workfront Proof SPF レコード

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] は、レビュー担当者に電子メール通知を [!DNL Workfront Proof] 電子メールアドレス (notification@proofing.yourdomain.comなど )。 受信者のメールサーバーがすべての [!DNL Workfront Proof] 電子メール通知の場合は、 [!UICONTROL 送信者ポリシーフレームワーク] (SPF) レコードを使用して、 [!DNL Workfront Proof] アカウント ( 例： **proofing.yourdomain.com**) をクリックします。

SPF レコードを設定するには、プライマリドメインに使用する SPF レコードを含める必要があります。

1. を追加します。 **[!UICONTROL DNS TXT]** 次の値を持つドメインのエントリ：

   `v=spf1 a:mx.proofhq.com -all`

   この設定は、メール管理者または IT 担当者がお手伝いします。

   >[!TIP]
   >
   >無料ツールは、 [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) レビュー [!DNL Workfront] SPF レコード。
