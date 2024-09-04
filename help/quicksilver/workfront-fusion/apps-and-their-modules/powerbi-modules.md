---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Power BI モジュール
description: Adobe Workfront Fusion を使用するには、Adobe Workfront ライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 8dbb29b297d4f8840d5ecb81f819e89b5325f62c
workflow-type: tm+mt
source-wordcount: '2471'
ht-degree: 97%

---

# [!DNL Power BI] モジュール

[!DNL Power BI] は、データを視覚化し、関係者に提示できるアプリケーションです。様々なソースからデータを取得できます。

>[!NOTE]
>
>[!DNL Workfront Fusion] はデータソースではありません。[!DNL Workfront Fusion] はデータソースを作成して使用でき、データは保存されません。


## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
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
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Power BI] モジュールとそのフィールド

[!DNL Power BI] を設定すると、[!DNL Workfront Fusion] には以下のフィールドが表示されます。これらと共に、アプリやサービスのアクセスレベルなどの要因に応じて、追加のフィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[Adobe Workfront Fusion でのモジュール間の情報のマッピング](../../workfront-fusion/mapping/map-information-between-modules.md)を参照してください。

![](assets/map-toggle-350x74.png)

* [ダッシュボード](#dashboards)
* [レポート](#reports)
* [データセット](#dataset)
* [アプリ](#apps)
* [その他](#other)

### ダッシュボード

* [ダッシュボードの作成](#create-a-dashboard)
* [ダッシュボードの取得](#get-a-dashboard)
* [ダッシュボードタイルの取得](#get-a-dashboard-tile)
* [ダッシュボードタイルの一覧表示](#list-dashboard-tiles)
* [ダッシュボードのリスト](#list-dashboards)

#### [!UICONTROL ダッシュボードを作成]

このアクションモジュールは、新しいダッシュボードを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>ダッシュボードの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>新しいダッシュボードを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL ダッシュボードを取得]

このアクションモジュールは、指定されたダッシュボードのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>メタデータを取得するダッシュボードを選択するオプションを選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>メタデータを取得するダッシュボードの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>メタデータを取得するダッシュボードを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL ダッシュボードタイルを取得]

このアクションモジュールは、指定されたダッシュボードタイルのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
      <td>
        <p>オプションを選択またはマッピングしてて、取得するダッシュボードの詳細を選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard ID]</td>
      <td>
        <p>詳細を取得するダッシュボードの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tile ID]</td>
      <td>詳細を取得する [!DNL Power BI] タイルの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>取得するタイルを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL ダッシュボードタイルのリスト]

この検索モジュールは、ダッシュボードタイルのリストを取得します。

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Enter a Dashboard ID]</td>
    <td>
      <p>オプションを選択またはマッピングして、タイルをリストするダッシュボードを選択します。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard ID]</td>
    <td>
      <p>リストするタイルが含まれるダッシュボードの ID を入力またはマッピングします。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>リストするタイルを含むダッシュボードを所有するグループの ID を選択またはマッピングします。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL ダッシュボードのリスト]

この検索モジュールは、ダッシュボードのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>リストするダッシュボードを所有するグループの ID を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

### レポート

* [レポートのコピー](#copy-a-report)
* [レポートの削除](#delete-a-report)
* [レポートの取得](#get-a-report)
* [List Reports](#list-reports)

#### [!UICONTROL レポートをコピー]

このアクションモジュールは、既存のレポートをコピーします。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>コピーするレポートを選択するオプションを選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>コピーするレポートの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>コピーするレポートを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL New Copied Report Name]</td>
      <td>新しいレポートの名前を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レポートを削除]

このアクションモジュールは、レポートを削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>削除するレポートを選択するオプションを選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>削除するレポートの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>削除するレポートを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レポートを取得]

このアクションモジュールは、指定されたレポートのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>メタデータを取得するレポートを選択するオプションを選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>メタデータを取得するレポートの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>メタデータを取得するレポートを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レポートをリスト]

この検索モジュールは、レポートのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>リストするレポートを所有するグループの ID を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>


### データセット

* [データセットテーブルの行の追加/削除](#add-or-delete-rows-in-a-dataset-table)
* [データセットの作成](#create-a-dataset)
* [データセットの削除](#delete-a-dataset)
* [データセットの取得](#get-a-dataset)
* [リストデータセット](#list-datasets)
* [データセットを更新](#refresh-a-dataset)

#### [!UICONTROL データセットテーブルの行の追加または削除]

このアクションモジュールは、指定したプッシュデータセットテーブルの行を追加または削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a table]</td>
      <td>調整するテーブルが含まれるデータセットを選択するオプションを選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>追加または削除する行が含まれるデータセットの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>追加または削除する行を含むテーブルの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>データセットを所有するグループの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Select the Action]</td>
      <td>
        <p>実行するアクションを選択またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL Add rows]</p>
          </li>
          <li>
            <p>[!UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>
        <p>行フィールドを追加します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Key]</b>
            </p>
            <p>キー名を入力またはマッピングします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Field Type]</b>
            </p>
            <p>フィールドタイプを選択またはマッピングします。</p>
            <ul>
              <li>
                <p>ブール値</p>
              </li>
              <li>
                <p>日付</p>
              </li>
              <li>
                <p>テキスト</p>
              </li>
              <li>
                <p>数値</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Value]</p>
            <p>キー値を入力またはマッピングします。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットを作成]

このアクションモジュールは、新しいデータセットを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>データセットの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>新しいデータセットを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default Mode]</td>
      <td>
        <p>データセットのデフォルトモードを選択またはマッピングします。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>：次とのライブ接続を持つデータセット [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>：[!DNL On-premise Analysis] サービスとのライブ接続を持つデータセット</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>：次にデータをプッシュするためのプログラムでアクセスできるデータセット [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>：データストリーミングをサポートし、データを次にプログラムでプッシュするためのアクセスを可能にするデータセット [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>：データストリーミングをサポートするデータセット</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tables]</td>
      <td>データセットにテーブルを追加します。フィールドについては、<a href="#Table" class="MCXref_0">テーブルのフィールド</a>を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>データソースを追加します。フィールドについては、<a href="#Data" class="MCXref_0">データソースのフィールド</a>を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>データセットの意図的なポリシーを選択またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL None]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### テーブルのフィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  テーブルの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Columns]</td>
      <td>
        <p>列を追加します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>列名を入力（マッピング）します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL Data Type]</b>
            </p>
            <p>データタイプを選択またはマッピングします。</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Format String]</b>
            </p>
            <p>フォーマット文字列を入力（マッピング）します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rows]</td>
      <td>行の詳細を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Measures]</td>
      <td>テーブルの測定を追加します。</td>
    </tr>
  </tbody>
