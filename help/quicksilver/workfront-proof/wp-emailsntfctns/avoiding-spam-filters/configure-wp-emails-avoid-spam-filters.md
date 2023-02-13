---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 設定 [!DNL Workfront Proof] スパムフィルターを避けるための E メール
description: 「E メールクライアントのスパムフィルターは、重要な目的の 1 つです。迷惑で、場合によっては悪意のあるスパムメールからユーザーを保護する。 しかし、スパムフィルターに正しい設定がない場合、次の重要な情報が表示されない可能性があります [!DNL Workfront Proof] メール：配達確認用の E メール通知、ニュースレター、特別な通信。"
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 設定 [!DNL Workfront Proof] スパムフィルターを避けるための E メール

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

E メールクライアントのスパムフィルターは、重要な目的の 1 つです。迷惑で、場合によっては悪意のあるスパムメールからユーザーを保護する。 しかし、スパムフィルターに正しい設定がない場合、次の重要な情報が表示されない可能性があります [!DNL Workfront Proof] メール：配達確認用の電子メール通知、ニュースレターおよび特別な通信。

次の手順で [!DNL Workfront Proof] メールは常にスパムフォルダーではなく受信ボックスに転送されます。メールに次の内容を追加する必要があり許可リストます。

* [!DNL Workfront Proof] メールサーバ： **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL から]&quot;メールアドレス ( 例：notification@proofhq.com)

に追加する URL について詳しくは、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 記事内 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL から]&quot;件のメールアドレス

電子メールクライアントのタイプに応じて、 [!DNL Workfront Proof] &quot;[!UICONTROL から]「スパムフィルターが将来メールをスパムフォルダーにルーティングするのを防ぐために、次のいずれかの電子メールアドレスを使用します。

* 連絡先リスト
* お使いの [!UICONTROL 差出人セーフ] リスト
* これらのアドレスからインボックスに E メールを配信するために作成するフィルター

既存の [!DNL Workfront Proof] スパムフォルダーからの電子メールと、「[!UICONTROL から]「アドレスがブロック済みアドレス一覧にあります。 このヘルプページには、 [!DNL Workfront Proof] &quot;[!UICONTROL から]「アドレス」とは、次の E メールクライアントでスパムフィルターに追加する方法を示しています。

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>ここで説明する手順に関してご質問がある場合は、電子メールクライアントのヘルプを確認してください。

詳しくは、 [一般的な E メールクライアントのスパム設定](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## この [!DNL Workfront Proof] &quot;[!UICONTROL から]&quot;コピーするメールアドレス

次の手順で [!DNL Workfront Proof] メールがインボックスに届くには、2 つ追加する必要があります [!DNL Workfront Proof] e メールアドレスは、e メールクライアントのスパムフィルターとは別に、

* 一般的なサポートアドレス [!DNL support@proofhq.com]( [!DNL Workfront Proof] 多数の電子メール通信を送信
* 通知アドレス [!DNL Workfront Proof] 配達確認の作成者および配達確認へのリンクを含むレビュー担当者に配達確認通知 E メールを送信します。 これは、一般的なアドレス、notification@support.proofhq.com、またはカスタマイズされたサブドメインまたはホワイトラベルドメインがある場合の特定のアドレスです。

追加するには [!DNL Workfront Proof] &quot;[!UICONTROL から]&#39;&#39;アドレスをメールクライアントのフィルターに追加します：

1. 一般をコピー [!DNL Workfront Proof] サポート&quot;[!UICONTROL から]「電子メールアドレス (support@proofhq.com) 」と入力し、電子メールクライアントに指定されたフィールドに貼り付けます。
1. 次のいずれかの適切なをコピーします。 [!DNL Workfront Proof] &quot;[!UICONTROL から]»電子メールアドレスを入力し、電子メールクライアントに指定されたフィールドに個別に貼り付けます。

   * notification@support.proofhq.comカスタマイズされたサブドメインまたはホワイトラベルドメインがない場合
   * カスタマイズされたサブドメインがある場合はnotification@yoursubdomain.proofhq.comこのアドレスにサブドメイン名を置き換える
   * notification@yoursubdomain.yourdomain.com白いラベルのドメインがある場合；このアドレスにサブドメイン名とドメイン名を置き換えてください

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
