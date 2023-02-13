---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: データドグモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、データドグを使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# [!DNL Datadog] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Datadog]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Datadog] モジュールの場合、 [!DNL Datadog] アカウント

## 接続 [!DNL Datadog] から [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### API キーとアプリケーションキーの取得 {#retrieve-your-api-key-and-application-key}

次の手順で [!DNL Datadog] アカウント [!DNL Workfront Fusion] API キーとアプリケーションキーを [!DNL Datadog] アカウント

1. にログインします。 [!DNL Datadog] アカウント
1. 左側のナビゲーションパネルで、 **[!UICONTROL 統合]**&#x200B;を選択し、「 **[!UICONTROL API]**.
1. メイン画面で、 **[!UICONTROL API キー]**.
1. 紫色のバーにマウスポインターを置くと、API キーが表示されます。
1. API キーを安全な場所にコピーします。
1. メイン画面で、 **[!UICONTROL アプリケーションキー]**.
1. 紫色のバーにマウスポインターを置くと、アプリケーションキーが表示されます。
1. アプリケーションキーを安全な場所にコピーします。

### への接続の作成 [!DNL Datadog] in [!DNL Workfront Fusion]

次に、 [!DNL Datadog] 内部から直接アカウントを取得する [!UICONTROL データ] モジュール。

1. 任意の [!UICONTROL データ] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. モジュールのフィールドに次のように入力します。

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 接続タイプ ]</td> 
      <td> <p> [!UICONTROL [!DNL Datadog] への完全なアクセス権を取得するアプリケーション ] オプション [!DNL Datadog] API</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 接続名 ]</td> 
      <td> <p> 接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ドメイン ] </td> 
      <td> <p>接続するドメイン（米国または EU）を選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API キー ]</td> 
      <td> <p> を入力します。 [!DNL Datadog] API キー。 </p> <p>API キーの取得手順については、 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API キーとアプリケーションキーの取得</a> 」を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL アプリケーションキー ]</td> 
      <td> <p> を入力します。 [!DNL Datadog] アプリケーションキー。 </p> <p>アプリケーションキーの取得手順については、 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API キーとアプリケーションキーの取得</a> 」を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Datadog] モジュールとそのフィールド

設定時に [!DNL Datadog] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Datadog] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### アクション

* [[!UICONTROL 時系列ポイントの投稿]](#post-timeseries-points)
* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)

#### [!UICONTROL 時系列ポイントの投稿]

モジュールを使用すると、グラフ化可能な時系列データを投稿できます [!DNL Datadog]のダッシュボード。

圧縮ペイロードの上限は 3.2 MB(3200000) で、圧縮解除ペイロードの場合は 62 MB(62914560) です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Datadog] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">接続 [!DNL Datadog] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シリーズ ]</td> 
   <td> <p>送信先の時系列を追加します [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 指標 ]</strong> </p> <p>時系列の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL の種類 ]</strong> </p> <p>指標のタイプを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 間隔 ]</strong> </p> <p> 指標のタイプがレートまたはカウントの場合は、対応する間隔を定義します。</p> </li> 
     <li> <p><strong>[!UICONTROL ポイント ]</strong> </p> <p>指標に関連するポイントを追加します。</p> <p>これは、ポイントの JSON 配列です。 各ポイントの形式は次のとおりです。 <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>メモ:  <p>タイムスタンプは秒単位で指定する必要があります。</p> <p>タイムスタンプは最新である必要があります。 「現在」は、10 分以内または過去 1 時間以上と定義されます。</p> <p> 数値の形式は、浮動小数値にする必要があります。</p> </p> <p>このフィールドには少なくとも 1 つの項目を含める必要があります。</p> </li> 
     <li> <p><strong>[!UICONTROL ホスト ]</strong> </p> <p>指標を生成したホストの名前を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Datadog] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">接続 [!DNL Datadog] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://api.datadoghq.com/api/</code>. 例:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は、認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
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

**例：** 次の API 呼び出しは、 [!DNL Datadog] アカウント：

URL: `/v1/dashboard`

メソッド: `GET`

![](assets/datadog-api-example.png)

結果は、モジュールの出力（Bundle/Body/ダッシュボード）に表示されます。

この例では、3 つのダッシュボードが返されました。

![](assets/datadog-api-response-example.png)
