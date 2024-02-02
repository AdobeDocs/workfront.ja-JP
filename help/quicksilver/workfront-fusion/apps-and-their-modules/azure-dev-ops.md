---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Azure DevOps モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Azure DevOps] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1797'
ht-degree: 100%

---

# [!DNL Azure DevOps] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Azure DevOps] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Azure DevOps] モジュールを使用するには、[!DNL Azure] DevOps アカウントが必要です。

## [!DNL Workfront Fusion] を [!DNL Azure DevOps] に接続 {#connect-azure-devops-to-workfront-fusion}

1. [!DNL Azure DevOps] モジュールをシナリオに追加します。
1. 「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 「[!UICONTROL 接続タイプ]」フィールドで、「**[!DNL Azure DevOps]**」を選択します。

   >[!IMPORTANT]
   >
   >「[!UICONTROL [!DNL Azure DevOps] (すべてのスコープをリクエスト)]」接続タイプは、近い将来廃止される予定です。したがって、使用はお勧めしません。

1. 次のフィールドに入力します。

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Connection name]</td>
            <td>作成する接続の名前を入力します。</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>[!DNL Azure DevOps] アプリケーションを作成した組織の名前を入力します。</td>
        </tr>
    </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続の設定を終了し、シナリオの作成を続けます。

## [!UICONTROL Azure DevOps] モジュールとそのフィールド

[!DNL Azure DevOps] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Azure DevOps] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[モジュール間の情報のマッピング： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)を参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL 作業項目の監視]

このインスタントトリガーモジュールは、[!UICONTROL Azure DevOps] でレコードが追加、更新または削除されたときにシナリオを実行します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>モジュールの web フックを選択または追加します。</p> <p>トリガーモジュールの web フックについて詳しくは、<a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">インスタントトリガー（web フック）：[!DNL Adobe Workfront Fusion]</a>を参照してください。</p> <p>Web フックの作成方法については、<a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Web フック</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [カスタム API 呼び出し](#custom-api-call)
* [レコードの読み取り](#read-record)
* [レコードを作成](#create-a-record)
* [作業項目の更新](#update-a-work-item)
* [[!UICONTROL 添付ファイルのアップロード]](#upload-an-attachment)
* [添付ファイルのダウンロード](#download-an-attachment)
* [作業項目のリンク]（[!UICONTROL #link-work-items]）

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL Azure DevOps] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Azure DevOps] モジュールでは不可能なデータフロー自動処理を実現できます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] への [!DNL Azure DevOps] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Base URL]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントへの接続に使用するベース URL を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>この API 呼び出しの接続先となる相対 URL を入力します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>この API 呼び出しの接続先となる [!DNL Azure DevOps] API のバージョンを選択またはマッピングします。バージョンが選択されていない場合、[!DNL Workfront Fusion] は [!DNL Azure DevOps] API バージョン 5.1 に接続します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP リクエストメソッド：[!DNL Adobe Workfront Fusion]</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p>JSON で <code>if</code> のような条件文を使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、[!DNL Azure DevOps] の単一レコードからデータを読み取ります。

レコードの ID を指定します。

このモジュールは、レコードの ID および関連するフィールドと共に、接続を介してアクセスされるカスタムフィールドとその値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] への [!DNL Azure DevOps] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>プロジェクトを読み取るか作業アイテムを読み取るかを選択</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>：読み取るプロジェクトを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong>：読み取る作業アイテムを含むプロジェクトを選択し、作業アイテムのタイプを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。使用可能なフィールドは、作業アイテムのタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>読み取るレコードの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成]

このアクションモジュールは、新しいプロジェクトまたは作業アイテムを作成します。

