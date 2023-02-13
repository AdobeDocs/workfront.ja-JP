---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: での高度なエラー処理 [!DNL Adobe] Workfront Fusion
description: 高度なエラー処理技術には、フィルタリングやネストが含まれます。
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# での高度なエラー処理 [!DNL Adobe Workfront Fusion]

高度なエラー処理技術には、フィルタリングやネストが含まれます。

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## フィルタリング

エラーハンドラールートで実行できるフィルタリングには 2 種類があります。

* [エラーハンドラールートへのフィルターの追加](#adding-a-filter-to-the-error-handler-route)
* [ルータの追加とフィルタの追加をエラーハンドラルートに行う](#adding-a-router-followed-by-filters-to-the-error-handler)

### エラーハンドラールートへのフィルターの追加

フィルタを使用して、エラーハンドラルートで処理されるエラーを制御できます。 これにより、特定のタイプのエラーのみを処理できます。 エラーがフィルタを通過しない場合は、指定されたモジュールに対してエラーハンドラルートが定義されていないかのように扱われます。

>[!INFO]
>
>**例:**
>
>![](assets/filter-error-handling-350x238.png)

### の追加 [!UICONTROL 発送担当] その後に、エラーハンドラーに対するフィルターが続きます。

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>この例では、エラーは [!UICONTROL フォルダーの作成] モジュール (A) は、通常のルートとエラーハンドラルートを持ちます。 後者のルータの後に、特定のタイプのエラー (Data Error Takes Place) を定義するフィルタを持つルータが続き、その他のすべてのエラーのデフォルトルートを持つルータが続きます。 最初のルートは [!UICONTROL 再開] モジュール A から再開するシナリオの代替値を含むディレクティブ ([!UICONTROL フォルダーの作成]) で始まり、2 番目のルートが [!UICONTROL ロールバック] ディレクティブ：シナリオの実行を直ちに停止します。

詳しくは、 [でのエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) 様々なエラータイプの詳細および方法については、 [!DNL Workfront Fusion] を処理し、評価します。

### シナリオの例

この例を設定して、これらのフィルターがエラー処理でどのように機能するかを理解できます。

既存の [!DNL Dropbox] 新しいファイルを作成する代わりにファイルをアップロードするフォルダー

次の [!UICONTROL フォルダーの作成] モジュールオン [!DNL Dropbox] と同じ名前のフォルダーが既に存在します。モジュールは、次に示すようにデータエラーをスローします。

![](assets/dropbox-350x276.png)

完全なシナリオ：

![](assets/dropbox-scenario-350x190.png)

1. この [!UICONTROL ツール] > [!UICONTROL 変数を設定] モジュールにはフォルダー名が含まれます
1. この [!UICONTROL HTTP] >[!UICONTROL ファイルの取得] モジュールは、フォルダーにアップロードする必要があるファイルを取得します
1. この [!UICONTROL Dropbox] >[!UICONTROL フォルダーの作成] モジュールで、モジュール内にマッピングされたものと同じ名前のフォルダが既に存在する場合、モジュールはエラーをスローします
1. エラーハンドラルート（透明バブル）には、エラーをフィルタリングするルータが含まれます
1. 最初のルートは、既に知っているように、Data Error と呼ばれる特定のタイプのエラーに対するものです。

   1. データエラーが発生し、エラーの詳細がフィルターを通過すると、 [!UICONTROL Dropbox] >[!UICONTROL フォルダーモジュール内のすべてのファイル/サブフォルダーのリスト] にすべてのフォルダを一覧表示 [!DNL Dropbox]
   1. 後続のフィルターは、フォルダー名と一致します
   1. この [!UICONTROL 再開] ディレクティブは、既存のフォルダーのフォルダー ID とフォルダーパスを指定し、シナリオの実行は [!UICONTROL Dropbox] >[!UICONTROL フォルダーの作成] モジュールですが、新しいフォルダーを作成しようとする代わりに、今回は [!UICONTROL 再開] 次のモジュールに移動し、既存のフォルダーにファイルをアップロードするための命令

1. 2 番目のルートは、他のすべてのエラーに対するもので、 [!UICONTROL ロールバック] この命令は、シナリオを直ちに停止させます。

5 番目の文の詳細な説明を以下に示します。

後続のモジュール ([!UICONTROL ファイルのアップロード] 以下 )、エラーハンドラールートをモジュールに追加し、にマッピングするフォルダーパスを取得する必要があります。 [!UICONTROL 再開] 次に続くディレクティブモジュール：

![](assets/add-error-handler-route-350x113.png)

最初のルートのフィルターは、同じ名前のフォルダーが既に存在する場合に表示される特定のエラー (Data Error) のみを処理するように設定されます。

![](assets/condition-350x327.png)

この [!UICONTROL Dropbox] >[!UICONTROL フォルダー内のすべてのファイルのリスト] モジュールは、ターゲットフォルダー内のすべてのフォルダーを返すように設定されます。 次のフィルターは、最初に作成しようとしたフィルターのみを渡します（フォルダー名は 33 に保存されます）。 フォルダー名項目 ):

![](assets/condition2-350x193.png)

最終的に、 [!UICONTROL 再開] ディレクティブは、失敗したモジュールの出力として Folder path を指定します。 フォルダー ID は「 」では不要なので、空白のままにしておく必要があります[!UICONTROL ファイルのアップロード]&#39;モジュール：

![](assets/flow-control-350x190.png)

## ネスト

モジュールの場所に関係なく、エラーハンドラールートを作成し、ルーターを除くすべてのモジュールに実装できます。 したがって、別のモジュール用に作成された既存のエラーハンドラールートに既に含まれるモジュールに対して、エラーハンドラールートを作成することができます。

ネストされたエラーハンドラールートの例を次に示します。

![](assets/nested-error-handling-route-350x174.png)

このシナリオでは、2 番目のエラーハンドラールートは、最初のエラーハンドラールートの下にネストされます。 この場合、 [!UICONTROL Dropbox] >[!UICONTROL フォルダーモジュールの作成] エラーが発生した場合、実行はルート 1 に移動します ( [!UICONTROL データエラーが発生しました] フィルターが渡されると、次のモジュールが実行され、その後に [!UICONTROL 再開] エラーが [!UICONTROL Dropbox] >[!UICONTROL すべてのファイル/サブフォルダーのリスト] （フォルダーモジュール内）

ただし、 [!DNL Dropbox] モジュールの後、実行は Error Handler Route 2 に移動し、 [!UICONTROL 無視] ディレクティブ。 この [!UICONTROL Resume ディレクティブ] この場合、モジュールは実行されません。

これは、フィルタリングとネストのエラーハンドラーを組み合わせたものです。

