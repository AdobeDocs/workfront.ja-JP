---
product-area: documents
navigation-topic: proofing-overview
title: Web プルーフビューア拡張機能でのインタラクティブコンテンツのレビュー
description: Adobe Workfront レビューツールは、ZIP ファイルまたはURLを使用してインタラクティブコンテンツをプルーフできるブラウザー拡張機能です。
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
TQID: https://experienceleague.adobe.com/jwZKladWxKsiSvAjO8me1BWoxMx1UDB2TKl7k-jnjcY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 646
ht-degree: 3%

---

# Adobe Workfront レビューツールを使用したインタラクティブコンテンツのレビュー


>[!IMPORTANT]
>
> SSO認証を必要とするか、FigmaなどのiFramesでサイトを開かないweb サイトでホストされるインタラクティブコンテンツには、デスクトップ校正ビューアを使用することをお勧めします。

Adobe Workfront レビューツールは、インタラクティブコンテンツをZIP ファイルまたはURLでマークアップできるweb ベースのブラウザー拡張機能です。 Adobe Workfront レビューツールは、次のブラウザーで使用できます。

* Firefox
* Chrome
* Edge
* Safari

## 拡張機能のインストール

### 前提条件

* Adobe Workfront レビューツールを使用するには、従来のWeb ビューア拡張機能を削除する必要があります。

### 拡張機能のインストール

レビュー担当者と承認者は、Adobe Workfront レビューツールをインストールする必要があります。 次のいずれかのブラウザーで実行します。

* [Firefox拡張機能](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome拡張機能](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

* [Safari拡張機能](https://apps.apple.com/us/app/adobe-workfront-review-tool/id6741517062?mt=12)



インタラクティブなプルーフをAdobe Workfront レビューツールで自動的に開くには、Workfront管理者がWorkfrontのプルーフ設定を以下の節で説明するように更新する必要があります。

## GenStudio for Performance MarketingおよびCreative Cloud ExpressでのAdobe Workfront レビューツールの使用

この拡張機能は、GenStudio for Performance MarketingとCreative Cloud Expressのコンテンツを確認するために必要です。 Assetsは、web ビューアで自動的に開きます。 アカウント設定を更新する必要はありません。


## Workfront プルーフのデフォルトの更新

Workfront レビューツールをインタラクティブコンテンツのデフォルトビューアとして使用するには、Workfrontでプルーフデフォルトを更新する必要があります。

>[!IMPORTANT]
>
>レビューする必要があるコンテンツが次のweb サイトにある場合は、デスクトップ校正ビューアを使用することをお勧めします。
>
>* SSO認証が必要です
>* FigmaなどのiFramesでサイトを開かないようにします

### Adobe Workfront レビューツールをURLおよびZIP プルーフのデフォルトビューアーにする

Web レビューツールをURLおよびZIP プルーフに使用するには、Workfront管理者がインタラクティブプルーフのデフォルト設定を調整する必要があります。

1. Workfrontのメインメニューで、**プルーフ**&#x200B;をクリックします。
1. 「**アカウント設定**」をクリックし、「**設定**」タブをクリックします。
1. **プルーフの既定値** セクションで、**対話型プルーフ用デスクトップ プルーフ ビューア**&#x200B;を見つけて、**設定**&#x200B;をクリックします。
1. ドロップダウンメニューで、**無効**&#x200B;を選択します。 URLまたはZIP ファイルから作成されたインタラクティブプルーフが、web ベースのブラウザーであるAdobe Workfront レビューツールで自動的に開くようになりました。
1. 「**保存**」をクリックします。

>[!NOTE]
>
>この変更は、Workfront インスタンス内のすべてのインタラクティブなプルーフに適用されます。 実稼動環境で有効にする前に、プレビュー環境で新しいエクスペリエンスをテストすることをお勧めします。 **デスクトップ校正ビューアのインタラクティブ校正** アカウント設定を&#x200B;**すべてのインタラクティブ校正で有効**&#x200B;に戻すことで、デスクトップ ビューアに簡単に切り替えることができます。

### Adobe Workfront レビューツールをZIP プルーフ専用のデフォルトビューアーにする

Web レビューツールをZIP プルーフにのみ使用するには、Workfront管理者がインタラクティブプルーフのデフォルト設定を調整する必要があります。

1. Workfrontのメインメニューで、**プルーフ**&#x200B;をクリックします。
1. 「**アカウント設定**」をクリックし、「**設定**」タブをクリックします。
1. **プルーフの既定値** セクションで、**対話型プルーフ用デスクトップ プルーフ ビューア**&#x200B;を見つけて、**設定**&#x200B;をクリックします。
1. ドロップダウンメニューで、**有効は、URL**&#x200B;から作成されたインタラクティブなプルーフに対してのみ選択します。 ZIP ファイルから作成されたインタラクティブプルーフが、web ベースのブラウザーであるAdobe Workfront レビューツールで自動的に開くようになりました。 URLから作成されたインタラクティブなプルーフは、引き続きデスクトッププルーフビューアで開きます。
1. 「**保存**」をクリックします。

>[!NOTE]
>
>この変更は、Workfront インスタンス内のすべてのZIP プルーフに適用されます。 実稼動環境で有効にする前に、プレビュー環境で新しいエクスペリエンスをテストすることをお勧めします。 **デスクトップ校正ビューアのインタラクティブ校正** アカウント設定を&#x200B;**すべてのインタラクティブ校正で有効**&#x200B;に戻すことで、デスクトップ ビューアに簡単に切り替えることができます。

