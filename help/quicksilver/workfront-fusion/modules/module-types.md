---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: モジュールのタイプ
description: Adobe Workfront Fusion は、アクションモジュール、検索モジュール、トリガーモジュール、アグリゲーター、イテレーターの 5 種類のモジュールを区別します。アグリゲーターとイテレーターは詳細なシナリオ用です。
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '973'
ht-degree: 100%

---

# モジュールのタイプ

[!UICONTROL Adobe Workfront Fusion] は、アクションモジュール、検索モジュール、トリガーモジュール、アグリゲーター、イテレーターの 5 種類のモジュールを区別します。アグリゲーターとイテレーターは、詳細なシナリオ用です。

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
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明する機能を使用するには、Adobe Workfront Fusion と Adobe Workfront を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## アクションモジュール

アクションモジュールは、最も一般的なタイプのモジュールです。一般的なアクションモジュールは、1 つのバンドルを返し、次のモジュールに渡して処理を行います。

トリガーモジュールとは異なり、アクションモジュールは、シナリオの最初、中間または最後に配置できます。シナリオのアクションモジュールの数には制限はありません。

>[!INFO]
>
>**例：**
>
>* **[!DNL Workfront]／[!UICONTROL ファイルをアップロード]**&#x200B;で、[!DNL Workfront] にファイルを送信し、識別子を返します。
>* **[!UICONTROL 画像]／[!UICONTROL サイズ変更]**&#x200B;で、画像を受け取り、指定した寸法にサイズ変更し、サイズ変更した画像を次のアクションに渡します。

アクションタイプには、作成、読み取り、更新、削除の 4 つのサブタイプがあります。更新サブタイプでは、次の 3 つの操作が有効になります。

* **フィールドの内容を消去する**。この操作は、フィールドの内容がキーワードを消去するために評価されるときに行われます（*空白*&#x200B;と混同しないでください）。

  ![](assets/erase-content-of-field.png)

* **フィールドの内容を変更しない**。この操作は、フィールドが空白のままになっているか、フィールドの内容が空白と評価される（JSON の null で表される）場合に実行されます。

  ![](assets/leave-content-field-unchanged-350x231.png)

* **フィールドの内容を置き換える**。この操作は、上記の 2 つ以外のすべての場合に実行されます。

>[!NOTE]
>
>* `erase` キーワードがマッピングパネルに表示されない場合、モジュールが更新モジュールでないか、アプリの最新の仕様に更新されていません。
>* 「[!UICONTROL 空白]」はフィールドの内容を変更しません。フィールドを消去する必要がある場合は、次の数式を使用できます。
>
>![](assets/formula-ifempty-name-erase.png)
>
>フィールドの内容が空白として評価される場合にフィールドを変更しないままにすることは、現時点では不可能です。

## モジュールの検索

一般的な検索では、0 個、1 個、または複数のバンドルを返し、次のモジュールに渡して処理を行います。

シナリオの最初、中間または最後に検索を配置できます。

シナリオの検索の数には制限はありません。

>[!INFO]
>
>**例：**
>
>**[!DNL Workfront]／[!UICONTROL 関連レコードの読み取り]**&#x200B;では、特定の親オブジェクト内で、指定した検索クエリに一致するレコードを読み取ります。

## トリガーモジュール

トリガーは、特定のサービスに変更があった場合にバンドルを生成します。変更には、新しいレコードの作成、レコードの削除、レコードの更新などが含まれます。

各トリガーは、0 個、1 個または複数のバンドルを返し、次のモジュールに渡して処理を行います。

トリガーは、シナリオの先頭にのみ配置できます。

各シナリオにはトリガーを 1 つだけ含めることができます。

[!DNL Workfront Fusion] は、ポーリングトリガーとインスタントトリガーの 2 種類のトリガーを区別します。

### ポーリングトリガー

ポーリングトリガーは、前回の実行以降に変更がなかった場合でも、特定のサービスを定期的にポーリングします。ポーリングトリガーを含むシナリオを、一定の間隔で実行するようにスケジュールすることをお勧めします。*変更*&#x200B;がある場合、トリガーは変更に関する情報を含むバンドルを返します。*変更*&#x200B;がない場合、トリガーはバンドルを出力しません。シナリオのスケジュールの説明については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)でのシナリオのスケジュール設定を参照してください。

ポーリングトリガーでは、エポックパネルを介して出力する最初のバンドルを選択できます。パネルは、トリガーを保存した後、または設定を変更した後、自動的にトリガーされます。詳しくは、[[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md) でのトリガーモジュールの開始場所の選択を参照してください。

>[!NOTE]
>
>エポックパネルで行われた設定は、モジュールの最初の実行にのみ影響します。モジュールが実行されると、最後に出力されたバンドルが記憶され、エポックパネルを介して行われた設定が無効になります。

>[!INFO]
>
>**例：**
>
>* **[!DNL Workfront]／[!UICONTROL レコードを監視]**&#x200B;は、前回のシナリオ実行以降に新しく追加されたファイルを返します
>
>* **[!DNL Google Sheets]／[!UICONTROL 行を監視]**&#x200B;は、前回のシナリオ実行以降にユーザーが追加した新しい行を返します

### インスタントトリガー

インスタントトリガーを使用すると、サービスは&#x200B;*変更*&#x200B;について [!DNL Workfront Fusion] に即座に通知できます。即座に実行するインスタントトリガーを含むシナリオをスケジュールすることをお勧めします。手順については、[Adobe Workfront Fusion でのシナリオのスケジュール](../../workfront-fusion/scenarios/schedule-a-scenario.md)を参照してください。受信データの処理方法の詳細については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) のインスタントトリガー（Web フック）も参照してください。

>[!INFO]
>
>**例：**
>
>* **[!DNL Workfront]／[!UICONTROL イベントを監視]**&#x200B;は、タスクの作成など、Workfront で特定の種類のイベントが発生したときに情報を返します。
>* **[!DNL Google Sheets]／[!UICONTROL 変更を監視]**&#x200B;は、セルが更新されるたびに情報を返します。

## アグリゲーター

アグリゲーターとは、複数のバンドルを 1 つのバンドルに蓄積するモジュールの一種です。

各アグリゲーターは 1 つのバンドルのみを返し、次のモジュールに渡してさらに処理を行います。

アグリゲーターは、シナリオの途中にのみ配置できます。

シナリオに含めることができるアグリゲーターの数に制限はありません。

>[!INFO]
>
>**例：**
>
>* **[!UICONTROL アーカイブ]／[!UICONTROL アーカイブを作成]**&#x200B;は、受信したファイルを zip アーカイブに圧縮します
>* **[!UICONTROL CSV]／[!UICONTROL CSV に集計]**&#x200B;は、CSV ファイルから複数の文字列を 1 行に結合します。
>* **[!UICONTROL ツール]／[!UICONTROL テキストアグリゲーター]**&#x200B;は、複数の文字列を 1 つの文字列に組み合わせます。

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md) のアグリゲーターモジュールを参照してください。

## イテレータ

イテレーターは、配列を複数の個別のバンドルに分割するモジュールの一種です。

各イテレーターは 1 つ以上のバンドルを返し、次のモジュールに渡して処理します。

イテレーターは、シナリオの途中にのみ配置できます。

シナリオに含めることができるイテレーターの数に制限はありません。

>[!INFO]
>
>**例：**
>
>**[!UICONTROL メール]／[!UICONTROL 添付ファイルを取得]**&#x200B;は、添付ファイルの配列を別々のバンドルに分割します

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) のイテレーターモジュールおよび[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md) での配列マッピングを参照してください。
