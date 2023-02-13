---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizerモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Adobe Journey Optimizer]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] モジュール

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Adobe Journey Optimizer]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。 [!DNL Adobe Journey Optimizer] モジュールを使用すると、レコードの作成、読み取り、更新、削除をおこなうことも、 [!DNL Adobe Journey Optimizer] API


シナリオの作成手順については、 [シナリオの作成](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
      <td>
        <p>[!UICONTROL Pro] 以降</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
      <td>
        <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ]</p>
      </td>
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

使用する前に [!DNL Adobe Journey Optimizer] コネクタを使用する場合は、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!DNL Adobe Journey Optimizer] アカウント

## への接続の作成 [!DNL Adobe Journey Optimizer]

の接続を作成するには、以下を実行します。 [!DNL Adobe Journey Optimizer] モジュール：

1. 任意の [!DNL Adobe Journey Optimizer] モジュール、クリック **[!UICONTROL 追加]** をクリックします。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL 接続名 ]</td>
          <td>
            <p>この接続の名前を入力します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL クライアント ID]</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL クライアント ID]。 これは、 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL クライアント秘密鍵 ]。 これは、 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL テクニカルアカウント ID]</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL テクニカルアカウント ID]。 これは、 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 組織 ID]</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL 組織 ID]。 これは、 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL メタスコープ ]</td>
          <td>
            接続に必要なメタスコープを入力します。
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 秘密鍵 ]</td>
          <td>
            <p>秘密鍵を入力します。秘密鍵は、 [!DNL Adobe Developer Console]. </p>
            <p>秘密鍵または証明書を抽出するには：</p>
            <ol>
              <li value="1">
                <p>クリック <b>[!UICONTROL 抽出 ]</b>.</p>
              </li>
              <li value="2">
                <p>抽出するファイルの種類を選択します。</p>
              </li>
              <li value="3">
                <p>秘密鍵または証明書を含むファイルを選択します。</p>
              </li>
              <li value="4">
                <p>ファイルのパスワードを入力します。</p>
              </li>
              <li value="5">
                <p>クリック <b>[!UICONTROL 保存 ]</b> をクリックしてファイルを抽出し、接続設定に戻ります。</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. クリック **[!UICONTROL 続行]** 接続を保存し、モジュールに戻ります。

## [!DNL Adobe Journey Optimizer] モジュールとそのフィールド

設定時に [!DNL Adobe Journey Optimizer] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Adobe Journey Optimizer] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL カスタム API 呼び出しをおこなう]](#make-a-custom-api-call)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL レコードの更新]](#update-a-record)

#### [!UICONTROL レコードの作成]

このアクションモジュールは、配置、決定ルール、タグ、パーソナライズされたオファー、コレクションまたはフォールバックオファーを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
     <td>への接続を作成する手順 [!DNL Adobe Journey Optimizer]を参照してください。 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >への接続の作成 [!DNL Adobe Journey Optimizer]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL レコードタイプ ]
      </td>
      <td>
        作成するレコードのタイプを選択
        <ul>
        <li><b>[!UICONTROL Placement]</b>:続行 <a href="#placement-fields" >[!UICONTROL 配置 ] フィールド</a>.</li>
        <li><b>[!UICONTROL 決定ルール ]</b>:続行 <a href="#decision-rule-fields" >[!UICONTROL 決定ルール ] フィールド</a>.</li>
        <li><b>[!UICONTROL 決定 ]</b>:続行 <a href="#decision-fields" >[!UICONTROL 決定 ] フィールド</a>.</li>
        <li><b>[!UICONTROL タグ ]</b>:続行 <a href="#tag-fields" >[!UICONTROL タグ ] フィールド</a>.</li>
        <li><b>[!UICONTROL コレクション ]</b>:続行 <a href="#collection-fields" >[!UICONTROL コレクション ] フィールド</a>.</li>
        <li><b>[!UICONTROL フォールバックオファー ]</b>:続行 <a href="#fallback-offer-fields" >[!UICONTROL フォールバックオファー ] フィールド</a>.</li>
        <li><b>[!UICONTROL パーソナライズされたオファー ]</b>:続行 <a href="#personalized-offer-fields" >[!UICONTROL パーソナライズされたオファー ] フィールド</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 配置] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>配置の名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 説明 ]
      </td>
      <td>配置の説明を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 決定ルール] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>説明ルールの名前を入力またはマップします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 説明 ]
      </td>
      <td>決定ルールの説明を入力またはマッピングします。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 条件 ]
      </td>
      <td>決定ルールの条件を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 決定] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>説明ルールの名前を入力またはマップします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ステータス ]</td>
      <td>決定のステータスを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 開始日 ]</td>
      <td><p>決定の開始日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 終了日 ]</td>
      <td><p>決定の終了日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 配置 ]</td>
      <td>この決定に追加する配置を選択
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL コレクション ]</td>
      <td>この決定で考慮されるオファーを含むオファーコレクションを選択します。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL フォールバックオファー ]</td>
      <td>この決定のルールに一致しない顧客に提示されるフォールバックオファーを選択します。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL タグ] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>タグの名前を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL コレクション] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>コレクションの名前を入力またはマップします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL フィルターの種類 ]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL 要素 ]
      </td>
      <td>コレクションに含めるタグを選択します。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL フォールバックオファー] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>フォールバックオファーの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL ステータス ]
      </td>
      <td> フォールバックオファーのステータスを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Placement]
      </td>
      <td>フォールバックオファーの配置を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL パーソナライズされたオファー] フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
     <td>説明ルールの名前を入力またはマップします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ステータス ]</td>
      <td>決定のステータスを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">配置</td>
      <td>パーソナライズされたオファーの配置を選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 開始日 ]</td>
      <td><p>パーソナライズされたオファーの開始日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 終了日 ]</td>
      <td><p>パーソナライズされたオファーの終了日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 決定ルール ]</td>
      <td>このパーソナライズされたオファーに追加する決定ルールを選択します。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 優先度 ]</td>
      <td>このオファーの優先度を選択します。 優先度は、このオファーが別のオファーではなく提示されるかどうかに影響します。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL 上限制約 ]</td>
      <td>このオファーの表示回数を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、次の場所にある 1 つのレコードを削除します： [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
     <td>への接続を作成する手順 [!DNL Adobe Journey Optimizer]を参照してください。 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >への接続の作成 [!DNL Adobe Journey Optimizer]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL レコードタイプ ]
      </td>
      <td>
        削除するレコードのタイプを選択します
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL 決定ルール ]</li>
        <li>[!UICONTROL 決定 ]</li>
        <li>[!UICONTROL タグ ]</li>
        <li>[!UICONTROL コレクション ]</li>
        <li>[!UICONTROL フォールバックオファー ]</li>
        <li>[!UICONTROL パーソナライズされたオファー ]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        削除するレコードを選択します。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL カスタム API 呼び出しをおこなう]

