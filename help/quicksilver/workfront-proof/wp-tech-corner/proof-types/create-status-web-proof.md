---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: ' [!DNL Workfront Proof] を使用して web サイトの静的プルーフを作成'
description: web ページから静的プルーフを作成できます。さらに、キャプチャの画面解像度を定義することで、様々なデバイスをシミュレートできます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: ht
source-wordcount: '509'
ht-degree: 100%

---

# [!DNL Workfront Proof] を使用して web サイトの静的プルーフを作成

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品 [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内でのプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

web ページから静的プルーフを作成できます。さらに、キャプチャの画面解像度を定義することで、様々なデバイスをシミュレートできます。

## Web サイトの静的プルーフを作成

1. [ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成の説明に従って、[!UICONTROL 新しいプルーフ]ページを開きます。
1. URL を「**www.shareyourlink.com**」ボックスにペーストするか入力します。
1. この手順を繰り返して、複数の URL を追加できます。
1. このボックスのすぐ下で、解像度（デフォルトは 1366 x 768）をクリックし、「**[!UICONTROL スクリーンショットの解像度]**」ボックスで目的の解像度を選択します。
モバイルデバイスのデザインをプルーフする場合は、より小さな解像度を選択します。一般に、デザインは、画面／ブラウザーウィンドウの解像度に従って読み込まれます。

1. 入力した URL と同じドメイン／サブドメインにある接続されたページを含める場合は、「**[!UICONTROL サブページを探す]**」をクリックします。
   [!DNL Workfront Proof] は、接続されているページをスキャンし、「**[!UICONTROL サブページを探す]**」オプションの下に一覧表示します。含めるページを選択できます。

1. [!UICONTROL プルーフを結合]機能を使用すると、すべての web ページを単一の複数ページプルーフとして送信できます。
1. 「**[!UICONTROL 完了]**」をクリックし、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成の説明に従って、プルーフの設定を終了します。

## パスワードで保護されたページおよび認証が必要なページについて

[!DNL Workfront Proof] は、パスワードで保護された web サイトを静的プルーフとして取り込むことはできません。

認証が必要なページからプルーフを作成するには、web キャプチャツールが接続する際に経由する次の URL のいずれかを、IT チームが会社の許可リストに追加する必要があります。

**米国の AWS クラスター**：webcapture.proofhq.com

**米国の GCP クラスター**：webcapture.gcp.proofhq.com

**EMEA クラスター**：webcapture.proofhq.eu

>[!NOTE]
>
>認証およびパスワードで保護された web ページが必要な内部ページに対しては、静的プルーフではなく、インタラクティブプルーフをお勧めします。詳しくは、[インタラクティブコンテンツのプルーフの概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)を参照してください。

## Web サイトの静的プルーフの処理について

* アニメーション、埋め込みビデオ、スクリプト、インタラクションは、web サイトの静的プルーフに含めることはできません。インタラクティブコンテンツのプルーフを行う場合は、[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成にある[ [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) でプルーフを生成を参照してください。

* プルーフページは、通常、1 ページあたり約 20 秒のペースで取り込みの準備がされます。ただし、準備の総時間は、ページがホストされているサーバーによっても異なります。ツールは、送信されたそれぞれの URL が読み込まれるまで、60 秒待機します。この待機時間を超えると、プルーフは失敗します。
* 組み合わせプルーフの場合、いずれかの URL がキャプチャツールに応答しない場合、プルーフは失敗します。
* [!DNL Workfront Proof] は、ラスタライズの後、最大 195 インチの長さの web ページをキャプチャします。Web ページがこれより長い場合、プルーフは失敗します。
* テキスト抽出は、すべてのテキスト要素で使用できますが、画像として配置されたテキストは抽出されません。
* テキストのハイパーリンクはプルーフでクリックでき、リンクされたページがブラウザーの新しいタブに開きます。
* style=&quot;display:block&quot; 要素が `<a>` タグ内で使用されている場合、画像上のハイパーリンクはクリックできません。ページデザインのこれらの部分を調整することをお勧めします。
* 最良の結果を得るには、コーディングのベストプラクティスと広く知られている標準を使用してページを作成することをお勧めします。
