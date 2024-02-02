---
content-type: overview
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-desktop-proofing-viewer
title: デスクトッププルーフビューアーについて
description: デスクトッププルーフビューアは、インタラクティブコンテンツをプルーフする目的で設計されていますが、静的コンテンツやビデオコンテンツのプルーフにも使用できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 4610f24f-345a-4ebc-8a0c-382e34cac7b0
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: ht
source-wordcount: '543'
ht-degree: 100%

---

# デスクトッププルーフビューアーについて

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

デスクトッププルーフビューアは、インタラクティブコンテンツをプルーフする目的で設計されていますが、静的コンテンツやビデオコンテンツのプルーフにも使用できます。

Web プルーフビューアとは異なり、デスクトッププルーフビューアは、ワークステーションで実行されるアプリケーションです。ただし、プルーフを起動するときは、スタンドアロンアプリケーションとして実行するのではなく、[!DNL Workfront] または [!DNL Workfront Proof] からアクセスします（デスクトッププルーフビューアについて詳しくは、[デスクトッププルーフビューアのインストール](../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)を参照してください）。

## デスクトッププルーフビューアと他のプルーフビューアの比較

* [デスクトッププルーフビューアと web プルーフビューアの比較](#desktop-proofing-viewer-vs-web-proofing-viewer)
* [デスクトッププルーフビューアとレガシープルーフビューアの比較](#desktop-proofing-viewer-vs-legacy-proofing-viewer)

### デスクトッププルーフビューアと web プルーフビューアの比較 {#desktop-proofing-viewer-vs-web-proofing-viewer}

デスクトッププルーフビューアと web プルーフビューアを区別する主な 2 つの特徴は次のとおりです。

* デスクトッププルーフビューアでは、web サイト、ストリーミングビデオ、インタラクティブバナーなどのインタラクティブコンテンツをレビューできます。web プルーフビューアでは、静的なプルーフとビデオのプルーフのみをレビューできます。
* デスクトッププルーフビューアは、ローカルコンピューター上でアプリケーションとして実行され、web プルーフビューアはブラウザーで実行されます。

  >[!NOTE]
  >
  >   * セキュリティ上の理由でデスクトッププルーフビューアアプリを使用できない場合、[!DNL Workfront] 管理者は、ZIP アーカイブファイルにバンドルされたインタラクティブコンテンツを web プルーフビューアで確認できるようにシステムを設定できます。
  >   * プルーフの作成やブラウジングなどのプルーフ管理タスクは、[!DNL Workfront] または [!DNL Workfront Proof] で発生します。デスクトッププルーフビューアは、プルーフのレビュー用にのみ使用されます。


様々なプルーフビューアの機能について詳しくは、[Web プルーフビューアとデスクトッププルーフビューアの違いの概要](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)を参照してください。

### デスクトッププルーフビューアとレガシープルーフビューアの比較 {#desktop-proofing-viewer-vs-legacy-proofing-viewer}

レガシープルーフビューアは、ほとんどの環境で非推奨となっている Flash でサポートされているので、このビューアにはアクセスできない可能性があります。

デスクトッププルーフビューアには、レガシープルーフビューアに対して次の機能強化が含まれています。

* セキュリティで保護されている（HTTPS）サイトだけでなく、セキュリティで保護されていない（HTTP）サイトもレビューできます。
* iFrame で保護されたサイト（iFrame 内で表示できないサイト）をレビューできます。
* 様々なデバイス向けに事前に設定された解像度でコンテンツを表示します。\
   例えば、様々な標準のデスクトップ解像度や、iPhone 8 などの個々のデバイスでコンテンツがどのように表示されるかを確認できます。

レガシープルーフビューアは 2018 年末の 2018.3 リリースで [!DNL Workfront] から削除されます。

レガシープルーフビューアは、2018年7月の 2018.2 リリース後に [!DNL Workfront] を入手した顧客には提供されません。

## デスクトッププルーフビューアで非インタラクティブプルーフを開くためのユーザー設定

デスクトッププルーフビューアの主な目的はインタラクティブコンテンツをプルーフすることですが、この設定を使用して静的なプルーフやビデオのプルーフを行うこともできます。

ユーザーは、静的なプルーフやビデオのプルーフなど、あらゆる種類のプルーフを開いたときに、デスクトッププルーフビューアを自動的に起動するように設定できます。詳しくは、[プルーフビューア設定の指定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)を参照してください。

## プルーフ URL の入力

ワークステーションから直接デスクトッププルーフビューアを起動した場合は、プルーフ URL を指定してプルーフを開くことができます。これを行うには、表示するプルーフのプルーフ URL が必要です。

[!DNL Workfront] から直接プルーフを開くことをお勧めします。詳しくは、[プルーフのレビュー](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md)を参照してください。
