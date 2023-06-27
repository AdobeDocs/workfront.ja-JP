---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Azure DevOps モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Azure DevOps]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1797'
ht-degree: 0%

---

# [!DNL Azure DevOps] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Azure DevOps]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Azure DevOps] モジュールの場合、 [!DNL Azure] DevOps アカウント。

## 接続 [!DNL Azure DevOps] から [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. を追加します。 [!DNL Azure DevOps] モジュールをシナリオに追加します。
1. クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 内 [!UICONTROL 接続タイプ] フィールド、選択 **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >この [!UICONTROL [!DNL Azure DevOps] （すべてのスコープをリクエスト）] 接続タイプは近い将来非推奨となります。 したがって、使用はお勧めしません。

1. 次のフィールドに入力します。

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL 接続名 ]</td>
            <td>作成する接続の名前を入力します。</td>
        </tr>
      <tr>
            <td>[!UICONTROL 組織 ]</td>
            <td>作成した組織の名前を入力します。 [!DNL Azure DevOps] アプリケーション。</td>
        </tr>
    </table>

1. クリック **[!UICONTROL 続行]** 接続の設定を完了し、シナリオの作成を続行するには、次の手順に従います。

## [!UICONTROL Azure DevOps] モジュールとそのフィールド

設定時に [!DNL Azure DevOps] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Azure DevOps] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL 作業項目の監視]

このインスタントトリガーモジュールは、でレコードが追加、更新、または削除された場合にシナリオを実行します [!UICONTROL Azure DevOps].

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>モジュールの Webhook を選択または追加します。</p> <p>トリガーモジュールの Web フックの詳細については、 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">のインスタントトリガー（Web フック） [!DNL Adobe Workfront Fusion]</a>.</p> <p>Webhook の作成方法について詳しくは、 <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">ウェブフック</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [カスタム API 呼び出し](#custom-api-call)
* [レコードを読み取り](#read-record)
* [レコードの作成](#create-a-record)
* [作業項目の更新](#update-a-work-item)
* [[!UICONTROL 添付ファイルのアップロード]](#upload-an-attachment)
* [添付ファイルのダウンロード](#download-an-attachment)
* [作業項目をリンク]([!UICONTROL #link-work-items])

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Azure DevOps] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Azure DevOps] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ベース URL]</td> 
   <td> <p>の [!DNL Azure DevOps] アカウント</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 相対 URL]</td> 
   <td> <p>この API 呼び出しの接続先となる相対 URL を入力します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API バージョン ]</td> 
   <td>のバージョンを選択またはマッピング [!DNL Azure DevOps] この API 呼び出しの接続先となる API。 バージョンが選択されていない場合、 [!DNL Workfront Fusion] 接続先 [!DNL Azure DevOps] API バージョン 5.1。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> </td> 
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

#### [!UICONTROL レコードを読み取り]

このアクションモジュールは、 [!DNL Azure DevOps].

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>プロジェクトを読み取るか、作業項目を読み取るかを選択します</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL プロジェクト ]</strong>:読み取るプロジェクトを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 作業項目 ]</strong>:読み取る作業項目を含むプロジェクトを選択し、作業項目のタイプを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。 使用可能なフィールドは、作業項目のタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>読み取るレコードの ID を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの作成]

このアクションモジュールは、新しいプロジェクトまたは作業項目を作成します。

