---
product-area: documents
navigation-topic: proofing-overview
title: Web プルーフビューア拡張機能でのインタラクティブコンテンツのレビュー
description: Adobe Workfront レビューツールは、ZIP ファイルまたは URL を使用してインタラクティブコンテンツのプルーフを行うことができるブラウザー拡張機能です。
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 5a8bfdeae7f5d23ecf835e652cf0ff5efd5aa410
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 1%

---

# Adobe Workfront レビューツールを使用したインタラクティブコンテンツのレビュー

<span class="preview">Adobe Workfront レビューツールは、2024 年 11 月 7 日（PT）に利用可能になりました。 この拡張機能は現在ベータ版です。</span>

Adobe Workfront レビューツールは、ZIP ファイルまたは URL を使用してインタラクティブコンテンツのプルーフを行える、web ベースのブラウザー拡張機能です。 Adobe Workfront レビューツールは次のブラウザーで使用できます。

* Firefox
* Chrome
* Edge
* Safari

>[!IMPORTANT]
>
>この拡張機能は、GenStudio for Performance Marketingと Creative Cloud Express のコンテンツをレビューするために必要です。 Assetsは web ビューアで自動的に開きます。 アカウント設定を更新する必要はありません。


## 拡張機能のインストール

### 前提条件

* Adobe Workfront レビューツールを使用するには、従来の Web ビューア拡張機能を削除する必要があります。

### 拡張機能のインストール

レビュー担当者と承認者は、Adobe Workfront レビューツールをインストールする必要があります。 次のいずれかのブラウザーで以下を行います。

* [Firefox 拡張機能 ](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome拡張機能 ](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)


インタラクティブプルーフがAdobe Workfront レビューツールで自動的に開くには、以下の節で説明するように、Workfront管理者が workfront のプルーフ設定を更新する必要があります。

## Workfront プルーフのデフォルトの更新

Workfront レビューツールをインタラクティブコンテンツのデフォルトビューアとして使用するには、Workfrontでプルーフのデフォルトを更新する必要があります。

>[!NOTE]
>
>確認する必要があるコンテンツが Web サイト上にある場合は、デスクトッププルーフビューアを使用することをお勧めします。
>
>* SSO 認証が必要
>* Figma などの iFrame でサイトを開けないようにします

### Adobe Workfront レビューツールを URL と ZIP 配達確認のデフォルトビューアにする

Web レビューツールを URL および ZIP 配達確認に使用するには、Workfront管理者がインタラクティブ配達確認のデフォルト設定を調整する必要があります。

1. Workfrontのメインメニューで、「**プルーフ**」をクリックします。
1. **アカウント設定** をクリックしてから、**設定** タブをクリックします。
1. 「**プルーフのデフォルト**」セクションで、**インタラクティブプルーフのデスクトッププルーフビューア** を見つけて、**設定** をクリックします。
1. ドロップダウンメニューで、「**無効**」を選択します。 URL または ZIP ファイルから作成されたインタラクティブなプルーフが、web ベースのブラウザーであるAdobe Workfront レビューツールで自動的に開くようになりました。
1. **保存**&#x200B;をクリックします。

>[!NOTE]
>
>この変更は、Workfront インスタンスのすべてのインタラクティブなプルーフに適用されます。 実稼動で有効にする前に、プレビュー環境で新しいエクスペリエンスをテストすることをお勧めします。 **インタラクティブプルーフ用デスクトッププルーフビューア** アカウント設定を **すべてのインタラクティブプルーフで有効** に戻すと、デスクトップビューアに簡単に切り替えることができます。

### Adobe Workfront レビューツールを ZIP 配達確認のみのデフォルトビューアにする

Web レビューツールを zip 配達確認にのみ使用するには、Workfront管理者が、インタラクティブ配達確認のデフォルト設定を調整する必要があります。

1. Workfrontのメインメニューで、「**プルーフ**」をクリックします。
1. **アカウント設定** をクリックしてから、**設定** タブをクリックします。
1. 「**プルーフのデフォルト**」セクションで、**インタラクティブプルーフのデスクトッププルーフビューア** を見つけて、**設定** をクリックします。
1. ドロップダウンメニューで、「**URL から作成されたインタラクティブなプルーフでのみ有効**」を選択します。 ZIP ファイルから作成されたインタラクティブなプルーフが、web ベースのブラウザーであるAdobe Workfront レビューツールで自動的に開くようになりました。 URL から作成されたインタラクティブプルーフが、デスクトッププルーフビューアで開いたままになる。
1. **保存**&#x200B;をクリックします。

>[!NOTE]
>
>この変更は、Workfront インスタンスのすべての ZIP 配達確認に適用されます。 実稼動で有効にする前に、プレビュー環境で新しいエクスペリエンスをテストすることをお勧めします。 **インタラクティブプルーフ用デスクトッププルーフビューア** アカウント設定を **すべてのインタラクティブプルーフで有効** に戻すと、デスクトップビューアに簡単に切り替えることができます。

