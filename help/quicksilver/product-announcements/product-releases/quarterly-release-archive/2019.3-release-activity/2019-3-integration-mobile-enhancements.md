---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 統合およびモバイルの機能強化
description: このページでは、2019.3 リリースに含まれるすべての統合およびモバイルの機能強化について説明します。2019年8月19日（PT）の週に、実稼動環境で使用できるようになりました。
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 100%

---

# 2019.3 統合およびモバイルの機能強化

このページでは、2019.3 リリースに含まれるすべての統合およびモバイルの機能強化について説明します。2019年8月19日（PT）の週に、実稼動環境で使用できるようになりました。

2019.3 で行われたすべての変更のリストについては、[2019.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md)を参照してください。

## MS OneDrive 統合での共有アイテムのサポート

共有された OneDrive ファイルおよびフォルダーを Workfront オブジェクトにリンクできるようになりました。逆に、OneDrive の共有フォルダーに Workfront のファイルをアップロードできます。

詳細については、[外部アプリケーションからのドキュメントのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)の、[外部ドキュメントの Workfront へのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)、[1 つ以上の外部フォルダーのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder)、[Workfront からのドキュメントの更新と外部クラウドプロバイダーへのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents)節を参照してください。

詳細については、[外部アプリケーションからのドキュメントのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)の[ Workfront への外部ドキュメントのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)節を参照してください。

## すべての Workfront ログインにドメイン指定が必要

ドメインが Workfront URL でまだ指定されていない場合、ユーザーはすべての Workfront ログインでドメインの指定が必要になりました。この情報が必要になることで、Workfront インスタンスのセキュリティが高まります。さらに、Workfront の実装に複数のインスタンスがある場合、この機能強化により、実装内の Workfront の各インスタンスに同じユーザーを追加できるようになります。

この変更は、ユーザーログインと API 統合の両方に影響を与える可能性があります。

* **ユーザーログイン**

  会社のドメインが Workfront URL に含まれていない場合、ログイン画面に、「ユーザー名」フィールドと「パスワード」フィールドに加えて、新しい「ドメイン」フィールドが表示されるようになりました。

  ドメイン情報は既に Workfront URL に含まれているので、ほとんどのお客様は変更する必要はありません。例えば、「*ドメイン*.my.workfront.com.」です。

* **API 統合**

  ドメイン名が含まれていないアドレスに API コードを送信すると、その API コードは機能しなくなります。

詳しくは、[Adobe Workfront へのログイン](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md)を参照してください。

## iOS のモバイルアプリを使用してタスクとイシューをプロジェクトに変換

iOS の Workfront モバイルアプリで、個々のタスクとイシューをプロジェクトに変換できるようになりました。

## フィンガープリントまたは顔認証を使用してモバイルアプリにログイン

デバイスによっては、フィンガープリントまたは顔認識技術を使用した Workfront モバイルアプリへのログインを選択できます。モバイルアプリにログインすると、携帯電話がサポートする認証方法を使用してログインするかどうかを尋ねられます。

この機能の管理方法の詳細については、[Adobe Workfront for iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) または [Adobe Workfront for Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) を参照してください。

## モバイルでユーザーを自動的にログアウトさせる新しい設定

ユーザーや会社に対して Workfront モバイルアプリの安全性を高めるために、無操作状態が 15 日間続くとユーザーは自動的にログアウトされます。Workfront の管理者は、Web アプリケーションの設定／システム／環境設定で、この制限をカスタマイズできます。

詳しくは、[システムセキュリティの環境設定を指定](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

## ログイン時にモバイルアプリにドメインが必要

セキュリティが強化されたため、シングルサインオン資格情報を使用してログインしない場合、Workfront モバイルアプリではドメインの指定が必要になりました。

>[!NOTE]
>
>iOS の公開日：2019年6月12日（PT）
>
>実稼動環境の公開日：2019年6月17日（PT）

## iOS のモバイルアプリを使用したオブジェクトの削除

>[!NOTE]
>
>この機能は、2019年8月19日（PT）の週に iOS の App Store で利用できるようになりました。

iOS モバイルアプリで、タスク、イシュー、タイムシートなどのオブジェクトを削除できるようになりました。オブジェクトを削除するには、そのオブジェクトに対する正しい権限が必要です。

## モバイルアプリでの無効なプロジェクトでフィルタリング

>[!NOTE]
>
>この機能は、2019年8月19日（PT）の週に iOS と Android の両方のアプリストアで利用できるようになりました。

モバイルアプリの「プロジェクト」タブに、「停止したプロジェクト」がフィルターオプションとして追加されました。

## モバイルアプリを使用したパスワードのリセット

パスワードを忘れた場合は、Workfront Mobile アプリを使用して、パスワードをリセットできます。「パスワードを忘れた場合」をタップして、画面の指示に従います。モバイルアプリで SSO パスワードをリセットすることはできません。

## モバイルの新しいルックアンドフィール

Workfront Mobile アプリでエクスペリエンスを強化するために次のルックアンドフィールが改善されました。

* 詳細ページの上部のバーから、画面上でより目立つ領域に以下を移動しました。

   * 画面の左下隅にプラスアイコンが表示されます
   * 項目の操作を開始するためのチェックマークが、画面の中央上にある「作業開始」ボタンになりました

* 詳細ページの下部にある「詳細を表示」をタップして、添付されたカスタムフォームを表示できるようになりました。
* タスク、イシュー、リクエストの送信に使用するページの外観を変更しました。