モジュールは、新しく作成された作業項目のオブジェクト ID、または新しく作成されたプロジェクトの URL とステータスコードを出力します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>作業項目を作成するか、プロジェクトを作成するかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL プロジェクト ]</strong> </p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL 名前 ]</strong>：新しいプロジェクトの名前を入力またはマッピングします。</p> </li> 
       <li> <p><strong>[!UICONTROL 説明 ]</strong>：新しいプロジェクトの説明を入力またはマッピングします。 </p> </li> 
       <li> <p><strong>[!UICONTROL 表示 ]</strong>:プロジェクトを公開または非公開にするかを選択します。 ユーザーが非公開プロジェクトとやり取りするには、組織にサインインし、プロジェクトへのアクセス権を付与されている必要があります。 公開プロジェクトは、組織にサインインしていないユーザーには表示されます。</p> </li> 
       <li> <p><strong>[!UICONTROL バージョン管理 ]</strong>:プロジェクトで使用するかどうかを選択します [!DNL Git] または [!UICONTROL Team Foundation Version Control (TFCV)] のバージョン管理。</p> </li> 
       <li> <p><strong>[!UICONTROL 作業項目プロセス ]</strong>:プロジェクトに使用する作業プロセスを選択します。 [!UICONTROL Basic]、[!UICONTROL Scrum]、[!UICONTROL Capability Muraty Model Integration(CMMI)]、[!UICONTROL Agile] を選択できます。</p> <p>詳しくは、 [!DNL Azure DevOps] プロセスについては、 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">プロセスを選択</a> 内 [!DNL Azure DevOps] ドキュメント。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL 作業項目 ]</strong> </p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL プロジェクト ]</strong>:作業項目を作成するプロジェクトを選択します。</p> </li> 
       <li> <p><strong>[!UICONTROL 作業項目タイプ ]</strong>:作成する作業項目のタイプを選択します。</p> </li> 
       <li> <p><strong>[!UICONTROL その他のフィールド ]</strong>：これらのフィールドには、特定のプロパティに対して作業項目に含める値を入力します。 使用可能なフィールドは、作業項目のタイプによって異なります。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 作業項目の更新]

このアクションモジュールは、ID を使用して既存の作業項目を更新します。

このモジュールは、更新された作業項目の ID を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロジェクト ]</td> 
   <td>更新する作業項目を含むプロジェクトを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 作業項目タイプ ]</td> 
   <td> <p>更新する作業項目のタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL その他のフィールド ]</td> 
   <td>これらの各フィールドに、特定のプロパティに対して作業項目に持たせる値を入力します。 使用可能なフィールドは、作業項目のタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 作業項目 ID]</td> 
   <td>更新する作業項目の ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルのアップロード]

このアクションモジュールは、ファイルをアップロードし、作業項目に添付します。

モジュールは、添付ファイルの添付ファイル ID とダウンロード URL を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロジェクト ] </td> 
   <td> <p>添付ファイルをアップロードするプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 作業項目 ID]</td> 
   <td> <p>添付ファイルをアップロードする作業項目の ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コメント ]</td> 
   <td>アップロードする添付ファイルに追加するコメントのテキストを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ] </td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前と内容を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルのダウンロード]

このアクションモジュールは、添付ファイルをダウンロードします。

このモジュールは、添付ファイルのファイルコンテンツを返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 添付ファイル URL]</td> 
   <td> <p>ダウンロードする添付ファイルの URL を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 作業項目をリンク]

このアクションモジュールは、2 つの作業項目をリンクし、それらの間の関係を定義します。

このモジュールは、メイン作業項目と関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 作業項目 ID]</td> 
   <td>別の作業項目をリンクするメイン作業項目の ID を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リンクされた作業項目 ID]</td> 
   <td>メインの作業項目にリンクする作業項目の ID を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リンクタイプ ]</td> 
   <td> <p>リンクする作業項目間の関係を定義します。</p> <p>詳しくは、 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">リンクタイプの参照</a> （[!UICONTROL Azure DevOps] ドキュメント）を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コメント ]</td> 
   <td>コメントのテキストを入力またはマッピングします。 これは、リンクの推論や意図を説明するのに役立ちます。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL 作業項目のリスト]

このアクションモジュールは、 [!DNL Azure DevOps] プロジェクト。

このモジュールは、メイン作業項目と関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Azure DevOps] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">接続 [!DNL Azure DevOps] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロジェクト ]</td> 
   <td>作業項目を取得するプロジェクトを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 作業項目タイプ ]</td> 
   <td> <p>取得する作業項目のタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。 使用可能なフィールドは、取得する作業項目のタイプによって異なります。 少なくとも 1 つのプロパティを選択する必要があります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>最大作業項目数を入力またはマッピング [!DNL Workfront Fusion] は、1 回の実行サイクルでを返します。</td> 
  </tr> 
 </tbody> 
</table>
