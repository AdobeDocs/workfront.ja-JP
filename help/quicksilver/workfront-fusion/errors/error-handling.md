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
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# でのエラー処理 [!DNL Adobe Workfront Fusion]

シナリオの実行中にエラーが発生した場合、通常は、エラーが発生したためにサービスが利用できなくなったり、サービスが予期しないデータで応答したり、入力データの検証が失敗したりするからです。

モジュールがシナリオの実行中にエラーをスローし、モジュールにエラー処理ルートが添付されていない場合は、デフォルトのエラー処理ロジックが実行されます。詳しくは、 [でのエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

エラーハンドラールートをモジュールに追加することで、デフォルトのエラー処理ロジックを独自のエラー処理ロジックに置き換えることができます。 [!DNL Adobe Workfront Fusion] は、エラーハンドラールートの最後に挿入できる 5 つの異なるディレクティブを提供します。

詳しくは、 [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## エラーハンドラールート

モジュールにエラーハンドラールートを追加するには：

1. モジュールを右クリックし、「 」を選択します。 **[!UICONTROL エラーハンドラーを追加]**:

   ![](assets/error-handler-route.png)

   モジュールには、ディレクティブのリストと、シナリオで使用されているアプリが表示されます。

1. エラーハンドラーを追加したモジュールがルートの最後のモジュールの場合は、ディレクティブの 1 つを選択します。

   または

   1 つ以上のモジュールをエラーハンドラールートに追加します。

   ルートにモジュールを追加する場合、 [!UICONTROL 無視] デフォルトではディレクティブが適用され、エラーが発生した場合は、そのルートの後続のモジュールが処理されます。


>[!INFO]
>
>この例では、 [!UICONTROL フォルダーの作成] モジュール、 [!UICONTROL 無視] ディレクティブが自動的に適用され、シナリオはエラーハンドラルート上の次のモジュールに移動します。
>
>ただし、エラーがない場合、シナリオは [!UICONTROL フォルダーモジュール内のすべてのファイルのリスト] 通常のルートで
>
>![](assets/if-there-is-no-error-350x234.png)

エラーハンドラルートは透明な円で構成され、通常のルートは実線の円で構成されます。

## エラー処理ディレクティブ

次に、指令について簡単に説明します。 詳しくは、 [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

合計 5 つのディレクティブがあり、シナリオの実行を続行するかどうかに応じて、次のカテゴリにグループ化できます。

次のディレクティブを使用して、シナリオの実行が継続されるようにします。

* **[!UICONTROL 再開]**:エラーを含むモジュールの代替出力を指定できます。 シナリオの実行ステータスが成功とマークされます
* **[!UICONTROL 無視]**:はエラーを無視します。 シナリオの実行ステータスが成功とマークされます
* **[!UICONTROL 改行]**:不完全な実行のキューへの入力を格納します。 シナリオの実行ステータスは警告としてマークされます。 詳しくは、 [での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

エラーが発生したときにシナリオの実行が停止する場合は、次のいずれかのディレクティブを使用します。

* **[!UICONTROL ロールバック]**:シナリオの実行を直ちに停止し、そのステータスをエラーとしてマークします
* **[!UICONTROL コミット]**:シナリオの実行を直ちに停止し、ステータスを成功としてマークします

エラー処理の詳細については、以下を参照してください。

* [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [での高度なエラー処理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)