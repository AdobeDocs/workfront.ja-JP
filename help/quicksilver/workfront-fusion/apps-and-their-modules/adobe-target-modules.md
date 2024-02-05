---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target モジュール
description: ' [!DNL Adobe Workfront Fusion] シナリオ内で、 [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target]  モジュールを使用するワークフローを自動化すると、レコードの作成、読み取り、更新および削除、特定のタイプのすべてのレコードのリスト作成、指定した条件に基づくレコードの検索または  [!DNL Adobe Target]  API へのカスタム API 呼び出しの実行を行うことができます。'
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: c0be0a1f21d5db3a480485a39e019a129d248574
workflow-type: tm+mt
source-wordcount: '2665'
ht-degree: 100%

---

# [!DNL Adobe Target] モジュール

[!DNL Adobe Workfront Fusion] シナリオ内で、[!DNL Adobe Target] を使用し、複数のサードパーティのアプリケーションやサービスに接続するワークフローを自動化できます。[!DNL Adobe Target] モジュールを使用すると、レコードの作成、読み取り、更新または削除、特定のタイプのすべてのレコードのリスト作成、指定した条件に基づくレコードの検索または [!DNL Adobe Target] API へのカスタム API 呼び出しの実行を行うことができます。


シナリオの作成手順について詳しくは、[シナリオの作成](../../workfront-fusion/scenarios/create-a-scenario.md)を参照してください。

モジュールについては、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td>
    </tr>
    </tr>
  </tbody>
</table>


ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Adobe Target] コネクタを使用する前に、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!DNL Adobe Target] アカウントが必要です。

## [!DNL Adobe Target] への接続の作成

[!DNL Adobe Target] モジュールの接続を作成するには、次の手順に従います。

1. 「接続」ボックスの横に表示される「**[!UICONTROL 追加]**」をクリックします。

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
        <td>[!DNL Adobe] クライアント ID を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>[!DNL Adobe] クライアントの秘密鍵を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>[!DNL Adobe] 組織 ID を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>[!DNL Adobe] テクニカルアカウント ID を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tenant]</td>
        <td>
          <p> テナントを見つけるには、[!DNL Adobe Experience Cloud] にログインして、[!DNL Target] を開き、[!DNL Target] カードをクリックします。URL サブドメインで指定されているように、テナント ID の値を使用します。</p>
          <p>例えば、[!DNL Adobe Target] ログイン時に URL が <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> の場合、テナント ID は「mycompany」になります。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>入力 <code>ent_marketing_sdk</code>       </td>
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

## [!DNL Adobe Target] モジュールとそのフィールド

[!DNL Adobe Target] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Target] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#actions)

