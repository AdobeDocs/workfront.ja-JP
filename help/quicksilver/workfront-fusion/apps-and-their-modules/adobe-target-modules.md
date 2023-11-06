---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Targetモジュール
description: 内、 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] モジュールを使用すると、レコードの作成、読み取り、更新、削除、特定のタイプのすべてのレコードのリスト作成、指定した条件に基づくレコードの検索、または [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 51db439995430dad86e41190520824743216df69
workflow-type: tm+mt
source-wordcount: '2646'
ht-degree: 0%

---

# [!DNL Adobe Target] モジュール

内、 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Adobe Target]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。 [!DNL Adobe Target] モジュールを使用すると、レコードの作成、読み取り、更新、削除、特定のタイプのすべてのレコードのリスト作成、指定した条件に基づくレコードの検索、または [!DNL Adobe Target] API.


シナリオの作成手順については、 [シナリオの作成](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
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
      <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td>
    </tr>
    </tr>
  </tbody>
</table>


ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する前に、 [!DNL Adobe Target] コネクタを使用する場合は、次の前提条件が満たされていることを確認する必要があります。

* アクティブなが必要です [!DNL Adobe Target] アカウント。

## への接続の作成 [!DNL Adobe Target]

の接続を作成するには、以下を実行します。 [!DNL Adobe Target] モジュール：

1. クリック **[!UICONTROL 追加]** 「接続」ボックスの横に表示されます。

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
        <td>を入力します。 [!DNL Adobe] クライアント ID。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
        <td>を入力します。 [!DNL Adobe] クライアントの秘密鍵。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 組織 ID]</td>
        <td>を入力します。 [!DNL Adobe] 組織 ID。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL テクニカルアカウント ID]</td>
        <td>を入力します。 [!DNL Adobe] テクニカルアカウント ID。 これは、 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL テナント ]</td>
        <td>
          <p> テナントを見つけるには、 [!DNL Adobe Experience Cloud]，開く [!DNL Target]をクリックし、 [!DNL Target] カード。 URL サブドメインで指定されているように、テナント ID の値を使用します。</p>
          <p>例えば、 [!DNL Adobe Target] 次に該当 <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> テナント ID が「mycompany」になります。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL メタスコープ ]</td>
        <td>入力 <code>ent_marketing_sdk</code>       </td>
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

## [!DNL Adobe Target] モジュールとそのフィールド

