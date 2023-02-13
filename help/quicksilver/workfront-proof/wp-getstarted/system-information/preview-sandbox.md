---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: サンドボックステスト環境のプレビュー — [!DNL Workfront Proof]
description: プレビューサンドボックスは、ライブ環境のレプリカとして機能するテスト環境で、毎週末に [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# サンドボックステスト環境のプレビュー — [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

プレビューサンドボックスは、ライブ環境のレプリカとして機能するテスト環境で、毎週末に [!DNL Workfront Proof].

## プレビューサンドボックスについて

プレビューサンドボックスは、組織のユーザーが実稼動環境に影響を与えることなく、実稼動環境のデータを安全にテストし、操作できる環境の役割を果たします。 トレーニングセッションの実行、新機能のテスト、セットアップ機能の決定に最適です。

また、新しい製品機能は、実稼動環境に配信される前にプレビューサンドボックス環境にアップロードされます。 ユーザーは、実稼動環境での通常のワークフローに影響を与えることなく、そこで新しい機能を試すことができます。

プレビューサンドボックスには、実際の実稼動データが含まれています。 データフローは実稼動からプレビューに行われ、逆では行われません。 毎週末に更新されるので、データは実稼動環境から最大 1 週間遅れる場合があります。 最後の更新時間以降に作成された項目は、次の更新がおこなわれるまで、プレビューサンドボックス環境にあります。

## プレビューサンドボックスへのアクセス

デフォルトでは、システム管理者はプレビューサンドボックス環境にアクセスできます。 この節で説明するように、プレビューサンドボックス環境にアクセスできない場合は、 [!DNL Workfront] 管理者またはアドビのサポートチーム。

* [スタンドアロンとしてのプレビューサンドボックスへのアクセス [!DNL Workfront Proof] 顧客](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [プレビューサンドボックスへの AEM としてのアクセス [!DNL Workfront]+[!DNL Workfront Proof] 顧客](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### スタンドアロンとしてのプレビューサンドボックスへのアクセス [!DNL Workfront Proof] 顧客

1. 次の URL に移動します。  `https://preview.proofhq.com`.
1. プレビュー資格情報を使用してログインします。\
   プレビューの更新後に実稼動環境で変更しない限り、プレビューの資格情報は実稼動環境の資格情報と同じにする必要があります。 ログインは、毎週末に実行される更新が発生した場合にのみ同期されます。 自動的には同期されません。

### プレビューサンドボックスへの AEM としてのアクセス [!DNL Workfront+Workfront] 配達確認顧客

システム管理者は、 [!DNL Workfront Proof] を使用したサンドボックスのプレビュー [!DNL Workfront] インターフェイス。

次の手順で [!DNL Workfront Proof] サンドボックスをプレビュー：

1. にログインします。 [!DNL Workfront] 環境。
1. クリック **[!UICONTROL 設定]** （グローバルナビゲーションバー）
1. クリック **[!UICONTROL システム]** >**[!UICONTROL 環境設定]**.

1. 内 **[!UICONTROL テスト環境]** セクションで、 **[!UICONTROL サンドボックスプレビュー]**.

1. プレビュー資格情報を使用してログインします。\
   プレビューの更新後に実稼動環境で変更しない限り、プレビュー資格情報は実稼動環境の資格情報と同じにする必要があります。 ログインは、更新が発生した場合にのみ同期されます。 自動的には同期されません。
1. 次をクリック： [!DNL Workfront Proof] アイコンをクリックします。\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   この [!DNL Workfront Proof] プレビュー環境が表示されます。

## プレビューサンドボックスからの電子メールの受信

電子メール通知は、 [!DNL Workfront Proof] 環境をプレビューします。
