---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Adobe Journey Optimizer] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '1602'
ht-degree: 100%

---

# [!DNL Adobe Journey Optimizer] モジュール

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Adobe Journey Optimizer] を使用するワークフローを自動化したり、複数のサードパーティのアプリケーションやサービスに接続したりすることができます。[!DNL Adobe Journey Optimizer] モジュールを使用すると、レコードの作成、読み取り、更新、削除をしたり、[!DNL Adobe Journey Optimizer] API へのカスタム API 呼び出しを行ったりできます。


シナリオの作成手順が必要な場合は、[](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについては、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
      <td>
        <p>[!UICONTROL Pro] 以降</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
      <td>
        <p>[!UICONTROL Plan]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td>
      <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件がありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織が [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織が [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td>
    </tr>
  </tbody>
</table>


ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Adobe Journey Optimizer] コネクタを使用する前に、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!DNL Adobe Journey Optimizer] アカウントが必要です。

## [!DNL Adobe Journey Optimizer] への接続の作成

[!DNL Adobe Journey Optimizer] モジュールへの接続を作成するには、以下を実行します。

1. 任意の [!DNL Adobe Journey Optimizer] モジュールで、「接続」ボックスの横にある「**[!UICONTROL 追加]**」をクリックします。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>この接続の名前を入力します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]</td>
          <td>[!DNL Adobe] [!UICONTROL Client ID] を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>[!DNL Adobe] [!UICONTROL Client Secret] を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Technical account ID]</td>
          <td>[!DNL Adobe] [!UICONTROL Technical account ID] を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organization ID]</td>
          <td>[!DNL Adobe] [!UICONTROL Organization ID] を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta scopes]</td>
          <td>
            接続に必要なメタスコープを入力します。
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Private key]</td>
          <td>
            <p>[!DNL Adobe Developer Console] で資格情報が作成された際に生成された秘密鍵を入力します。 </p>
            <p>秘密鍵または証明書を抽出するには：</p>
            <ol>
              <li value="1">
                <p><b>[!UICONTROL Extract]</b> をクリックします。</p>
              </li>
              <li value="2">
                <p>抽出するファイルのタイプを選択します。</p>
              </li>
              <li value="3">
                <p>秘密鍵または証明書を含むファイルを選択します。</p>
              </li>
              <li value="4">
                <p>ファイルのパスワードを入力します。</p>
              </li>
              <li value="5">
                <p><b>[!UICONTROL Save]</b> をクリックしてファイルを抽出し、接続設定に戻ります。</p>
              </li>
            </ol>
          </td>
        </tr>
      </tbody>
    </table>
1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。

## [!DNL Adobe Journey Optimizer] モジュールとそのフィールド

[!DNL Adobe Journey Optimizer] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Journey Optimizer] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でのモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL レコードを作成]](#create-a-record)
* [[!UICONTROL カスタム API 呼び出しを実行]](#make-a-custom-api-call)
* [[!UICONTROL レコードを削除]](#delete-a-record)
* [[!UICONTROL レコードを更新]](#update-a-record)

#### [!UICONTROL レコードを作成]

このアクションモジュールは、配置、決定ルール、タグ、パーソナライズされたオファー、コレクションまたはフォールバックオファーを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>[!DNL Adobe Journey Optimizer] への接続を作成する手順について詳しくは、<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >[!DNL Adobe Journey Optimizer]</a> への接続の作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        作成するレコードのタイプを選択
        <ul>
        <li><b>[!UICONTROL Placement]</b>：<a href="#placement-fields" >「[!UICONTROL Placement]」フィールド</a>に進みます。</li>
        <li><b>[!UICONTROL Decision rule]</b>：<a href="#decision-rule-fields" >「[!UICONTROL Decision rule]」フィールド</a>に進みます。</li>
        <li><b>[!UICONTROL Decision]</b>：<a href="#decision-fields" >「[!UICONTROL Decision]」フィールド</a>に進みます。</li>
        <li><b>[!UICONTROL Tag]</b>：<a href="#tag-fields" >「[!UICONTROL Tag]」フィールド</a>に進みます。</li>
        <li><b>[!UICONTROL Collection]</b>：<a href="#collection-fields" >「[!UICONTROL Collection]」フィールド</a>に進みます。</li>
        <li><b>[!UICONTROL Fallback offer]</b>：<a href="#fallback-offer-fields" >「[!UICONTROL Fallback offer]」フィールド</a>に進みます。</li>
        <li><b>[!UICONTROL Personalized offer]</b>：<a href="#personalized-offer-fields" >「[!UICONTROL Personalized offer]」フィールド</a>に進みます。</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 「[!UICONTROL 配置]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>配置の名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>配置の説明を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>


##### 「[!UICONTROL 決定ルール]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>説明ルールの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Description]
      </td>
      <td>決定ルールの説明を入力またはマッピングします。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Condition]
      </td>
      <td>決定ルールの条件を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>

##### 「[!UICONTROL 決定]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>説明ルールの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>決定のステータスを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>決定の開始日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>決定の終了日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Placements]</td>
      <td>この決定に追加する配置を選択
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Collection]</td>
      <td>この決定で考慮されるオファーを含むオファーコレクションを選択します。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fallback offer]</td>
      <td>この決定のルールに一致しない顧客に提示されるフォールバックオファーを選択します。
      </td>
    </tr>
  </tbody>
</table>

##### 「[!UICONTROL タグ]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>タグの名前を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

##### 「[!UICONTROL コレクション]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>コレクションの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Filter Type]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elements]
      </td>
      <td>コレクションに含めるタグを選択します。
      </td>
    </tr>
  </tbody>
</table>

##### 「[!UICONTROL フォールバックオファー]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>フォールバックオファーの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
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

##### 「[!UICONTROL パーソナライズされたオファー]」フィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>説明ルールの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>決定のステータスを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">プレースメント</td>
      <td>パーソナライズされたオファーの配置を選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Start date]</td>
      <td><p>パーソナライズされたオファーの開始日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL End date]</td>
      <td><p>パーソナライズされたオファーの終了日を入力またはマッピングします。</p><p>サポートされる日付形式のリストについては、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Decision rules]</td>
      <td>このパーソナライズされたオファーに追加する決定ルールを選択します。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>このオファーの優先度を選択します。優先度は、このオファーが別のオファーと比較して提示されるかどうかに影響します。
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Capping constraint]</td>
      <td>このオファーの表示回数を入力またはマッピングします。
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、[!DNL Adobe Journey Optimizer] 内のレコードを 1 つ削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
     <td>[!DNL Adobe Journey Optimizer] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >[!DNL Adobe Journey Optimizer]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        削除するレコードのタイプを選択
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        削除するレコードを選択します。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL カスタム API 呼び出しを実行]

