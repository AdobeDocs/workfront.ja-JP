---
title: 22.2 統合の強化
description: 22.2 統合の強化
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2 統合の強化

このページでは、プレビュー環境の 2.2 リリースでおこなわれたすべての統合の機能強化について説明します。 これらの機能強化は、実稼動環境で利用できるようになります

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022 年 4 月 4 日の週。

22.2 リリースで使用可能なすべての変更点の一覧については、 [22.2 リリースの概要](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfrontと Anaplan の統合が利用可能に

Workfrontプロジェクトの財務面に関するより柔軟性とインサイトを得るために、Workfrontを Anaplan アカウントと統合できるようになりました。 Workfrontオブジェクトを Anaplan オブジェクトにリンクすると、2 つのアカウント間の情報を自動的に更新し、両方の情報が最新で同一であることを確認できます。 また、Workfrontのアクションに基づいて、Analypan で自動化されたプロセスをトリガー化することもできます（またはその逆も可能です）。

例えば、Analypan でキャンペーンを作成し、そのキャンペーンにリンクされたWorkfrontプロジェクトまたはプログラムを作成できます。 その後、Workfrontで追跡されたコストを Anaplan にアップロードして、キャンペーンのパフォーマンスを確認できます。

Workfrontから Analypan への統合を使用する際に考慮すべきその他のワークフローは次のとおりです。

* 新しいWorkfrontプロジェクトからの Analyplan 予算リクエストの作成
* 新しい Anaplan リスト項目からのWorkfrontプロジェクトの作成
* Workfrontプロジェクトからの Analyplan 仕入先要求の開始

詳しくは、 [Adobe Workfrontとアナプラン](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Workfront forExperience Manager強化コネクタの更新

Workfront forExperience Manager強化コネクタに、次の更新が含まれるようになりました。

* 複数のプロジェクトリンクフォルダー設定がある場合でも、Adobe WorkfrontとAdobe Experience Manager Assetsas a Cloud Serviceの間にリンクされたフォルダーを作成できるようになりました。
* イベント購読のページネーションのサポートを追加しました。
* AEM 6.4.x のサポートを追加しました。
* プロキシ環境のサポートを追加しました。
* パートナーやお客様のご意見に基づいた、いくつかのバグ修正がおこなわれました。

詳しくは、 [Workfront forExperience Manager強化コネクタの概要](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>このコネクタのデプロイと設定には、認定されたパートナーが必要です。 詳しくは、 [Workfront forExperience Manager拡張コネクタのインストール](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) を参照してください。

## Adobe Creative Cloud統合で OAuth2 が使用されるようになりました

セキュリティを強化し、統合全体でより一貫したエクスペリエンスを得るために、Adobe Creative Cloud統合を更新して、ユーザーを認証する業界標準の方法である OAuth2 認証を使用するようにしました。 これで、ユーザーがログインすると、統合がアクセスできる特定のアクションや領域を確認し、アクセスを許可できるようになります。 その後は、頻繁にログインする必要はありません。

詳しくは、 [Workfront Extension for IllustratorとInDesignの使用](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## カスタム OAuth2 または JWT 統合のクライアント秘密鍵の詳細を表示する

カスタム OAuth2 および JWT 統合の使用に対する透明性を高めるため、統合で使用するクライアントシークレットの詳細を確認できるようにしました。 これで、クライアントシークレットが作成され、最後に使用された日付を確認できます。 また、クライアントシークレットに関する独自のメモを追加して表示することもできます。

以前は、これらの詳細は不明でした。

OAuth2 または JWT カスタム統合でのクライアントシークレットについて詳しくは、 [Workfront統合用の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## カスタム OAuth2 アプリケーションのリストで認証のタイプを参照する

これで、組織内のカスタム OAuth2 アプリケーションのリストを表示すると、各アプリケーションがユーザー認証とサーバー認証のどちらを使用しているかを確認できます。

以前は、この情報は、各アプリケーションの編集オプションからのみ表示できました。

詳しくは、 [Workfront統合用の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## カスタム OAuth2 統合での更新トークンの有効期限の設定

カスタム OAuth2 統合のアクセスとセキュリティをより適切に制御するために、更新トークンの有効期間をカスタマイズできるようになりました。 ユーザーの更新トークンの有効期限が切れた後、統合に再度ログインする必要があります。

詳しくは、 [Workfront統合用の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## サーバー間アプリ用のカスタム OAuth2 統合で公開鍵と秘密鍵を使用する

カスタム統合でサーバー間 OAuth2 アプリケーションを設定できるようになりました。 公開鍵と秘密鍵を設定することで、Workfrontがログイン資格情報を使用せずに別のアプリケーションと通信できるようになります。

以前は、カスタム OAuth2 アプリケーションのすべての認証で、ユーザーのログイン資格情報が使用されていました。

詳しくは、 [Workfront統合用の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Google G Suite の統合で OAuth2 が使用されるようになりました。

セキュリティを強化し、統合全体でより一貫したエクスペリエンスを得るために、Google G Suite 統合を更新し、ユーザーを認証する業界標準の方法である OAuth2 認証を使用するようにしました。 これで、ユーザーがログインすると、統合がアクセスできる特定のアクションや領域を確認し、アクセスを許可できるようになります。 その後は、頻繁にログインする必要はありません。

詳しくは、 [Adobe Workfront for G Suite へのログインとログアウト](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
