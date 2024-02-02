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
workflow-type: ht
source-wordcount: '961'
ht-degree: 100%

---

# ID プロバイダーの SAML 2.0 メタデータの更新

{{important-admin-console-onboard}}

次の節では、Active Directory フェデレーションサービス（ADFS）を ID プロバイダーとして使用する場合に、Security Assertion Markup Language（SAML）2.0 メタデータを更新する方法について説明します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ID プロバイダーとして ADFS を使用

SAML 2.0 証明書を更新する前またはそれ以降に、Adobe Workfront の ADFS メタデータを更新できます。Workfront の SAML 2.0 証明書を更新する前に、ADFS メタデータを更新する場合は、追加の手順が必要です。

* [ADFS メタデータを更新](#update-your-adfs-metadata)
* [ADFS メタデータの更新を強制](#force-your-adfs-metadata-to-update)

### ADFS メタデータを更新 {#update-your-adfs-metadata}

ADFS メタデータを自動的に更新するように設定するには、この節の手順を実行します。

デフォルトでは、ADFS は、すべての証明書利用者の信頼メタデータの更新を自動的に確認するように設定されていますが、デフォルトでは 24 時間ごとにのみポーリングするように設定されています。この値は、powershell コマンドで変更できます。

1. ADFS サーバーにログインし、ADFS 管理コンソールを開きます。
1. 左側のパネルで、**ADFS 2.0**、**信頼関係**&#x200B;の順に展開します。

1. **証明書利用者の信頼**&#x200B;フォルダーをクリックします。
1. Workfront と共に使用するように以前に設定した証明書利用者の信頼を選択し、右側のパネルで、「**フェデレーションメタデータから更新**」をクリックします。
1. （条件付き）このオプションがグレー表示の場合（既にメタデータファイルを使用して証明書利用者の信頼が設定されていたことを意味する）、次の手順を実行します。

   1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

   1. **システム**／**シングルサインオン（SSO）**&#x200B;をクリックします。

   1. 「**設定の編集**」をクリックします。
   1. 「**設定を編集**」をクリックし、****&#x200B;ドロップダウンリストを入力内で「**SAML 2.0**」を選択します。

   1. 次にような&#x200B;**メタデータ URL**&#x200B;をコピーします。

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. ADFS サーバーで、以前に設定した証明書利用者の信頼を右クリックし、「**プロパティ**」をクリックします。
   1. 「**監視**」タブをクリックし、Workfront からコピーした URL を&#x200B;**証明書利用者のフェデレーションメタデータ URL**&#x200B;フィールドにペーストします。

   1. 「**証明書利用者の監視**」および「**証明書利用者を自動的に更新**」のオプションをオンにします。

   1. 「**OK**」をクリックします。
   1. Workfront と共に使用するように以前に設定した証明書利用者の信頼を選択し、右側のパネルで、「**フェデレーションメタデータから更新**」をクリックします。

1. 「**OK**」をクリックして、フェデレーションメタデータ内の一部のコンテンツが ADFS 2.0 でサポートされていないことに関するメッセージを無視します。
1. **Windows Powershell モジュール**&#x200B;を開きます。
1. すべてのモジュールが読み込まれたら、powershell で次のコマンドを実行します。

   `Get-ADFSProperties`

1. **監視間隔**&#x200B;の横にある値を探します。

   ポーリング間の分数を表す数値です。デフォルト値は 1440（1440 分= 24 時間）になります。

1. powershell で次のコマンドを実行して、新しい値を設定します。

   `Set-ADFSProperties -MonitoringInterval 1`

   これにより、監視間隔が 24 時間ごとから 1 分ごとに変更されます。ポーリング頻度を減らしたい場合は、1 を大きい別の値に変更できます。

1. これが正しく機能していることを確認するには、**イベントビューアー**&#x200B;を使用して ADFS 2.0 ログで次の情報を探します。

   **イベント ID 156 および 157**

### ADFS メタデータの更新を強制 {#force-your-adfs-metadata-to-update}

ADFS メタデータを更新するには、次の節の手順を実行します。

Active Directory フェデレーションサービス（ADFS）の使用時に、Workfront と SAML 2.0 プロバイダー間でメタデータを強制的に交換するには、次の手順を実行します。

>[!NOTE]
>
>これらの変更の一部は、IT 部門が行う必要がある場合があります。

1. ADFS サーバーにログインし、**ADFS 管理コンソール**&#x200B;を開きます。
1. 左側のパネルで、「**ADFS 2.0**」を展開し、「**信頼関係**」を開きます。

1. **証明書利用者の信頼**&#x200B;フォルダーをクリックします。
1. Workfront と共に使用するように事前に設定した証明書利用者の信頼を選択し、右側のパネルで、「**フェデレーションメタデータから更新**」をクリックします。

   このオプションが淡色表示され、選択できない場合は、次の手順を実行します。

   （このオプションは、メタデータファイルを使用して証明書利用者の信頼が事前に設定された場合にのみ淡色表示になります）。

   1. Workfrontの「設定」領域で、Workfront のシングルサインオン設定画面から&#x200B;**メタデータ URL** をコピーします。

      **メタデータ URL** の項目の情報にアクセスするには、次の手順を実行します。

      1. Adobe Workfront の右上隅付近にあるグローバルナビゲーションバーの「**設定**」をクリックします。
      1. **システム**／**シングルサインオン（SSO）**&#x200B;をクリックします。
      1. 「**設定を編集**」をクリックします。
      1. 「**設定を編集**」をクリックし、**タイプ**&#x200B;ドロップダウンリストから「**SAML 2.0**」を選択します。
      1. 次のような&#x200B;**メタデータ URL** をコピーします。

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. ADFS サーバーで、事前に設定した証明書利用者の信頼を右クリックし、「**プロパティ**」をクリックします。
   1. 「**監視**」タブをクリックし、Workfront からコピーした URL を「**証明書利用者のフェデレーションメタデータ URL**」フィールドにペーストします。
   1. 「**証明書利用者の監視**」および「**証明書利用者の自動更新**」のオプションにチェックを付けます。
   1. 「**OK**」をクリックします。
   1. Workfront と共に使用するように以前設定した証明書利用者の信頼を選択し、右側のパネルで、「**フェデレーションメタデータから更新**」をクリックします。

1. 「**OK**」をクリックして、フェデレーションメタデータ内の一部のコンテンツが ADFS 2.0 でサポートされていないことに関するメッセージを無視します。
1. 「**更新**」をクリックして、フェデレーションメタデータの更新を完了します。

Workfront ログイン資格情報を使用してネイティブログイン画面から Workfront にアクセスできるユーザーは、（これは「**アクセス**」セクションの各ユーザーのプロファイルページから設定できます）`https://<yourdomain>.my.workfront.com/Workfront/login.cmd` の URL に移動して、Workfront ユーザー名とパスワードを使用してログインできます。

## 他の ID プロバイダーの使用

ADFS 以外の ID プロバイダー（Ping、Okta、Centrify など）を使用する場合は、Workfront メタデータを ID プロバイダーに再アップロードする必要があります。

新しい Workfront メタデータ URL の取得方法について詳しくは、[ADFS メタデータの更新](#update-your-adfs-metadata)を参照してください。

Workfront で SAML 2.0 と Active Directory フェデレーションサービス（ADFS）の使用について詳しくは、[ADFS を使用した SAML 2.0 での Adobe Workfront の設定](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)を参照してください。
