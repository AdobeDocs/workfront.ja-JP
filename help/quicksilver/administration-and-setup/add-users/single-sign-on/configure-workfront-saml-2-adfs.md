---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: ADFS を使用した SAML 2.0 でのAdobe Workfrontの設定
description: SAML 2.0 でWorkfrontに対する認証を有効にできます。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# ADFS を使用した SAML 2.0 でのAdobe Workfrontの設定

{{important-admin-console-onboard}}

Adobe Workfront管理者は、Active Directory フェデレーションサービス (ADFS) の使用中に、シングルサインオン用の Security Assertion Markup Language(SAML)2.0 ソリューションとWorkfrontを統合できます。

このガイドでは、自動プロビジョニングまたは属性マッピングを使用しない ADFS の設定に焦点を当てています。 自動プロビジョニングを設定する前に、設定を完了してテストすることをお勧めします。

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

## SAML 2.0 でのWorkfrontに対する認証の有効化

SAML 2.0 を使用してWorkfront Web アプリケーションとWorkfrontモバイルアプリケーションに対する認証を有効にするには、次の節を完了します。

* [Workfront SSO メタデータファイルの取得](#retrieve-the-workfront-sso-metadata-file)
* [証明書利用者信頼の構成](#configure-relying-party-trusts)
* [要求ルールの構成](#configure-claim-rules)
* [メタデータファイルをアップロードし、接続をテストします。](#upload-the-metadata-file-and-test-the-connection)

### Workfront SSO メタデータファイルの取得 {#retrieve-the-workfront-sso-metadata-file}

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).
1. 左側のパネルで、 **システム** > **シングルサインオン (SSO)**.
1. 内 **タイプ** ドロップダウンメニューで、 **SAML 2.0** をクリックして、追加の情報とオプションを表示します。
1. の後に表示される URL をコピーします。 **メタデータ URL**.
1. 次の節に進みます。 [証明書利用者信頼の構成](#configure-relying-party-trusts).

### 証明書利用者信頼の構成 {#configure-relying-party-trusts}

1. を開きます。 **ADFS マネージャ** Windows Server 2008 R2 の使用（バージョンは異なる場合があります）
1. に移動します。 **開始します。**
1. クリック **管理ツール。**
1. クリック **ADFS 2.0 管理**
1. 選択 **ADFS** および展開 **信頼関係**.
1. 右クリック **証明書利用者信託**&#x200B;を選択し、「 **証明書利用者信頼の追加** をクリックして、証明書利用者信頼の追加ウィザードを起動します。
1. 次の **ようこそページ**&#x200B;を選択します。 **開始**.
1. 内 **日付ソースを選択** 「 」セクションで、Workfrontのメタデータ URL を貼り付けます。
1. クリック **次へ**.
1. クリック **OK** をクリックして、警告メッセージを確認します。
1. 内 **表示名を指定** セクションに、 **表示名** および **メモ** 信頼を区別するには、 **次へ**.
1. 選択 **すべてのユーザーがこの証明書利用者にアクセスすることを許可** ( または **なし** 後で設定する場合 )。
1. クリック **次へ**.

   これにより、 **信頼の追加準備完了** 」セクションに入力します。

1. 次の節に進みます。 [要求ルールの構成](#configure-claim-rules).

### 要求ルールの構成 {#configure-claim-rules}

1. クリック **次へ** 内 **信頼の追加準備完了** セクションで、 **[ 要求ルールの編集 ] ダイアログボックスを開きます** 」オプションが選択されている。

   これにより、後のステップで要求ルールを編集できます。

1. 「**閉じる**」をクリックします。
1. クリック **ルールを追加します。**
1. 選択 **LDAP 属性を要求として送信**.
1. クリック **次へ** 表示する **要求ルールの構成** 手順
1. 要求ルールを構成するには、次の最小要件を指定します。( これは **フェデレーション ID** を使用して、誰がログインしているかを区別します。)


   <table >                
      <tbody>
            <tr>
               <td>要求ルール名
               </td>
               <td>要求ルールの名前を指定します。 例：「Workfront」</td>
            </tr>
            <tr>
               <td>属性ストア</td>
               <td >選択 <b>Active Directory</b> を選択します。</td>
            </tr>
            <tr>
               <td>LDAP 属性</td>
               <td>任意のタイプの属性を指定できます。 次を使用することをお勧めします。 <b>SAM-Account-Name</b> （この属性）。</td>
            </tr>
            <tr>
               <td>送信する要求の種類</td>
               <td>次を選択する必要があります。 <b>名前 ID</b> 発信する要求のタイプとして</td>
            </tr>
      </tbody>
   </table>

1. （オプション）自動プロビジョニングを確立するには、「LDAP 属性」と「送信要求タイプ」の両方に次の要求を追加します。

   * 名
   * 姓
   * 電子メールアドレス

1. クリック **完了**&#x200B;を選択し、「 **OK** 次の画面で
1. 新しい **証明書利用者信頼**&#x200B;を選択し、「 **プロパティ**.
1. を選択します。**「詳細」タブ**. およびの下 **Secure Hash Algorithm** 「SHA-1」または「SHA-256」を選択します。

   >[!NOTE]
   >
   >「Secure Hash Algorithm」で選択するオプションは、「設定」>「システム」>「シングルサインオン (SSO)」の「Workfront」の「Secure Hash Algorithm」フィールドと一致する必要があります。

1. 次の節に進みます。 [メタデータファイルをアップロードし、接続をテストします。](#upload-the-metadata-file-and-test-the-connection).

### メタデータファイルをアップロードし、接続をテストします。 {#upload-the-metadata-file-and-test-the-connection}

1. ブラウザーを開き、に移動します。 `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   メタデータファイル FederationMetadata.xml ファイルをダウンロードする必要があります。

1. クリック **ファイルを選択** under **ID プロバイダーメタデータからのフィールドの入力**&#x200B;をクリックし、 **FederationMetadata.xml** ファイル。

1. （オプション）証明書の情報にメタデータファイルが設定されていない場合は、ファイルを個別にアップロードできます。 選択 **ファイルを選択** 内 **証明書** 」セクションに入力します。

1. クリック **接続をテスト**. 正しく設定すると、次のようなページが表示されます。

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >属性マッピングを設定する場合は、「接続をテスト」から「ディレクトリ属性」に属性をコピーします。 詳細は、「ユーザー属性のマッピング」を参照してください。

1. 選択 **管理の除外** :Workfront管理者がバイパス url を持つWorkfront資格情報を使用してログインできるようにします。

   を指すブックマーク `<yourdomain>`.my.workfront.com/loginリダイレクトをバイパスします。

1. を選択します。 **有効にする** ボックスを使用して設定を有効にします。
1. 「**保存**」をクリックします。

## SSO のユーザーの更新について

このガイドに従って、 **SSO ユーザー名** 彼らの **Active Directory ユーザー名**.

Workfront管理者は、SSO 用にユーザーを一括更新できます。 SSO のユーザーの更新の詳細は、 [シングルサインオンのユーザーを更新](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Workfront管理者は、ユーザーのプロファイルを編集するフェデレーション ID を手動で割り当て、「フェデレーション ID 」フィールドに入力することもできます。 ユーザーの編集について詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>ユーザーのプロファイルを編集してフェデレーション ID を含める場合は、「 」を選択します。 **SAML 2.0 認証のみを許可** バイパス url(`<yourdomain>`.my.workfront.com/login) です。
