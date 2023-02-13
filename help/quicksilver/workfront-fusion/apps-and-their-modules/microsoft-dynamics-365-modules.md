---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Microsoft Dynamics 365 を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Microsoft Dynamics 365]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

>[!NOTE]
>
>この [!DNL Microsoft Dynamics 365] コネクタはをサポートしていません [!DNL Dynamics Finance and Operations].

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

使用する [!DNL Microsoft Dynamics] 365、 [!DNL Microsoft Dynamics 365] アカウント

## Microsoft Dynamics 365 をWorkfront Fusion に接続する

次に、 [!DNL Microsoft Dynamics 365] 内部から直接アカウント [!DNL Microsoft Dynamics 365] モジュール。

1. 任意の [!DNL Microsoft Dynamics 365] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 接続の名前を入力します。
1. 内 **[!UICONTROL リソース]** フィールドに、 [!DNL Dynamics 365] アカウント、なし `https://`.
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

>[!NOTE]
>
>登録時 [!DNL Workfront Fusion] の [!DNL Microsoft Azure] ポータルでは、次のリダイレクト URI を使用します。
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`



## [!DNL Microsoft Dynamics 365] モジュールとそのフィールド

設定時に [!DNL Microsoft Dynamics 365] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Microsoft Dynamics 365] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL レコードの監視（スケジュール済み）]](#watch-records-scheduled)
* [[!UICONTROL レコードを監視（リアルタイム）]](#watch-records-real-time)
* [[!UICONTROL レコードを作成]](#create-record)
* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)
* [[!UICONTROL レコードを削除]](#delete-record)
* [[!UICONTROL レコードの読み取り]](#read-records)
* [[!UICONTROL レコードを更新]](#update-record)
* [[!UICONTROL レコードを検索]](#search-records)

### [!UICONTROL レコードの監視（スケジュール済み）]

このスケジュールトリガーモジュールは、指定したオブジェクト内のレコードが、 [!DNL Dynamics 365].

モジュールの出力は、検出されたレコードが新規か更新かを示します（期間内に追加および更新された場合、新規としてマークされます）。 この情報は、シナリオの後続のモジュールにマッピングできます。

この処理は、指定した定期的なスケジュール間隔で実行されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>モジュールを監視するかどうかを選択します <strong>[!UICONTROL 新規レコードのみ ]</strong>, <strong>[!UICONTROL 更新されたレコードのみ ]</strong>または <strong>[!UICONTROL 新しいレコードとすべての変更 ]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>シナリオで監視する [!UICONTROL Microsoft Dynamics 365] レコードタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最大レコード数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを監視（リアルタイム）]

このインスタントトリガーモジュールは、指定したレコード（オブジェクト）が [!DNL Dynamics 365].

このモジュールには Webhook が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>このモジュールで使用する Webhook を選択します。 </p> <p>新しい Webhook を追加するには：</p> 
    <ol> 
     <li value="1"> <p>クリック <strong>[!UICONTROL 追加 ]</strong> ウェブフックフィールドの右側に</p> </li> 
     <li value="2"> <p>内 <strong>[!UICONTROL Webhook]</strong> 「名前」フィールドに、Webhook を説明する名前を入力します。</p> </li> 
     <li value="3"> <p>内 <strong>[!UICONTROL 接続 ]</strong> フィールドで、選択した接続を使用する接続を選択します</p> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </li> 
     <li value="4"> <p>クリック <strong>[!UICONTROL 保存 ]</strong> をクリックし、webhook を保存してモジュールに戻ります。</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを作成]

このアクションモジュールは、予定やタスクなどのエンティティを作成します。

作成するエンティティに関する情報を指定します。

このモジュールは、新しいエンティティと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>モジュールで作成するエンティティのタイプを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL プロパティフィールド ]</td> 
   <td>これらのフィールドには、特定のプロパティに対して作業項目に含める値を入力します。 使用可能なフィールドは、エンティティタイプによって異なります。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、 [!DNL Microsoft Dynamics 365] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Microsoft Dynamics 365] モジュール。

モジュールは、ステータスコード、ヘッダーおよび本文に関する情報を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

詳しくは、 [!DNL Microsoft] 使用に関するドキュメント [!DNL Dynamics 365 Customer Engagement Web API].

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>相対パスを入力 <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> <p>詳しくは、</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
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

### [!UICONTROL レコードを削除]

このアクションモジュールは、エンティティを削除します。

エンティティの ID を指定します。

このモジュールは、エンティティの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td> <p>モジュールで削除するエンティティのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>一意の [!DNL Microsoft Dynamics 365] モジュールで削除するレコードの ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの読み取り]

このアクションモジュールは、 [!DNL Microsoft Dynamics 365].

エンティティの ID を指定します。

このモジュールは、エンティティの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>モジュールで読み取るエンティティのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>一意の [!DNL Microsoft Dynamics 365] モジュールが読み取るレコードの ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを更新]

このアクションモジュールは、エンティティを更新します。

エンティティの ID を指定します。

このモジュールは、更新されたレコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>モジュールで更新するエンティティのタイプを選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL プロパティフィールド ]</td> 
   <td>これらのフィールドには、特定のプロパティに対して作業項目に含める値を入力します。 使用可能なフィールドは、エンティティタイプによって異なります。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>一意の [!DNL Microsoft Dynamics] 365 モジュールを更新するレコードの ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを検索]

この検索モジュールは、 [!DNL Microsoft Dynamics 365] 指定した検索クエリに一致する この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Microsoft Dynamics 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">接続 [!DNL Microsoft Dynamics 365] から [!DNL Workfront Fusion]</a> 」を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>モジュールで更新するエンティティのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>この検索に使用するフィルターを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 標準フィルター ]</strong> </p> <p>フィールドと演算子を選択し、検索する値を入力またはマッピングして、フィルターを設定します。 AND または OR ルールを使用してフィルターを作成できます。</p> </li> 
     <li> <p><strong>[!UICONTROL クエリ関数 ]</strong> </p> <p>次を入力します。 [!DNL Dynamics 365] 検索に使用する web API クエリ関数。 </p> <p>クエリ関数について詳しくは、 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API クエリ関数リファレンス</a> 内 [!DNL Microsoft] ドキュメント。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え ]</td> 
   <td> <p>返される項目の順序を指定します。 複数の並べ替えを追加できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL フィールド ]</strong> </p> <p>結果を並べ替えるフィールドを指定します。</p> </li> 
     <li> <p><strong>[!UICONTROL 方向 ]</strong> </p> <p>並べ替えの方向（昇順または降順）を指定します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最大レコード数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>