設定時に [!DNL Adobe Target] モジュール、 [!DNL Workfront Fusion] に、以下のフィールドを示します。 これらと共に、 [!DNL Adobe Target] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [であるモジュールから別のモジュールに情報をマッピングします。 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#actions)

* [検索](#searches)


### アクション

* [[!UICONTROL レコードの作成]](#create-a-record)

* [[!UICONTROL カスタム API 呼び出しをおこなう]](#make-a-custom-api-call)

* [[!UICONTROL レコードの削除]](#delete-a-record)

* [[!UICONTROL レコードを読み取る]](#read-a-record)

* [[!UICONTROL レコードの更新]](#update-a-record)


#### [!UICONTROL レコードの作成]

このアクションモジュールは、AB または XT のアクティビティ、オファーまたはオーディエンスを作成します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL 接続 ]</td>
    <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL レコードタイプ ]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>作成するレコードのタイプを選択します。</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>続行 <a href="#ab-activity-fields" class="MCXref xref" >AB アクティビティフィールド</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT アクティビティ ]</p>
          <p>続行 <a href="#xt-activity-fields" class="MCXref xref" >XT アクティビティフィールド</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p>続行 <a href="#offer-fields" class="MCXref xref" >オファーフィールド</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>続行 <a href="#audience-fields" class="MCXref xref" >オーディエンスフィールド</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB アクティビティフィールド

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>このアクティビティの名前を入力またはマップします。 名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL オプション ]</td>
      <td>
        <p>アクティビティに追加する各オプションで、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>API リクエストをまたいでオプションを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>オプションの名前を入力またはマッピングします。 名前は 250 文字以下にする必要があります。</p>
          </li>
          <li>
            <p><b>[!UICONTROL オファー ID]</b>
            </p>
          </li>
          <li>
            <p>「 」オプションに関連付けられたオファーを選択またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL の場所 ]</td>
      <td>
        <p>アクティビティに追加する mbox ごとに、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p>
        <ul>
          <li>
            <p>[!UICONTROL オーディエンス ID]</p>
            <p>Mbox に追加するオーディエンスごとに、 <b>[!UICONTROL 項目を追加 ]</b> 「オーディエンス ID 」を選択します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL 場所のローカル ID]</b>
            </p>
            <p>API リクエストをまたいで場所を追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>ロケーションの名前を入力またはマッピングします。 名前は 250 文字以下にする必要があります。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL エクスペリエンス ]</td>
      <td>
        <p>コンテンツオファーが提供されるページ上の場所のリスト。 場所には次の情報が含まれます。
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>エクスペリエンスの ID を入力またはマッピング</p>
          </li>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>エクスペリエンスの名前を入力またはマッピング

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>エクスペリエンスを表示するオーディエンスごとに、 <b>[!UICONTROL 項目を追加 ]</b> オーディエンス ID を入力します。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL 訪問者の割合 ]</b>
            </p>
            <p>エクスペリエンスに割り当てられる訪問者の割合を入力またはマッピングします</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 指標 ]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL サードパーティ ID]</td>
      <td>このアクティビティを識別する ID を入力またはマッピングします。 この ID を選択できます。 この ID は、他のアクティビティと同じにすることはできません。また、250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 開始：]</td>
      <td>アクティビティを開始する日付と時刻を、形式で入力またはマッピングします <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 終了時刻：]</td>
      <td>アクティビティを終了する日付と時刻を形式で入力またはマッピングします <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 状態 ]</td>
      <td>
        <p>アクティビティの状態を入力またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL 承認済み ]</p>
          </li>
          <li>
            <p>[!UICONTROL 非アクティブ化済み ]</p>
          </li>
          <li>
            <p>[!UICONTROL 一時停止 ]</p>
          </li>
          <li>
            <p>[!UICONTROL が保存されました ] </p>
          </li>
          <li>
            <p>[!UICONTROL 削除済み ]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 優先度 ]</td>
      <td>アクティビティの優先度を定義する数値を入力します。 数値が大きいほど、優先度が高くなります。 この値は 0 ～ 999 の範囲で設定する必要があります。 デフォルト値は 5 です。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 自動配分トラフィック ]</td>
      <td>
        <p>トラフィックを自動配分するには、このオプションを有効にします。 自動配分では、より多くのトラフィックを、より成功したエクスペリエンスに送信します。</p>
        <p>どのエクスペリエンスがより効果が高いかを判断するための評価基準を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>アクティビティが関連付けられているワークスペースを入力またはマッピングします</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL プロパティ ID] </td>
      <td>アクティビティに追加する各プロパティで、 <b>[!UICONTROL 項目を追加 ]</b> プロパティの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting Audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>アクティビティに追加するレポートオーディエンスごとに、「[!UICONTROL 項目を追加 ]」をクリックし、次の情報を入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience Local ID]</b>
            </p>
            <p>API リクエストをまたいでレポート用オーディエンスを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>レポートで使用するセグメントを入力またはマッピングします</p>
          </li>
          <li>
            <p><b>[!UICONTROL 指標ローカル ID]</b>
            </p>
            <p>API リクエストをまたいで指標を追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### XT アクティビティフィールド

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>このアクティビティの名前を入力またはマップします。 名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL オプション ]</td>
      <td>
        <p>アクティビティに追加する各オプションで、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>API リクエストをまたいでオプションを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>オプションの名前を入力またはマッピングします。 名前は 250 文字以下にする必要があります。</p>
          </li>
          <li>
            <p><b>[!UICONTROL オファー ID]</b>
            </p>
          </li>
          <li>
            <p>「 」オプションに関連付けられたオファーを選択またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL の場所 ]</td>
      <td>
        <p>アクティビティに追加する mbox ごとに、 <b>[!UICONTROL 項目を追加 ]</b> 次のフィールドに入力します。</p>
        <ul>
          <li>
            <p>[!UICONTROL オーディエンス ID]</p>
            <p>Mbox に追加するオーディエンスごとに、 <b>[!UICONTROL 項目を追加 ]</b> 「オーディエンス ID 」を選択します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL 場所のローカル ID]</b>
            </p>
            <p>API リクエストをまたいで場所を追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>ロケーションの名前を入力またはマッピングします。 名前は 250 文字以下にする必要があります。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL エクスペリエンス ]</td>
      <td>
        <p>コンテンツオファーが提供されるページ上の場所のリスト。 場所には次の情報が含まれます。
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>エクスペリエンスの ID を入力またはマッピング</p>
          </li>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>エクスペリエンスの名前を入力またはマッピング

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>エクスペリエンスを表示するオーディエンスごとに、 <b>[!UICONTROL 項目を追加 ]</b> オーディエンス ID を入力します。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL 訪問者の割合 ]</b>
            </p>
            <p>エクスペリエンスに割り当てられる訪問者の割合を入力またはマッピングします</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 指標 ]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL サードパーティ ID]</td>
      <td>このアクティビティを識別する ID を入力またはマッピングします。 この ID を選択できます。 この ID は、他のアクティビティと同じにすることはできません。また、250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 開始：]</td>
      <td>アクティビティを開始する日付と時刻を、形式で入力またはマッピングします <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 終了時刻：]</td>
      <td>アクティビティを終了する日付と時刻を形式で入力またはマッピングします <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 状態 ]</td>
      <td>
        <p>アクティビティの状態を入力またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL 承認済み ]</p>
          </li>
          <li>
            <p>[!UICONTROL 非アクティブ化済み ]</p>
          </li>
          <li>
            <p>[!UICONTROL 一時停止 ]</p>
          </li>
          <li>
            <p>[!UICONTROL が保存されました ] </p>
          </li>
          <li>
            <p>[!UICONTROL 削除済み ]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 優先度 ]</td>
      <td>アクティビティの優先度を定義する数値を入力します。 数値が大きいほど、優先度が高くなります。 この値は 0 ～ 999 の範囲で設定する必要があります。 デフォルト値は 5 です。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 自動配分トラフィック ]</td>
      <td>
        <p>トラフィックを自動配分するには、このオプションを有効にします。 自動配分では、より多くのトラフィックを、より成功したエクスペリエンスに送信します。</p>
        <p>どのエクスペリエンスがより効果が高いかを判断するための評価基準を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>アクティビティが関連付けられているワークスペースを入力またはマッピングします</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL プロパティ ID] </td>
      <td>アクティビティに追加する各プロパティで、 <b>[!UICONTROL 項目を追加 ]</b> プロパティの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting Audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>アクティビティに追加するレポートオーディエンスごとに、「[!UICONTROL 項目を追加 ]」をクリックし、次の情報を入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience Local ID]</b>
            </p>
            <p>API リクエストをまたいでレポート用オーディエンスを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>レポートで使用するセグメントを入力またはマッピングします</p>
          </li>
          <li>
            <p><b>[!UICONTROL 指標ローカル ID]</b>
            </p>
            <p>API リクエストをまたいで指標を追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### オファーフィールド

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>このアクティビティの名前を入力またはマップします。 名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コンテンツ ]</td>
      <td>
        <p>ユーザーに表示するオファーのコンテンツを入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>オファーに関連付けられているワークスペースの ID を入力またはマッピングします。 空白の場合、オファーはアカウントのデフォルトのワークスペースに関連付けられます。 この機能は、 [!DNL Target] プレミアムアカウント。</p>
      </td>
    </tr>
  </tbody>
