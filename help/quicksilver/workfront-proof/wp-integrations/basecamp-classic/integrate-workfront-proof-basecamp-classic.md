---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: ' [!DNL Workfront Proof]  を Basecamp Classic と統合'
description: プロジェクト管理用の  [!DNL Basecamp]  を使用する場合は、 [!DNL Workfront Proof] を使用して、プロジェクトチームにより豊富なレビューと承認ツールを提供できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: ht
source-wordcount: '770'
ht-degree: 100%

---

# [!DNL Workfront Proof] を [!DNL Basecamp Classic] と統合

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

プロジェクト管理用に [!DNL Basecamp] を使用する場合は、[!DNL Workfront Proof] を使用して、プロジェクトチームにより豊富なレビューと承認ツールを提供できます。

## [!DNL Workfront] との [!DNL Basecamp] 統合について

[!DNL Basecamp] との統合により、ユーザーは、[!DNL Basecamp] 内でプルーフの表示、レビュー、承認を行うことができます。ユーザーはプルーフを [!DNL Workfront Proof] アカウントに送信し、それらを [!DNL Basecamp] プロジェクトと接続できます。レビュアーは、Basecamp メッセージに埋め込まれたミニプルーフを使用して、[!DNL Basecamp] 経由で[プルーフビューアでプルーフを決定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を作成できます。

[!DNL Workfront Proof] と統合されている場合、[!DNL Basecamp] では、ユーザーはプルーフを使用して次の操作を実行できます。

* ユーザーは、[!DNL Basecamp Classic] 内のプルーフをレビューし、承認できます。
* ユーザーにはいつでも使用できるレビューツールが用意されます。
* プロジェクトレビューチームがレビューと承認用のミニプルーフを使用して [!DNL Basecamp] 内のメッセージを受け取ります。
* ユーザーは、フルページのプルーフに切り替えてレビューや承認を行うことができます。
* ユーザーは、ミニサイズとフルサイズの両方のプルーフにコメントやマークアップを追加できます。

  >[!NOTE]
  >
  >コメントの返信後に、コメントの編集や削除を行うことはできません。

* レビュアーは、他のレビュアーが作成したマークアップに応答できます。
* 新しいバージョンのプルーフが使用可能になると、ユーザーに警告が表示されます。
* [!DNL Workfront Proof] ユーザーではないユーザーは、[!DNL Basecamp] でプルーフの作業を行うことができます。

[!DNL Basecamp] との [!DNL Workfront Proof] の統合は、次の 2 つのレベルで設定する必要があります。

* [アカウント設定での [!DNL Basecamp] の設定：](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)これにより、組織全体で Basecamp 統合が有効になります。
* 詳しくは、[ [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) との  [!DNL Basecamp]  統合の有効化を参照してください。
* [個人設定](https://support.workfront.com/hc/ja-jp/sections/115000921168-Personal-settings)での [!DNL Basecamp] の設定：プルーフ作成者と所有者が自分の [!DNL Basecamp] アカウントに接続し、[!DNL Workfront Proof] アクセスを許可できます。詳しくは、[個人設定の指定](#configuring-personal-settings)を参照してください。

[!DNL Basecamp] または [!DNL Basecamp Classic] のどちらかと [!DNL Workfront] を統合できます。[!DNL Basecamp] の各バージョンは、異なる API を使用しているので、異なる設定手順が必要です。

[!DNL Basecamp Classic] の設定について詳しくは、この記事内の[ [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) との  [!DNL Basecamp]  統合の有効化を参照してください。

[!DNL Basecamp] の設定について詳しくは、[ [!DNL Workfront Proof]  と [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md) を統合を参照してください。

## [!DNL Workfront Proof] との [!DNL Basecamp] 統合の有効化

[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) のプルーフ権限プロファイルまたは[ [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) のプルーフ権限プロファイルとして、[アカウント設定](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)でアカウント全体のBasecamp 統合を設定できます。

1. [アカウント設定](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)に移動します。
1. 「**[!UICONTROL 統合]**」タブ（1）を開きます。
1. Basecamp 統合を有効にするには、「**[!UICONTROL 有効化]**」をクリックします。（2）
1. [!DNL Basecamp Classic] は、（3）と統合しているバージョンであることを確認します。
1. （条件付き）[!DNL Basecamp] URL が表示されなかったら（4）、「**[!UICONTROL 編集]**」をクリックし、[!DNL Basecamp] アカウントの URL（http:// を除く）を入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。（5）\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. （オプション）[!DNL Basecamp Classic] アカウントにログインした後にブラウザー内の [!DNL Basecamp] の URL をチェックします（6）。

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   [!DNL Workfront Proof] と [!DNL Basecamp] を統合したら、ユーザーは個人設定を指定できます。個人設定の実行について詳しくは、[個人設定の実行](#configuring-personal-settings)を参照してください。

   [!DNL Basecamp] の統合を有効にできない場合は、[!DNL Workfront Proof]アカウント ID が、[!DNL Basecamp] で使用するアカウント ID と同じではない可能性があります。

## 個人設定の実行

組織の[アカウント設定](https://support.workfront.com/hc/ja-jp/sections/115000912147-Account-settings)を実行した後、プルーフを作成、送信する作成者はそれぞれに、[個人設定](https://support.workfront.com/hc/ja-jp/sections/115000921168-Personal-settings)を実行する必要があります。

>[!NOTE]
>
>次の手順を実行すると容易にできます。[!DNL Basecamp] セッションを 1 つのブラウザーウィンドウで開き、[!DNL Workfront Proof] セッションを別のウィンドウで開きます。

* [ [!DNL Basecamp]  API トークンの取得](#retrieving-your-basecamp-api-token)
* [ [!DNL Basecamp]  個人設定への API トークンの追加](#adding-your-basecamp-api-token-to-your-personal-settings)

### [!DNL Basecamp] API トークンの取得

[!DNL Workfront Proof] 内で個人レベルの統合を完了するには、ユーザーは [!DNL Basecamp] API 用に個人の認証トークンが必要です。

[!DNL Basecamp] API トークンを取得します。

1. [!DNL Basecamp] アカウントにログインします。
1. 画面の右上隅にある&#x200B;**[!UICONTROL ユーザー情報]**（1）をクリックします。\
   [!UICONTROL ユーザー情報]ページが表示されます。\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. [!UICONTROL 認証トークン]セクションで、「**[!UICONTROL トークンを表示]**」（2）をクリックして、個人認証トークンを表示します。
1. **[!UICONTROL フィードリーダー用のトークン]**&#x200B;または **[!UICONTROL Basecamp API]**（3）を選択し、次に、トークンをクリップボードにコピーします。

1. [!DNL Basecamp] API トークンを[!UICONTROL フィードリーダー用のトークン]または [!UICONTROL Basecamp API] のボックスに貼り付けます。\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### 個人設定への [!DNL Basecamp] API トークンの追加

[!DNL Basecamp] APIトークンを [!DNL Workfront Proof] の[個人設定](https://support.workfront.com/hc/ja-jp/sections/115000921168-Personal-settings)に張り付けるには、次の手順に従います。

1. [個人設定](https://support.workfront.com/hc/ja-jp/sections/115000921168-Personal-settings)（1）の[[!UICONTROL 統合] - ユーザー設定](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md)に移動します。\
   管理者は最初に [!DNL Basecamp Classic] の統合を有効にして、個人設定を有効にする必要があります。統合の設定について詳しくは、この記事の [ [!DNL Basecamp]  と  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) の統合の有効化を参照してください。

1. 「[!DNL Basecamp] API トークン」ボックス（2）で、[!DNL Basecamp] の[!UICONTROL 個人情報]ページからコピーしたトークンをフィールド（3）に貼り付けます。\
   [!DNL Basecamp] API トークンのコピーについて詳しくは、[ [!DNL Basecamp]  API トークンの取得](#retrieving-your-basecamp-api-token)を参照してください。

1. 「**[!UICONTROL 保存]**」（4）をクリックします。

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

[!DNL Workfront Proof] の[個人設定](https://support.workfront.com/hc/ja-jp/sections/115000921168-Personal-settings)が [!DNL Basecamp Classic] アカウントと統合されました。
