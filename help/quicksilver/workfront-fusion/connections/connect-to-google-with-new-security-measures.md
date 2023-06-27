---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: connections-annd-webhooks
title: 接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] 最新のセキュリティ対策を採用
description: Googleは最近、ユーザーが API を使用する方法に関する制限を導入しました。 この記事では、接続方法について説明します [!DNL Adobe Workfront Fusion] Googleへの移行（これらの更新セキュリティ対策を考慮）
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# 接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] 最新のセキュリティ対策を採用

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] 制限

[!DNL Google] では、2020 年 6 月 1 日現在、ユーザーが API を使用する方法に関する制限を導入しています。 これらのセキュリティ対策は、 [!DNL Google] ～に関する個人データの漏洩や悪用からの利用者 [!DNL Google]. 制限は、 [!DNL Gmail] および [!DNL Google Drive] アプリ これらの制限の詳細については、 [[!DNL Google] API サービスのユーザーデータポリシー](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

制限されたスコープにアクセスするには、接続されたサービス ([!DNL Adobe Workfront Fusion] または、API を使用してユーザーのデータにアクセスする他のサービスを検証し、評価状を持って、サービスがデータの使用方法に関して安全で透明性が高いことを証明する必要があります。 [!DNL Workfront Fusion] すべてに従う [!DNL Google]制限されたスコープへのアクセスに関するの要件。 ただし、 [!DNL Workfront Fusion] 査定状を持っていないため、準拠していません [!DNL Google] キーワード。 そのため [!DNL Workfront Fusion] は、これらのサービスにデータを送信できません。

## 例外 [!DNL Google Services] 制限

評価書を持たない未承認のサードパーティサービスに対して、新しい制限に違反することなくデータを送信できる例外がいくつかあります。 彼らは [!DNL G Suite] と [!DNL Workfront Fusion] OAuth クライアント [!DNL G Suite] 別の OAuth クライアントとの間、または [!DNL @gmail.com] および [!DNL @google.mail.com].

* [[!DNL G suite] と [!DNL Workfront Fusion] OAuth クライアント](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] を別の OAuth クライアントと共に使用](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] および [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] と [!DNL Workfront Fusion] OAuth クライアント

[!DNL Workfront Fusion] は [!UICONTROL ドメイン全体のインストール] 例外です。 ドメイン全体のインストールは、 [!DNL G Suite] ユーザーおよびを使用すると、ユーザーは無制限に未承認のサービスを統合できます。 G Suite のユーザーは、追加の手順を実行する必要がなく、未承認のサービスに直接接続することができます。

### [!DNL G suite] 別の OAuth クライアントと

[!DNL G Suite] を使用する代わりに独自の OAuth クライアントを使用するユーザー [!DNL Workfront Fusion] OAuth クライアントは次に接続できます： [!DNL Google Services] から [!UICONTROL 内部] アプローチを使用します。 このオプションは、上級のユーザー向けです。 手順については、 [接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] および [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

アクセスするユーザー [!DNL Google Services] 経由 [!DNL @gmail.com] または [!DNL @googlemail.com] 接続可能 [!DNL Google Services] 個人使用のアプローチを通じて このオプションは、上級のユーザー向けです。 手順については、 [接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQ

* [のアプリ [!DNL Adobe Workfront Fusion] 影響を受ける？](#what-apps-in-adobe-workfront-fusion-are-affected)
* [[!DNL G Suite] アカウントをお持ちですか？](#do-i-have-a-g-suite-account)
* [自分が [!DNL @gmail.com] または [!DNL @googlemail.com] ユーザー？](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [[!DNL G Suite] ユーザーの場合はどうすればよいですか？](#what-should-i-do-if-im-a-g-suite-user)

### のアプリ [!DNL Adobe Workfront Fusion] 影響を受ける？ {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]、および E メール ( 接続先 [!DNL Gmail] アカウント )。

### 次をお持ちですか？ [!DNL G Suite] アカウント？ {#do-i-have-a-g-suite-account}

電子メールアドレスが [!DNL @gmail.com] または [!DNL @googlemail.com] アカウントが [!DNL G Suite] アカウント 次に、 [!DNL Google] アカウントが@my-company.com などのカスタムドメインで終わる場合は、 [!DNL G Suite] アカウント

### 自分が [!DNL @gmail.com] または [!DNL @googlemail.com] ユーザー？ {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

これらの新しい制限は、 [!DNL Google Drive] または [!DNL Gmail]. 接続先 [!DNL Google Drive] または [!DNL Gmail]、

* 切り替え先 [!DNL G Suite]

  または

* カスタム OAuth クライアントを作成します。 このオプションは、上級のユーザー向けです。

  手順については、 [接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

次以外のサービスを統合する場合： [!DNL Google Drive] または [!DNL Gmail]の場合、これらの制限は適用されません。

他の [!DNL Google Services] から [!DNL Workfront Fusion]を参照してください。 [モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 記事内 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 自分が [!DNL G Suite] ユーザー？ {#what-should-i-do-if-im-a-g-suite-user}

必要なアクションはありません。
