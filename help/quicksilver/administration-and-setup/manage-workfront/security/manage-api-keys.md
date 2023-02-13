---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API キーの管理
description: API セキュリティの脆弱性を最小限に抑えるために、Adobe Workfront管理者は、ユーザーに代わってアプリケーションがWorkfrontにアクセスできるようにするために使用する API キーを管理できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 2%

---

# API キーの管理

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

API セキュリティの脆弱性を最小限に抑えるために、Adobe Workfront管理者は、ユーザーに代わってアプリケーションがWorkfrontにアクセスできるようにするために使用する API キーを管理できます。

現在の管理者 API キーのリセットまたは削除、期限切れに設定、すべてのユーザーの API キーの削除をおこなうことができます。

Workfront API を利用するアプリケーションの例を次に示します。

* ドキュメントの統合 (Dropbox、Google Drive、Workfront DAM など )
* Workfront mobile applications

>[!IMPORTANT]
>
>API キーをリセットまたは削除する場合、Workfrontに再びアクセスできるように、Workfront API を利用し、この API キーを介してWorkfrontに認証するアプリケーションを再設定する必要があります。

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

## Workfront API キー

Workfrontの各ユーザーは一意の API キーを持っています。 このキーは、ユーザーがWorkfront API(Workfrontモバイルアプリやドキュメント統合など ) を利用した統合にアクセスした時点で、ユーザー単位で生成されます。

>[!NOTE]
>
> 実稼動環境で生成した API キーは、週の更新中にプレビュー環境にコピーされます。 プレビュー環境で生成した API キーは、毎週の更新中に実稼動用 API キーで上書きされます。

また、Workfront管理者には固有の API キーが割り当てられています。 アプリケーションで管理者 API キーを使用してWorkfrontにアクセスする場合、そのアプリケーションにはWorkfrontへの管理者アクセス権があります。

## 管理者 API キーを管理

管理者ユーザーアカウントの API キーを生成、リセット、または削除できます。

>[!NOTE]
>
>API を使用して API キーを生成することもできます。 詳しくは、 [イベント購読 API](../../../wf-api/general/event-subs-api.md) セクション [イベント購読 API](../../../wf-api/general/event-subs-api.md).

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム >** **顧客情報。**
1. （条件付き）次のいずれかの操作を実行します。

   API キーを生成するには：内 **API キー設定** セクションで、 **API キーを生成**.

   または\
   API キーをリセットするには：内 **API キー設定** セクションで、 **リセット**&#x200B;を、**リセット。**

   または

   API キーを削除するには：内 **API キー設定** セクションで、 **削除**&#x200B;を、 **削除**.

## 管理者以外のユーザー向けの API キーの生成

Workfront管理者以外の役割を持つユーザーの API キーを生成および管理できます。

>[!NOTE]
>
>組織のWorkfrontインスタンスで「Adobe IMS」が有効になっている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

1. （条件付き）組織がシングルサインオン (SSO) アクセス管理を使用している場合、SSO 認証を必要とするオプションを一時的に無効にします。

   1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

   1. 展開 **システム**&#x200B;を選択し、「 **シングルサインオン (SSO)**.\
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)

   1. SSO 認証が必要なチェックボックスを無効にします。

      例えば、組織が SAML 2.0 を使用している場合は、を無効にします。 **SAML 2.0 認証のみを許可**.

1. ブラウザーのアドレスバーに、次の API 呼び出しを入力します。

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**ユーザー名**&amp;password=**パスワード**&amp;method=PUT

   置換 `<domain>` Workfrontのドメイン名、およびユーザーのWorkfront資格情報を使用したユーザー名とパスワード。

1. （条件付き）手順 1 で SSO 認証を無効にした場合、SSO 認証が必要なオプションを有効にします。

   1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

   1. 展開 **システム**&#x200B;を選択し、「 **シングルサインオン (SSO)**.

   1. SSO メソッドを **タイプ** ドロップダウンメニュー。
   1. SSO 認証が必要なチェックボックスをオンにします。

## API キーの有効期限を設定

