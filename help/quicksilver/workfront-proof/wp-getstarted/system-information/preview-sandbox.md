---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: サンドボックステスト環境のプレビュー -  [!DNL Workfront Proof]
description: プレビューサンドボックスは、ライブ環境のレプリカとして機能するテスト環境で、 [!DNL Workfront Proof] によって毎週末にアップデートされます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: ht
source-wordcount: '436'
ht-degree: 100%

---

# サンドボックステスト環境のプレビュー - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

プレビューサンドボックスは、ライブ環境のレプリカとして機能するテスト環境で、[!DNL Workfront Proof] によって毎週末に更新されます。

## プレビューサンドボックスについて

プレビューサンドボックスは、組織のユーザーが実稼動環境に影響を与えることなく、実稼動環境のデータを安全にテストし、操作できる環境の役割を果たします。トレーニングセッションの実行、新機能のテスト、セットアップ機能の決定に最適です。

また、新しい製品機能は、実稼動環境に配信される前にプレビューサンドボックス環境にアップロードされます。ユーザーは、実稼動環境での通常のワークフローに影響を与えることなく、この環境で新しい機能を試すことができます。

プレビューサンドボックスには、実際の実稼動データが含まれています。データフローは実稼動からプレビューに行われ、逆では行われません。毎週末に更新されるので、データは実稼動環境から最大 1 週間遅れる場合があります。最後の更新時間以降に作成された項目は、次の更新が行われるまで、プレビューサンドボックス環境にあります。

## プレビューサンドボックスへのアクセス

デフォルトでは、システム管理者はプレビューサンドボックス環境にアクセスできます。この節で説明するように、プレビューサンドボックス環境にアクセスできない場合は、[!DNL Workfront] 管理者またはアドビのサポートチームにお問い合わせください。

* [スタンドアロンの  [!DNL Workfront Proof]  顧客としてプレビューサンドボックスにアクセスする](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [ [!DNL Workfront]+[!DNL Workfront Proof]  顧客としてプレビューサンドボックスにアクセスする](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### スタンドアロンの [!DNL Workfront Proof] 顧客としてプレビューサンドボックスにアクセスする

1. 次の URL に移動：`https://preview.proofhq.com`
1. プレビューの資格情報を使用してログインします。\
   プレビューのアップデート後に実稼動環境で変更しない限り、プレビューの資格情報は実稼動環境の資格情報と同じにする必要があります。ログインは、毎週末に実行されるアップデートが発生した場合にのみ同期されます。自動的には同期されません。

### [!DNL Workfront+Workfront] Proof の顧客としてプレビューサンドボックスにアクセスする

システム管理者は、[!DNL Workfront] のインターフェイスを介して [!DNL Workfront Proof] プレビューサンドボックスにアクセスできます。

次の手順で [!DNL Workfront Proof] プレビューサンドボックスにアクセスします。

1. [!DNL Workfront] 環境にログインします。
1. グローバルナビゲーションバーで「**[!UICONTROL 設定]**」をクリックします。
1. **[!UICONTROL システム]**／**[!UICONTROL 環境設定]**&#x200B;をクリックします。

1. Adobe Analytics の「**[!UICONTROL テスト環境]**」セクションで「**[!UICONTROL サンドボックスプレビュー]**」をクリックします。

1. プレビュー資格情報を使用してログインします。\
   プレビューのアップデート後に実稼動環境で変更しない限り、プレビュー資格情報は実稼動環境の資格情報と同じにする必要があります。ログインは、アップデートが発生した場合にのみ同期されます。自動的には同期されません。
1. グローバルナビゲーションバーで [!DNL Workfront Proof] アイコンをクリックします。\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   [!DNL Workfront Proof] プレビュー環境が表示されます。

## プレビューサンドボックスからのメールを受信

[!DNL Workfront Proof] プレビュー環境からメール通知が送られることはありません。