* [検索](#searches)


### アクション

* [[!UICONTROL レコードを作成]](#create-a-record)

* [[!UICONTROL カスタム API 呼び出しを実行]](#make-a-custom-api-call)

* [[!UICONTROL レコードを削除]](#delete-a-record)

* [[!UICONTROL レコードの読み取り]](#read-a-record)

* [[!UICONTROL レコードを更新]](#update-a-record)


#### [!UICONTROL レコードを作成]

このアクションモジュールは、AB または XT のアクティビティ、オファーまたはオーディエンスを作成します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続を作成を参照してください。</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Record type]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>作成するレコードのタイプを選択します。</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p><a href="#ab-activity-fields" class="MCXref xref" >AB アクティビティフィールド</a>に進みます。</p>
        </li>
        <li>
          <p>[!UICONTROL XT Activity]</p>
          <p><a href="#xt-activity-fields" class="MCXref xref" >XT アクティビティフィールド</a>に進みます。</p>
        </li>
        <li>
          <p>[!UICONTROL Offer]</p>
          <p><a href="#offer-fields" class="MCXref xref" >オファーフィールド</a>に進みます。</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p><a href="#audience-fields" class="MCXref xref" >オーディエンスフィールド</a>に進みます。</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>このアクティビティの名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>アクティビティに追加する各オプションで、<b>[!UICONTROL Add item]</b> をクリックして、次のフィールドに入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>API リクエストをまたいでオプションを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>オプションの名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>オプションに関連付けられたオファーを選択またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>アクティビティに追加する mbox ごとに、<b>[!UICONTROL Add item]</b> をクリックして、次のフィールドに入力します。</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>mbox に追加するオーディエンスごとに、<b>[!UICONTROL Add item]</b> をクリックして、「オーディエンス ID 」を選択します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>API リクエスト全体で場所を追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>場所の名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>コンテンツオファーが提供されるページ上の場所のリスト。場所には次の情報が含まれます。
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>エクスペリエンスの ID の入力またはマッピング</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>エクスペリエンスの名前を入力またはマッピング

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>エクスペリエンスを表示するオーディエンスごとに、<b>[!UICONTROL Add item]</b> をクリックして、オーディエンス ID を入力します。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>エクスペリエンスに割り当てられる訪問者の割合を入力またはマッピングします</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>このアクティビティを識別する ID を入力またはマッピングします。この ID を選択できます。この ID は、他のアクティビティと同じにすることはできません。また、250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>アクティビティを開始する日付と時刻を <code>YYYY-MM-DD hh:mm:ss.z</code> 形式で入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>アクティビティを終了する日付と時刻を <code>YYYY-MM-DD hh:mm:ss.z</code> 形式で入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>アクティビティの状態を入力またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>アクティビティの優先度を定義する数値を入力します。数値が大きいほど、優先度が高くなります。この値は 0 ～ 999 の範囲で設定する必要があります。デフォルト値は 5 です。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>トラフィックを自動配分するには、このオプションを有効にします。自動配分により、より多くのトラフィックがより効果の高いエクスペリエンスに送信されます。</p>
        <p>どのエクスペリエンスがより効果が高いかを判断するための評価基準を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>アクティビティが関連付けられているワークスペースを入力またはマッピングします</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>アクティビティに追加する各プロパティで、「<b>[!UICONTROL Add item]</b>」をクリックして、プロパティの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>アクティビティに追加するレポートオーディエンスごとに、「[!UICONTROL Add item]」をクリックし、次の情報を入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>API リクエスト全体でレポートオーディエンスを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>レポートで使用するセグメントを入力またはマッピングします</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>API リクエスト全体で指標を追跡するために使用する文字列を入力またはマッピングします。</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>このアクティビティの名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>アクティビティに追加する各オプションで、<b>[!UICONTROL Add item]</b> をクリックして、次のフィールドに入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>API リクエストをまたいでオプションを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>オプションの名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>オプションに関連付けられたオファーを選択またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Locations]</td>
      <td>
        <p>アクティビティに追加する mbox ごとに、<b>[!UICONTROL Add item]</b> をクリックして、次のフィールドに入力します。</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>mbox に追加するオーディエンスごとに、<b>[!UICONTROL Add item]</b> をクリックして、「オーディエンス ID 」を選択します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>API リクエスト全体で場所を追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>場所の名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>コンテンツオファーが提供されるページ上の場所のリスト。場所には次の情報が含まれます。
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>エクスペリエンスの ID の入力またはマッピング</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>エクスペリエンスの名前を入力またはマッピング

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>エクスペリエンスを表示するオーディエンスごとに、<b>[!UICONTROL Add item]</b> をクリックして、オーディエンス ID を入力します。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>エクスペリエンスに割り当てられる訪問者の割合を入力またはマッピングします</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>このアクティビティを識別する ID を入力またはマッピングします。この ID を選択できます。この ID は、他のアクティビティと同じにすることはできません。また、250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>アクティビティを開始する日付と時刻を <code>YYYY-MM-DD hh:mm:ss.z</code> 形式で入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>アクティビティを終了する日付と時刻を <code>YYYY-MM-DD hh:mm:ss.z</code> 形式で入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>アクティビティの状態を入力またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>アクティビティの優先度を定義する数値を入力します。数値が大きいほど、優先度が高くなります。この値は 0 ～ 999 の範囲で設定する必要があります。デフォルト値は 5 です。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>トラフィックを自動配分するには、このオプションを有効にします。自動配分により、より多くのトラフィックがより効果の高いエクスペリエンスに送信されます。</p>
        <p>どのエクスペリエンスがより効果が高いかを判断するための評価基準を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>アクティビティが関連付けられているワークスペースを入力またはマッピングします</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>アクティビティに追加する各プロパティで、「<b>[!UICONTROL Add item]</b>」をクリックして、プロパティの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>アクティビティに追加するレポートオーディエンスごとに、「[!UICONTROL Add item]」をクリックし、次の情報を入力します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>API リクエスト全体でレポートオーディエンスを追跡するために使用する文字列を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>レポートで使用するセグメントを入力またはマッピングします</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>API リクエスト全体で指標を追跡するために使用する文字列を入力またはマッピングします。</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>このアクティビティの名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>ユーザーに表示するオファーのコンテンツを入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>オファーに関連付けられているワークスペースの ID を入力またはマッピングします。空白の場合、オファーはアカウントのデフォルトのワークスペースに関連付けられます。この機能は、[!DNL Target] Premium アカウントのみに適用します。</p>
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
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>このオーディエンスの名前を入力またはマッピングします。名前は 250 文字以下にする必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>このオーディエンスの説明を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>切替スイッチを有効にしてルールを AND にすることで、すべてのルールが適用されるようにする必要があります。</p>
        <p>オーディエンスに適用する各ルールで、「<b>[!UICONTROL Add item]</b>」をクリックして、適用するルールの JSON を入力します。 </p>
        <div class="example"><span class="autonumber"><span><b>例：</b></span></span>
          <p>例：</p>
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
        <p>オーディエンスに関連付けられたワークスペースの ID を入力またはマッピングします。空白の場合、オファーはアカウントのデフォルトのワークスペースに関連付けられます。この機能は、[!DNL Target Premium] アカウントのみに適用します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL カスタム API 呼び出しを行う]

このモジュールは、[!DNL Adobe Target] API に対してカスタム API 呼び出しを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続の作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Base URL]</td>
      <td>[!DNL Target] ベース URL を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>{baseURL}/ に対する相対パスの入力</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例： <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 認証ヘッダーおよび x-api-key ヘッダーを自動的に追加します。</p>
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
  </tbody>
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、1 つの AB アクティビティ、XT アクティビティ、オファーまたはオーディエンスを削除します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続を作成を参照してください。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>削除するレコードのタイプを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
    <td>削除するレコードの ID を入力またはマッピングします。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、1 つのアクティビティ、オファー、オーディエンス、プロパティまたはレポートのデータを取得します。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続を作成を参照してください。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>読み取るレコードのタイプを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record ID]</td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>
        <p>更新するレコードのタイプを選択します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>詳しくは、<a href="#create-a-record" class="MCXref xref" >レコードの作成</a>の <a href="#ab-activity-fields" class="MCXref xref" >AB アクティビティフィールド</a>のフィールド説明を参照してください。</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT Activity]</b>
            </p>
            <p>詳しくは、<a href="#create-a-record" class="MCXref xref" >レコードの作成</a>の <a href="#xt-activity-fields" class="MCXref xref" >XT アクティビティフィールド</a>のフィールド説明を参照してください。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Other Activity]</b>
            </p>
            <p>値を更新するフィールドを選択し、そのフィールドに新しい値を入力します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer]</b>
            </p>
            <p>詳しくは、<a href="#create-a-record" class="MCXref xref" >レコードの作成</a>の<a href="#offer-fields" class="MCXref xref" >オファーフィールド</a>のフィールド説明を参照してください。</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>詳しくは、<a href="#create-a-record" class="MCXref xref" >レコードの作成</a>の<a href="#audience-fields" class="MCXref xref" >オーディエンスフィールド</a>のフィールド説明を参照してください。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>更新するレコードのタイプを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sort by]</td>
      <td>並べ替えるフィールドごとに、「<b>[!UICONTROL Add item]</b>」をクリックして、フィールドを選択して、返される結果を昇順または降順のどちらにするかを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts At]</td>
      <td>
        <p>レコードを取得する最も早い日付を入力します。 </p>
        <p>サポートされる日付と時刻の形式のリストについて詳しくは、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends At]</td>
      <td>
        <p>レコードを取得する最新の日付を入力します。 </p>
        <p>サポートされる日付と時刻の形式のリストについて詳しくは、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制を参照してください。</p>
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
    <td role="rowheader">[!UICONTROL Connection]</td>
    <td>[!DNL Adobe Target] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-target" class="MCXref xref" >[!DNL Adobe Target]</a> への接続を作成を参照してください。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record type]</td>
    <td>更新するレコードのタイプを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Sort by]</td>
    <td>並べ替えるフィールドごとに、「<b>[!UICONTROL Add item]</b>」をクリックして、フィールドを選択し、返される結果を昇順または降順のどちらにするかを選択します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Search criteria]</td>
    <td>設定するルールごとに、フィールド、演算子および値を選択します。「<b>[!UICONTROL Add AND rule]</b>」をクリックして、追加のルールを作成します。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>モジュールが返す最初の応答の数を入力します。最初に返された応答のオフセットは <code>0</code> です。このフィールドを [!UICONTROL Maximum number of returned results] フィールドと組み合わせて使用し、応答をページ番号付けします。</p>
      <p>例えば、応答の 3 ページ目を表示する際、各ページに 10 件の応答がある場合、[!UICONTROL Offset] を 20 に、[!UICONTROL Maximum number of returned] の結果を 10 に設定します。</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Maximum number of returned results]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。このフィールドを [!UICONTROL Offset] フィールドと組み合わせて使用し、応答をページ番号付けします。</p>
      <p>例えば、応答の 3 ページ目を表示する際、各ページに 10 件の応答がある場合、[!UICONTROL Offset] を 20 に、[!UICONTROL Maximum number of returned] の結果を 10 に設定します。</p>
    </td>
  </tr>
</tbody>
</table>