API キーは、システム内のすべてのユーザーの有効期限が切れるように設定できます。 ユーザーの API キーの有効期限が切れたら、Workfrontにアクセスするには、Workfront API を使用するアプリケーションに対して再認証する必要があります。 API キーの有効期限が切れる頻度を変更できます。 また、ユーザーのパスワードの有効期限が切れたときに API キーを期限切れにするかどうかを設定することもできます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **顧客情報**.
1. 内 **API キー設定** 領域、 **作成後**, **API キーの有効期限：** ドロップダウンリストから、API キーの有効期限を選択します。

   このオプションを変更すると、変更を加えた時点から新しい期間が開始されます。 例えば、このオプションを *1 か月* から *6 か月*&#x200B;に設定した場合、API キーは変更を加えてから 6 ヶ月で有効期限が切れます。

   デフォルトでは、API キーは毎月期限が切れます。

1. ユーザーのパスワードが期限切れになった時点で期限切れになるように API キーを設定するには、 **ユーザーのパスワードが期限切れになったら API キーを削除する**.

   デフォルトでは、このオプションは選択されていません。

   ユーザーパスワードが失効するように設定する方法については、 [システムセキュリティの環境設定の構成](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. 「**保存**」をクリックします。

## すべてのユーザーの API キーを削除します

Workfrontシステムに関する特定のセキュリティ違反を懸念する場合は、すべてのユーザーの API キーを同時に削除できます。

>[!IMPORTANT]
>
>すべてのユーザーの API キーを削除すると、システム内のすべてのユーザーの API キーがすべて無効になります。 この操作を実行すると、Workfrontで新しい API キーを生成し、すべての統合を更新するまで、Workfrontでのすべての統合が失敗します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **システム**&#x200B;を選択し、「 **顧客情報。**

1. 内 **API キー設定** 領域、クリック **すべての API キーを削除**&#x200B;を選択し、「 **削除** **すべて**.

## X.509 証明書を使用した API ログインの制限

>[!IMPORTANT]
>
>この節で説明する手順は、まだAdobeビジネスプラットフォームに転送されていない組織にのみ適用されます。 組織がWorkfront Business Platform にオンボーディングされている場合、Adobe API を使用してWorkfrontにログインすることはできません。
>
>組織がAdobeビジネスプラットフォームにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

サードパーティアプリケーションは、API を介してWorkfrontと通信できます。 X.509 証明書をWorkfrontにアップロードすることで、Workfrontサイトのセキュリティを強化するために API ログインリクエストを制限するようWorkfrontを設定できます。 有効にしたら、API を介したすべてのログインリクエストには、ユーザー名とパスワードに加えて、クライアント証明書が含まれている必要があります。

>[!NOTE]
>
>組織のWorkfrontインスタンスで「Adobe IMS」が有効になっている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。

* [X.509 証明書の取得](#obtain-the-x-509-certificate)
* [証明書をWorkfrontにアップロード](#upload-the-certificate-to-workfront)
* [API ログイン呼び出しが制限されていることを確認します](#verify-api-login-calls-are-restricted)

### X.509 証明書の取得 {#obtain-the-x-509-certificate}

有効な X.509 証明書を信頼できる証明機関（Verisign など）から取得し、ワークステーションの一時的な場所に配置します。

### 証明書をWorkfrontにアップロード {#upload-the-certificate-to-workfront}

認証局から X.509 証明書を取得したら、Workfrontにアップロードする必要があります。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **システム**&#x200B;を選択し、「 **顧客情報**.

1. 内 **API キー設定** 領域、選択 **X.509 証明書を有効にする**.
1. ワークステーションで、以前にダウンロードした X.509 証明書を参照して選択します。
1. （オプション）「 **詳細を表示** 証明書名の横に、証明書に関する次の詳細が表示されます。

   * 件名の共通名
   * 件名の組織
   * 件名の組織単位
   * 発行者の共通名
   * 発行者の組織
   * 発行者組織の単位
   * シリアル番号
   * 問題の日付
   * 有効期限

1. 「**保存**」をクリックします。

### API ログイン呼び出しが制限されていることを確認します {#verify-api-login-calls-are-restricted}

X.509 証明書を必要とするようにWorkfrontのインスタンスを設定する前に、 `/login` 有効なユーザー名およびパスワードパラメーターを使用するエンドポイント。 sessionID を含む 200 件の応答を受け取ります。

Workfrontのインスタンスの顧客情報ページで X.509 証明書を要件に合わせた後、再度ログインを試みます。 今回は、次のメッセージと共に 500 エラー応答が返されます。「信頼できない要求です。 システム管理者に連絡し、証明書を添付してください。」

X.509 証明書が必要であることを確認したら、証明書の値に apiCertificate の追加パラメーターを設定して、同じログイン要求を実行します。 この操作が正しく実行された場合は、有効な sessionID を含む 200 件の応答を受け取ります。
