---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Salesforce モジュール
description: Adobe Workfront Fusion のシナリオでは、Salesforce を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# [!DNL Salesforce] モジュール

Adobe Workfront Fusion シナリオでは、 [!DNL Salesforce]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* の全エディションではありません [!DNL Salesforce] API にアクセスできます。 詳しくは、 [!DNL Salesforce] の API アクセスを使用するエディション [!DNL Salesforce] コミュニティサイト。
>* 次の [!DNL Salesforce] API( [!DNL Salesforce] API ドキュメント。 また、 [!DNL Salesforce] サービスの停止が発生する可能性がある API。
>

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
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

## 前提条件

使用する [!DNL Salesforce] モジュールの場合、 [!DNL Salesforce] アカウント

## 検索について [!DNL Salesforce] オブジェクト

オブジェクトを検索する場合は、個々の検索語を入力するか、ワイルドカードおよび演算子を使用してより複雑なクエリを作成できます。

* アスタリスクワイルドカード (\*) は、0 文字以上の文字の代わりに使用します。 たとえば、Ca\*を検索すると、Ca で始まる項目が検索されます
* 疑問符ワイルドカード (?) を 1 文字の代わりに使用します。 例えば、「Jo?n」を検索すると、「John」または「Joan」という語を含む項目が検索され、「Jon」は検索されません
* 完全に一致するフレーズを検索するには、引用符演算子 (&quot; &quot;) を使用します。 例：&quot;月曜の会議&quot;

検索の可能性について詳しくは、 [!DNL Salesforce] SOQL および SOSL に関する開発者向けドキュメント。

## [!DNL Salesforce] モジュールとそのフィールド

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

* [[!UICONTROL レコードを監視]](#watch-for-records)
* [[!UICONTROL 送信メッセージを見る]](#watch-outbound-messages)
* [[!UICONTROL フィールドを見る]](#watch-a-field)

#### [!UICONTROL レコードを監視]

このトリガーモジュールは、オブジェクト内のレコードが作成または更新されたときにシナリオを実行します。 このモジュールは、レコードまたはレコードに関連付けられているすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL の種類 ] </td> 
   <td> <p>タイプを選択 [!DNL Salesforce] レコードを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードフィールド ]</td> 
   <td>モジュールで監視するフィールドを選択します。 使用可能なフィールドは、レコードのタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードの最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ウォッチ ]</td> 
   <td> <p>選択したタイプの新しいレコードのみをシナリオで監視するか、選択したタイプの新しいレコードと、そのタイプのレコードに対するその他すべての変更をシナリオで監視するかを決定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 送信メッセージを見る]

このトリガーモジュールは、誰かがメッセージを送信したときにシナリオを実行します。 このモジュールは、レコードまたはレコードに関連付けられているすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールには、追加の設定が必要です。

1. 次に移動： [!DNL Salesforce] 設定ページを開きます。

   設定ページにアクセスするには、「[!UICONTROL 設定]」 [!DNL Salesforce] アカウント 次の [!DNL Salesforce] 設定ページで、「[!UICONTROL クイック検索/検索]「左側の棒。 「[!UICONTROL ワークフロールール].&quot;

1. クリック **[!UICONTROL ワークフロールール]**.
1. を [!UICONTROL ワークフロールール] 表示されるページで、 **[!UICONTROL 新規ルール]** ルールを適用するオブジェクトの種類 ( 例：[!UICONTROL 商談]&quot;商談レコードの更新を監視する場合は&quot;)。
1. クリック **[!UICONTROL 次へ]**.
1. ルール名、評価基準およびルール条件を設定し、「 **[!UICONTROL 保存]** および **[!UICONTROL 次へ]**.

1. クリック **[!UICONTROL 完了]**.
1. 新しく作成したワークフロールールで、 **[!UICONTROL 編集]**...
1. 次の **[!UICONTROL ワークフローアクションを追加]** ドロップダウンリストで、「 **[!UICONTROL 新しい送信メッセージ]**.

1. 新しいアウトバウンドメッセージに含める名前、説明、エンドポイント URL およびフィールドを指定し、「 **[!UICONTROL 保存]**.

   この **[!UICONTROL エンドポイント URL]** フィールドには、 [!DNL Salesforce] [!UICONTROL 送信メッセージ] in [!DNL Workfront Fusion].

1. 次で始まるシナリオを設定します： [!UICONTROL 送信メッセージ] イベント。

