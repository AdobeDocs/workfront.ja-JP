---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: ID プロバイダーの SAML 2.0 メタデータの更新
description: ID プロバイダーで SAML 2.0 メタデータを更新できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# ID プロバイダーの SAML 2.0 メタデータの更新

{{important-admin-console-onboard}}

次の節では、Active Directory フェデレーションサービス (ADFS) を ID プロバイダーとして使用する場合に、Security Assertion Markup Language (SAML) 2.0 メタデータを更新する方法について説明します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ID プロバイダーとして ADFS を使用

SAML 2.0 証明書を更新する前またはそれ以降に、Adobe Workfrontの ADFS メタデータを更新できます。 Workfrontの SAML 2.0 証明書を更新する前に ADFS メタデータを更新する場合は、追加の手順が必要です。

* [ADFS メタデータを更新する](#update-your-adfs-metadata)
* [ADFS メタデータの更新を強制](#force-your-adfs-metadata-to-update)

### ADFS メタデータを更新する {#update-your-adfs-metadata}

ADFS メタデータを自動的に更新するように設定するには、この節の手順を実行します。

デフォルトでは、ADFS は、すべての証明書利用者信頼メタデータに対する更新を自動的に確認するように設定されています。ただし、デフォルトでは、24 時間ごとにのみポーリングが設定されています。 この値は、powershell コマンドで変更できます。

1. ADFS サーバーにログインし、ADFS 管理コンソールを開きます。
1. 左側のパネルで、を展開します。 **ADFS 2.0,** 次に、展開します。 **信頼関係。**

1. 次をクリック： **証明書利用者信託** フォルダー。
1. Workfrontと共に使用するように以前に設定した証明書利用者信頼を選択し、右側のパネルで、**フェデレーションメタデータから更新**.
1. （条件付き）このオプションが淡色表示の場合（既にメタデータファイルを使用して証明書利用者信頼が設定されていたことを意味します）、次の手順を実行します。

   1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

   1. クリック **システム** > **シングルサインオン (SSO)**.

   1. クリック **設定を編集します。**
   1. クリック **設定を編集**&#x200B;を選択し、「 **SAML 2.0** 内 **タイプ** 」ドロップダウンリストから選択できます。

   1. を **メタデータ URL**&#x200B;は次のようになります。

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. ADFS サーバーで、以前に設定した証明書利用者の信頼を右クリックし、 **プロパティ。**
   1. 次をクリック： **監視** 」タブをクリックし、Workfrontからコピーした URL を **証明書利用者のフェデレーションメタデータ URL** フィールドに入力します。

   1. 次のオプションを選択します。 **証明書利用者の監視** および **証明書利用者を自動的に更新**.

   1. クリック **はい。**
   1. Workfrontと共に使用するように以前に設定した証明書利用者信頼を選択します。次に、右側のパネルで、 **フェデレーションメタデータから更新します。**

1. クリック **OK** フェデレーションメタデータ内の一部のコンテンツが ADFS 2.0 でサポートされていないことに関するメッセージを無視する場合。
1. 開く **Windows Powershell モジュール。**
1. すべてのモジュールが読み込まれたら、powershell で次のコマンドを実行します。

   `Get-ADFSProperties`

1. 次の隣の値を探します。 **監視間隔。**

   ポーリング間の分数を表す数値です。 デフォルト値は 1440（1440 分= 24 時間）である必要があります。

1. powershell で次のコマンドを実行して、新しい値を設定します。

   `Set-ADFSProperties -MonitoringInterval 1`

   これにより、監視間隔が 24 時間ごとから 1 分ごとに変更されます。 ポーリング頻度を減らしたい場合は、1 を大きい別の値に変更できます。

1. これが正しく機能していることを確認するには、 **イベントビューア** ADFS 2.0 ログで次の情報を探します。

   **イベント ID 156 および 157**

### ADFS メタデータの更新を強制 {#force-your-adfs-metadata-to-update}

ADFS メタデータを更新するには、次の節の手順を実行します。

Active Directory フェデレーションサービス (ADFS) の使用時に、Workfrontと SAML 2.0 プロバイダー間でメタデータを強制的に交換するには、次の手順を実行します。

>[!NOTE]
>
>これらの変更の一部は、お客様の IT 部門が行う必要がある場合があります。

1. ADFS サーバーにログインし、 **ADFS 管理コンソール**.
1. 左側のパネルで、を展開します。 **ADFS 2.0**&#x200B;を展開し、 **信頼関係**.

1. 次をクリック： **証明書利用者信託** フォルダー。
1. Workfrontと共に使用するように以前に設定した証明書利用者信頼を選択し、右側のパネルで、 **フェデレーションメタデータから更新**.

   このオプションが淡色表示になり、選択できない場合は、次の手順を実行します。

   （このオプションは、メタデータファイルを使用して証明書利用者の信頼が以前に設定された場合にのみ淡色表示になります）。

   1. Workfrontの「設定」領域で、 **メタデータ URL** Workfrontのシングルサインオン設定画面から。

      次の項目の情報にアクセスするには **メタデータ URL**:

      1. クリック **設定** グローバルナビゲーションバーのAdobe Workfrontの右上隅付近
      1. /をクリックします。 **システム** > **シングルサインオン (SSO)**.
      1. クリック **設定を編集します。**
      1. クリック **設定を編集**&#x200B;を選択し、「 **SAML 2.0** 内 **タイプ** 」ドロップダウンリストから選択できます。
      1. を **メタデータ URL**&#x200B;は次のようになります。

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. ADFS サーバーで、以前に設定した証明書利用者の信頼を右クリックし、 **プロパティ。**
   1. 次をクリック： **監視** 」タブをクリックし、Workfrontからコピーした URL を **証明書利用者のフェデレーションメタデータ URL** フィールドに入力します。
   1. 次のオプションを選択します。 **証明書利用者の監視** および **証明書利用者を自動的に更新**.
   1. クリック **OK**.
   1. Workfrontと共に使用するように以前に設定した証明書利用者信頼を選択し、右側のパネルで、 **フェデレーションメタデータから更新します。**


1. クリック **OK** フェデレーションメタデータ内の一部のコンテンツが ADFS 2.0 でサポートされていないことに関するメッセージを無視する場合。
1. クリック **更新** フェデレーションメタデータの更新を完了するには、以下を実行します。

Workfrontログイン資格情報を使用してネイティブログイン画面からWorkfrontにアクセスできるユーザー ( これは、 **アクセス** （セクション）Workfrontのユーザー名とパスワードを使用して、次の URL に移動してログインできます。 `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## 他の ID プロバイダーの使用

ADFS 以外の ID プロバイダー（Ping、Okta、Centrify など）を使用する場合は、Workfrontメタデータを ID プロバイダーに再アップロードする必要があります。

新しいWorkfrontメタデータ URL の取得方法について詳しくは、 [ADFS メタデータを更新する](#update-your-adfs-metadata).

Workfrontでの SAML 2.0 での Active Directory フェデレーションサービス (ADFS) の使用に関する詳細は、 [ADFS を使用した SAML 2.0 でのAdobe Workfrontの設定](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
