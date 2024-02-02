---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: connections-annd-webhooks
title: 更新されたセキュリティ対策を使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続
description: Google は最近、ユーザーによる API の使用方法に関する制限を導入しました。この記事では、これらの更新セキュリティ対策を考慮しつつ、 [!DNL Adobe Workfront Fusion]  を Google に接続する方法について説明します。
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '669'
ht-degree: 100%

---

# 更新されたセキュリティ対策を使用して [!DNL Adobe Workfront Fusion] を [!DNL Google Services] に接続

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select]または[!UICONTROL Prime]の [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Google Services] 制限

[!DNL Google] は、2020年6月1日（PT）に、ユーザーが API を使用する方法に関する制限を導入しました。これらのセキュリティ対策は、[!DNL Google] に関する個人データの漏洩や悪用から [!DNL Google] ユーザーを保護します。制限は、[!DNL Gmail] および [!DNL Google Drive] アプリに関連します。これらの制限について詳しくは、[[!DNL Google] API サービスのユーザーデータポリシー](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)の「特定の API 範囲に関する追加要件」を参照してください。

制限された範囲にアクセスするには、接続されたサービス（[!DNL Adobe Workfront Fusion] または、API を使用してユーザーのデータにアクセスする他のサービス）を検証し、評価証明書を取得して、サービスがデータの使用方法に関して安全で透明性が高いことを証明する必要があります。[!DNL Workfront Fusion] は、制限された範囲へのアクセスに関する [!DNL Google] の要件のすべてを満たしています。ただし、[!DNL Workfront Fusion] のサードパーティの接続されたサービスのほとんどは評価状を持っていないため、[!DNL Google] の条件を満たしていません。そのため、[!DNL Workfront Fusion] は、これらのサービスにデータを送信できません。

## [!DNL Google Services] 制限の例外

評価証明書を持たない未承認のサードパーティサービスが新しい制限に違反することなくデータを送信できるようにする例外措置がいくつかあります。彼らは、[!DNL G Suite] と [!DNL Workfront Fusion] OAuth クライアント、[!DNL G Suite] と別の OAuth クライアント、または [!DNL @gmail.com] と [!DNL @google.mail.com] で異なります。

* [[!DNL G suite] と  [!DNL Workfront Fusion]  OAuth クライアント](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] と別の OAuth クライアント](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] および  [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] と [!DNL Workfront Fusion] OAuth クライアント

[!DNL Workfront Fusion] は [!UICONTROL ドメイン全体のインストール] の例外を使用します。ドメイン全体のインストールは、[!DNL G Suite] ユーザーに適しており、ユーザーは無制限に未承認のサービスを統合できます。G Suite のユーザーは、追加の手順を実行する必要がなく、未承認のサービスに直接接続することができます。

### [!DNL G suite] と別の OAuth クライアント

[!DNL Workfront Fusion] OAuth クライアントを使用する代わりに自分の OAuth クライアントを使用したい [!DNL G Suite] ユーザーは、[!UICONTROL 内部] 使用アプローチ経由で [!DNL Google Services] に接続できます。このオプションは、上級ユーザー向けです。手順について詳しくは、[カスタム OAuth クライアントを使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)を参照してください。

### [!DNL @gmail.com] および [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

[!DNL @gmail.com] または [!DNL @googlemail.com] 経由で [!DNL Google Services] にアクセスするユーザーは、個人使用アプローチ経由で [!DNL Google Services] に接続できます。このオプションは、上級ユーザー向けです。手順について詳しくは、[カスタム OAuth クライアントを使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)を参照してください。

## よくある質問

* [ [!DNL Adobe Workfront Fusion]  のどのアプリが影響を受けますか？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [私は [!DNL G Suite] アカウントを持っていますか？](#do-i-have-a-g-suite-account)
* [私が  [!DNL @gmail.com]  または  [!DNL @googlemail.com]  ユーザーの場合はどうすればよいですか？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [私が [!DNL G Suite] ユーザーの場合はどうすればよいですか？](#what-should-i-do-if-im-a-g-suite-user)

### [!DNL Adobe Workfront Fusion] のどのアプリが影響を受けますか？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive]、[!DNL Gmail] およびメール（[!DNL Gmail] アカウントに接続）。

### 私は [!DNL G Suite] アカウントを持っていますか？ {#do-i-have-a-g-suite-account}

メールアドレスの末尾が [!DNL @gmail.com] または [!DNL @googlemail.com] の場合、アカウントは [!DNL G Suite] アカウントではありません。[!DNL Google] アカウントが @my-company.com などのカスタムドメインで終わる場合は、[!DNL G Suite] アカウントです。

### 私が [!DNL @gmail.com] または [!DNL @googlemail.com] ユーザーの場合はどうすればよいですか？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

これらの新しい制限は、[!DNL Google Drive] または [!DNL Gmail] と統合する場合にのみ適用されます。[!DNL Google Drive] または [!DNL Gmail] を使用する場合、以下のことができます。

* [!DNL G Suite] に切り替える

  または

* カスタム OAuth クライアントを作成。 このオプションは、上級ユーザー向けです。

  手順については、[接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントを使用](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)を参照してください。

[!DNL Google Drive] または [!DNL Gmail] 以外のサービスを統合する場合、これらの制限は適用されません。

他の [!DNL Google Services] を [!DNL Workfront Fusion] に接続する手順については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でシナリオを作成の記事の、[モジュールのアプリまたはウェブサービスを  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) に接続を参照してください。

### 私が [!DNL G Suite] ユーザーの場合はどうすればよいですか？ {#what-should-i-do-if-im-a-g-suite-user}

必要なアクションはありません。
