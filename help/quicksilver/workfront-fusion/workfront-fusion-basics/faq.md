---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion FAQ
description: この記事では、 [!DNL Adobe Workfront Fusion]（Fusion ワークフローで一般的に使用されるオブジェクトに関する情報を含む）
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# Adobe Workfront Fusion FAQ

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## シナリオとは

### 回答

シナリオは、が実行する一連の手順を定義します [!DNL Adobe Workfront Fusion]. 各シナリオでは、データソース、データの処理方法、使用するデータと無視するデータを指定します。 [!DNL Workfront Fusion] では、必要なだけ複雑なシナリオを作成できます。最も高度なシナリオが可能です。

詳しくは、 [でのプラクティス統合シナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## 1 つのシナリオで複数のモジュールを使用できますか？ それとも単なるトリガーと行動？

### 回答

1 つのシナリオで必要な数のモジュールを使用できます。 独立したルートを作成し、それらを通るデータを指定できます。 また、個々のアクションから返された結果を使用して、次のアクションに渡すこともできます。

## 可能 [!DNL Workfront Fusion] ファイルを操作しますか？

### 回答

はい。使用 [!DNL Workfront Fusion]、ファイルの受信、保存、変換、変換、暗号化などをおこなうことができます。 さらに [!DNL Workfront Fusion] は、ユーザーがファイルに含まれるデータを効果的かつクリエイティブに操作できるように設計された、様々な組み込み機能を提供します。

詳しくは、 [でのファイルのマッピングについて [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## 放したらどうなる？ [!DNL Workfront Fusion] 複数の添付ファイルを含む電子メールを処理しますか？

### 回答

次の [!UICONTROL 電子メール] モジュール [!UICONTROL 添付ファイルの取得]の場合、各添付ファイルは、シナリオ内の残りのモジュールを通じて個別に送信されます。 同様のモジュールは、複数のファイルを一度に受け取る他のアプリでも使用できます。

詳しくは、 [[!UICONTROL 電子メール] モジュール](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## 一部のトリガーでは、シナリオを即座に実行できます。 「即時」とは何を意味しますか。

### 回答

一般的なシナリオは、指定したスケジュールに従って、間隔をおいて実行されます（例えば、毎時、5 分ごと、月に 1 回など）。 特定のサービスからデータを受け取った直後にシナリオを開始できる、インスタントトリガー（Web フック）と呼ばれる特別なトリガーがあります。 インスタントトリガーは非常に役に立つ場合があります。 可能な限り使用することをお勧めします。 操作数を減らすのに役立ちます。 受信したデータは、次にスケジュールされた実行を待たずに、即座に処理されます。 例えば、 [!DNL Google Sheets] モジュール [!UICONTROL 変更を監視] は、セルの更新直後にシナリオを開始します。

## 集約とは

### 回答

An [!UICONTROL 集約] データを 1 つのコレクションに結合します。 例えば、ファイルを圧縮して zip アーカイブにし、電子メールの添付ファイルとして送信する場合です。

詳しくは、 [[!UICONTROL 集約] モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 操作とは

### 回答

操作とは、モジュールが実行する任意のタスクです。 操作は、例えば、トリガーが実行されるたびに、アクションがタスクを実行するたびに発生します。

## データ転送とは

### 回答

データ転送は、シナリオを通じて転送されたデータの量を指します。 例えば、FTP から 100 KB の画像を取得し、そのサイズを 50 KB に減らして、両方の画像を次の場所に保存するシナリオがあるとします。 [!DNL Dropbox]. このシナリオで使用されるデータの量は 250 KB です。

## 接続とは

### 回答

接続は、 [!DNL Workfront Fusion] アカウントと、使用するサードパーティのサービス。 シナリオの編集時に、接続を簡単に作成できます。 接続を追加するには、 **[!UICONTROL 追加]** ボタンをクリックし、手順に従って手順を進めます。

詳しくは、 [接続について [!DNL Adobe Workfront Fusion] アプリまたはサービスに](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
