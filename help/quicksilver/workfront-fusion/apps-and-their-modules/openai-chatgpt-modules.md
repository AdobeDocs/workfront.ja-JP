---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: OpenAI(ChatGPT) モジュール
description: Adobe Workfront Fusion シナリオでは、OpenAIT(ChatGPT) を使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続することができます。
author: Becky
feature: Workfront Fusion
source-git-commit: aa672a81b0899c45c1c7e6abba03b6d975dc7017
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 28%

---

# [!DNL OpenAI (ChatGPT & DALL-E)] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL OpenAI (ChatGPT & DALL-E)] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

次を使用するには： [!DNL OpenAI (ChatGPT & DALL-E)] モジュールの場合は、 [!DNL OpenAI] アカウント（API キーと組織 ID を含む）。

## [!DNL OpenAI (ChatGPT & DALL-E)] を [!DNL Workfront Fusion] に接続

[!DNL OpenAI (ChatGPT & DALL-E)] アカウントへの接続を、[!DNL OpenAI (ChatGPT & DALL-E)] モジュール内から直接作成できます。

1. 任意の [!DNL OpenAI (ChatGPT & DALL-E)] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>新しい接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>API キーは OpenAI のユーザー設定で見つけることができます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 組織 ID] </td> 
      <td>組織 ID は、OpenAI の組織設定ページで確認できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。


## [!DNL OpenAI (ChatGPT & DALL-E)] モジュールとそのフィールド

[!DNL OpenAI (ChatGPT & DALL-E)] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL OpenAI (ChatGPT & DALL-E)] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

### 完了の作成

>[!IMPORTANT]
>
>このモジュールは非推奨です。

<!--

This action module creates a completion for the provided prompt or chat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Enter or map the ID of the model to use. You can use the Get models module to see all of your available models. </td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating completions in the <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### モデレートの作成

このアクションモジュールは、テキストが OpenAI のコンテンツポリシーに違反しているかどうかを判定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> 含めるテキストのサンプルごとに、 <b>項目を追加</b> テキストを入力またはマッピングします。 テキストサンプル全体を含めます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL モデル ]</td> 
   <td> 使用するモデルの ID を入力またはマッピングします。 モデルの取得モジュールを使用して、使用可能なすべてのモデルを表示できます。 </td> 
  </tr> 
 </tbody> 
</table>

### 編集の作成

このアクションモジュールは、指示に従って、指定したプロンプトの編集バージョンを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL モデル ]</td> 
   <td> 使用するモデルの ID を入力またはマッピングします。 モデルの取得モジュールを使用して、使用可能なすべてのモデルを表示できます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> 編集するテキストを入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 命令 ]</td> 
   <td> 編集の手順を入力またはマッピングします。 例： "スペルミスを修正します。" </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 詳細設定 ]</td> 
   <td> <p>このモジュールのオプションの詳細設定について詳しくは、 <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">OpenAI API ドキュメント</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 埋め込みの作成

このアクションモジュールは、入力テキストを表す埋め込みベクトルを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL モデル ]</td> 
   <td> 使用するモデルの ID を入力またはマッピングします。 モデルの取得モジュールを使用して、使用可能なすべてのモデルを表示できます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 埋め込むテキストを入力 ]</td> 
   <td> 埋め込むテキストを入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User ID]</td> 
   <td> OpenAI が不正使用を監視および検出するのに役立つ、エンドユーザーを表す一意の識別子を入力またはマッピングします </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> 各シナリオの実行サイクル中に、モジュールが操作する最大編集数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### チャット完了を作成

会話を説明するメッセージのリストを指定すると、このアクションモジュールは応答を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL モデル ]</td> 
   <td> 使用するモデルの ID を入力またはマッピングします。 モデルの取得モジュールを使用して、使用可能なすべてのモデルを表示できます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ]</td> 
   <td>メッセージは、これまでの会話を説明します。 追加するメッセージごとに、 <b>項目を追加</b> をクリックし、次の情報を入力します。
   <ul>
   <li> <b>役割</b>：このメッセージの作成者の役割を選択します。</li>
   <li> <b>コンテンツ</b>：このメッセージのコンテンツを入力またはマッピングします。</li>
   <li> <b>名前</b>：このメッセージの作成者の名前を入力またはマッピングします。 名前には、大文字と小文字、数字、アンダースコアを含めることができます。 名前の最大長は 64 文字です。</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 詳細設定 ]</td> 
   <td> <p>このモジュールのオプションの詳細設定については、 <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">OpenAI API ドキュメント</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### 画像を生成

このアクションモジュールは、Dall-E モデルを使用して画像を生成または操作します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 目的の画像のテキスト説明 ]</td> 
   <td> 目的の画像の説明を入力またはマッピングします。 説明の長さの上限は 1,000 文字です。 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL 詳細設定 ]</td> 
   <td> <p>このモジュールのオプションの詳細設定について詳しくは、 <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">OpenAI API ドキュメント</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### モデルの取得

このモジュールは、OpenAI API で使用できる様々なモデルの一覧と説明を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> すべてのモデルのリストを取得するか、特定のモデルを取得するかを選択します。
    <ul>
    <li><p><b>モデルのリスト </b></p><p>このアクションには、現在使用可能なモデルが一覧表示され、所有者や可用性など、各モデルに関する基本情報が提供されます。</p></li>
    <li><p><b>モデルを取得 </b></p><p>取得するモデルの ID を入力またはマッピングします。 </p></li>
   </ul>
 </td> 
 </tbody> 
</table>

### カスタム API 呼び出しの実行

このアクションは、OpenAI API へのカスタム HTTP リクエストをモジュール化します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>相対パスを入力 <code>https://api.openai.com/v1/</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件文を JSON で使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### ファイルを管理

このアクションモジュールは、ファイルまたはファイルコンテンツをリスト、削除、取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td> 実行するアクションを選択します。 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> ファイルを削除する場合、またはファイルまたはファイルの内容を取得する場合は、ファイルの ID を入力またはマッピングします。 
  </tr> 
</tbody>
</table>

### 微調整を管理

微調整ジョブを管理して、特定のトレーニングデータに合わせてモデルを調整します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続方法については、 [!DNL OpenAI (ChatGPT & DALL-E)] Workfront Fusion へのアカウントについては、 <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">接続中 [!DNL OpenAI (ChatGPT & DALL-E)] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 操作を選択 ]</td> 
   <td> 実行するアクションを選択します。
   <ul>
   <li><p>データセットからのモデルの微調整</p><p>目的の画像の説明を入力またはマッピングします。</p>
     <li><p>微調整ジョブに関する情報を取得します</p><p>ジョブの ID を入力またはマッピングします。</p>
   <li><p>微調整ジョブのキャンセル</p><p>ジョブの ID を入力またはマッピングします。</p>
   <li><p>微調整ジョブのキャンセル</p><p>ジョブの ID を入力またはマッピングします。</p>
   <li><p>微調整ジョブのステータスの更新を取得します</p><p>ジョブの ID を入力またはマッピングし、これらの更新をストリーミングするかどうかを選択します。</p>
   <li><p>微調整されたモデルを削除する</p><p>削除するモデルの ID を入力またはマッピングします。</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> ファイルを削除する場合、またはファイルまたはファイルの内容を取得する場合は、ファイルの ID を入力またはマッピングします。 
  </tr> 
</tbody>