モジュールは、新しく作成された作業アイテムのオブジェクト ID、または新しく作成されたプロジェクトの URL とステータスコードを出力します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!DNL Azure DevOps] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>作業アイテムを作成するか、プロジェクトを作成するかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>：新しいプロジェクトの名前を入力またはマッピングします。</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong>：新しいプロジェクトの説明を入力またはマッピングします。 </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>：プロジェクトを公開または非公開にするかを選択します。ユーザーが非公開プロジェクトとやり取りするには、組織にサインインし、プロジェクトへのアクセス権を付与されている必要があります。公開プロジェクトは、組織にサインインしていないユーザーに表示されます。</p> </li> 
       <li> <p><strong>[!UICONTROL Version control]</strong>：プロジェクトでバージョン管理に[!DNL Git]または[!UICONTROL Team Foundation Version Control (TFCV)]を使用するかどうかを選択します。</p> </li> 
       <li> <p><strong>[!UICONTROL Work item process]</strong>：プロジェクトに使用する作業プロセスを選択します。[!UICONTROL Basic]、[!UICONTROL Scrum]、[!UICONTROL Capability Maturity Model Integration (CMMI)]、[!UICONTROL Agile]を選択できます。</p> <p>[!DNL Azure DevOps]プロセスについて詳しくは、「[!DNL Azure DevOps]</a> ドキュメントで<a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">プロセスを選択」を参照してください。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong> </p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>：作業アイテムを作成するプロジェクトを選択します。</p> </li> 
       <li> <p><strong>[!UICONTROL Work item type]</strong>：作成する作業アイテムのタイプを選択します。</p> </li> 
       <li> <p><strong>[!UICONTROL Other fields]</strong>：これらのフィールドには、特定のプロパティに対して作業アイテムに含める値を入力します。使用可能なフィールドは、作業アイテムのタイプによって異なります。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 作業アイテムを更新]

このアクションモジュールは、ID を使用して既存の作業アイテムを更新します。

このモジュールは、更新された作業アイテムの ID を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!DNL Azure DevOps] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>更新する作業アイテムを含むプロジェクトを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work Item Type]</td> 
   <td> <p>更新する作業アイテムのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Other Fields]</td> 
   <td>これらの各フィールドに、特定のプロパティに対して作業アイテムに与える値を入力します。使用可能なフィールドは、作業アイテムのタイプによって異なります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>更新する作業アイテムの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルをアップロード]

このアクションモジュールは、ファイルをアップロードし、作業アイテムに添付します。

モジュールは、添付ファイルの添付ファイル ID とダウンロード URL を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!DNL Azure DevOps] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>添付ファイルをアップロードするプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td> <p>添付ファイルをアップロードする作業アイテムの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>アップロードされた添付ファイルに追加するコメントのテキストを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file] </td> 
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
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!DNL Azure DevOps] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment URL]</td> 
   <td> <p>ダウンロードする添付ファイルの URL を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 作業アイテムをリンク]

このアクションモジュールは、2 つの作業アイテムをリンクし、それらの間の関係を定義します。

このモジュールは、主な作業アイテムの ID と関連するフィールドのほか、接続でアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!DNL Azure DevOps] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>別の作業アイテムをリンクするメイン作業アイテムの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linked work item ID]</td> 
   <td>メインの作業アイテムにリンクする作業アイテムの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>リンクする作業アイテム間の関係を定義します。</p> <p>詳しくは、[!UICONTROL Azure DevOps]ドキュメントの<a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">リンクタイプの参照</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>コメントのテキストを入力またはマッピングします。これは、リンクの根拠や意図を説明するのに役立ちます。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL 作業アイテムのリスト]

このアクションモジュールは、[!DNL Azure DevOps] プロジェクトの特定のタイプのすべての作業アイテムを取得します。

このモジュールは、主な作業アイテムの ID と関連するフィールドのほか、接続でアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Azure DevOps] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">[!DNL Azure DevOps] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>作業アイテムを取得するプロジェクトを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item type]</td> 
   <td> <p>取得する作業アイテムのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。使用可能なフィールドは、取得する作業アイテムのタイプによって異なります。1 つ以上のプロパティを選択する必要があります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>1 回の実行サイクル中に、[!DNL Workfront Fusion] が返す作業アイテムの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
