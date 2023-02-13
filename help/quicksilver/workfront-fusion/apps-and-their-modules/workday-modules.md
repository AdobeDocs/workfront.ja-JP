---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Workdayモジュール
description: Adobe Workfront Fusion シナリオでは、 [!DNL Workday]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 1%

---

# [!DNL Workday] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Workday]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

次の手順で [!DNL Workday] モジュールは、次の要件を満たす必要があります。

* 以下をお持ち： [!DNL Workday] アカウント

* で OAuth アプリケーションを作成します。 [!DNL Workday]. 手順については、 [!DNL Workday] ドキュメント。

## 接続 [!DNL Workday] から [!DNL Workfront Fusion]

1. 任意の [!DNL Workfront Fusion] モジュール、クリック [!UICONTROL 追加] の横 [!UICONTROL 接続] フィールド

2. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL 接続名 ]</p>
                </td>
                <td>接続名を入力</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td>アドレスを入力 [!DNL Workday] ～を伴わない宿主 <code>https://</code>. 例： <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL サービス URL]</td>
                <td>アドレスを入力 [!DNL Workday] web サービスなし <code>https://</code>. 例： <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL テナント名 ]</td>
                <td>このテナントを入力 [!DNL Workday] アカウント テナントは組織の識別子で、Workdayへのログインに使用する URL に表示されます。 例：住所内 <code>https://www.myworkday.com/mycompany</code>、テナントは <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL クライアント ID]</td>
                <td>のクライアント ID を入力します。 [!DNL Workday] この接続で使用するアプリケーション。 これは、でアプリケーションを作成する際に取得します。 [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
                <td>のクライアント秘密鍵を入力します。 [!DNL Workday] この接続で使用するアプリケーション。 これは、でアプリケーションを作成する際に取得します。 [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL セッションタイムアウト（分）]</td>
                <td >認証トークンの有効期限を分単位で入力します。</td>
            </tr>
        </tbody>
    </table>


3. クリック [!UICONTROL 続行] 接続を保存してモジュールに戻るには

## [!DNL Workday] モジュールとそのフィールド

設定時に [!DNL Workday] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Workday] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#action)

* [検索](#search)


### アクション

* [[!UICONTROL レコードの作成]](#create-a-record)

* [[!UICONTROL レコードの削除]](#delete-a-record)

* [[!UICONTROL カスタム API 呼び出しをおこなう]](#make-a-custom-api-call)

* [[!UICONTROL レコードの更新]](#update-a-record)


#### [!UICONTROL レコードの作成]

このアクションモジュールは、 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL 接続 ]</td>
            <td>接続方法 [!DNL Workday] Workfront Fusion へのアカウントについては、 <a href="#Connect" class="MCXref xre[!DNL ]f" >接続 [!DNL Workday] から [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL レコードタイプ ]</td>
            <td>作成するレコードのタイプを選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>作成するレコードの ID を入力またはマッピングします。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL サブリソース ID]</td>
            <td >作成するサブリソースの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、次の場所にある 1 つのレコードを削除します： [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL 接続 ]</td>
            <td>接続方法 [!DNL Workday] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#Connect" class="MCXref xre[!DNL ]f" >接続 [!DNL Workday] から [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL レコードタイプ ]</td>
            <td>削除するレコードのタイプを選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 特定のレコードタイプ ]</td>
            <td>削除するレコードの特定のタイプを選択します。 これらは、選択したレコードタイプに基づきます。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL サブリソース ID]</td>
            <td>削除するサブリソースの ID を入力またはマッピングします。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >削除するレコードの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL カスタム API 呼び出しをおこなう]

このアクションモジュールを使用すると、 [!DNL Workday] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Workday] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

このモジュールは、ステータスコードと共に、API 呼び出しのヘッダーと本文を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>接続方法 [!DNL Workday] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#Connect" class="MCXref xre[!DNL ]f" >接続 [!DNL Workday] から [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] によって認証ヘッダーが追加されます。</p> </td> 
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

#### [!UICONTROL レコードの更新]

このアクションモジュールは、 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL 接続 ]</td>
            <td>接続方法 [!DNL Workday] Workfront Fusion へのアカウントについては、 <a href="#Connect" class="MCXref xref" >[!UICONTROL 接続 [!DNL Workday] Workfront Fusion] に</a></td>
        </tr>
        <tr>
            <td  role="rowheader">レコードタイプ</td>
            <td>更新するレコードのタイプを [!UICONTROL ] から選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>更新するレコードの ID を入力またはマッピングします。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL サブリソース ID]</td>
            <td >更新するサブリソースの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>

### 検索

* [[!UICONTROL レコードを読み取る]](#read-a-record)

* [[!UICONTROL レコードのリスト]](#list-records)


#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、単一のレコードを読み取ります。

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL 接続 ]</td>
            <td>接続方法 [!DNL Workday] Workfront Fusion へのアカウントについては、 <a href="#Connect" class="MCXref xref" >[!UICONTROL 接続 [!DNL Workday] Workfront Fusion] に</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL レコードタイプ ]</td>
            <td>削除するレコードのタイプを選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL 特定のレコードタイプ ]</td>
            <td>読み取るレコードの種類を選択します。 これらは、選択したレコードタイプに基づきます。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >削除するレコードの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL レコードのリスト]

この検索モジュールは、指定されたタイプのレコードのリストを取得します。

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL 接続 ]</td>
              <td>接続方法 [!DNL Workday] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#Connect" class="MCXref xref" >接続 [!DNL Workday] から [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL レコードタイプ ]</td>
              <td>取得するレコードのタイプを選択します。</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL 制限 ]</td>
              <td >
                  <p>各シナリオの実行サイクル中に、モジュールで取得するレコードの最大数を入力またはマッピングします。</p>
              </td>
          </tr>
      </tbody>
  </table>
