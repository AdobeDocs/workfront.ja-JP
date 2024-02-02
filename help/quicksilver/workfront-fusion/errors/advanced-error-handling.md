---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe]  Workfront Fusion での高度なエラー処理'
description: 高度なエラー処理技術には、フィルタリングやネストが含まれます。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '957'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] での高度なエラー処理

高度なエラー処理技術には、フィルタリングやネストが含まれます。

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## フィルタリング

エラーハンドラールートで実行できるフィルタリングには 2 種類あります。

* [エラーハンドラールートへのフィルターの追加](#adding-a-filter-to-the-error-handler-route)
* [エラーハンドラルートへのルーターとフィルターの追加](#adding-a-router-followed-by-filters-to-the-error-handler)

### エラーハンドラールートへのフィルターの追加

フィルターを使用して、エラーハンドラールートで処理されるエラーを制御できます。これにより、特定のタイプのエラーのみを処理できます。エラーがフィルターを通過しない場合は、指定されたモジュールに対してエラーハンドラールートが定義されていないものとして扱われます。

>[!INFO]
>
>**例：**
>
>![](assets/filter-error-handling-350x238.png)

### エラーハンドラールートへの[!UICONTROL ルーター]とフィルターの追加

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>この例では、エラーは[!UICONTROL フォルダーを作成]モジュール (A) で発生します。これには、通常のルートとエラーハンドラールートがあります。後者のルーターの後に、特定のタイプのエラー（データエラーが発生する）を定義するフィルターを持つルーターが続き、その他のすべてのエラーのデフォルトルートを持つルーターが続きます。最初のルートは[!UICONTROL 再開]ディレクティブで終了します。このディレクティブには、モジュール A（[!UICONTROL フォルダーを作成]）から再開するシナリオの代替値が含まれています。一方、2 番目のルートはシナリオの実行を直ちに停止する、[!UICONTROL ロールバック]ディレクティブで終了します。

様々なエラータイプと、[!DNL Workfront Fusion] がそれらを処理および評価する方法について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) のエラー処理を参照してください。

### シナリオの例

このシナリオの例を設定して、これらのフィルターがエラー処理でどのように機能するかを理解できます。

ファイルをアップロードするには、新しいフォルダーを作成する代わりにに既存の [!DNL Dropbox] を使用します。

[!DNL Dropbox] で[!UICONTROL フォルダーを作成]モジュールを使用し、同じ名前のフォルダーが既に存在する場合、モジュールは以下に示すようなデータエラーをスローします。

![](assets/dropbox-350x276.png)

完全なシナリオは次のとおりです。

![](assets/dropbox-scenario-350x190.png)

1. [!UICONTROL ツール]／[!UICONTROL 変数設定]モジュールにはフォルダー名が含まれます。
1. [!UICONTROL HTTP]／[!UICONTROL ファイルを取得]モジュールは、フォルダーにアップロードする必要があるファイルを取得します。
1. [!UICONTROL Dropbox]／[!UICONTROL フォルダーを作成]モジュールで、モジュール内にマッピングされたものと同じ名前のフォルダーが既に存在する場合、モジュールはエラーをスローします。
1. エラーハンドラルート（透明なバブル）には、エラーをフィルタリングするルーターが含まれます。
1. 最初のルートは、既に知っているように、データエラーと呼ばれる特定のタイプのエラーに対するものです。

   1. データエラーが発生し、エラーの詳細がフィルターを通過すると、[!UICONTROL Dropbox]／[!UICONTROL フォルダーモジュール内のすべてのファイル／サブフォルダーをリスト]に [!DNL Dropbox] のすべてのフォルダーが一覧表示されます。
   1. 後続のフィルターは、フォルダー名と一致します。
   1. [!UICONTROL 再開]ディレクティブでは、既存のフォルダーのフォルダー ID とフォルダーパスを指定し、シナリオの実行が [!UICONTROL Dropbox]／[!UICONTROL フォルダーを作成]モジュールから再開されます。ただし、今回は新しいフォルダーを作成しようとするのではなく、[!UICONTROL 再開]ディレクティブの値を使用して次のモジュールに移動し、既存のフォルダーにファイルをアップロードします。

1. 2 番目のルートは、他のすべてのエラーに対するもので、[!UICONTROL ロールバック]ディレクティブで終了し、シナリオが即時に停止されます。

5 番目のステートメントの詳細な説明を以下に示します。

後続のモジュール（下記の[!UICONTROL ファイルをアップロード]）で既存のフォルダーを使用するには、モジュールにエラーハンドラールートを追加し、後に続く[!UICONTROL 再開]ディレクティブモジュールにマッピングされるフォルダーパスを取得する必要があります。

![](assets/add-error-handler-route-350x113.png)

最初のルートのフィルターは、同じ名前のフォルダーが既に存在する場合に表示される、特定のエラー（データエラー）のみを処理するように設定されます。

![](assets/condition-350x327.png)

[!UICONTROL Dropbox]／[!UICONTROL フォルダー内のすべてのファイルのリスト]モジュールは、ターゲットフォルダー内のすべてのフォルダーを返すように設定されます。次のフィルターは、最初に作成しようとしたフィルターのみを渡します（フォルダー名は「33。  フォルダー名」項目に保存されます）。

![](assets/condition2-350x193.png)

最終的に、[!UICONTROL 再開]ディレクティブは、失敗したモジュールの出力としてフォルダーパスを指定します。フォルダー ID は[!UICONTROL ファイルをアップロード]モジュールでは不要なので、空白のままにしておく必要があります。

![](assets/flow-control-350x190.png)

## ネスト

モジュールの場所に関係なく、エラーハンドラールートを作成し、ルーターを除くすべてのモジュールに実装することができます。したがって、別のモジュール用に作成された既存のエラーハンドラールートの一部であるモジュールの、エラーハンドラールートを作成することができます。

ネストされたエラーハンドラールートの例を次に示します。

![](assets/nested-error-handling-route-350x174.png)

このシナリオでは、2 番目のエラーハンドラールートは、最初のエラーハンドラールートの下にネストされます。[!UICONTROL Dropbox]／[!UICONTROL フォルダーを作成モジュール]でエラーが発生した場合、実行はルート 1 に移動します。「[!UICONTROL データエラーが発生する]」フィルターを通過すると、次のモジュールが実行され、フォルダーモジュールの [!UICONTROL Dropbox]／[!UICONTROL フォルダー内のすべてのファイル／サブフォルダーを一覧表示]でエラーが発生しなかった場合は、続いて[!UICONTROL 再開]ディレクティブモジュールが実行されます。

ただし、この [!DNL Dropbox] モジュールでエラーが発生した場合、実行はエラーハンドラールート 2 に移動し、[!UICONTROL 無視]ディレクトで終了します。この場合、[!UICONTROL 再開ディレクティブ]モジュールは実行されません。

これは、フィルタリングとネストのエラーハンドラーを組み合わせたものです。