</table>

##### オーディエンスフィールド

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>このオーディエンスの名前を入力またはマッピングします。 名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コンテンツ ]</td>
      <td>
        <p>このオーディエンスの説明を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target ルール ]</td>
      <td>
        <p>切り替えを有効にしてルールを AND にする（つまり、すべてのルールを適用する）。</p>
        <p>オーディエンスに適用する各ルールで、 <b>[!UICONTROL 項目を追加 ]</b> をクリックし、適用するルールの JSON を入力します。 </p>
        <div class="example"><span class="autonumber"><span><b>例: </b></span></span>
          <p>例:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>オーディエンスに関連付けられたワークスペースの ID を入力またはマッピングします。 空白の場合、オファーはアカウントのデフォルトのワークスペースに関連付けられます。 この機能は、 [!DNL Target Premium] アカウント。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL カスタム API 呼び出しをおこなう]

このモジュールは、 [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] ベース URL]</td>
      <td>を入力またはマッピングします。 [!DNL Target] ベース URL。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL パス ]</p>
      </td>
      <td>
        <p>相対パスを入力 {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL メソッド ]</p>
      </td>
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">での HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p>
        <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] は、認証ヘッダーと x-api-key ヘッダーを自動的に追加します。</p>
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
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件ステートメント ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、1 つの AB アクティビティ、XT アクティビティ、オファーまたはオーディエンスを削除します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL 接続 ]</td>
    <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL レコードタイプ ]</td>
    <td>削除するレコードのタイプを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL レコード ID]</td>
    <td>削除するレコードの ID を入力またはマッピングします。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、1 つのアクティビティ、オファー、オーディエンス、プロパティ、またはレポートのデータを取得します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL 接続 ]</td>
    <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL レコードタイプ ]</td>
    <td>読み取るレコードの種類を選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL レコード ID]</td>
    <td>読み取るレコードの ID を入力またはマップします。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは、アクティビティ、オファーまたはオーディエンスを更新します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レコードタイプ ]</td>
      <td>
        <p>更新するレコードのタイプを選択します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>詳しくは、 <a href="#ab-activity-fields" class="MCXref xref" >AB アクティビティフィールド</a> under <a href="#create-a-record" class="MCXref xref" >レコードの作成</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT アクティビティ ]</b>
            </p>
            <p>詳しくは、 <a href="#xt-activity-fields" class="MCXref xref" >XT アクティビティフィールド</a> under <a href="#create-a-record" class="MCXref xref" >レコードの作成</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL その他のアクティビティ ]</b>
            </p>
            <p>値を更新するフィールドを選択し、そのフィールドに新しい値を入力します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>詳しくは、 <a href="#offer-fields" class="MCXref xref" >オファーフィールド</a> under <a href="#create-a-record" class="MCXref xref" >レコードの作成</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>詳しくは、 <a href="#audience-fields" class="MCXref xref" >オーディエンスフィールド</a> under <a href="#create-a-record" class="MCXref xref" >レコードの作成</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レコード ID]</td>
      <td>更新するレコードの ID を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### 検索

