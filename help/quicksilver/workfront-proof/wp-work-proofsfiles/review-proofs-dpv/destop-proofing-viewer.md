---
content-type: overview
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-desktop-proofing-viewer
title: デスクトップ校正ビューアについて
description: デスクトップ校正ビューアは、インタラクティブコンテンツを校正する目的で設計されていますが、静的コンテンツやビデオコンテンツの校正にも使用できます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 4610f24f-345a-4ebc-8a0c-382e34cac7b0
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# デスクトップ校正ビューアについて

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

デスクトップ校正ビューアは、インタラクティブコンテンツを校正する目的で設計されていますが、静的コンテンツやビデオコンテンツの校正にも使用できます。

Web 校正ビューアとは異なり、デスクトップ校正ビューアは、お使いのワークステーションで実行されるアプリケーションです。 ただし、次の場所からアクセスします。 [!DNL Workfront] またはから [!DNL Workfront Proof] スタンドアロンアプリケーションとして実行するのではなく、配達確認を起動するとき ( デスクトップ校正ビューアのインストールの詳細については、 [デスクトップ校正ビューアのインストール](../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)) をクリックします。

## デスクトップ校正ビューアと他の校正ビューアとの比較

* [デスクトップ校正ビューアと Web 校正ビューア](#desktop-proofing-viewer-vs-web-proofing-viewer)
* [デスクトップ校正ビューアとレガシー校正ビューアの比較](#desktop-proofing-viewer-vs-legacy-proofing-viewer)

### デスクトップ校正ビューアと Web 校正ビューア {#desktop-proofing-viewer-vs-web-proofing-viewer}

デスクトップ校正ビューアと Web 校正ビューアを区別する主な 2 つの特徴は次のとおりです。

* デスクトップ校正ビューアを使用すると、Web サイト、ストリーミングビデオ、インタラクティブバナーなどのインタラクティブコンテンツをレビューできます。Web 校正ビューアでは、静的およびビデオの配達確認のみをレビューできます。
* デスクトップ校正ビューアは、ローカルコンピュータ上でアプリケーションとして実行されます。ブラウザで Web 校正ビューアが実行されます。

   >[!NOTE]
   >
   >   * セキュリティ上の理由からデスクトップ校正ビューアアプリを使用できない場合は、 [!DNL Workfront] 管理者は、ZIP アーカイブファイルにバンドルされているインタラクティブコンテンツを Web 校正ビューアで確認できるように、システムを設定できます。
   >   * 配達確認の作成や参照などの配達確認管理タスクは、 [!DNL Workfront] または [!DNL Workfront Proof]. デスクトップ校正ビューアは、配達確認のレビュー用にのみ使用されます。



様々な校正ビューアの機能について詳しくは、 [Web 校正ビューアとデスクトップ校正ビューアの違いの概要](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)

### デスクトップ校正ビューアとレガシー校正ビューアの比較 {#desktop-proofing-viewer-vs-legacy-proofing-viewer}

レガシー校正ビューアは、ほとんどの環境で非推奨となっているFlashでサポートされているので、このビューアにアクセスできない可能性があります。

デスクトップ校正ビューアには、従来の校正ビューアに対して次の機能強化が含まれています。

* セキュリティで保護されていない (HTTPS) サイトだけでなく、セキュリティで保護されていない (HTTP) サイトを確認します。
* iFrame で保護されたサイト（iFrame 内で表示できないサイト）を確認します。
* 様々なデバイス向けに事前に設定された解像度でコンテンツを表示します。\
   例えば、様々な標準のデスクトップ解像度や、iPhone 8 などの個々のデバイスでコンテンツがどのように表示されるかを確認できます。

以前のバージョンの校正ビューアは [!DNL Workfront] 2018 年末の 2018.3 リリースと共に。

旧来の校正ビューアは、 [!DNL Workfront] 2018 年 7 月の 2018.2 リリース以降。

## デスクトップ校正ビューアで非インタラクティブ校正を開くためのユーザー設定

デスクトップ校正ビューアの主な目的はインタラクティブコンテンツを校正することですが、これを使用して静的配達確認やビデオ配達確認を行うこともできます。

ユーザーは、静的配達確認やビデオ配達確認など、あらゆる種類の配達確認を開いたときに、デスクトップ校正ビューアを自動的に起動するように設定できます。 詳しくは、 [校正ビューアの設定を行う](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

## 配達確認 URL の入力

ワークステーションから直接デスクトップ校正ビューアを起動した場合は、配達確認 URL を指定して配達確認を開くことができます。 これをおこなうには、表示する配達確認の配達確認 URL が必要です。

次の場所から直接配達確認を開くことをお勧めします。 [!DNL Workfront]. 詳しくは、 [配達確認の確認](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).