1. 次をクリック： **&lt;/>** アイコンをクリックし、指定した URL をコピーします。
1. に戻る **[!UICONTROL ワークフロールール]** ページで、新しく作成されたルールを探し、 **[!UICONTROL 有効化]**.

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>送信メッセージの監視に使用する Webhook を選択します。 ウェブフックを追加するには、 <strong>[!UICONTROL 追加 ]</strong> ウェブフックの名前と接続を入力します。</p> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion] への接続の作成 — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ] </td> 
   <td> <p>タイプを選択 [!DNL Salesforce] レコードを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フィールド ]</td> 
   <td> <p>モジュールが送信メッセージを監視するフィールドを選択します。 使用可能なフィールドは、レコードのタイプによって異なります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL フィールドを見る]*

このトリガーモジュールは、 [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ] </td> 
   <td> <p>モジュールが監視するフィールドが含まれているレコードのタイプを選択します。 [!UICONTROL Field History] がオンになっているレコードタイプを選択する必要があります。 [!DNL Salesforce] 設定。 詳しくは、 <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">フィールド履歴の追跡</a> 内 [!DNL Salesforce] ドキュメント。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フィールド ]</td> 
   <td> <p>モジュールで変更を監視するフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返すフィールドの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL 添付ファイル/ドキュメントをアップロード]](#upload-attachmentdocument)
* [[!UICONTROL 添付ファイル/ドキュメントをダウンロード]](#download-attachmentdocument)

#### [!UICONTROL レコードの作成]

このアクションモジュールは、オブジェクトに新しいレコードを作成します。

モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。 これにより、モジュールを設定する際にスクロールしなければならないフィールドの数が減ります。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL レコードタイプ ] </p> </td> 
   <td> <p>タイプを選択 [!DNL Salesforce] を記録します。 フィールドは、「[!UICONTROL レコードタイプ ]」フィールドで選択したレコードのタイプに基づいて使用できるようになります。 これらのフィールドは、 [!DNL Salesforce] API</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL マッピングするフィールドを選択 ]</td> 
   <td> <p>新しいレコードを作成する際にモジュールで設定するフィールドを選択します。 必須フィールドはリストの上部にあります。 </p> <p>選択したフィールドがこのフィールドの下に開きます。 これらのフィールドに値を入力できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、 [!DNL Salesforce].

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL レコードタイプ ]</td>
    <td>タイプを選択 [!DNL Salesforce] モジュールに [action].read を設定するレコードです。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL レコードフィールド ]</td>
    <td>モジュールが読み取るフィールドを選択します。 少なくとも 1 つのフィールドを選択する必要があります。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>一意の [!DNL Salesforce] モジュールが読み取るレコードの ID。</p> <p>ID を取得するには、 [!DNL Salesforce] オブジェクトを選択して、URL の末尾にある最後のスラッシュ (/) の後のテキストをコピーします。 例： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、オブジェクト内の既存のレコードを削除します。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードタイプ ] </td> 
   <td> <p>タイプを選択 [!DNL Salesforce] を記録します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>一意の [!DNL Salesforce] モジュールで削除するレコードの ID。</p> <p>ID を取得するには、 [!DNL Salesforce] オブジェクトを選択して、URL の末尾にある最後のスラッシュ (/) の後のテキストをコピーします。 例： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Salesforce] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Salesforce] モジュール。

このモジュールは、次の値を返します。

* **[!UICONTROL ステータスコード]** （数値）:HTTP リクエストの成功または失敗を示します。 これらはインターネット上で検索できる標準コードです。
* **[!UICONTROL ヘッダー]** （オブジェクト）:出力本文に関連しない応答/ステータスコードのより詳細なコンテキスト。 応答ヘッダーに表示されるすべてのヘッダーが応答ヘッダーではないので、役に立たないヘッダーも含まれている可能性があります。

  応答ヘッダーは、モジュールの設定時に選択した HTTP リクエストによって異なります。

* **[!UICONTROL 本文]** （オブジェクト）:モジュールの設定時に選択した HTTP リクエストに応じて、一部のデータを受け取る場合があります。 そのデータ ( [!UICONTROL GET] リクエストは、このオブジェクトに含まれます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>使用可能なエンドポイントの一覧については、 <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API 開発者ガイド</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code>. Workfront Fusion は、認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。次に例を示します。 <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** 次の API 呼び出しは、 [!DNL Salesforce] アカウント：
>
>* **URL**: `query`
>
>* **メソッド**: [!UICONTROL GET]
>
>* **クエリ文字列**:
>
>* **キー**: `q`
>
>* **値**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>検索結果は、モジュールの「出力」の「 **[!UICONTROL バンドル] > [!UICONTROL 本文] > [!UICONTROL レコード]**.
>
>この例では、6 人のユーザーが返されました。
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL 添付ファイル/ドキュメントをアップロード]

