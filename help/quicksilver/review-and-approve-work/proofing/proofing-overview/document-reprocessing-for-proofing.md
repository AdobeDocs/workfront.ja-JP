---
product-area: documents
navigation-topic: proofing-overview
title: プルーフ用のドキュメントの再処理の概要
description: ドキュメント（DOCX、PDF、XLSX、AI）をプルーフ用に送信すると、Adobe Workfront によって再処理され、作成時に使用したソフトウェアアプリケーションがなくても、プルーフビューアで表示できるようになります。
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 100%

---

# プルーフ用のドキュメントの再処理の概要

ドキュメント（DOCX、PDF、XLSX、AI）をプルーフ用に送信すると、Adobe Workfront によって再処理され、作成時に使用したソフトウェアアプリケーションがなくても、プルーフビューアで表示できるようになります。 

ドキュメントの各ページが、プルーフビューアにサムネール画像として表示されます。サムネールをクリックすると、ビットマップバージョンのページに、100％、200％、400％でズームインできます。高さか幅が 800 mm を超えるプルーフの場合、最大ズームレベルは 200％です。

ドキュメントのカラーは、最新のアドビライブラリの色変換によって sRGB で表示されます。プルーフビューアは、ドキュメントに埋め込まれたインターナショナルカラーコンソーシアム（ICC）プロファイルをサポートしています。

ドキュメントをシステムにアップロードする際に、正しいファイル拡張子が含まれている限り、すべてのフォントテキストがそのレイヤーに抽出されます。画像または曲線として含まれているテキストは表示されません。

>[!NOTE]
>
>Workfront は現在、最大 2000 ページを含むドキュメントをサポートしています。これには組み合わせプルーフも含まれます。詳しくは、[複数ページのプルーフを作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)を参照してください。

## 一般的なヒント

* PDF ファイルは最も標準化されていて、信頼性が高いので、ドキュメントをこの形式に変換してからアップロードすることをお勧めします。
* ソフトウェアの最新バージョンを使用して、元のドキュメントを作成します。
* ドキュメントを作成したアプリケーションでドキュメントを保存または書き出す際に使用する設定が不明な場合は、デフォルト設定を使用します。 
* ドキュメント内に、使用するすべてのフォントを埋め込みます。カスタムフォントを使用する場合、それらのフォントがインストールされているコンピューター上でのみ、ドキュメントに表示されます。ただし、カスタムフォントはプルーフシステムに含まれていないので、埋め込んであったとしても、ファイルの生成時にカスタムフォントを使用できません。
* 可能であれば、すべてのテキスト要素をデザインの一番上のレイヤーに配置します。これにより、テキストが抽出され、テキスト注釈ツールで選択可能になります。
* ドキュメントのすべての画像と要素をドキュメント内に配置します。画像や要素を外部のソース（コンピューター上の別のファイルなど）からリンクした場合、作成したプルーフには表示されません。
* ドキュメントのタイプに推奨される標準を使用してドキュメントを作成し、アップロード前に最適化します。これにより、ドキュメントがプルーフビューア、および他のすべてのアプリケーションやプラットフォームで正常に開くようになります。
* デザインソフトウェアで「プリフライト」オプションを実行してみて、ドキュメントで警告が発生したかどうかを確認します。これらのオプションはほとんどのアプリケーションで、出力プレビューや印刷工程などで利用できます。詳しくは、アプリケーションのドキュメントを参照してください。
* ドキュメント全体でカラー設定の一貫性を確保します。
* ドキュメントがファイルのコピーなどの操作から保護されている場合、プルーフ抽出ツールでそのコンテンツにアクセスできない可能性があります。

## 処理時間

通常、処理には 1 ページあたり数秒かかります。ただし、ネットワークトラフィックや帯域幅、ローカル接続の速度、国際接続の速度（米国以外のユーザーの場合）など、様々な要因によってこの処理が長引く可能性があります。次の要素も処理時間に影響する場合があります。

* 静的ドキュメントおよび画像の場合：ページ数、ページの寸法、テキスト量、画像やオブジェクトの複雑さ（複数のベクター要素、レイヤー、透明度などの要素）。
* ビデオの場合：時間の長さ、寸法の大きさ、使用されているコーデック。
* Web キャプチャの場合：web ページの読み込み時間とページの寸法。

## 処理手順

送信されたファイルに対して、次の手順の一部またはすべてが実行されます。

1. **送信**。ドキュメントをシステムにアップロードする際に、新しいプルーフページを使用するか、アプリケーションプログラミングインターフェイス（API）を使用して実行します。
1. **キュー**. トラフィックが多い期間では、システムの過負荷を防ぐために、Workfront は送信をキューに入れることが必要な場合があります。ほとんどのプルーフは、キューでの待機は数秒しかかかりません。
1. **処理しています.**&#x200B;ファイルは、コンテンツタイプに従って処理マシンに送られます。ビデオのプルーフや、web キャプチャ、静的画像およびドキュメントの処理には、様々なツールを使用しています。リッチメディアコンテナ（ZIP）およびインタラクティブ web キャプチャの送信は、処理を必要としません。
