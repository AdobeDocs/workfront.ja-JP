---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: ツール
description: ' [!DNL Adobe Workfront Fusion Tools]  セクションには、シナリオを強化できる便利なモジュールがいくつか含まれています。'
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '2290'
ht-degree: 100%

---

# [!UICONTROL ツール]

[!DNL Adobe Workfront Fusion Tools] セクションには、シナリオを強化できる便利なモジュールがいくつか含まれています。

[!UICONTROL ツール]モジュールは、アプリのリストまたは画面の下部の[!UICONTROL ツール]アイコン![](assets/tools-icon-small.png)から使用できます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL ツール]とそのフィールド

* [トリガー](#triggers)
* [アクション](#actions)
* [アグリゲーター](#aggregators)
* [変換サービス](#transformers)

### トリガー

#### [!UICONTROL 基本トリガー]

このモジュールでは、カスタムトリガーを作成し、その入力バンドルを定義できます。

例えば、連絡先や、指定したメールアドレス（[!UICONTROL メール]／[!UICONTROL メールの送信]または [!DNL Gmail]／[!UICONTROL メールを送信]モジュール）、または必要に応じてトリガーされる簡単なリマインダーとして使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>配列項目を追加して、カスタムバンドルを作成します。この配列は、名前と値のペアで構成されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 複数の変数を取得]](#get-multiple-variables)
* [[!UICONTROL 変数を取得]](#get-variable)
* [[!UICONTROL 増分関数]](#increment-function)
* [[!UICONTROL 複数の変数を設定]](#set-multiple-variables)
* [[!UICONTROL 変数を設定]](#set-variable)
* [[!UICONTROL スリープ]](#sleep)

#### [!UICONTROL 複数の変数を取得]

このモジュールは、[!UICONTROL 変数を設定]または[!UICONTROL 複数の変数を設定]モジュールによって以前に作成された値を取得します。

このモジュールは、[!UICONTROL 複数の変数を取得]モジュールが配置されている場所とは異なるルートに変数が設定されている場合でも、シナリオ内の任意の場所に設定された変数を読み取ることができます。唯一の要件は、[!UICONTROL ツール]／[!UICONTROL 変数の設定]または[!UICONTROL ツール]／[!UICONTROL 複数の変数の設定]モジュールが、[!UICONTROL ツール]／[!UICONTROL 複数変数の取得]モジュールの前に実行されることです。モジュールの実行順序について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md)のルーターモジュールを参照してください。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>モジュールから取得する変数を追加します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variable name]</td>
        <td>追加する変数ごとに、取得する変数の名前をマッピングします。</td>
    </tr>
</table>

>[!INFO]
>
>**例：**&#x200B;以下は、（複数の）変数を[!UICONTROL 設定]／[!UICONTROL 取得]モジュールの可能な使用例です。
>
>* 異なる経路でも、計算値を後で使用するために保存する場合。これは、値が複数のモジュールで使用され、値を計算する数式が過度に複雑な場合に役立ちます。
>* 式をデバッグする場合。モジュールで使用されている数式が正しい結果を提供していないように見える場合は、数式をコピーし、関連するモジュールの前に挿入する[!UICONTROL 変数を設定]モジュールに貼り付けます。[!UICONTROL 変数を設定]モジュールの後でモジュールを切断し、シナリオを実行します。[!UICONTROL 変数の設定]モジュールの出力を確認し、数式を調整または簡素化し、シナリオを再実行して、問題が解決するまで引き続き実行します。


#### [!UICONTROL 変数の取得]

このモジュールは、[!UICONTROL 変数の設定]または[!UICONTROL 複数の変数の設定]モジュールによって以前に作成された値を取得します。

このモジュールは、[!UICONTROL 変数の取得]モジュールが配置されている場所とは異なるルートに変数が設定されている場合でも、シナリオ内の任意の場所に設定された変数を読み取ることができます。唯一の要件は、[!UICONTROL ツール]／[!UICONTROL 変数の設定]または[!UICONTROL ツール]／[!UICONTROL 複数の変数の設定]モジュールが、[!UICONTROL ツール]／[!UICONTROL 変数の取得]モジュールの前に実行されることです。モジュールの実行順序の詳細情報については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md)のルーターモジュールを参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable name]</td> 
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
   <td role="rowheader">[!UICONTROL Reset a value]</td> 
   <td> <p>モジュールで値を増分する場合に選択します。 </p> 
    <ul> 
     <li>[!UICONTROL After one cycle]</li> 
     <li>[!UICONTROL After one scenario run]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**
>
>モジュールを使用する目的の 1 つは、タスク、リード、メールなどの「総当たり的な」割り当てをグループ内のユーザーに実装することです。アルゴリズムは、ある合理的な順序でグループから割り当て先を選択します。通常は、リストの上から下に移動します。アルゴリズムがリストの最後に到達すると、次の割り当てをリストの一番上のユーザーに行い、リストの下方に向かって割り当てを続けて行います。
>
>次のシナリオでは、奇数番号のシナリオを実行するたびに最初の受信者にメールを送信し、偶数番号のシナリオを実行するたびに 2 番目の受信者にメールを送信します。
>
>![](assets/example-email-350x246.gif)
>
>1. このシナリオを作成するには：
>1. モジュールの「**[!UICONTROL 値をリセット]**」フィールドを「なし」に設定します。
>1. 奇数値のルートを設定します。`1` の値に等しいモジュロ演算関数を使用して、このルートのフィルターを設定します。
>
>   ![](assets/odd-350x459.png)
>
>  **メモ**：「[!UICONTROL 次と等しい]」演算子を、デフォルトの「[!UICONTROL テキスト]」演算子から「[!UICONTROL 数値]」演算子に必ず変更します。
>
>1. `0` の値に等しいモジュロ演算関数を使用して、このルートのフィルターを設定します。
>
>増分関数は、シナリオが実行されるたびに 1 つ追加します。フィルターで増分を確認し、その値に基づいて処理されるので、メールは均等に配信されます。

#### [!UICONTROL 複数の変数を設定]

このモジュールでは、ルート内の他のモジュールでマッピングできる変数を作成します。変数は、シナリオ内の任意のルートについて、[!UICONTROL 変数を取得]または[!UICONTROL 複数の変数を取得]モジュールにマッピングすることもできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>モジュールで設定する変数を追加します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>各変数に、変数名を入力します。この名前は、他のモジュールで変数をマッピングする際に表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>各変数に、変数の値を入力します。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>変数の有効期間を選択します（同じ値を維持）。</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>：変数は 1 サイクルの間有効です。1 回のシナリオ実行で複数の web フックを受け取る場合に役立ちます（より多くの web フック = より多くのサイクル）。 </li> 
     <li><strong>[!UICONTROL One execution]</strong>：変数は、1 回のシナリオ実行において有効です。1 つの実行に 1 つ以上のサイクルを含めることができます。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 変数を設定]

このモジュールでは、ルート内の他のモジュールによってマッピングできる変数を作成します。変数は、シナリオ内の任意のルートについても、[!UICONTROL 変数を取得]モジュールまたは[!UICONTROL 複数の変数を取得]モジュールにマッピングすることができます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>変数名を入力します。この名前は、他のモジュールで変数をマッピングする際に表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>変数の有効期間を選択します（同じ値を維持）。</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>：変数は 1 サイクルの間有効です。1 回のシナリオ実行で複数の web フックを受け取る場合に役立ちます（より多くの web フック = より多くのサイクル）。 </li> 
     <li><strong>[!UICONTROL One execution]</strong>：変数は、1 回のシナリオ実行において有効です。1 つの実行に 1 つ以上のサイクルを含めることができます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>変数の値を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL スリープ]

このモジュールにより、シナリオのフローを最大 300 秒（5 分）まで遅延することができます。

この機能は、例えば、[!DNL target] サービスサーバーの読み込みの負荷を下げたり、SMS やメールの一括送信時に人間の動作を模倣したりする場合に有効です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>シナリオを一時停止する秒数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>フローの一時停止の時間を長くする場合は、シナリオを次の 2 つのシナリオに分割することをお勧めします。
>
>* 最初のシナリオに、一時停止の前半部分を含める。
>* 2 つ目のシナリオに、後半部分を含める。
>
>最初のシナリオでは、必要な情報がすべて、現在のタイムスタンプと共にデータストアに保存されます。2 つ目のシナリオでは、意図した遅延よりも古いタイムスタンプを持つレコードをデータストアで定期的に確認し、そのレコードを取得し、データの処理を完了したら、データストアからそのレコードを削除します。
>
>データストアについて詳しくは、「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md) のデータストア」を参照してください。
>
>特定のデータストアモジュールについて詳しくは、[[!UICONTROL データストア]モジュール](../../workfront-fusion/apps-and-their-modules/data-store-modules.md)を参照してください。

### アグリゲーター

* [[!UICONTROL 数値アグリゲーター]](#numeric-aggregator)
* [[!UICONTROL テーブルアグリゲーター]](#table-aggregator)
* [[!UICONTROL テキストアグリゲーター]](#text-aggregator)

#### [!UICONTROL 数値アグリゲーター]

このモジュールでは、数値を取得し、選択した関数（SUM、AVG、COUNT、MAX、MIN）の 1 つを適用して、結果を 1 つのバンドルで返すことができます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>フィールドの集計元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>値の集計に使用する関数を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>集約出力をグループ化する式を定義します。この式には、1 つ以上のマッピングされた項目を含めることができます。集計されたデータは、この式の値を使用してグループに分割されます。各グループは、キー（評価された式）と値（集計値）を持つ個別のバンドルとして出力されます。キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>集計する値を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルアグリゲーター]

このモジュールは、受け取ったバンドルの選択されたフィールドの値を、指定された列と行の区切り記号（テーブルの作成に使用）を使用して 1 つのバンドルに結合します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>フィールドの集計元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td> <p> 上で選択したモジュールから、1 つのバンドルに集計する値を含むフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Column separator]</p> </td> 
   <td> <p>結果のバンドルでフィールド値の列を区切る区切り文字の種類を選択または入力します。[!UICONTROL Other] を選択した場合は、値の区切りに使用する文字を区切り文字フィールドに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>結果のバンドルでフィールド値の行を区切る区切り文字の種類を選択または入力します。[!UICONTROL Other] を選択した場合は、値の区切りに使用する文字を区切り文字フィールドに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>集約出力をグループ化する式を定義します。この式には、1 つ以上のマッピングされた項目を含めることができます。集約されたデータは、この式の値を使用してグループに分割されます。各グループは、キー（評価された式）と値（集計値）を持つ個別のバンドルとして出力されます。キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テキストアグリゲーター]

このモジュールは、受け取ったバンドルの選択されたフィールドの値を 1 つのバンドルに結合します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>フィールドの集計元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>結果のバンドルでフィールド値の行を区切る区切り文字の種類を選択または入力します。[!UICONTROL Other] を選択した場合は、値の区切りに使用する文字を区切り文字フィールドに入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>マッピングされた項目を 1 つ以上含む式を定義します。集計データは、同じ式の値を持つグループの下で分割されます。各グループは、評価された式と集計テキストを付属したキーを含む個別のバンドルとして出力されます。これにより、キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> モジュールを集計するテキストを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**&#x200B;テキスト集約を使用すると、1 つのバンドルにさらに多くの値（顧客名やメモなど）を挿入し、メールの本文または件名にあるすべての値を含むメールを送信できます。

### 変換サービス

* [[!UICONTROL 文字列を構成]](#compose-a-string)
* [[!UICONTROL テキストのエンコーディングを変換]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 切り替え]](#switch)

#### [!UICONTROL 文字列を構成]

任意の値を文字列データタイプ（テキスト）に変換します。これにより、バイナリデータなどのマッピングが容易になります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
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
   <td> <p>[!UICONTROL Input data]</p> </td> 
   <td> <p>変換するコンテンツを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>入力データのエンコーディングタイプを選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>ターゲット（出力）データのエンコーディングタイプを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 切り替え]

入力値が提供された値のリストと一致するかどうかを確認します。結果に基づいて出力を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>評価する式を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use regular expressions to match]</td> 
   <td> <p>正規表現を使用するには、このオプションを有効にします。モジュールは、完全一致ではなく、正規表現に基づいて大文字と小文字を判断します。</p> 
    <div> 
     <p>正規表現とは、各文字が特別な意味を持つメタ文字、またはリテラルの意味を持つ正規文字のいずれかである文字のシーケンスです。これらの文字とメタ文字は、テキストの検索に使用できるパターンを識別します。例えば、名前を検索する場合、大文字で始まる 2 つの連続した単語で構成されるパターンを検索する正規表現を設定できます。正規表現は、テキストを検索および操作するための強力なツールです。</p> 
     <p>正規表現についての詳しい説明は、この記事の範囲外です。次のリソースをお勧めします。</p> 
     <ul> 
      <li>メタ文字の完全なリストについては、MDN web ドキュメントの<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">正規表現</a>を参照してください。</li> 
      <li>正規表現の作成方法に関するチュートリアルには、<a href="https://regexone.com/">RegexOne</a> をお勧めします。</li> 
      <li>正規表現の試行には、<a href="https://regex101.com/">正規表現の基本</a>の web サイトをお勧めします。左パネルで ECMAScript（JavaScript）FLAVOR を選択します。</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cases] </td> 
   <td> <p>入力に、[!UICONTROL Pattern] フィールドに入力された値が含まれている場合、[!UICONTROL Output] フィールドに入力された値が返されます。</p> <p>入力が、[!UICONTROL Pattern] フィールドに設定した値のいずれにも一致しない場合、次のいずれかが発生します。</p> 
    <ul> 
     <li>[!UICONTROL Else] フィールドの値が返されます。</li> 
     <li>[!UICONTROL Else] フィールドに値がない場合、出力は返されません。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Cases フィールドに設定された条件が満たされない場合に、返される値を入力します。 </p> </td> 
  </tr> 
 </tbody> 
</table>
