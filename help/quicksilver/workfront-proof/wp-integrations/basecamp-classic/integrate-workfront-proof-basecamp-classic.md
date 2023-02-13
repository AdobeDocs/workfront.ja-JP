---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: 統合 [!DNL Workfront Proof] Basecamp Classic を使用
description: 次を使用する場合、 [!DNL Basecamp] プロジェクト管理では、 [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# 統合 [!DNL Workfront Proof] と [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

次を使用する場合、 [!DNL Basecamp] プロジェクト管理では、 [!DNL Workfront Proof].

## について [!DNL Basecamp] との統合 [!DNL Workfront]

との統合 [!DNL Basecamp] ユーザーは、 [!DNL Basecamp]. ユーザーは配達確認を [!DNL Workfront Proof] アカウントを使用して、 [!DNL Basecamp] プロジェクト。 レビュー担当者が [校正ビューアで配達確認を決定する](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) 経由 [!DNL Basecamp]:Basecamp メッセージに埋め込まれたミニ配達確認を使用します。

と統合されている場合 [!DNL Workfront Proof], [!DNL Basecamp] では、ユーザーは配達確認を使用して次の操作を実行できます。

* ユーザーは、 [!DNL Basecamp Classic].
* ユーザーは、すぐに使用できるレビューツールを持っています。
* プロジェクトレビューチームは、 [!DNL Basecamp] レビューおよび承認用のミニ配達確認を含む
* ユーザーは、レビューと承認のために、完全なページの配達確認に切り替えることができます。
* ユーザーは、ミニサイズとフルサイズの両方の配達確認にコメントとマークアップを追加できます。

   >[!NOTE]
   >
   >コメントの返信後は、コメントの編集や削除はできません。

* レビュー担当者は、他のレビュー担当者が作成したマークアップに応答できます。
* 新しいバージョンの配達確認が使用可能になると、ユーザーに警告が表示されます。
* 以下でないユーザー [!DNL Workfront Proof] ユーザーは、 [!DNL Basecamp].

の統合 [!DNL Workfront Proof] と [!DNL Basecamp] は次の 2 つのレベルで設定する必要があります。

* 設定 [!DNL Basecamp] in [アカウント設定：](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) これにより、組織全体で Basecamp 統合が有効になります。
* 詳しくは、 [の有効化 [!DNL Basecamp] との統合 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* 設定 [!DNL Basecamp] in [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):これにより、配達確認の作成者と所有者が自分の個人情報に接続できるようになります [!DNL Basecamp] アカウントおよび承認 [!DNL Workfront Proof] にアクセスします。 詳しくは、 [個人設定の指定](#configuring-personal-settings).

統合可能な [!DNL Workfront] どちらか [!DNL Basecamp] または [!DNL Basecamp Classic]. の各バージョン [!DNL Basecamp] は異なる API を使用しているので、異なる設定手順が必要です。

設定に関する情報 [!DNL Basecamp Classic]を参照してください。 [の有効化 [!DNL Basecamp] との統合 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) 」を参照してください。

設定に関する情報 [!DNL Basecamp]を参照してください。 [統合 [!DNL Workfront Proof] と [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## の有効化 [!DNL Basecamp] との統合 [!DNL Workfront Proof]

As a [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) または [の配達確認権限プロファイル [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)の場合、 [アカウント設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. に移動します。 [アカウント設定。](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. を開きます。 **[!UICONTROL 統合]** 」タブ (1) をクリックします。
1. Basecamp 統合を有効にするには、 **[!UICONTROL 有効にする]** (2)
1. 確認する [!DNL Basecamp Classic] は、(3) と統合しているバージョンです。
1. （条件付き） [!DNL Basecamp] URL が (4) 表示されたら、 **[!UICONTROL 編集]** をクリックし、 [!DNL Basecamp] アカウント (http://を除く ) を使用します。
1. クリック **[!UICONTROL 保存]** (5)\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. （オプション） [!DNL Basecamp] にログインした後のブラウザー内の URL [!DNL Basecamp Classic] アカウント (6)

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   統合後 [!DNL Workfront Proof] と [!DNL Basecamp]を設定しない場合、ユーザーは個人設定を指定できます。 個人設定の設定について詳しくは、 [個人設定の指定](#configuring-personal-settings).

   を有効にできない場合は、 [!DNL Basecamp] 統合、 [!DNL Workfront Proof] アカウント ID が、 [!DNL Basecamp].

## 個人設定の指定

設定後 [アカウント設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 組織の場合、配達確認を作成または送信する各作成者が、  [個人設定。](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>以下の手順を実行すると、 [!DNL Basecamp] 1 つのブラウザーウィンドウでセッションを開き、 [!DNL Workfront Proof] セッションは別のウィンドウで開きます。

* [の取得 [!DNL Basecamp] API トークン](#retrieving-your-basecamp-api-token)
* [の追加 [!DNL Basecamp] 個人設定への API トークン](#adding-your-basecamp-api-token-to-your-personal-settings)

### の取得 [!DNL Basecamp] API トークン

個々のレベルで統合を完了するには、 [!DNL Workfront Proof]、ユーザーには [!DNL Basecamp] API

次の手順で [!DNL Basecamp] API トークン：

1. ログイン先 [!DNL Basecamp] アカウント
1. クリック **[!UICONTROL マイ情報]** (1) をクリックします。\
   この [!UICONTROL マイ情報] ページが表示されます。\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. 内 [!UICONTROL 認証トークン] セクションで、 **[!UICONTROL トークンを表示]** (2) 個人認証トークンを表示します。
1. を選択します。 **[!UICONTROL フィードリーダー用のトークン]** または **[!UICONTROL Basecamp API]** (3) 次に、トークンをクリップボードにコピーします。

1. を貼り付けます。 [!DNL Basecamp] API トークンを [!UICONTROL フィードリーダー用のトークン] または [!UICONTROL Basecamp API] ボックス\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### の追加 [!DNL Basecamp] 個人設定への API トークン

を貼り付けるには、以下を実行します。 [!DNL Basecamp] API トークンを [!DNL Workfront Proof] [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. 次に移動： [[!UICONTROL 統合]  — ユーザー設定](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) の [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1)\
   管理者が最初に [!DNL Basecamp Classic] の統合を使用して、個人設定を有効にすることができます。 統合の設定について詳しくは、 [の有効化 [!DNL Basecamp] との統合 [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) 」を参照してください。

1. 内 [!DNL Basecamp] API トークンボックス (2)、 [!DNL Basecamp] [!UICONTROL マイ情報] ページをフィールド (3) に挿入します。\
   コピーに関する情報 [!DNL Basecamp] API トークン（を参照） [の取得 [!DNL Basecamp] API トークン](#retrieving-your-basecamp-api-token) 」を参照してください。

1. クリック **[!UICONTROL 保存]** (4)

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

お使いの [!DNL Workfront Proof] [個人設定](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) は、 [!DNL Basecamp Classic] アカウント
