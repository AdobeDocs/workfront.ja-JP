---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'シングルサインオン [!DNL Workfront Proof]:AD FS 構成'
description: AD サーバーの管理者は、AD FS をインストールして構成できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# シングルサインオン [!DNL Workfront Proof]:AD FS の構成

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

AD サーバーの管理者は、AD FS をインストールして構成できます。

## AD FS のインストールと構成

1. ダウンロード [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) をコンピューターに追加します。
1. ダウンロードした AdfsSetup.exe ファイルを開き、ADFS （Active Directory フェデレーションサービス）インストールウィザードを起動します。
1. [ サーバーの役割 ] 画面で、オプションの 1 つを選択します（少なくともフェデレーションサーバーが必要です）。
1. AD サーバー上の IIS をインターネットに公開しない場合（HTTP と HTTPS のポート 80 と 443）、最初にファイアウォールの背後にフェデレーションサーバーを設定し、次に、ファイアウォールを介してフェデレーションサーバーに要求を渡す 2 つ目のフェデレーションサーバープロキシを作成します。
1. AD FS の設定が完了したら、 **[!UICONTROL AD FS 2.0 管理スナップインを開始します]**&#x200B;を選択し、「 **[!UICONTROL 完了]**. これが完了したら、AD FS 2.0 管理ウィンドウがすぐに開きます。 表示されない場合は、次の場所から開くことができます。 **[!UICONTROL 開始]** > **[!UICONTROL 管理ツール]** > **[!UICONTROL AD FS 2.0 管理]**. これは、主な AD FS 制御アプリケーションです。

1. 最初に、[ AD FS 2.0 Federation Server Configuration Wizard ] をクリックします。
AD FS を設定し、IIS 経由でインターネットと AD の両方に接続するのに役立ちます。
1. 新しい AD FS サーバを構成する場合は、[ ] を選択します。 **[!UICONTROL 新しいフェデレーションサービスを作成する]**.
1. 選択 **[!UICONTROL スタンドアロンフェデレーションサーバ]** （テストおよび評価の目的で）。

1. 高可用性と負荷分散を行うには、[ 新しいフェデレーションサーバーファーム ] をクリックします。
1. フェデレーションサービス名を指定します。
デフォルトでは、設定ウィザードは IIS のデフォルト Web サイトにバインドされた SSL 証明書を取得し、そこで指定されたサブジェクト名を使用します。 ワイルドカード証明書を使用する場合は、フェデレーションサービス名を入力する必要があります。
IIS で SSL 証明書が構成されていない場合、構成ウィザードはローカルコンピューターの証明書ストアで有効な証明書を検索します。 これらは、「 SSL 証明書」ドロップダウンに表示されます。 証明書が見つからない場合は、IIS の Server Certificate Generator を使用して証明書を作成できます。

1. 設定を続行し、「 **[!UICONTROL 閉じる]** 完了したら、

## 設定 [!DNL Workfront Proof] シングルサインオン

次の場合、 [!DNL Workfront Proof] 管理者は、 [!DNL Workfront Proof] サイド。 詳しくは、 [シングルサインオン [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. クリック **[!UICONTROL 設定]** > **[!UICONTROL アカウント設定]**&#x200B;をクリックし、 **[!UICONTROL シングルサインオン]** タブをクリックします。

1. 内 **SSO URL** 」ボックスに、エンティティ ID を貼り付けます。
エンティティ ID の例を以下に示します。http://*&lt;adfs.your-company.com>*/adfs/services/trust エンティティ ID は、フェデレーションメタデータ XML ファイルにあります。
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. フェデレーションメタデータは、AD FS 2.0 スナップイン/サービス/エンドポイントフォルダーにあります。 「メタデータ」セクションで、フェデレーションメタデータタイプを持つものを探します。 メタデータを表示するには、このエンドポイントをブラウザーに貼り付けます。 このリンクに直接アクセスすることもできます。https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xmlを、{adfs.your-company.com} を独自の詳細に置き換えた後に追加します。
1. 内 **[!UICONTROL ログイン URL]** ボックスに、SSO ログインを貼り付けます。
1. SSO ログインの例を次に示します。
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. このリンクは、フェデレーションメタデータ XML ファイルにあります。
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. 内 **[!UICONTROL ログアウト URL]** 」ボックスにリンクを入力し、保存します。
次に、ログアウト URL の例を示します。https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. AD FS マネージャー/信頼関係/証明書利用者の信頼 — ProofHQ プロパティに移動します。
   1. エンドポイントの下で、 [!UICONTROL 追加してエントリ] 次の詳細を含む

      * エンドポイントの種類= SAML ログアウト
      * 連結=POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * この手順は、AD FS で証明書利用者信頼（以下を参照）を構成した後に完了できます。
   1. 内 **[!UICONTROL 証明書のフィンガープリント]** ボックスに、証明書のデータを入力します。
   1. ADFS 2.0 スナップインに移動して、[ サービス ] > [ 証明書 ] > [ トークン署名 ] に移動します。
   1. このエントリを右クリックして、証明書を表示します。
   1. 次の [!UICONTROL 証明書の詳細] タブで拇印をコピーし、次の場所に貼り付けます。 **[!UICONTROL Workfront Proof シングルサインオン]** 「設定」タブに表示されます。

   1. 指紋文字はコロンやスペースで区切ることができますが、削除することをお勧めします。 シングルサインオンの設定に問題がある場合は、カスタマーサポートチームにお問い合わせください。


## 証明書利用者信頼の追加

設定が完了したら、AD FS の Relying Party Trusts セクションで作業する必要があります。

1. に移動します。 **[!UICONTROL 信頼関係]** > **[!UICONTROL 証明書利用者信託]** フォルダーを選択し、「 **[!UICONTROL 証明書利用者信頼を追加する]** をクリックして、設定ウィザードを起動します。

1. データソースを選択します。
のすべてのメタデータ [!DNL ProofHQ] アカウントは、次のようなリンクに配置されます。https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phqこれは、ほとんどの証明書利用者信頼を構成します。

   >[!NOTE]
   >
   >* URL からの接続の確立で問題が発生した場合は、メタデータをファイルとして保存し、ファイルからデータを読み込むことを選択します。
   >* 完全なカスタムドメイン (www.your-proofing.comなど ) を [!DNL ProofHQ] アカウントは、「{yoursubdomain}.proofhq.com」部分全体を独自のドメインに置き換えて、 [!DNL ProofHQ] メタデータリンク。



## 要求ルールの構成

証明書利用者信頼構成が完了したら、要求ルールを構成して設定を完了する準備が整いました。 ProofHQ 用に 2 つの要求ルールを設定します。電子メールおよび名前 ID。

1. を開きます。 **[!UICONTROL 要求ルールの編集]** ダイアログボックス
1. に移動します。 **[!UICONTROL ProofHQ 証明書利用者信頼]**&#x200B;を選択し、「 **[!UICONTROL 要求ルールの編集]** (1)\
   信頼の設定の最後でこのオプションを選択した場合は、ポップアップが自動的に開きます。

1. クリック **[!UICONTROL ルールを追加]** (2) をクレーム設定ウィンドウを開きます。

   * 電子メール（LDAP 属性を要求ルール・テンプレートとして送信）
   * NameID （受信要求ルールテンプレートの変換）
