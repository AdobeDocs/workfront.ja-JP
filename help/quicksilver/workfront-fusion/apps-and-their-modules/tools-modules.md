---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: ツール
description: この [!DNL Adobe Workfront Fusion Tools] セクションには、シナリオを強化できる便利なモジュールがいくつか含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2290'
ht-degree: 0%

---

# [!UICONTROL ツール]

この [!DNL Adobe Workfront Fusion Tools] セクションには、シナリオを強化できる便利なモジュールがいくつか含まれています。

[!UICONTROL ツール] モジュールは、アプリのリストまたは [!UICONTROL ツール] アイコン ![](assets/tools-icon-small.png) 画面の下部に表示されます。

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ツール] そして彼らのフィールド

* [トリガー](#triggers)
* [アクション](#actions)
* [集約](#aggregators)
* [変換サービス](#transformers)

### トリガー

#### [!UICONTROL 基本トリガー]

このモジュールでは、カスタムトリガーを作成し、その入力バンドルを定義できます。

例えば、連絡先や、指定した電子メールアドレス ( [!UICONTROL 電子メール] >[!UICONTROL メールの送信]または [!DNL Gmail] >[!UICONTROL メールの送信] モジュール )、または必要に応じてトリガーされる簡単なリマインダーとして使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL バンドル ]</td> 
   <td> <p>配列項目を追加してカスタムバンドルを作成します。 この配列は、名前と値のペアで構成されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 複数の変数の取得]](#get-multiple-variables)
* [[!UICONTROL 変数を取得]](#get-variable)
* [[!UICONTROL Increment 関数]](#increment-function)
* [[!UICONTROL 複数の変数を設定]](#set-multiple-variables)
* [[!UICONTROL 変数を設定]](#set-variable)
* [[!UICONTROL スリープ]](#sleep)

#### [!UICONTROL 複数の変数の取得]

このモジュールは、以前に [!UICONTROL 変数を設定] または [!UICONTROL 複数の変数を設定] モジュール。

このモジュールは、変数が [!UICONTROL 複数の変数の取得] モジュールが見つかります。 唯一の要件は、 [!UICONTROL ツール] > [!UICONTROL 変数を設定] または [!UICONTROL ツール] > [!UICONTROL 複数の変数を設定] モジュールは [!UICONTROL ツール] > [!UICONTROL 複数の変数の取得] モジュール。 モジュールの実行順序について詳しくは、 [のルーターモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 変数 ]</td>
        <td>モジュールから取得する変数を追加します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 変数名 ]</td>
        <td>追加する変数ごとに、取得する変数の名前をマッピングします。</td>
    </tr>
</table>

>[!INFO]
>
>**例：**  以下は、 [!UICONTROL 設定]/[!UICONTROL （複数の）変数を取得] モジュール：
>
>* 異なる経路でも、計算値を後で使用するために記憶する。 これは、値が複数のモジュールで使用され、値を計算する数式が過度に複雑な場合に便利です。
>* 式をデバッグする場合。 モジュールで使用される数式が正しい結果を提供しないように見える場合は、数式をコピーして、 [!UICONTROL 変数を設定] 関連するモジュールの前に挿入するモジュール。 次の時間が経過した後で、モジュールを切断します。 [!UICONTROL 変数を設定] モジュール化し、シナリオを実行します。 を確認します。 [!UICONTROL 変数を設定] モジュールの出力、数式の調整または簡素化、シナリオの再実行、問題が解決するまで引き続き実行します。


#### [!UICONTROL 変数を取得]

このモジュールは、以前に [!UICONTROL 変数を設定] または [!UICONTROL 複数の変数を設定] モジュール。

このモジュールは、変数が [!UICONTROL 変数を取得] モジュールが見つかります。 唯一の要件は、 [!UICONTROL ツール] > [!UICONTROL 変数を設定] または [!UICONTROL ツール] > [!UICONTROL 複数の変数を設定] モジュールは [!UICONTROL ツール] > [!UICONTROL 変数を取得] モジュール。 モジュールの実行順序について詳しくは、 [のルーターモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 変数名 ]</td> 
   <td> <p>モジュールから取得する変数の名前をマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Increment 関数]

このモジュールは、各モジュールの操作後に 1 ずつ増加する値を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値のリセット ]</td> 
   <td> <p>モジュールで値を増分する場合に選択します。 </p> 
    <ul> 
     <li>[!UICONTROL 1 サイクル後 ]</li> 
     <li>[!UICONTROL 1 回のシナリオ実行後 ]</li> 
     <li>[!UICONTROL なし ]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例:**
>
>モジュールの使用の 1 つは、タスク、リード、E メールなどの「ラウンドロビン」割り当てをグループ内のユーザーに実装することです。 アルゴリズムは、ある合理的な順序でグループから担当者を選択します。通常は、リストの上から下に移動します。 アルゴリズムがリストの最後に到達すると、次の割り当てがリストの最上部にあるユーザーに与えられ、引き続きリストの下に割り当てが行われます。
>
>次のシナリオでは、奇数番号のシナリオを実行するたびに最初の受信者に E メールを送信し、偶数番号のシナリオを実行するたびに 2 番目の受信者に E メールを送信します。
>
>![](assets/example-email-350x246.gif)
>
>1. このシナリオを作成するには：
>1. モジュールの **[!UICONTROL 値をリセット]** フィールドを「なし」に設定します。
>1. 奇数値のルートを設定します。 次の値に等しい剰余数演算関数を使用して、このルートのフィルタを設定します。 `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **注意**:忘れずに [!UICONTROL 次と等しい] 演算子をデフォルトの [!UICONTROL テキスト] 演算子を [!UICONTROL 数値] 演算子
>
>1. 等しい係数計算関数を使用して偶数値のルートを設定 `0`:
>
>増分関数は、シナリオが実行されるたびに 1 つ追加します。 フィルターは、増分をチェックし、その値に基づいて処理するので、E メールが均等に配分されます。

#### [!UICONTROL 複数の変数を設定]

このモジュールは、ルート内の他のモジュールによってマッピング可能な変数を作成します。 変数は、 [!UICONTROL 変数を取得] または [!UICONTROL 複数の変数の取得] シナリオ内の任意のルートのモジュール。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 変数 ]</td> 
   <td>モジュールで設定する変数を追加します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変数名 ] </td> 
   <td>各変数に、変数名を入力します。 この名前は、他のモジュールで変数をマッピングする際に表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変数値 ] </td> 
   <td>各変数に、変数の値を入力します。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変数の有効期間 ] </td> 
   <td> <p>変数を有効にしておく期間を選択します（同じ値を維持）。</p> 
    <ul> 
     <li><strong>[!UICONTROL 1 サイクル ]</strong>:変数は 1 サイクルで有効です。 1 回のシナリオ実行で複数の Web フックを受け取る場合に役立ちます（より多くの Web フック=より多くのサイクル）。 </li> 
     <li><strong>[!UICONTROL 1 回の実行 ]</strong>:変数は、1 つのシナリオの実行に対して有効です。 1 つの実行に 1 つ以上のサイクルを含めることができます。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 変数を設定]

このモジュールは、ルート内の他のモジュールによってマッピングできる変数を作成します。 変数は、 [!UICONTROL 変数を取得] または [!UICONTROL 複数の変数の取得] シナリオ内の任意のルートのモジュール。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 変数名 ] </td> 
   <td>変数名を入力します。 この名前は、他のモジュールで変数をマッピングする際に表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変数の有効期間 ] </td> 
   <td> <p>変数を有効にしておく期間を選択します（同じ値を維持）。</p> 
    <ul> 
     <li><strong>[!UICONTROL 1 サイクル ]</strong>:変数は 1 サイクルで有効です。 1 回のシナリオ実行で複数の Web フックを受け取る場合に役立ちます（より多くの Web フック=より多くのサイクル）。 </li> 
     <li><strong>[!UICONTROL 1 回の実行 ]</strong>:変数は、1 つのシナリオの実行に対して有効です。 1 つの実行に 1 つ以上のサイクルを含めることができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変数値 ] </td> 
   <td>変数の値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL スリープ]

このモジュールでは、シナリオのフローを最大 300 秒（5 分）まで遅延させることができます。

この関数は、例えば、 [!DNL target] サービスサーバーの読み込み時、または一括 SMS や電子メールを送信する際に人間の行動を模倣する場合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 遅延 ]</p> </td> 
   <td> <p>シナリオを一時停止する秒数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>フローをより長い期間一時停止する場合は、シナリオを次の 2 つのシナリオに分割することをお勧めします。
>
>* 最初のシナリオには、一時停止の前の部分が含まれます。
>* 2 つ目のシナリオでは、その後の部分が含まれます。
>
>最初のシナリオでは、必要な情報をすべて現在のタイムスタンプと共にデータストアに保存します。 2 つ目のシナリオでは、データストアで、意図した遅延よりも古いタイムスタンプを持つレコードを定期的にチェックし、レコードを取得し、データの処理を完了し、データストアからレコードを削除します。
>
>データストアの詳細については、 [のデータストア [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>特定のデータストアモジュールについて詳しくは、 [[!UICONTROL データストア] モジュール](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### 集約

* [[!UICONTROL 数値集計]](#numeric-aggregator)
* [[!UICONTROL テーブル集約]](#table-aggregator)
* [[!UICONTROL テキスト集約]](#text-aggregator)

#### [!UICONTROL 数値集計]

このモジュールでは、数値を取得し、選択した関数 (SUM、AVG、COUNT、MAX、MIN) の 1 つを適用して、結果を 1 つのバンドルで返すことができます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL ソースモジュール ]</p> </td> 
   <td> <p>フィールドの集計元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 集計関数 ]</p> </td> 
   <td> <p>値の集計に使用する関数を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>集計出力をグループ化する式を定義します。 この式には、1 つ以上のマッピングされた項目を含めることができます。 集計されたデータは、この式の値を使用してグループに分割されます。 各グループは、キー（評価された式）と値（集計値）を持つ個別のバンドルとして出力されます。 キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 空の集計後に処理を停止 ]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 値 ]</p> </td> 
   <td> <p>集計する値を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブル集約]

このモジュールは、受け取ったバンドルの選択されたフィールドの値を、指定された列と行の区切り記号（テーブルを作成できる）を使用して 1 つのバンドルに結合します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL ソースモジュール ]</p> </td> 
   <td> <p>フィールドの集計元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 集計フィールド ]</td> 
   <td> <p> 上で選択したモジュールから、1 つのバンドルに集計する値を含むフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 列区切り記号 ]</p> </td> 
   <td> <p>結果のバンドルでフィールド値の列を区切る区切り文字のタイプを選択または入力します。 「その他」を選択した場合は、値の区切りに使用する文字を「区切り文字」フィールドに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 行の区切り文字 ]</p> </td> 
   <td> <p>結果のバンドルでフィールド値行を区切る区切り文字のタイプを選択または入力します。 「その他」を選択した場合は、値の区切りに使用する文字を「区切り文字」フィールドに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>集計出力をグループ化する式を定義します。 この式には、1 つ以上のマッピングされた項目を含めることができます。 集計されたデータは、この式の値を使用してグループに分割されます。 各グループは、キー（評価された式）と値（集計値）を持つ個別のバンドルとして出力されます。 キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 空の集計後に処理を停止 ]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テキスト集約]

このモジュールは、受け取ったバンドルの選択されたフィールドの値を 1 つのバンドルに結合します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL ソースモジュール ]</p> </td> 
   <td> <p>フィールドの集計元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 行の区切り文字 ]</p> </td> 
   <td> <p>結果のバンドルでフィールド値行を区切る区切り文字のタイプを選択または入力します。 「その他」を選択した場合は、値の区切りに使用する文字を「区切り文字」フィールドに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>1 つ以上のマッピングされた項目を含む式を定義します。 集計データは、同じ式の値を持つグループの下で分割されます。 各 Group は、評価された式と集計されたテキストを含むキーを含む個別のバンドルとして出力します。 これにより、キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テキスト ]</td> 
   <td> <p> モジュールを集計するテキストを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 空の集計後に処理を停止 ]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** テキスト集約を使用すると、1 つのバンドルにさらに多くの値（顧客名やメモなど）を挿入し、E メールの本文または件名に含まれるすべての値を含む E メールを送信できます。

### 変換サービス

* [[!UICONTROL 文字列を構成]](#compose-a-string)
* [[!UICONTROL テキストのエンコーディングを変換]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 切り替え]](#switch)

#### [!UICONTROL 文字列を構成]

任意の値を文字列データ型（テキスト）に変換します。 これにより、バイナリデータなどのマッピングが容易になります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL テキスト ]</td> 
   <td> <p>テキストに変換するデータを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テキストのエンコーディングを変換]

入力された入力テキスト（またはバイナリデータ）を選択されたエンコーディングに変換します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 入力データ ]</p> </td> 
   <td> <p>変換するコンテンツを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 入力データコードページ ]</td> 
   <td> <p>入力データのエンコーディングタイプを選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 出力データコードページ ]</p> </td> 
   <td> <p>ターゲット（出力）データのエンコーディングタイプを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 切り替え]

指定された値のリストと一致するかどうかを入力値で確認します。 結果に基づいて出力を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 入力 ]</p> </td> 
   <td> <p>評価する式を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 一致に正規表現を使用 ]</td> 
   <td> <p>正規表現を使用するには、このオプションを有効にします。 モジュールは、完全一致ではなく、正規表現に基づいて大文字と小文字を決定します。</p> 
    <div> 
     <p>正規表現とは、各文字がメタ文字で、特殊な意味を持つ文字、またはリテラル意味を持つ正規文字のシーケンスです。 これらの文字とメタ文字は、テキストの検索に使用できるパターンを識別します。 例えば、名前を検索する場合、大文字で始まる 2 つの連続する単語で構成されるパターンを検索する正規表現を設定できます。 正規表現は、テキストを検索および操作するための強力なツールです。</p> 
     <p>正規表現の議論は、この記事の範囲外です。 次のリソースをお勧めします。</p> 
     <ul> 
      <li>メタ文字の完全なリストについては、 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">正規表現</a> MDN web ドキュメントの。</li> 
      <li>正規表現の作成方法に関するチュートリアルについては、 <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>正規表現を試す場合は、 <a href="https://regex101.com/">正規表現 101</a> web サイト。 左側のパネルで ECMAScript (JavaScript) FLAVOR を選択します。</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ケース ] </td> 
   <td> <p>入力に「[!UICONTROL パターン ]」フィールドに入力された値が含まれている場合、「[!UICONTROL 出力 ]」フィールドに入力された値が返されます。</p> <p>[!UICONTROL パターン ] フィールドに設定した値のいずれにも入力が一致しない場合、次のいずれかが発生します。</p> 
    <ul> 
     <li>[!UICONTROL Else] フィールドの値が返されます</li> 
     <li>[!UICONTROL Else] フィールドに値がない場合、出力は返されません。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>「ケース」フィールドに設定された条件が満たされない場合に返される値を入力します。 </p> </td> 
  </tr> 
 </tbody> 
</table>