このアクションモジュールは、ファイルをアップロードし、指定したレコードに添付するか、ドキュメントをアップロードします。

このモジュールは、添付ファイルまたはドキュメントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アップロードのタイプ ]</td> 
   <td>モジュールで添付ファイルとドキュメントのどちらをアップロードするかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>添付ファイルのアップロード先のオブジェクトの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ]</td> 
   <td>モジュールにアップロードするファイルを含むフォルダーを選択します。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイル/ドキュメントをダウンロード]

このアクションモジュールは、レコードからドキュメントまたは添付ファイルをダウンロードします。

レコードの ID と、必要なダウンロードのタイプを指定します。

このモジュールは、添付ファイルまたはドキュメントの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL ダウンロードのタイプ ]</td>
    <td> <p>Salesforce からダウンロードするファイルの種類を指定します。</p> 
     <ul> 
      <li>[!UICONTROL 添付ファイル ]</li> 
      <li>[!UICONTROL ドキュメント ]</li> 
      <li>[!UICONTROL ContentDocument] ( これは、 [!DNL Saleforce CRM Content] または [!DNL Salesforce Files].)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL 添付ファイル ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>一意の [!DNL Salesforce] モジュールをダウンロードするレコードの ID。</p> <p>ID を取得するには、 [!DNL Salesforce] オブジェクトを選択して、URL の末尾にある最後のスラッシュ (/) の後のテキストをコピーします。 例： <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL レコードの更新]

このアクションモジュールは、オブジェクト内のレコードを編集します。

モジュールを使用すると、モジュールで使用可能なオブジェクトのフィールドを選択できます。 これにより、モジュールを設定する際にスクロールしなければならないフィールドの数が減ります。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>更新するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL レコードタイプ ] </p> </td> 
   <td> <p>タイプを選択 [!DNL Salesforce] を記録します。 フィールドは、「レコードタイプ」フィールドで選択したレコードのタイプに基づいて使用可能になります。 これらのフィールドは、 [!DNL Salesforce] API</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL マッピングするフィールドを選択 ]</td> 
   <td> <p>新しいレコードを作成する際にモジュールで設定するフィールドを選択します。 必須フィールドはリストの上部にあります。 </p> <p>選択したフィールドがこのフィールドの下に開きます。 これらのフィールドに値を入力できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL クエリで検索]

この検索モジュールは、 [!DNL Salesforce] 指定した検索クエリに一致する この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索タイプ ]</td> 
   <td> <p>モジュールで実行する検索のタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL シンプル ]</p> </li> 
     <li> <p>[!UICONTROL SOSL(Salesforce Object Search Language)] の使用</p> </li> 
     <li> <p>[!UICONTROL SOQL (Salesforce Object Query Language)) を使用 ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL の種類 ] </p> </td> 
   <td> <p>簡易検索タイプを選択した場合、 [!DNL Salesforce] を記録します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ ] / [!UICONTROL SOSL クエリ ] / [!UICONTROL SOQL クエリ ]</td> 
   <td> <p>検索するクエリを入力します。</p> <p>SOSL の詳細については、 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce オブジェクト検索言語 (SOSL)</a> 内 [!DNL Salesforce] ドキュメント。</p> <p>SOQL について詳しくは、 <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce オブジェクトクエリ言語 (SOQL)</a> 内 [!DNL Salesforce] ドキュメント。</p> <p>注意：パラメーターの値 <code>RETURNING </code>は、モジュールの出力に影響を与えます。 次を使用する場合、 <code>LIMIT</code>, [!DNL Fusion] [!UICONTROL レコードの最大数 ] フィールドの設定が無視されます。 制限を設定しない場合、Fusion は値 [!UICONTROL LIMIT = Maximal count of records] を挿入します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコードの最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 検索]

このアクションモジュールは、指定された条件を満たすすべてのレコードを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>接続方法 [!DNL Salesforce] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成[!DNL  Adobe Workfront Fusion]  — 基本手順</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ]</td> 
   <td> <p>検索するオブジェクトのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索条件 ]</td> 
   <td>検索するフィールド、クエリで使用する演算子、および「 」フィールドで検索する値を選択します。 AND または OR を使用してクエリを接続できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結果セット ]</td> 
   <td>モジュールで「All Matching Records」を返すか、「First Matching Records」のみを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最大 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールで取得するレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
