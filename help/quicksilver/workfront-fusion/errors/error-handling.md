---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: でのエラー処理 [!DNL Adobe Workfront Fusion]
description: シナリオの実行中にエラーが発生した場合、通常は、エラーが発生したためにサービスが利用できなくなったり、サービスが予期しないデータで応答したり、入力データの検証が失敗したりするからです。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# でのエラー処理 [!DNL Adobe Workfront Fusion]

シナリオの実行中にエラーが発生した場合、通常は、エラーが発生したためにサービスが利用できなくなったり、サービスが予期しないデータで応答したり、入力データの検証が失敗したりするからです。

>[!NOTE]
>
>モジュールがシナリオの実行中にエラーをスローし、モジュールにエラー処理ルートが添付されていない場合は、デフォルトのエラー処理ロジックが実行されます。詳しくは、 [でのエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

エラーハンドラールートをモジュールに追加することで、デフォルトのエラー処理ロジックを独自のエラー処理ロジックに置き換えることができます。 [!DNL Adobe Workfront Fusion] は 5 つの異なるディレクティブを提供し、その任意のディレクティブをエラーハンドラールートの最後に挿入できます。 詳しくは、 [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## エラーハンドラールート

モジュールにエラーハンドラールートを追加するには（Module X と呼びます）、モジュールを右クリックし、 **[!UICONTROL エラーハンドラーを追加]**:

![](assets/error-handler-route.png)

モジュールには、ディレクティブのリストと、シナリオで使用されているアプリが表示されます。 Module X がルート内の最後のモジュールの場合は、ディレクティブの 1 つを選択する必要があります。 または、に移動して、1 つ以上のモジュールをルートに追加できます。 この場合、 [!UICONTROL 無視] デフォルトでは、ディレクティブはモジュール X に適用され、エラーが発生した場合は、そのルート上の後続のモジュールが処理されます。

![](assets/directives-350x426.png)

以下に示すように、 [!UICONTROL フォルダーの作成] モジュール、 [!UICONTROL 無視] ディレクティブが自動的に適用され、「Data Error Takes Place」フィルタが 1 つ以上のバンドルを返した場合、シナリオはエラーハンドラルート上の次のモジュールに移動します。

ただし、エラーがない場合、シナリオは [!UICONTROL フォルダーモジュール内のすべてのファイルのリスト] 通常のルートで

![](assets/if-there-is-no-error-350x234.png)

また、エラーハンドラルートを通常のルートと区別するために、前者は上記のように透明な円で構成されます。

## エラー処理ディレクティブ

次に、指令について簡単に説明します。 詳しくは、 [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

合計 5 つのディレクティブがあり、シナリオの実行を続行するかどうかに応じて、次のカテゴリにグループ化できます。

次のディレクティブを使用して、シナリオの実行が継続されるようにします。

* **[!UICONTROL 再開]** エラーを含むモジュールの代替出力を指定でき、シナリオの実行ステータスは成功とマークされます
* **[!UICONTROL 無視]** は単にエラーを無視し、シナリオの実行ステータスが成功とマークされます
* **[!UICONTROL 改行]** には不完全な実行のキューへの入力が格納され、シナリオの実行ステータスは警告としてマークされます。 詳しくは、 [での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

一方、シナリオの実行を停止する場合は、次のいずれかのディレクティブを使用する必要があります。

* **[!UICONTROL ロールバック]** シナリオの実行を直ちに停止し、そのステータスをエラーとしてマークします
* **[!UICONTROL コミット]** シナリオの実行を直ちに停止し、そのステータスを成功としてマークします

## その他のリソース

* [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [での高度なエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) ( 上記のDropboxシナリオの設定を含む )
