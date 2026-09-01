---
title: Workfront OAuth2からAdobe Developer Consoleへの移行
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Workfrontの従来のカスタム OAuth2 アプリケーションサービスは廃止されています。 変更点、影響を受けるユーザー、Adobe Developer Consoleにカスタム統合を移行する方法について説明します。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# Workfront OAuth2からAdobe Developer Consoleへの移行

Workfrontの従来のカスタム OAuth2 アプリケーションサービス（**Setup** > **System** > **OAuth2**&#x200B;で設定した統合）は廃止されています。 今後、Workfrontに対して認証を行うすべてのカスタム統合では、代わりにAdobe Developer Console（developer.adobe.com）認証フローを使用する必要があります。

この変更は、Workfrontが発行するOAuth2 クライアント IDとシークレットを使用して現在認証しているカスタムビルドの統合、スクリプト、またはサードパーティツールに影響します。 Workfrontへのログイン方法には影響せず、Adobeが個別に移行するパッケージ化されたMicrosoft TeamsやSlackの統合など、Adobeが管理する標準の統合にも影響しません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront アクセスレベル設定</td> 
   <td><p>システム管理者</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Developer Consoleの権利</td> 
   <td><p>Workfront用Adobe Developer Consoleにアクセスするには、IMS組織の完全な管理者権限が必要です。 これは、Adobe組織全体とその下のすべての製品を管理するため、Workfront製品管理者の役割よりも幅広い役割です。</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## 重要な日付

| 日付 | マイルストーン | アドビにとっての意味 |
|---|---|---|
| 2026年11月1日（PT） | 新しいアプリの作成が無効です | Workfrontで新しいカスタム OAuth2 アプリケーションを作成できなくなりました。 既存のアプリケーションは引き続き機能します。 |
| 2027年2月1日（PT） | 従来のサービスは廃止されました | 既存のカスタム OAuth2 アプリケーションは完全に動作しなくなります。 Adobe Developer Consoleに移行していないインテグレーションは、この時点でWorkfront APIにアクセスできなくなります。 |

>[!IMPORTANT]
>
>2026年11月1日（PT）より前に移行を計画して完了することを強くお勧めします。そのため、統合は中断することなく実行され続けるため、2027年2月1日（PT）のハードデッドラインに移行しないでください。

## 影響を受ける組織

Workfrontの従来のOAuth2設定画面を通じて発行されたカスタム OAuth2 クライアント IDとシークレットを使用してWorkfrontに接続する統合、スクリプト、またはツールがある場合、この変更の影響を受けます。 一般的な例には、次のようなものがあります。

* エンジニアリングチームがWorkfront APIに対して管理するカスタムビルドの統合。
* Workfrontが発行するクライアント IDで設定されたサードパーティ製またはパートナーが構築したコネクタ。 統合がどのように認証されるかわからない場合は、ベンダーに確認することをお勧めします。
* Workfront APIを直接呼び出す社内の自動化、レポート、データ同期スクリプト。

お客様の組織がこれらのアプリケーションを持っているかどうかわからない場合、Workfront管理者は、**Setup** > **System** > **OAuth2**&#x200B;の下にあるOAuth2 アプリケーション リストを確認して、現在登録されているものを確認できます。 詳しくは、[ カスタム OAuth2 アプリケーションの表示と管理](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md)を参照してください。

## Adobe Developer Console認証の種類について

Adobe Developer Consoleは、複数の認証方法をサポートしています。 統合の動作に合ったタイプを選択できます。

* **サーバー間の認証**: バックエンドで実行中のアプリケーションで、組織の代理でAdobe APIを呼び出し、エンドユーザーが関与していない場合。 これは、クライアント IDとシークレットで動作する従来のWorkfront OAuth2 パターンに最も近い一致であり、ほとんどのカスタム Workfront統合、スクリプト、およびオートメーションで使用する必要があるタイプです。
* **User Authentication**: アプリケーションでデータを表示または編集する前に、Adobe ユーザーがログインして同意を付与する必要がある場合。 組織全体ではなく、特定のサインイン済みWorkfront ユーザーの代理として統合機能を実行する必要がある場合は、代わりにこの種類を使用してください。

  ユーザー認証を選択した場合、アプリケーションのアーキテクチャに応じて、さらに3つのオプションがあります。

  * **OAuth Web App**: フロントエンド UIとバックエンド サーバーを持つアプリケーションの場合。 サーバーはクライアントの秘密鍵を安全に保存し、トークンを取得します。
  * **OAuth シングルページアプリ**: バックエンドサーバーを持たないブラウザーのみのweb アプリケーション用。 Web アプリ自体がトークンを取得します。
  * **OAuth ネイティブアプリ**: デバイス上でネイティブに実行され、バックエンドサーバーを持たないモバイルアプリケーションまたはデスクトップアプリケーションの場合。 ネイティブアプリはトークンを取得します。

従来のOAuth2 サービスのバックエンド統合、スクリプト、または自動化を移行するほとんどの組織では、サーバー間の認証が必要です。

## 機能の比較：従来のOAuth2とAdobe Developer Consoleの比較

従来のWorkfront OAuth2 サービス （Fount in **Setup** > **System** > **OAuth2 Applications**）では、3つのアプリケーションタイプが提供され、Workfront インスタンスごとに10個のOAuth2 アプリケーションが制限されます。 ここでは、そうした側面をAdobe Adobe Developer Consoleと比較します。

