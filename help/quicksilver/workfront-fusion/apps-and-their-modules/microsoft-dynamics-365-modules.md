---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 モジュール
description: ' [!DNL Adobe Workfront Fusion] シナリオでは、Microsoft Dynamics 365 を使用するワークフローを自動化したり、このモジュールを複数のサードパーティアプリケーションおよびサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1589'
ht-degree: 100%

---

# [!DNL Microsoft Dynamics 365 modules]

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Microsoft Dynamics 365] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

>[!NOTE]
>
>[!DNL Microsoft Dynamics 365] コネクタでは [!DNL Dynamics Finance and Operations] をサポートしていません。

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

[!DNL Microsoft Dynamics] 365 を使用するには、[!DNL Microsoft Dynamics 365] アカウントが必要です。

## Workfront Fusion への Microsoft Dynamics 365 の接続

[!DNL Microsoft Dynamics 365] アカウントへの接続を、[!DNL Microsoft Dynamics 365] モジュール内から直接作成できます。

1. 任意の [!DNL Microsoft Dynamics 365] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続に名前を入力します。
1. 「**[!UICONTROL リソース]**」フィールドに、`https://` を除いた [!DNL Dynamics 365] アカウントのアドレスを入力します。
1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

>[!NOTE]
>
>[!DNL Microsoft Azure] ポータルでの [!DNL Workfront Fusion] の登録時に、次のリダイレクト URI を使用します。
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] モジュールとそのフィールド

[!DNL Microsoft Dynamics 365] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これら以外に、アプリまたはサービスでのアクセスレベルなどの要因に応じて、追加の[!DNL Microsoft Dynamics 365] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) におけるモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [[!UICONTROL レコードの監視（定期）]](#watch-records-scheduled)
* [[!UICONTROL レコードの監視（リアルタイム）]](#watch-records-real-time)
* [[!UICONTROL レコードの作成]](#create-record)
* [[!UICONTROL API 呼び出しの実行]](#make-an-api-call)
* [[!UICONTROL レコードの削除]](#delete-record)
* [[!UICONTROL レコードの読み取り]](#read-records)
* [[!UICONTROL レコードの更新]](#update-record)
* [[!UICONTROL レコードの検索]](#search-records)

### [!UICONTROL レコードの監視（定期）]

この定期的なトリガーモジュールでは、[!DNL Dynamics 365] でのスケジュールされた最後の実行後に、指定したオブジェクト内のレコードが作成または更新されたときにシナリオを実行します。

このモジュールの出力は、検出されたレコードが新規か更新かを示します（期間内に追加された場合も更新された場合も、新規としてマークされます）。この情報は、シナリオ内の後続のモジュールにマッピングできます。

この処理は、指定した間隔で定期的に実行されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Microsoft Dynamics 365] の接続を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>このモジュールで監視する対象として、<strong>[!UICONTROL Only new records]</strong>、<strong>[!UICONTROL Updated records only]</strong>、<strong>[!UICONTROL New records and all changes]</strong> のいずれかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>このシナリオで監視する [!UICONTROL Microsoft Dynamics 365] レコードタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの監視（リアルタイム）]

このインスタントトリガーモジュールでは、指定したレコード（オブジェクト）が [!DNL Dynamics 365] で作成または更新されたときにシナリオを実行します。

このモジュールには web フックが必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>このモジュールで使用する web フックを選択します。 </p> <p>新規の web フックを追加するには、次の手順に従います。</p> 
    <ol> 
     <li value="1"> <p>「Web フック」フィールドの右にある「<strong>[!UICONTROL Add]</strong>」をクリックします。</p> </li> 
     <li value="2"> <p>「<strong>[!UICONTROL Webhook name]</strong>」フィールドに、web フックのわかりやすい名前を入力します。</p> </li> 
     <li value="3"> <p>「<strong>[!UICONTROL Connection]</strong>」フィールドで、使用する接続を選択します。</p> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Microsoft Dynamics 365] の接続を参照してください。 </p> </li> 
     <li value="4"> <p>「<strong>[!UICONTROL Save]</strong>」をクリックして web フックを保存し、モジュールに戻ります。</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの作成]

このアクションモジュールでは、アポイントメントやタスクなどのエンティティを作成します。

作成するエンティティに関する情報を指定します。

このモジュールは、新規エンティティの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Microsoft Dynamics 365] の接続を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>このモジュールで作成するエンティティのタイプを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>これらのフィールドに、特定のプロパティに対して作業アイテムに与える値を入力します。使用可能なフィールドは、エンティティタイプによって異なります。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 呼び出しの実行]

このアクションモジュールでは、[!DNL Microsoft Dynamics 365] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Microsoft Dynamics 365] モジュールでは達成できないデータフローの自動化を作成できます。

このモジュールは、ステータスコード、ヘッダーおよび本文に関する情報を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

詳しくは、[!DNL Dynamics 365 Customer Engagement Web API] の使用に関する [!DNL Microsoft] のドキュメントを参照してください。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Microsoft Dynamics 365] の接続を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p><code>&lt;Instance URL>/api/data/v9.1/</code> からの相対パスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> <p>詳しくは、</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p>JSON で <code>if</code> などの条件文を使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの削除]

このアクションモジュールは、エンティティを削除します。

エンティティの ID を指定します。

このモジュールは、エンティティの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の<a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365] を [!DNL Workfront Fusion]</a> に接続を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>このモジュールで削除するエンティティのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>このモジュールで削除するレコードの一意の [!DNL Microsoft Dynamics 365] ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの読み取り]

このアクションモジュールは、[!DNL Microsoft Dynamics 365] の 1 つのエンティティからデータを読み取ります。

エンティティの ID を指定します。

このモジュールは、エンティティの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Microsoft Dynamics 365] の接続を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>このモジュールで読み取るエンティティのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>このモジュールで読み取るレコードの一意の [!DNL Microsoft Dynamics 365] ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの更新]

このアクションモジュールは、エンティティを更新します。

エンティティの ID を指定します。

このモジュールは、更新したレコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365] を [!DNL Workfront Fusion]</a> へ接続を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>モジュールで更新するエンティティのタイプを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>これらのフィールドに、特定のプロパティに対して作業アイテムに与える値を入力します。使用可能なフィールドは、エンティティタイプによって異なります。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>モジュールで更新するレコードの一意の [!DNL Microsoft Dynamics] 365 ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを検索]

この検索モジュールは、指定した検索クエリに一致する [!DNL Microsoft Dynamics 365] 内のオブジェクトのレコードを検索します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Microsoft Dynamics 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">[!DNL Microsoft Dynamics 365] を [!DNL Workfront Fusion]</a> へ接続を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>モジュールで更新するエンティティのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>この検索に使用するフィルターを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standard Filters]</strong> </p> <p>フィールドと演算子を選択し、検索する値を入力またはマッピングして、フィルターを設定します。AND または OR ルールを使用してフィルターを作成できます。</p> </li> 
     <li> <p><strong>[!UICONTROL Query Functions]</strong> </p> <p>検索に使用する [!DNL Dynamics 365] web API クエリ関数を入力します。 </p> <p>クエリ関数について詳しくは、[!DNL Microsoft] ドキュメントの <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">web API クエリ関数リファレンス</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>返される項目の順序を指定します。複数の並べ替えを追加できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>結果の並べ替えに使用するフィールドを指定します。</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>並べ替えの方向（昇順または降順）を指定します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>
