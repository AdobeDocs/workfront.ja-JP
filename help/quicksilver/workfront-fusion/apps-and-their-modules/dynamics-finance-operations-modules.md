---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 の財務および運用モジュール
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 19b00ee8-dc05-4cde-9a76-d857090fa543
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 31%

---

# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [Microsoft Dynamics 365 財務および運用モジュール ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/dynamics-finance-operations-modules.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Microsoft Dynamics 365] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

>[!NOTE]
>
>[!DNL Microsoft Dynamics 365 Finance and Operations] コネクタでは [!DNL Dynamics 365] をサポートしていません。
>
>Microsoft Dynamics 365 モジュールについては、[[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md) を参照してください。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

## 接続の作成

Microsoft Dynamics 365 Finance and Operations モジュールの接続を作成するには：

1. Microsoft Dynamics 365 Finance and Operations モジュールで、「接続」ボックスの横にある「**[!UICONTROL 追加]** をクリックします。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>Dynamics Finance and Operations の標準接続を作成するか、認証コードを使用して接続を作成するかを選択します。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>この接続の名前を入力します。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Dynamics Finance and Operations [!UICONTROL クライアント ID] を入力します。</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Dynamics Finance and Operations [!UICONTROL クライアント シークレット ] を入力します。 </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL テナント ID]</td>
        <td>Dynamics Finance and Operations テナント ID を入力します。</td>
        </tr>
        <tr>
        <td role="rowheader">リソース</td>
        <td>Dynamics Finance and Operations アカウントの URL （https://なし）を入力します</td>
        </tr>
      </tbody>
    </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。



## Microsoft Dynamics 365 の財務および運用モジュールとそのフィールド

>[!IMPORTANT]
>
>Dynamics 365 F&amp;O API を通じて使用できるデータエンティティは、インスタンスによって異なる場合があります。 API を通じて使用できるエンティティが不明な場合は、「data」エンドポイントを使用してインスタンス内のエンティティを調べると便利です。 Dynamics 365 Finance and Operations の「data」エンドポイントは、OData サービスにアクセスするためのルート URL です。 このエンドポイントを使用すると、標準の OData プロトコルを使用して、システムで公開されている様々なデータエンティティを操作できます。
>
>これらのエンティティは、カスタム API 呼び出しモジュールを使用して取得できます。
>
><!--For more information -->



### エンティティ項目を作成

この操作モジュールは、Microsoft Dynamics 365 Finance and Operations に新しいエンティティ項目を作成します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Microsoft Dynamics 365 Finance and Operations と [!DNL Workfront Fusion] の連携については、この記事の <a href="#create-a-connection" class="MCXref xref"> 連携の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL エンティティ ]</td>
     <td>作成する Dynamics Finance and Operations エンティティの種類を入力またはマップします。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>新しいエンティティ項目に含めるデータを含む JSON 本文を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>



### エンティティ項目を削除

このアクション モジュールは、Dynamics Finance and Operations からエンティティ アイテムを削除します。 項目は、プライマリキーフィールドで識別されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Microsoft Dynamics 365 Finance and Operations と [!DNL Workfront Fusion] の連携については、この記事の <a href="#create-a-connection" class="MCXref xref"> 連携の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL エンティティ ]</td>
     <td>削除する Dynamics Finance and Operations エンティティの種類を入力またはマップします。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROLプライマリキーフィールド ]</td>
     <td> プライマリキーフィールドは、項目を識別します。 指定する主キーフィールドごとに、「<b> 項目を追加 </b>」をクリックし、その項目を識別する一意のキーと値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

### カスタム API 呼び出しの実行

このアクション モジュールは、Dynamics Finance and Operations API へのカスタム呼び出しを行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>Microsoft Dynamics 365 Finance and Operations と [!DNL Workfront Fusion] の連携については、この記事の <a href="#create-a-connection" class="MCXref xref"> 連携の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Dynamics Finance and Operations の URL に対する相対パスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。これにより、リクエストのコンテンツタイプが決まります。</p> <p>例：<code> {"Content-type":"application/json"}</code></p> <p>メモ：エラーが表示され、エラーの発生元を特定するのが困難な場合は、[!DNL Workfront] ドキュメントを基に、ヘッダーを変更することを考慮してください。カスタム API 呼び出しで 422 HTTP リクエストエラーが返される場合は、<code>"Content-Type":"text/plain"</code> ヘッダーを使用してみてください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> <p>ヒント：情報は、クエリパラメーターではなく、JSON 本文を使用して送信することをお勧めします。</p> </td> 
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



### エンティティ項目を読み取り

このアクションモジュールは、エンティティアイテムからデータを返します。 項目は、プライマリキーフィールドで識別されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Microsoft Dynamics 365 Finance and Operations と [!DNL Workfront Fusion] の連携については、この記事の <a href="#create-a-connection" class="MCXref xref"> 連携の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL エンティティ ]</td>
     <td>読み取る Dynamics Finance and Operations エンティティの種類を入力またはマップします。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROLプライマリキーフィールド ]</td>
     <td> プライマリキーフィールドは、項目を識別します。 指定する主キーフィールドごとに、「<b> 項目を追加 </b>」をクリックし、その項目を識別する一意のキーと値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

### エンティティ項目を更新

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>Microsoft Dynamics 365 Finance and Operations と [!DNL Workfront Fusion] の連携については、この記事の <a href="#create-a-connection" class="MCXref xref"> 連携の作成 </a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL エンティティ ]</td>
     <td>更新する Dynamics Finance and Operations エンティティの種類を入力またはマップします。</td> 
  </tr>  
  <tr> 
    <td>[!UICONTROLプライマリキーフィールド ]</td>
     <td> プライマリキーフィールドは、項目を識別します。 指定する主キーフィールドごとに、「<b> 項目を追加 </b>」をクリックし、その項目を識別する一意のキーと値を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>新しいエンティティ項目に含めるデータを含む JSON 本文を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

この検索モジュールは、指定した条件に基づいて結果を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Workfront] アプリを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事にある <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">[!DNL Workfront] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL エンティティ ]</td> 
   <td>検索する Dynamics Finance and Operations エンティティの種類を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search criteria]</td> 
   <td> <p>検索するフィールド、クエリで使用する演算子、およびそのフィールドで検索する値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sort by]</td> 
   <td> <p>結果の並べ替え基準にするフィールドを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
