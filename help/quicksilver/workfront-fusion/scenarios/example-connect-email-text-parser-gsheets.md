---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 「Adobe Workfront Fusion シナリオの例：メール、テキストパーサー および Google シートを接続」
description: このシナリオでは、すべてのメールメッセージのログを作成し、スプレッドシートでさらにアクションを行うためにタグ付けします。スプレッドシート内の 2 つの異なるテーブルに、検索パターンとして正規表現（Regex）を使用してメールの本文を取り込みます。第 1 のパターンは、あるフレーズを検索し、第 2 のパターンは、同じフレーズとメールアドレスを検索します。
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1214'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] シナリオの例：メール、[!UICONTROL テキストパーサー]、および [!DNL Google Sheets] を接続

このシナリオでは、すべてのメールメッセージのログを作成し、スプレッドシートでさらにアクションを行うためにタグ付けします。スプレッドシート内の 2 つの異なるテーブルに、検索パターンとして正規表現（Regex）を使用してメールの本文を取り込みます。第 1 のパターンは、あるフレーズを検索し、第 2 のパターンは、同じフレーズとメールアドレスを検索します。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront]プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

このチュートリアルでは、正規表現に関する基本的な知識が必要です。正規表現については、[https://regexone.com](https://regexone.com/) を参照してください。

最初のモジュールを追加し、設定します。

1. メールを検索して、トリガーとして&#x200B;**[!UICONTROL メールを監視]**&#x200B;を選択します。

   >[!NOTE]
   >
   > メールモジュールを使用して [!DNL Google] アカウントを接続することもできますが、[!DNL Gmail] モジュールを使うこともできます。

1. [!DNL Google] アカウントまたはその他の IMAP ベースのメールクライアント（[!DNL Outlook]）を接続します。
1. 接続が完了したら、[!UICONTROL インボックス]など、受信メールを監視したいフォルダーを選択します。
1. [!UICONTROL 条件]の下で、**[!UICONTROL すべてのメール]**&#x200B;を選択します（または、読み取り済みか、未読のメールで絞り込みます）。

   取得したメールを既読または未読としてマークすることも選択できます。

1. [!UICONTROL 結果の最大数]を 1 に設定します。

   ![](assets/save-max-as-1-350x304.png)

   これは、受信するメッセージの量に応じて変更できます。ただし、低い値を設定し、シナリオを実行する頻度を増やすことをお勧めします。

1. 下部にある「**[!UICONTROL 詳細設定を表示]**」をクリックします。

   ![](assets/show-adv-settings-350x332.png)

1. [!UICONTROL 送信者のアドレス]、[!UICONTROL 件名]、および[!UICONTROL フレーズ]でメールをフィルタリングします。

   これにより、関連するメールのみを視聴できます。この例では、件名フィルターのみを追加し、残りの 2 つは空白のままにします。

   >[!NOTE]
   >
   >[!UICONTROL 一致パターン]イテレーターと検索パターンとしての正規表現（Regex）により、メール内のフレーズを検索するルーターを追加します。これにより、マルチユーティリティシナリオを構築することもできます。

1. 設定が完了し、メールの監視を開始する場所を指定するよう求められたら、「**[!DNL From now on]**」をクリックします。

   ![](assets/from-now-on-350x236.png)

1. [[!UICONTROL フローコントロール]を検索して[!UICONTROL ルーター]](#search-for-flow-control-and-add-a-router)を追加に進みます。

## [!UICONTROL フローコントロール]を検索して[!UICONTROL ルーター]を追加

1. ルーターを任意のモジュールの後に追加して、データを分割または複製してから次のモジュールに送信します。

   ここでは、[!DNL Google Sheet] でメールの本文テキストを 2 つの異なる表に送信するために[!UICONTROL ルーター]を使用しました。

   ![](assets/search-for-flow-control-350x220.png)

## [!UICONTROL テキストパーサー]モジュールを使用

1. [!UICONTROL 一致パターン]変換サービスを追加して、メール内のフレーズを検索します。

   すべての受信メールで、「[!UICONTROL テキストパーサーモジュール]」というフレーズを検索し、このフレーズに一致する本文テキストと送信者名を取り込みます。

   1. パターンを正規表現として記述します。

      text\sparser\smodule

   1. （オプション）その他のパターンオプションを使用します。

      ![](assets/pattern-350x318.png)

      複数行は、テキストが複数行に分かれ、各行でパターンを検索する必要がある場合に便利です。このチュートリアルでは、メールの本文テキスト全体のパターンを検索する必要があるので、チェックを外したままにします。

   1. [!UICONTROL テキスト]フィールドで、リスト内の「**テキストコンテンツ**」属性をクリックします。

      ![](assets/text-content-350x264.png)

      これは、パターンを検索するメール本文のテキストを保存する属性です。

1. 同じフレーズとメールアドレスを検索する別の[!UICONTROL 一致パターン]を追加します。

   これは、複数のユーザーを持つ顧客アカウントがある場合に特に便利です。時間を節約するために、作成した[!UICONTROL テキストパーサー]モジュールのクローンを作成し、ルーターにリンクできます。

   ![](assets/clone.png)

1. パターンを次のように編集します。

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   このパターンは、「[!UICONTROL テキストパーサーモジュール]」および john.doe@gmail.com のようなメールアドレスのフレーズを検索し、そのメールアドレスのみを返します。

   >[!NOTE]
   >
   >受け入れるメールアドレスの仕様に従って正規表現を記述することが重要ですが、上記の正規表現は、ほとんどの標準的なメールアドレスを処理します。

   * メールアドレスのみを検索する場合は、次の正規表現を使用できます。

     ([\w.-]+@[\w.-]+)

   * また、次の正規表現を使用して、電話番号のみを検索することもできます。

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
上記のパターンには、電話番号が書き込まれる最も一般的な形式があります。

   パターンをテストするには、Flavor として [!DNL javascript] を持つ [[!DNL https://regex101.com]](https://regex101.com/) を使用することをお勧めします。

   残りの設定は、以前の設定と同じです。

## [!DNL Google Sheets] モジュールを追加

[!DNL Sheets] の場合、最初に必要なヘッダーを含むスプレッドシートを作成する必要があります。

1. ユーザーデータを取り込む列を持つスプレッドシートを作成します（既存のファイルも自由にご使用ください）。

   例えば、「メールデータ：サポートチケット」というスプレッドシートを作成し、送信者名、送信者のメール、メールの内容を列として作成します。ワークシートに「次を含む：テキストパーサーモジュール」という名前を付けます。

1. 「**[!UICONTROL 行を追加]**」アクションを持つ [!UICONTROL Google Sheets] モジュールを追加します。

   ![](assets/add-a-row-350x174.png)

1. [!DNL Google] アカウントを接続します（まだ接続していない場合）。以前に作成したファイル、データを取り込むワークシートの順に選択します。

   設定は次のようになります。

   ![](assets/connect-google-acct-350x279.png)

1. 関連するフィールド（列）の属性をマッピングして、モジュールの設定を完了します。

   ![](assets/map-attributes-350x282.png)

1. 作成したモジュールのクローンを作成し、2 番目の[!UICONTROL テキストパーサー]モジュールにリンクします。

   1. スプレッドシートに移動し、以前に作成したワークシートを複製して、名前を付けます。

      例えば、「次を含む：テキストパーサーモジュールとメール」という名前を付けます。

   1. メール本文に含まれるメールアドレスを保存する別の列を追加します。

      例えば、「共有のメールアドレス」という名前を付けます。

   1. クローンを作成した [!DNL Google Sheets] モジュールをクリックし、設定を行います。
   1. ワークシートを、先ほど作成した新しいワークシートに変更します。
   1. [!UICONTROL 一致パターン]モジュール（$1）から、メールアドレス（共有されたメールアドレス）を保存する列に出力をマッピングします。

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. **[!UICONTROL OK]** をクリックし、シナリオを保存して、テストの実行に使用します。

      次のように、2 通の別々のメールを、結び付けられたメールアドレスに送信する必要があります。

      * 「[!UICONTROL テキストパーサーモジュール]」というフレーズを含む（メールアドレスは含まれません）

        ![](assets/text-parser-module-350x103.png)

      * 上記のフレーズとメールアドレスを含む

        ![](assets/above-phrase-and-email-350x106.png)

        設定にエラーがない場合は、最初のワークシートが「[!UICONTROL テキストパーサーモジュール]」というフレーズを含むすべてのメールをキャプチャしており、2 番目のワークシートでは「[!UICONTROL テキストパーサーモジュール]」というフレーズとメールアドレスを含むメールのみをキャプチャしていることが確認できます。以下のスクリーンショットを参照してください。

        ワークシート 1：

        ![](assets/worksheet-1-350x57.png)

        ワークシート 2：

        ![](assets/worksheet-2-350x41.png)

## リソース

* 正規表現について学ぶ[無料の演習](https://regexone.com/)
* 正規表現の使用した[電話番号の照合を学ぶ](https://regexone.com/problem/matching_phone_numbers)
* 正規表現を使用した[メールの照合を学ぶ](https://regexone.com/problem/matching_emails)
* [正規表現をテスト](https://regex101.com/)
