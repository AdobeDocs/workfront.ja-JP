---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: スパムフィルターを回避するための  [!DNL Workfront Proof]  メールの設定
description: メールクライアントのスパムフィルターは、迷惑な、おそらく悪意のあるスパムメールからユーザーを保護するという重要な目的を果たします。 ただし、スパムフィルターに正しい設定が設定されていない場合、プルーフメール通知、ニュースレター、特別なコミュニケーションなどの重要な [!DNL Workfront Proof]  メールが表示されない可能性があります。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
TQID: https://experienceleague.adobe.com/QMtIDexmxDDuKqTg-Z47-lMnQ27zDEdMtwg-8OUe3Uw
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
source-wordcount: 498
ht-degree: 94%

---

# スパムフィルターを回避するための [!DNL Workfront Proof] メールの設定

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。 [!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

メールクライアントのスパムフィルターは、迷惑な、おそらく悪意のあるスパムメールからユーザーを保護するという重要な目的を果たします。 しかし、スパムフィルターの設定が正しくない場合、プルーフメール通知、ニュースレター、特別なお知らせなどの重要な [!DNL Workfront Proof] メールが表示されなくなる可能性があります。

[!DNL Workfront Proof] メールがスパムフォルダーではなく、常にインボックスにルーティングされるようにするには、以下を許可リストに追加する必要があります。

* [!DNL Workfront Proof] メールサーバー：**[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof]「[!UICONTROL 送信者]」のメールアドレス（例：notification@proofhq.com）

許可リストに追加する URL について詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)の記事にある[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

## [!DNL Workfront Proof]「[!UICONTROL 送信者]」のメールアドレス

メールクライアントのタイプによっては、今後スパムフィルタによってメールがスパムフォルダにルーティングされないようにするために、[!DNL Workfront Proof]「[!UICONTROL 送信者]」メールアドレスを以下のいずれかに追加する必要が生じる場合があります。

* 連絡先リスト
* [!UICONTROL 信頼できる送信者]リスト
* これらのアドレスからのメールをインボックスに配信するために作成するフィルター

また、既存の [!DNL Workfront Proof] メールをスパムフォルダーから削除し、「[!UICONTROL 送信者]」アドレスがブロックアドレスリストに含まれているかどうかを確認する必要がある場合もあります。 このヘルプページには、[!DNL Workfront Proof]「[!UICONTROL 送信者]」アドレスがリスト表示され、以下のメールクライアントのスパムフィルターにアドレスを追加する方法が示されています。

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>ここで説明する手順に関して不明点がある場合は、メールクライアントのヘルプを確認してください。

詳しくは、[一般的なメールクライアント向けのスパム設定](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md)を参照してください。

## コピーする [!DNL Workfront Proof]「[!UICONTROL 送信者]」のメールアドレス

[!DNL Workfront Proof] メールがインボックスに確実に届くようにするには、2 つの [!DNL Workfront Proof] メールアドレスをメールクライアントのスパムフィルターに個別に追加する必要があります。

* 一般的なサポートアドレス [!DNL support@proofhq.com]。[!DNL Workfront Proof] はここから多数のメール通信を送信
* 通知アドレス。[!DNL Workfront Proof] はここからプルーフ作成者とレビュアーに、プルーフへのリンクを含むプルーフ通知メールを送信します。 カスタマイズされたサブドメインまたはホワイトラベルドメインがある場合、これは一般的なアドレス、notification@support.proofhq.com、あるいは特定のアドレスになります。

[!DNL Workfront Proof]「[!UICONTROL 送信者]」アドレスをメールクライアントのフィルターに追加するには、以下のように行います。

1. 一般的な [!DNL Workfront Proof] サポートの「[!UICONTROL 送信者]」メールアドレス（support@proofhq.com）をコピーし、メールクライアント向けに指定されたフィールドにペーストします。
1. 次の [!DNL Workfront Proof]「[!UICONTROL 送信者]」メールアドレスのうちの適切なものをコピーし、メールクライアント向けに指定されたフィールドに個別にペーストします。

   * notification@support.proofhq.com（カスタマイズされたサブドメインまたはホワイトラベルドメインがない場合）
   * notification@yoursubdomain.proofhq.com（カスタマイズされたサブドメインがある場合は、このアドレスのサブドメイン名を置き換えてください）
   * notification@yoursubdomain.yourdomain.com（ホワイトラベルドメインがある場合は、このアドレスのサブドメイン名とドメイン名を置き換えてください）

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