このモジュールは、 [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL 接続 ]</td>
     <td>への接続を作成する手順 [!DNL Adobe Journey Optimizer]を参照してください。 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >への接続の作成 [!DNL Adobe Journey Optimizer]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL パス ]</p>
      </td>
      <td>
        <p>次で始まる {baseURL} に対する相対パスを入力<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL メソッド ]</p>
      </td>
      <td>
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p>
        <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion は、認証ヘッダーと x-api-key ヘッダーを自動的に追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL クエリ文字列 ]  </td>
      <td>
        <p>リクエストクエリ文字列を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 本文 ]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>モジュールが 1 回の実行サイクルで返す結果の最大数を入力します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、次の場所にある 1 つのレコードを削除します： [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL 接続 ]</td>
     <td>への接続を作成する手順 [!DNL Adobe Journey Optimizer]を参照してください。 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >への接続の作成 [!DNL Adobe Journey Optimizer]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL レコードタイプ ]
      </td>
      <td>
        削除するレコードのタイプを選択します
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL 決定ルール ]</li>
        <li>[!UICONTROL 決定 ]</li>
        <li>[!UICONTROL タグ ]</li>
        <li>[!UICONTROL コレクション ]</li>
        <li>[!UICONTROL フォールバックオファー ]</li>
        <li>[!UICONTROL パーソナライズされたオファー ]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        削除するレコードを選択します。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは、配置、決定、決定ルール、タグ、パーソナライズされたオファー、コレクションまたはフォールバックオファーを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL 接続 ]</td>
     <td>への接続を作成する手順 [!DNL Adobe Journey Optimizer]を参照してください。 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >への接続の作成 [!DNL Adobe Journey Optimizer]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL レコードタイプ ]
      </td>
      <td>
        更新するレコードのタイプを選択
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL 決定ルール ]</li>
        <li>[!UICONTROL 決定 ]</li>
        <li>[!UICONTROL タグ ]</li>
        <li>[!UICONTROL コレクション ]</li>
        <li>[!UICONTROL フォールバックオファー ]</li>
        <li>[!UICONTROL パーソナライズされたオファー ]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        更新するレコードを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL フィールド ]
      </td>
      <td>更新する各フィールドに対して、次の操作を実行します。
      <ol>
      <li>クリック <b>[!UICONTROL 追加 ]</b>.</li>
      <li>値の追加、置換、削除のどれを行うかを選択します。</li>
      <li>更新するフィールドを入力します。</li>
      <li>フィールドの新しい値を入力します。</li>
      </td>
    </tr>

</tbody>
</table>


### 検索

#### [!UICONTROL レコードのリスト]

この検索モジュールは、選択したタイプのレコードをリストし、指定した条件に基づいて結果を返します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL 接続 ]</td>
     <td>への接続を作成する手順 [!DNL Adobe Journey Optimizer]を参照してください。 <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >への接続の作成 [!DNL Adobe Journey Optimizer]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコードタイプ ]</p>
      </td>
      <td>
        <p>リストするレコードの種類を選択します。</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL 決定ルール ]</li>
        <li>[!UICONTROL 決定 ]</li>
        <li>[!UICONTROL タグ ]</li>
        <li>[!UICONTROL コレクション ]</li>
        <li>[!UICONTROL フォールバックオファー ]</li>
        <li>[!UICONTROL パーソナライズされたオファー ]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL クエリ演算子 ]</p>
      </td>
      <td>
        <p>クエリ内のパラメーターに適用する演算子を選択</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL フィールド ]</td>
      <td><p>検索を特定のフィールドに限定する場合は、フィールドを入力します。 検索範囲を制限する各フィールドに対して、「[!UICONTROL 項目を追加 ]」をクリックし、フィールド名を入力します。</p><p>パス式は、ドット区切りのパス ( 例： <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>結果を並べ替えるプロパティを入力またはマッピングします。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 順序の方向 ]</td>
   <td>昇順または降順のどちらで結果を並べ替えるかを選択します。
    </td>
     </tr>
  </tbody>
</table>