| 従来のWorkfront タイプ | フロー/認証方法 | Developer Console当量 | フィット |
|---|---|---|---|
| マシンラーニングアプリケーション（CLI、デーモン、バックエンドスクリプト） | 公開鍵と秘密鍵のペアを持つJWT | サーバー間認証 | エンドユーザーを関与させないという目的は同じですが、メカニズムは変わります。 従来のフローでは、公開鍵と秘密鍵のペアとJWTを使用し、サーバー間のフローでは、OAuth クライアント認証情報の付与とともにクライアント IDとクライアントシークレットを使用します。 これはドロップイン資格情報の入れ替えではありません。 統合の認証コードは、資格情報の値だけでなく、変更する必要があります。 詳しくは、[ カスタム OAuth 2 アプリケーションに対するJWT フローの使用](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)を参照してください。 |
| Web アプリケーション（サーバーサイドアプリ：Go、Java、.NET、Node、PHP） | OAuth 2.0認証コードフロー | OAuth Web アプリ（ユーザー認証の下） | 最も近い1:1の一致。 これは同じフローを持ち、バックエンドサーバーがクライアントの秘密鍵を保存するのと同じ基本形状を持ちます。 詳しくは、「[ カスタム OAuth 2 アプリケーションの認証コードフロー](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)」を参照してください。 |
| シングルページ Web アプリケーション（JS、Angular、React、Vue） | PKCEを使用した認証コードフロー、クライアントシークレットなし | OAuth シングルページアプリ（ユーザー認証の下） | 最も近い1:1の一致これは、同じPKCE ベースのシークレットレスフローを持っています。 詳しくは、「[OAuth 2 アプリケーションでのPKCE フローの使用](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md)」を参照してください。 |
| （レガシーに相当するものはありません） | — | OAuth ネイティブアプリ（ユーザー認証の下） | これは新しい機能です。 従来のWorkfront OAuth2には、ネイティブモバイルアプリケーションやデスクトップアプリケーション専用のタイプはありません。 |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## 移行手順

### Workfront System Administratorの場合

>[!NOTE]
>
>Workfront製品の管理者であって、組織管理者ではない場合は、組織管理者と協力して移行を完了するか、移行を依頼する必要があります。

1. [developer.adobe.com](https://developer.adobe.com)にログインし、新しいプロジェクトを作成します。 プロジェクトとは、コンソールが様々な統合やクライアントアプリを整理する方法です。
1. プロジェクトからAPIを追加し、**Adobe Workfront**&#x200B;を選択します。 このAPIは、Experience Cloud カテゴリの下にあります。 プランニング、ワークフロー、レビューと承認を含むあらゆるWorkfront APIは、この1つのAPIを共有します。
1. **サーバー間**&#x200B;認証オプションを選択し、IMS組織に複数のWorkfront インスタンスがある場合は、正しいインスタンスを選択します。

   認証タイプの選択に関するガイダンスについては、この記事の「[Adobe Developer Console認証タイプについて](#understand-adobe-developer-console-authentication-types)」を参照してください。
1. プロジェクト ページで、新しいOAuth サーバー間の資格情報の詳細を開き、クライアント ID、クライアント秘密鍵、およびアクセストークンの生成に必要な情報を見つけます。
1. 統合、スクリプト、またはツールを更新して、古いWorkfront OAuth2 クライアント IDとシークレットの代わりに、これらの新しい資格情報で認証します。
1. Workfrontでのアクセスを確認します。 API クライアントを作成すると、Workfront ユーザー「`techacct`」として自動的に追加されます。 デフォルトでは、アクセスが制限されたコントリビューターとして追加されますが、他のユーザーと同様にアクセスレベルを調整できます。
1. （オプション） `techacct` ユーザー管理者権限を付与するには、テクニカルアカウントの電子メールを、関連する製品プロファイルの管理者としてAdmin Consoleに追加します。
1. エンドツーエンドの統合をテストします。
1. 新しい接続が機能していることを確認したら、Workfrontの古いOAuth2 アプリケーションエントリを廃止します。

完全な手順の詳細とスクリーンショットについては、Adobe Developer Console ドキュメントの[ アクセスの取得](https://developer.adobe.com/workfront-apis/guides/gaining_access/)を参照してください。

### システム管理者でない場合

Adobe Developer Consoleで新しい資格情報を設定するには、そのレベルのアクセスが必要なため、組織のIMS組織管理者をループして移行を完了する必要があります。 統合を管理または管理する場合で、組織のIMS組織管理者が誰であるかを把握している場合は、次のいずれかの連絡を取ります。

* Workfrontのアカウントチーム
* 社内IT チーム
* エンジニアリング担当者

## 移行しない場合

2027年2月1日以降も従来のOAuth2 クライアント ID/シークレット パターンを引き続き使用している統合は、Workfront APIに対する認証ができなくなり、依存するワークフロー、同期、または自動化が失敗します。 この日付を過ぎて拡張が計画されていないので、事前に統合を移行してください。

## よくある質問

**これは、Adobeが提供するパッケージ統合（SlackやMicrosoft Teamsなど）に影響しますか？**

いいえ。 Adobeで管理されているグローバルアプリケーションは、Adobeによって直接移行されるので、ユーザー側での操作は必要ありません。

**2027年2月1日より前に、既存の統合が機能しなくなります。**

いいえ。 既存のカスタム OAuth2 アプリケーションは、2027年2月1日まで引き続き正常に機能します。 新しいカスタム OAuth2 アプリケーションを作成する機能のみが影響を受けます（2026年11月1日以降）。

**移行にかかる費用はありますか？**

いいえ。Adobe Developer Consoleを通じた認証に関連する追加費用は発生しません。

**ヘルプはどこで入手できますか？**

特定の連携やスケジュールについて質問がある場合は、Workfrontのアカウントチームにお問い合わせいただくか、サポートケースを開いてください。 スクリーンショットを使用した公式の最新の設定チュートリアルについては、Adobe Developer Console ドキュメントの[ アクセスの取得](https://developer.adobe.com/workfront-apis/guides/gaining_access/)を参照してください。
