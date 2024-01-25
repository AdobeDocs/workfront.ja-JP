---
product-area: documents
navigation-topic: proofing-overview
title: インタラクティブコンテンツの配達確認の概要
description: インタラクティブコンテンツは、複数の方法でビューアを操作できます。 代理店は、このコンテンツに対する回答から収集した分析を使用して、キャンペーンの成功を測定できます。
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# インタラクティブコンテンツの配達確認の概要

<!-- Audited: 01/2024 -->

インタラクティブコンテンツは、複数の方法でビューアを操作できます。 代理店は、このコンテンツに対する回答から収集した分析を使用して、キャンペーンの成功を測定できます。

インタラクティブコンテンツの例を次に示します。

* Web サイト
* 埋め込みビデオまたはストリーミングビデオ
* インタラクティブバナー
* HTML5 アニメーション
* マイクロサイト
* インタラクティブ E メール

## インタラクティブコンテンツの配達確認の作成について

インタラクティブコンテンツの配達確認は、次のいずれかの方法で作成できます。

* インタラクティブコンテンツを含む ZIP ファイルから配達確認を作成します。

  Adobe Workfrontは、ZIP ファイルからコンテンツを解凍し、Workfrontサーバーに保存します。 この方法で保存されるので、配達確認のレビューサイクルを通じて、同じコンテンツを信頼できます。

* コンテンツの URL を指定します。

  これは、インタラクティブコンテンツの配達確認を作成する最も簡単な方法です。 また、ユーザーがインターネット上でコンテンツを体験する際に、コンテンツをインタラクティブに確認できるのは、この方法のみです。

  このアプローチでは、Workfrontが不明な外部サーバーがコンテンツを保存およびホストします。

  大規模な Web サイトでは、大規模な Web サイトを構成するすべてのファイルを収集するのが困難なので、この方法をお勧めします。 ただし、配達確認のコンテンツは外部に保存されるので、作業中の開発者が加えた変更からWorkfrontで保護することはできないので、配達確認のレビューサイクル全体で同じコンテンツを信頼できない可能性があります。

## ZIP ファイル内のインタラクティブコンテンツを校正用に準備する方法について

インタラクティブコンテンツを ZIP ファイルにバンドルして校正する場合は、次の仕様が含まれていることを確認してください。

* CSS、JavaScript、ビデオ、サウンド、画像などのすべてのアセットをバンドルファイルに含める必要があります。
* インタラクティブコンテンツには、メインファイル (index.html、index.htm) を含める必要があります。 このファイルがルートの場所に配置されていない場合、ツールは自動的にフォルダーを検索して見つけます。 メインファイルの名前を index.html/index.htmにする必要はありませんが、メインの場所に配置できる.html/.htm ファイルは 1 つだけです。
* ファイルには、1 つ以上の静的ファイル Web ページが含まれている必要があります。
* 最大バンドルサイズは 500 MB です。
* iOSで作成した.zip ファイルの場合、このツールはコンテンツが配置されているフォルダーを自動的に識別します。
* インタラクティブプロジェクトは.zip アーカイブとしてのみサポートされます。 標準の.zip ファイルの送信は失敗します。
* Web サイトはセキュリティで保護されている必要があります (HTTPS)。

  これは、デスクトップ校正ビューアを使用する場合は不要です。

  詳しくは、 [デスクトップ校正ビューアについて](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Web サイトを iframe で表示できるようにする必要があります。

  これは、デスクトップ校正ビューアを使用する場合は不要です。

  詳しくは、 [デスクトップ校正ビューアについて](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## インタラクティブな配達確認の作成について

ZIP バンドルファイルを準備したら、インタラクティブな配達確認を作成します。

詳しくは、 [ZIP ファイル内のインタラクティブコンテンツの配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

また、Workfront Proof を使用している場合は、 [インタラクティブコンテンツの配達確認を生成](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) 記事内 [Workfrontの配達確認で配達確認を生成](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## インタラクティブな配達確認のレビューについて

インタラクティブな配達確認のデフォルトのビューアとして、スタンドアロンのデスクトップ校正ビューアを使用することをお勧めします。 ただし、組織のポリシーで Desktop Proofing Viewer アプリケーションの使用が許可されていない場合は、ZIP アーカイブファイルにバンドルされたインタラクティブコンテンツを Web 校正ビューアで確認できるように、Workfront管理者がシステムを設定できます。 デスクトップ校正ビューアと Web 校正ビューアの比較情報については、 [Web 校正ビューアとデスクトップ校正ビューアの違いの概要](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