</table>

##### データソースフィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Database]  </td>
      <td>
        <p>使用するデータベースを入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>使用するサーバーの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>使用する URL を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source ID]</td>
      <td>
        <p>  データソースの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data source Type]  </td>
      <td>
        <p>データソースタイプを選択またはマッピングします。（例： SQL）。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>使用するゲートウェイの ID を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットの削除]

このアクションモジュールでは、データセットを削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>削除するデータセットを選択するオプションを選択するか、マッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>削除するデータセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>削除するデータセットを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットを取得]

このアクションモジュールは、指定したデータセットのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a Report ID]</td>
      <td>
        <p>メタデータを取得するレポートを選択するオプションを選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>メタデータを取得するデータセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>メタデータを取得するデータセットを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットをリスト]

この検索モジュールは、データセットのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>メタデータを取得するレポートを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>各シナリオ実行サイクルでモジュールに実行させる「アクション」の対象となるレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットの更新]

このアクションモジュールは、指定したデータセットを更新します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Enter a dataset]</td>
      <td>更新するデータセットを選択するオプションを選択するか、マッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dataset ID]</td>
      <td>更新するデータセットの ID を入力するか、マッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Table Name]  </td>
      <td>
        <p>追加または削除する行を含むテーブルの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>データセットを所有するグループの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Notify Option]  </td>
      <td>
        <p>通知するオプションを選択またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL No Notification]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### アプリ

* [アプリの取得](#get-an-app)
* [アプリのダッシュボードの取得](#get-an-apps-dashboard)
* [アプリのレポートの取得](#get-an-apps-report)
* [アプリのダッシュボードの一覧表示](#list-apps-dashboards)
* [アプリのレポートのリスト](#list-apps-reports)
* [アプリのリスト](#list-apps)
* [アプリを見る](#watch-apps)

#### [!UICONTROL アプリの入手]

このアクションモジュールでは、指定されたアプリのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>取得するアプリの ID を選択またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのダッシュボードの取得]

このアクションモジュールでは、指定したアプリのダッシュボードのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>取得するダッシュボードを含むアプリの ID を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  取得するダッシュボードの ID を選択またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのレポートの取得]

このアクションモジュールでは、指定したアプリのレポートのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>取得するレポートを含むアプリの ID を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Report ID]</td>
      <td>
        <p>  取得するレポートの ID を選択またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのリスト]

この検索モジュールでは、インストールされているすべてのアプリのリストが取得されます。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのダッシュボードのリスト]

この検索モジュールでは、指定されたアプリからダッシュボードのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>ダッシュボードのリスト元となるアプリの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのレポートのリスト]

この検索モジュールでは、指定したアプリからすべてのレポートのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>レポートのリスト元となるアプリの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリの監視]

このトリガーモジュールでは、アプリが更新された時点でシナリオを開始します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

### その他

#### [!UICONTROL API 呼び出しの実行]

このアクションモジュールは、[!DNL Power BI] API に対して API 呼び出しを実行します。　

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td> <p>[!DNL Power BI] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe [!DNL Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p><code>https://api.powerbi.com</code> への相対パスを入力します。例：<code>/v1.0/myorg/datasets</code>。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
        <p>API 呼び出しを設定する必要がある [!UICONTROL HTTP] リクエストメソッドを選択します。詳しくは、[!UICONTROL HTTP] リクエストメソッドを参照してください。</p>
      </td>
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
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件文を JSON で使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
