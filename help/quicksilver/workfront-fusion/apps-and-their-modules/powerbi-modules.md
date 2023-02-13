---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Power BIモジュール
description: Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 6d6aaa4e85690307f93dfc5179a489a09e9a2381
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 0%

---

# [!DNL Power BI] モジュール

[!DNL Power BI] は、データを視覚化し、関係者に提示できるアプリケーションです。 様々なソースからデータを取得できます。

>[!NOTE]
>
>[!DNL Workfront Fusion] はデータソースではありません。 While [!DNL Workfront Fusion] はデータソースを作成して使用でき、データは保存されません。


## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

&#42;&#42;詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] モジュールとそのフィールド

設定時に [!DNL Power BI], [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、アプリやサービスでのアクセスレベルなどの要因に応じて、追加のフィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [Adobe Workfront Fusion で、モジュール間の情報のマッピング](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### ダッシュボード

#### [!UICONTROL ダッシュボードのリスト]

この検索モジュールは、ダッシュボードのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>リストするダッシュボードを所有するグループの ID を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
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
    <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ダッシュボード ID を入力 ]</td>
    <td>
      <p>「 」オプションを選択またはマッピングして、タイルを一覧表示するダッシュボードを選択します。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL ダッシュボード ID]</td>
    <td>
      <p>リストに表示するタイルが含まれるダッシュボードの ID を入力またはマッピングします。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Group ID]  </td>
    <td>リストするタイルを含むダッシュボードを所有するグループの ID を選択またはマッピングします。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL 制限 ]  </td>
    <td>
      <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL ダッシュボードの取得]

このアクションモジュールは、指定されたダッシュボードのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ダッシュボード ID を入力 ]</td>
      <td>
        <p>メタデータを取得するダッシュボードを選択するオプションを選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ダッシュボード ID]</td>
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

#### [!UICONTROL ダッシュボードタイルを取得する]

このアクションモジュールは、指定されたダッシュボードタイルのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ダッシュボード ID を入力 ]</td>
      <td>
        <p>「 」オプションを選択またはマッピングして、取得するダッシュボードの詳細を選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ダッシュボード ID]</td>
      <td>
        <p>詳細を取得するダッシュボードの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL タイル ID]</td>
      <td>の ID を入力またはマッピング [!DNL Power BI] 詳細を取得するタイル。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>取得するタイルを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL ダッシュボードの作成]

このアクションモジュールは、新しいダッシュボードを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>ダッシュボードの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>新しいダッシュボードを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### レポート

#### [!UICONTROL リストレポート]

この検索モジュールは、レポートのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>
        <p>リストするレポートを所有するグループの ID を選択またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レポートの取得]

このアクションモジュールは、指定されたレポートのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レポート ID の入力 ]</td>
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

#### [!UICONTROL レポートのコピー]

このアクションモジュールは、既存のレポートをコピーします。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レポート ID の入力 ]</td>
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
      <td role="rowheader">[!UICONTROL 新しくコピーされたレポート名 ]</td>
      <td>新しいレポートの名前を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL レポートの削除]

このアクションモジュールは、レポートを削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レポート ID の入力 ]</td>
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

### データセット

#### [!UICONTROL リストデータセット]

この検索モジュールは、データセットのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>メタデータを取得するレポートを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが [action] に設定するレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットの取得]

このアクションモジュールは、指定したデータセットのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レポート ID の入力 ]</td>
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

#### [!UICONTROL データセットの作成]

