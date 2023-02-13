---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: を使用した静的 Web サイトの配達確認の作成 [!DNL Workfront Proof]
description: Web ページから静的配達確認を作成できます。 さらに、キャプチャの画面解像度を定義することで、様々なデバイスをシミュレートできます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# を使用した静的 Web サイトの配達確認の作成 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

Web ページから静的配達確認を作成できます。 さらに、キャプチャの画面解像度を定義することで、様々なデバイスをシミュレートできます。

## 静的 Web サイトの配達確認の作成

1. を開きます。 [!UICONTROL 新しい配達確認] ページ、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. URL を **www.shareyourlink.com** ボックス
1. この手順を繰り返して、複数の URL を追加できます。
1. このボックスのすぐ下で、解像度（デフォルトは 1366 x 768）をクリックし、 **[!UICONTROL スクリーンショットの解決]** ボックス
モバイルデバイスのデザインを配達確認する場合は、より小さい解像度を選択します。 一般に、デザインは、画面/ブラウザーウィンドウの解像度に従って読み込まれます。

1. クリック **[!UICONTROL サブページを検索]** を追加します。
   [!DNL Workfront Proof] は、接続されているページをスキャンし、 **[!UICONTROL サブページを検索]** オプション。 含めるページを選択できます。

1. を使用 [!UICONTROL 配達確認を結合] 機能を使用すると、すべての web ページを単一の複数ページの配達確認として送信できます。
1. クリック **[!UICONTROL 完了]**&#x200B;その後、配達確認の設定を完了します。詳しくは、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## パスワードで保護されたページおよび認証が必要なページについて

[!DNL Workfront Proof] は、パスワードで保護された web サイトを静的配達確認として取り込むことはできません。

認証が必要なページから配達確認を作成するには、IT チームが Web キャプチャツールを接続する際に使用する会社のに次の URL のいずれかを追加する必要がありま許可リストす。

**米国のAWSクラスター**:webcapture.proofhq.com

**米国の GCP クラスター**:webcapture.gcp.proofhq.com

**EMEA クラスタ**:webcapture.proofhq.eu

>[!NOTE]
>
>認証およびパスワードで保護された Web サイトを必要とする内部ページに対しては、静的校正ではなく、インタラクティブ校正をお勧めします。 詳しくは、 [インタラクティブコンテンツの配達確認の概要](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## 静的 Web サイトの配達確認の処理について

* アニメーション、埋め込みビデオ、スクリプトおよびインタラクションは、静的 Web サイトの配達確認に含めることはできません。 インタラクティブコンテンツの配達確認を行う場合は、 [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [で配達確認を生成 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* 配達確認ページは、通常、1 ページあたり約 20 秒の速度で取り込まれます。 ただし、全体的な準備時間は、ページがホストされているサーバーによっても異なります。 ツールは、送信された URL が読み込まれるまで 60 秒待ちます。 この待ち時間を超えると、配達確認は失敗します。
* 組み合わせ配達確認の場合、いずれかの URL がキャプチャツールに応答しない場合、配達確認は失敗します。
* [!DNL Workfront Proof] は、ラスタライズの後、最大 195 インチの長さの Web ページをキャプチャします。 Web ページがこれより長い場合、配達確認は失敗します。
* テキスト抽出は、すべてのテキスト要素で使用できますが、画像として配置されたテキストは抽出されません。
* 配達確認でテキストのハイパーリンクをクリックでき、リンクされたページが新しいブラウザータブに開きます。
* style=&quot;display:block&quot;要素が `<a>` タグ。 ページデザインのこれらの部分を調整することをお勧めします。
* 最良の結果を得るには、ベストコーディングのベストプラクティスと認識済みの標準を使用してページを作成することをお勧めします。
