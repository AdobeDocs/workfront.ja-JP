---
title: 22.2 統合の機能強化
description: 22.2 統合の機能強化
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 100%

---

# 22.2 統合の機能強化

このページでは、プレビュー環境の 2.2 リリースで行われたすべての統合の機能強化について説明します。これらの機能強化は、

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日（PT）の週に実稼動環境で公開されます。

22.2 リリースで利用可能なすべての変更点の一覧については、[22.2 リリースの概要](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)を参照してください。

## Adobe Workfront と Anaplan の統合が利用可能

Workfront プロジェクトの財務面における柔軟性とインサイトの向上させるために、Workfront を Anaplan アカウントと統合できるようになりました。Workfront オブジェクトを Anaplan オブジェクトにリンクすると、2 つのアカウント間の情報を自動的に更新し、確実に両方の情報が最新で同一にすることができます。また、Workfront のアクションに基づいて、Analypan で自動化されたプロセスをトリガーすることもできます（またはその逆も可能です）。

例えば、Analypan でキャンペーンを作成し、そのキャンペーンにリンクされた Workfront プロジェクトまたはプログラムを作成できます。その後、Workfront で追跡されたコストを Anaplan にアップロードして、キャンペーンのパフォーマンスを確認できます。

Workfront から Analypan への統合を使用する際に考慮すべきその他のワークフローは次のとおりです。

* 新しい Workfront プロジェクトからの Analyplan 予算リクエストの作成
* 新しい Anaplan リスト項目からの Workfront プロジェクトの作成
* Workfront プロジェクトからの Analyplan サプライヤーリクエストの実行

詳しくは、[Adobe Workfront と Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md) を参照してください。

## Workfront for Experience Manager 拡張コネクタのアップデート

Workfront for Experience Manager 拡張コネクタに、次のアップデートが含まれるようになりました。

* 複数のプロジェクトリンクフォルダー設定がある場合でも、Adobe Workfront と Adobe Experience Manager Assets as a Cloud Service の間にリンクされたフォルダーを作成できるようになりました。
* イベント登録のページネーションのサポートを追加
* AEM 6.4.x のサポートを追加
* プロキシ環境のサポートを追加
* パートナーやお客様のご意見に基づいた、いくつかのバグ修正

詳しくは、[Workfront for Experience Manager 拡張コネクタの概要](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md)を参照してください。

>[!NOTE]
>
>このコネクタのデプロイと設定には、認定されたパートナーが必要です。詳しくは、[Workfront for Experience Manager 拡張コネクタのインストール](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=ja#)を参照してください。

## Adobe Creative Cloud 統合で OAuth2 が使用されるようになりました

セキュリティを強化し、統合全体でより一貫したエクスペリエンスを得るために、Adobe Creative Cloud 統合を更新して、ユーザーを認証する業界標準の方法である OAuth2 認証を使用するようにしました。ユーザーがログインすると、ユーザーに統合機能でアクセスできる特定のアクションやエリアが表示され、アクセスを許可できるようになりました。その後は、頻繁にログインする必要はありません。

詳しくは、[Illustrator および InDesign での Workfront 拡張機能の使用](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md)を参照してください。

## カスタム OAuth2 または JWT 統合のクライアント秘密鍵の詳細の表示

カスタム OAuth2 および JWT 統合の使用に対する透明性を高めるため、統合で使用するクライアント秘密鍵の詳細を確認できるようにしました。これで、クライアントの秘密鍵が作成された日付および最後に使用された日付を確認できます。また、クライアントの秘密鍵に関する独自のメモを追加して表示することもできます。

以前は、これらの詳細を表示することはできませんでした。

OAuth2 または JWT カスタム統合でのクライアントの秘密鍵について詳しくは、[Workfront 統合の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## カスタム OAuth2 アプリケーションのリストで認証のタイプを参照

これで、組織内のカスタム OAuth2 アプリケーションのリストを表示すると、各アプリケーションがユーザー認証とサーバー認証のどちらを使用しているかを確認できます。

以前は、この情報は、各アプリケーションの編集オプションからのみ表示できました。

詳しくは、[Workfront 統合の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## カスタム OAuth2 統合での更新トークンの有効期限の設定

カスタム OAuth2 統合のアクセスとセキュリティをより適切に制御するために、更新トークンの有効期間をカスタマイズできるようになりました。ユーザーの更新トークンの有効期限が切れた後、統合に再度ログインする必要があります。

詳しくは、[Workfront 統合の OAuth2 アプリケーションの作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## サーバー間アプリでのカスタム OAuth2 統合における公開鍵および秘密鍵の使用

カスタム統合でサーバー間の OAuth2 アプリケーションを設定できるようになりました。公開鍵と秘密鍵を設定することで、Workfront がログイン資格情報を使用せずに別のアプリケーションと通信できるようになります。

以前は、カスタム OAuth2 アプリケーションのすべての認証で、ユーザーのログイン資格情報が使用されていました。

詳しくは、[Workfront 統合用の OAuth2 アプリケーションを作成](../../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## Google G Suite の統合で OAuth2 が使用されるようになりました

セキュリティを強化し、統合全体でより一貫したエクスペリエンスを得るために、Google G Suite 統合を更新し、ユーザーを認証する業界標準の方法である OAuth2 認証を使用するようにしました。ユーザーがログインすると、ユーザーに統合機能でアクセスできる特定のアクションやエリアが表示され、アクセスを許可できるようになりました。その後は、頻繁にログインする必要はありません。

詳しくは、[Adobe Workfront for G Suite へのログインとログアウト](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md)を参照してください。