* [[!UICONTROL レコードの取得]](#get-records)

* [[!UICONTROL 検索]](#search)


#### [!UICONTROL レコードの取得]

この検索モジュールは、選択したタイプのレコードのリストを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レコードタイプ ]</td>
      <td>更新するレコードのタイプを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td>
      <td>並べ替えるフィールドごとに、 <b>[!UICONTROL 項目を追加 ]</b> 「 」フィールドで、および返される結果を昇順と降順のどちらにするかを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 開始時刻 ]</td>
      <td>
        <p>レコードを取得する最も早い日付を入力します。 </p>
        <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 終了時刻 ]</td>
      <td>
        <p>レコードを取得する最新の日付を入力します。 </p>
        <p>サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 検索]

この検索モジュールは、指定した条件に基づいてアクティビティ、オファーまたはオーディエンスを検索します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL 接続 ]</td>
    <td>への接続を作成する手順については、 [!DNL Adobe Target]を参照してください。 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >への接続の作成 [!DNL Adobe Target]</a> 」を参照してください。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL レコードタイプ ]</td>
    <td>更新するレコードのタイプを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td>
    <td>並べ替えるフィールドごとに、 <b>[!UICONTROL 項目を追加 ]</b> 「 」フィールドで、および返される結果を昇順と降順のどちらにするかを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 検索条件 ]</td>
    <td>設定するルールごとに、フィールド、演算子および値を選択します。 クリック <b>[!UICONTROL AND ルールの追加 ]</b> をクリックして、追加のルールを作成します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL オフセット ]</td>
    <td>
      <p>モジュールが返す最初の応答の数を入力します。 最初に返された応答のオフセットは <code>0</code>. このフィールドを「返される結果の最大数」フィールドと組み合わせて使用し、回答をページ番号付けします。</p>
      <p>例えば、応答の 3 ページ目を表示するには、各ページに 10 件の応答がある場合、[!UICONTROL Offset] を 20 に、[!UICONTROL Maximum number of returned] の結果を 10 に設定します。</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 返される結果の最大数 ]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。 このフィールドを [!UICONTROL Offset] フィールドと組み合わせて使用し、回答をページ番号付けします。</p>
      <p>例えば、応答の 3 ページ目を表示するには、各ページに 10 件の応答がある場合、[!UICONTROL Offset] を 20 に、[!UICONTROL Maximum number of returned] の結果を 10 に設定します。</p>
    </td>
  </tr>
</tbody>
</table>