このアクションモジュールは、新しいデータセットを作成します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>データセットの名前を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>新しいデータセットを所有するグループの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL デフォルトモード ]</td>
      <td>
        <p>データセットのデフォルトモードを選択またはマッピングします。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>:へのライブ接続を持つデータセット [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>:へのライブ接続を持つデータセット [!DNL On-premise Analysis] サービス</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>:データをにプッシュするためのプログラムによるアクセスを可能にするデータセット [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>:データストリーミングをサポートし、データをにプログラムでプッシュするためのアクセスを可能にするデータセット [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>:データストリーミングをサポートするデータセット</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL テーブル ]</td>
      <td>データセットにテーブルを追加します。 フィールドについては、 <a href="#Table" class="MCXref_0">テーブルフィールド</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>データソースを追加します。 フィールドについては、 <a href="#Data" class="MCXref_0">データソースフィールド</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>データセットの意図的なポリシーを選択またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL なし ]</p>
          </li>
          <li>
            <p>[!UICONTROL 基本 FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### テーブルフィールド

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 名前 ]</td>
      <td>
        <p>  テーブルの名前を入力またはマップします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 列 ]</td>
      <td>
        <p>列を追加します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 名前 ]</b>
            </p>
            <p>列名を入力（マップ）します。</p>
          </li>
          <li>
            <p><b>[!UICONTROL データ型 ]</b>
            </p>
            <p>データタイプを選択またはマッピングします。</p>
            <ul>
              <li>
                <p>[!UICONTROL 文字列 ]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL 日時 ]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL 形式文字列 ]</b>
            </p>
            <p>フォーマット文字列を入力（マップ）します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 行 ]</td>
      <td>行の詳細を入力またはマップします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 測定 ]</td>
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
      <td role="rowheader">[!UICONTROL データベース ]  </td>
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
      <td role="rowheader">[!UICONTROL データソース ID]</td>
      <td>
        <p>  データソースの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Data Source Type]  </td>
      <td>
        <p>データソースタイプを選択またはマッピングします。 例：SQL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ゲートウェイ ID]  </td>
      <td>使用するゲートウェイの ID を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットテーブルの行の追加または削除]

このアクションモジュールは、指定したプッシュデータセットテーブルの行を追加または削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL テーブルを入力 ]</td>
      <td>調整するテーブルが含まれるデータセットを選択するオプションを選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL データセット ID]</td>
      <td>追加または削除する行が含まれるデータセットの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL テーブル名 ]  </td>
      <td>
        <p>追加または削除する行を含むテーブルの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>データセットを所有するグループの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アクションを選択 ]</td>
      <td>
        <p>実行するアクションを選択またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL 行の追加 ]</p>
          </li>
          <li>
            <p>[!UICONTROL すべての行を削除 ]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 行 ]</td>
      <td>
        <p>行フィールドを追加します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL キー ]</b>
            </p>
            <p>キー名を入力またはマップします。</p>
          </li>
          <li>
            <p><b>[!UICONTROL フィールドタイプ ]</b>
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
            <p>[!UICONTROL 値 ]</p>
            <p>キー値を入力またはマッピングします。</p>
          </li>
        </ul>
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
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL データセットを入力 ]</td>
      <td>更新するデータセットを選択するオプションを選択するか、マッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL データセット ID]</td>
      <td>更新するデータセットの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL テーブル名 ]  </td>
      <td>
        <p>追加または削除する行を含むテーブルの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Group ID]  </td>
      <td>データセットを所有するグループの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 通知オプション ]  </td>
      <td>
        <p>通知するオプションを選択またはマッピングします。</p>
        <ul>
          <li>
            <p>[!UICONTROL 完了時のメール ]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail on Failure]</p>
          </li>
          <li>
            <p>[!UICONTROL 通知なし ]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL データセットの削除]

このアクションモジュールは、データセットを削除します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レポート ID の入力 ]</td>
      <td>
        <p>削除するデータセットを選択するには、「 」オプションを選択するか、マッピングします。</p>
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

### アプリ

#### [!UICONTROL ウォッチアプリ]

このトリガーモジュールは、アプリが更新されるとシナリオを開始します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのリスト]

この検索モジュールは、インストールされているすべてのアプリのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのレポートのリスト]

この検索モジュールは、指定したアプリからすべてのレポートのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アプリ ID]</td>
      <td>レポートのリストを表示するアプリの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのダッシュボードのリスト]

この検索モジュールは、指定されたアプリからダッシュボードのリストを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アプリ ID]</td>
      <td>ダッシュボードのリストを表示するアプリの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]  </td>
      <td>
        <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリの入手]

このアクションモジュールは、指定されたアプリのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アプリ ID]  </td>
      <td>
        <p>取得するアプリの ID を選択またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アプリのレポートの取得]

このアクションモジュールは、指定したアプリのレポートのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アプリ ID]  </td>
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

#### [!UICONTROL アプリのダッシュボードを取得する]

このアクションモジュールは、指定したアプリのダッシュボードのメタデータを取得します。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アプリ ID]  </td>
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

### その他

#### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールは、 [!DNL Power BI] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Power BI] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL パス ]</p>
      </td>
      <td>
        <p>相対パスを入力 <code>https://api.powerbi.com</code>. 例: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL メソッド ]</p>
      </td>
      <td>
        <p>API 呼び出しを設定する必要がある [!UICONTROL HTTP] リクエストメソッドを選択します。 詳しくは、[!UICONTROL HTTP] リクエストメソッドを参照してください。</p>
      </td>
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
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
