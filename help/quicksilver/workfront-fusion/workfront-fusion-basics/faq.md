---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion FAQ
description: この記事では、Fusion ワークフローで一般的に使用されるオブジェクトについての情報など、 [!DNL Adobe Workfront Fusion] に関するよくある質問を紹介します。
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: ht
source-wordcount: '668'
ht-degree: 100%

---

# Adobe Workfront Fusion FAQ

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## シナリオとは何ですか？

### 回答

シナリオは、[!DNL Adobe Workfront Fusion] によって実行される一連の手順を定義するものです。各シナリオでは、データソース、データの処理方法、使用するデータと無視するデータを指定します。[!DNL Workfront Fusion] では必要に応じて、複雑なシナリオや非常に高度なシナリオを作成できます。

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md) での練習用統合シナリオの作成を参照してください。

## 1 つのシナリオで複数のモジュールを使用できますか？使用できるのはトリガーとアクションのみですか？

### 回答

必要な数のモジュールを 1 つのシナリオで使用できます。独立したルートを作成し、そのルートを移動するデータを指定できます。また、個々のアクションから返された結果を使用して、次のアクションに渡すこともできます。

## [!DNL Workfront Fusion] ではファイルを操作できますか？

### 回答

はい。[!DNL Workfront Fusion] を使用して、ファイルの受信、保存、変換、暗号化などを行うことができます。さらに [!DNL Workfront Fusion] は、ユーザーがファイルに含まれるデータを効果的かつクリエイティブに操作できるように設計された、様々なビルトイン機能を備えています。

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md) でのファイルのマッピングについてを参照してください。

## [!DNL Workfront Fusion] で複数の添付ファイルを含むメールを処理するとどうなりますか？

### 回答

[!UICONTROL メール]モジュールの[!UICONTROL 添付ファイルの取得]を使用すると、各添付ファイルは、シナリオ内の残りのモジュールを通じて個別に送信されます。複数のファイルを一度に受け取る他のアプリでも、同様のモジュールを使用できます。

詳しくは、[[!UICONTROL メール]モジュール](../../workfront-fusion/apps-and-their-modules/email-modules.md)を参照してください。

## 一部のトリガーではシナリオを即座に実行できます。「即座」とは何を意味しますか？

### 回答

一般的なシナリオは、指定したスケジュールに従って定期的に実行されます（例えば、1 時間ごと、5 分ごと、1 ヶ月に 1 回など）。インスタントトリガー（Web フック）と呼ばれる特別なトリガーがあり、特定のサービスからデータを受け取った直後にシナリオを開始できます。インスタントトリガーは非常に便利なので、。可能な限り使用することをお勧めします。そうすることで、操作の数を減らすことができます。受信したデータは、次にスケジュールされた実行を待たずに、すぐに処理されます。例えば、[!DNL Google Sheets] モジュールの[!UICONTROL 変更の監視]では、セルの更新後すぐにシナリオが開始されます。

## アグリゲータとはどのようなものですか？

### 回答

[!UICONTROL アグリゲータ]は、データを 1 つのコレクションに結合するものです。例えば、ファイルを zip アーカイブに圧縮して、メールの添付ファイルとして送信するなどです。

詳しくは、[[!UICONTROL  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md) のアグリゲータ]モジュールを参照してください。

## 操作とは何ですか？

### 回答

操作とは、モジュールが実行する任意のタスクです。例えば、トリガーが実行されたり、アクションがタスクを実行したりするたびに、操作が発生します。

## データ転送量とは何ですか？

### 回答

データ転送量とは、シナリオを通じて転送されたデータの量を指します。例えば、FTP から 100 KB の画像を取得し、そのサイズを 50 KB に減らして両方の画像を [!DNL Dropbox] に保存するシナリオがあるとします。このシナリオで使用されるデータの量は 250 KB です。

## 接続とは何ですか？

### 回答

接続とは、[!DNL Workfront Fusion] アカウントと、使用するサードパーティのサービスとの間のリンクです。接続は、シナリオの編集時に簡単に作成できます。接続を追加するには、モジュール設定の「**[!UICONTROL 追加]**」ボタンをクリックし、段階的な手順に従います。

詳しくは、[アプリまたはサービスへの  [!DNL Adobe Workfront Fusion]  の接続について](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)を参照してください。