このモジュールは、[!DNL Adobe Journey Optimizer] API に対してカスタム API 呼び出しを実行します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>[!DNL Adobe Journey Optimizer] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >[!DNL Adobe Journey Optimizer]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>次で始まる {baseURL} に対する相対パスを入力<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例： <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion は、認証ヘッダーと x-api-key ヘッダーを自動的に追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>リクエストクエリ文字列を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>モジュールが 1 回の実行サイクルで返す結果の最大数を入力します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、[!DNL Adobe Journey Optimizer] 内のレコードを 1 つ削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>[!DNL Adobe Journey Optimizer] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >[!DNL Adobe Journey Optimizer]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        削除するレコードのタイプを選択
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        削除するレコードを選択します。
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL レコードを更新]

このアクションモジュールは、配置、決定、決定ルール、タグ、パーソナライズされたオファー、コレクションまたはフォールバックオファーを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>[!DNL Adobe Journey Optimizer] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >[!DNL Adobe Journey Optimizer]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record type]
      </td>
      <td>
        更新するレコードのタイプを選択
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Placement]/[!UICONTROL Decision rule]/[!UICONTROL Decision]/[!UICONTROL Tag]/[!UICONTROL Collection]/[!UICONTROL Fallback offer]/[!UICONTROL Personalized offer]
      </td>
      <td>
        更新するレコードを選択します。
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Fields]
      </td>
      <td>更新する各フィールドに対して、次の操作を実行します。
      <ol>
      <li>「<b>[!UICONTROL Add]</b>」をクリックします。</li>
      <li>値の追加、置換、削除のどれを行うかを選択します。</li>
      <li>更新するフィールドを入力します。</li>
      <li>フィールドの新しい値を入力します。</li>
      </td>
    </tr>

</tbody>
</table>


### 検索

#### [!UICONTROL レコードをリスト]

この検索モジュールは、選択したタイプのレコードをリストし、指定した条件に基づいて結果を返します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>[!DNL Adobe Journey Optimizer] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >[!DNL Adobe Journey Optimizer]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type]</p>
      </td>
      <td>
        <p>リストに表示するレコードのタイプを選択します。</p>
        <ul>
        <li>[!UICONTROL Placement]</li>
        <li>[!UICONTROL Decision rule]</li>
        <li>[!UICONTROL Decision]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Collection]</li>
        <li>[!UICONTROL Fallback offer]</li>
        <li>[!UICONTROL Personalized offer]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>クエリ内のパラメーターに適用する演算子を選択する</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Fields]</td>
      <td><p>検索を特定のフィールドに限定する場合は、フィールドを入力します。検索範囲を制限する各フィールドに対して、「[!UICONTROL Add item]」をクリックし、フィールド名を入力します。</p><p>パス式は、<code>_instance.xdm:name</code> などのドットで区切られたパスの形式です。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by] </td>
      <td>結果を並べ替えるプロパティを入力またはマッピングします。
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order direction]</td>
   <td>昇順または降順のどちらで結果を並べ替えるかを選択します。
    </td>
     </tr>
  </tbody>
</table>
