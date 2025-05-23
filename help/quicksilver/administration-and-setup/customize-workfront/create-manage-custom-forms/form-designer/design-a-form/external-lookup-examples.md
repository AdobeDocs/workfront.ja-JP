---
title: カスタムフォームの外部参照フィールドの例
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: カスタムフォームの外部参照フィールドが外部 API を呼び出し、ドロップダウンフィールドのオプションとして値を返します。 この記事では、外部検索フィールドを使用して、同じWorkfront インスタンスまたはパブリック API を呼び出す例を示します。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: b3a4945cf2db1ba11b42742f0da685b32a6d0dd9
workflow-type: tm+mt
source-wordcount: '1438'
ht-degree: 45%

---

# カスタムフォームの外部検索フィールドの例

カスタムフォームの外部参照フィールドが外部 API を呼び出し、ドロップダウンフィールドのオプションとして値を返します。 カスタムフォームが添付されているオブジェクトを使用するユーザーは、ドロップダウンからこれらのオプションを 1 つ以上選択できます。

この記事では、外部検索フィールドを使用して、同じWorkfront インスタンスまたはパブリック API を呼び出す例を示します。 また、外部参照を使用して、Jira、Salesforce、ServiceNow などの外部システムと通信することもできます。

外部検索フィールドをカスタムフォームに追加する方法と、外部検索コンポーネントのその他の定義について詳しくは、[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront プラン </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>カスタムフォームへの管理アクセス権 </td> 
  </tr>  
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfrontの同じインスタンスに対して外部検索フィールドを設定する

外部検索を使用して、Workfront インスタンスからカスタムフォームにデータを取り込むことができます。

### 外部検索でのネイティブのWorkfront フィールド値の使用

この例では、Workfront API を呼び出し、「Status Query」カスタムフィールドの値と$$QUERY を使用した検索語句を使用してステータスでフィルタリングされた外部検索フィールドにプロジェクトのリストを入力する方法を示しています。

1. カスタムフォームを開きます。
1. 画面の左側で、「**外部ルックアップ**」を見つけて、キャンバス上のセクションにドラッグします。
1. フィールドの&#x200B;**ラベル**&#x200B;と&#x200B;**名前**&#x200B;を入力します。
1. フィールドの&#x200B;**形式**&#x200B;を選択します。
1. API 呼び出しを「**ベース API URL**」フィールドに入力します。

   * $$HOST を使用して、カスタムフォームがあるWorkfrontの同じインスタンスを参照します。
   * $$QUERY を使用して、ユーザー入力に基づいて結果を動的にフィルタリングします。

   **API 呼び出しの例**
   `$$HOST/attask/api/v15.0/project/search?status={DE:Status Query}&description=$$QUERY`

1. API 呼び出しで参照されるフィールドの **依存関係** を確認します。

   依存関係フィールドには、オブジェクトで使用可能な任意のカスタムフィールドまたはネイティブフィールドを使用できます。 例えば、外部検索フィールドを含むグループのカスタムフォームを作成する場合、依存関係フィールドには、グループで使用可能な任意のフィールドを含めることができます。

   この例では、`{DE:Status Query}` は、現在のグループの「ステータスクエリ」カスタムフィールドの値に動的に置き換えられます。 そのため、フォームをグループ A に添付すると、`{DE:Status Query}` はそのグループの「ステータスクエリ」フィールドに設定された値に置き換えられます。

1. 「**HTTP メソッド**」を選択します。

   これは、ほとんどの場合、**Get** になります。

1. **JSON パス**&#x200B;を入力して、API 呼び出しの結果を取得します。

   **例**
   `$.data[*].name`

   >[!NOTE]
   >
   >同じ Workfront インスタンスに対して呼び出しを行う場合は、**ヘッダー**&#x200B;の情報は必要ありません。

1. 「**適用**」をクリックします。

   ![カスタムフォームでの Workfront に対する API 呼び出しの設定](assets/external-lookup-to-workfront.png)

   カスタムフォームが Workfront オブジェクト（この例ではプロジェクト）に追加されると、次のようになります。

   ![「外部ルックアップ」フィールドを含むカスタムフォーム](assets/external-lookup-project-status-example1.png)

   ![ステータスに基づく「外部ルックアップ」オプション](assets/external-lookup-project-status-example2.png)

### 外部参照でのカスタムフィールド値の使用

この例では、Workfront API を呼び出し、カスタムフィールドから外部検索フィールドにデータを取り込む方法を示しています。 例えば、カスタムフィールドは「Custom Colors」と呼ばれます。

1. カスタムフォームを開きます。
1. 画面の左側で、「**外部ルックアップ**」を見つけて、キャンバス上のセクションにドラッグします。
1. フィールドの&#x200B;**ラベル**&#x200B;と&#x200B;**名前**&#x200B;を入力します。
1. フィールドの&#x200B;**形式**&#x200B;を選択します。
1. API の URL 呼び出しを「**ベース API の URL**」フィールドに入力します。

   **例**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. このルックアップフィールドが API で参照しているフィールドの&#x200B;**依存関係**&#x200B;を確認します。

   「依存関係」フィールドには、オブジェクトの詳細ページに存在する任意のカスタムフィールドまたはネイティブフィールドを使用できます。

1. 「**HTTP メソッド**」を選択します。

   これは、ほとんどの場合、**Get** になります。

1. **JSON パス**&#x200B;を入力して、API 呼び出しの結果を取得します。

   **例**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * 「parameterValues」は、操作しているオブジェクトのWorkfront内のカスタムフィールドを指します。
   * 例えば、「DE:Combo Colors」は、取得する値を含む特定のカスタムフィールドです。

   >[!NOTE]
   >
   >同じ Workfront インスタンスに対して呼び出しを行う場合は、**ヘッダー**&#x200B;の情報は必要ありません。

1. 「**適用**」をクリックします。

   カスタムフォームがWorkfront オブジェクトに追加されると、「コンボカラー」フィールドのすべての値が外部検索フィールドドロップダウンに表示されます。

## Workfront Planning API 用の外部参照フィールドの設定

Workfront Planning API では、Get メソッドを使用してレコードタイプ ID でレコードを検索するためのエンドポイントを使用できます。 このエンドポイントを使用して、外部参照フィールドで Planning レコードを参照できます。

* **ベース API の URL:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **HTTP メソッド：** Get
* **JSON パス：** `$.records[*].data.{fieldID}`

  **{fieldID}** は、エンドユーザーのカスタムフォーム上で外部検索の検索結果に表示するフィールドです。

詳しくは、[Workfront Planning API](/help/quicksilver/planning/general/planning-api-basics.md) を参照してください。

## パブリック API 用の外部参照フィールドの設定

外部検索を使用して、外部のパブリック API を呼び出し、データを取得できます。

この例では、ドロップダウンオプションにすべての国名をハードコーディングする必要がないように、国の API（<https://api.first.org/data/v1/countries> など）を呼び出す方法を示します。

1. カスタムフォームを開きます。
1. 画面の左側で、「**外部ルックアップ**」を見つけて、キャンバス上のセクションにドラッグします。
1. フィールドの&#x200B;**ラベル**&#x200B;と&#x200B;**名前**&#x200B;を入力します。
1. フィールドの&#x200B;**形式**&#x200B;を選択します。
1. API の URL 呼び出しを「**ベース API の URL**」フィールドに入力します。

   * $$QUERY を追加すると、エンドユーザーに対するクエリフィルタリングを実装できます。

   **例**
すべての国を一覧表示します。<https://api.first.org/data/v1/countries>

   ユーザーがドロップダウンフィールド内の任意の国を検索できるようにします。<https://api.first.org/data/v1/countries?q=$$QUERY>

   ユーザーが地域内の国を検索できるようにします。<https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * 使用可能なは、Workfront の別のカスタムフィールドで定義されます。
   * ユーザーがフォーム上で地域を選択すると、外部検索フィールドには、その地域の国（API で地域が定義されている国）のみが表示されます。 また、ユーザーは、選択した地域の国を検索することもできます。

1. このルックアップフィールドが API で参照しているフィールドの&#x200B;**依存関係**&#x200B;を確認します。

   「依存関係」フィールドには、オブジェクトの詳細ページに存在する任意のカスタムフィールドまたはネイティブフィールドを使用できます。

   この例では、`{DE:Region}` は、地域カスタムフィールドの値に置き換えられます。

1. 「**HTTP メソッド**」を選択します。

   これは、ほとんどの場合、**Get** になります。

1. **JSON パス**&#x200B;を入力して、API 呼び出しから結果を取得します。

   このオプションを使用すると、API URL から返された JSON からデータを抽出できます。これは、JSON 内のどの値がドロップダウンオプションに表示されるかを選択する手段の役割を果たします。

   **例**
   `$.data[*].country`

1. （オプション）「**ヘッダーを追加**」をクリックし、API での認証に必要なキーと値のペアを入力するか貼り付けます。

   >[!NOTE]
   >
   >「ヘッダー」フィールドは、資格情報を保存する安全な場所ではないので、入力して保存する内容には注意する必要があります。

1. （オプション）ユーザーがドロップダウンで複数の値を選択できるようにするには、「**複数選択ドロップダウン**」を選択します。

1. 「**適用**」をクリックします。

   ![カスタムフォームでのパブリック API への API 呼び出しの設定](assets/external-lookup-to-api-for-countries.png)

   カスタムフォームが Workfront オブジェクト（この例ではプロジェクト）に追加されると、次のようになります。

   ![「外部ルックアップ」フィールドを含むカスタムフォーム](assets/external-lookup-countries-example1.png)

   ![地域に基づく国の「外部ルックアップ」オプション](assets/external-lookup-countries-example2.png)

## 外部検索フィールドのその他のユースケース

外部参照を作成するユースケースは他にも多数あります。

**ユースケース：** typeahead フィールドは、レポートで問題を引き起こす可能性があるので、置き換えます。
**解決策：** システム内の既存のオブジェクトへの API 呼び出しを使用します。

typeahead フィールドを置き換えるためのテンプレートのベース API URL の例：
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**ユースケース：** より多くの機能を含むドロップダウンフィールドを作成する（例えば、外部 eookup フィールドに折り返し線がある）。
**解決策：** システム内の既存のオブジェクトへの API 呼び出しを使用するか、新しいオブジェクトを作成してこのオブジェクトへの API 呼び出しを使用します。

**ユースケース：** ユーザーがカスタムフォーム領域外で独自のフィールドを維持する方法を定義します。 外部検索フィールドを設定し、フィールドを構成するオブジェクトにユーザーを指定できます。 このオプションは、メンテナンスの多いフィールドやチームに適しています。
**解決策：** 新しいオブジェクトを作成し、このオブジェクトへの API 呼び出しを使用します。

**ユースケース：**&#x200B;Workfront外のオブジェクトとの統合。 例えば、typeahead フィールドで制限されているのではなく、別のシステムにアクセスして各ユーザーの名前を取得するような場合です。
**解決策：** 他のシステムに接続するための Webhook/Fusion 自動処理。

