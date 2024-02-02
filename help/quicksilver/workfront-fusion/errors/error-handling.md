---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion] でのエラー処理'
description: シナリオの実行中にエラーが発生する場合、通常、その原因は、サービスが障害により利用できないか、サービスが予期しないデータで応答するか、入力データの検証が失敗するすることなどです。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '616'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのエラー処理

シナリオの実行中にエラーが発生する場合、通常、その原因は、サービスが障害により利用できないか、サービスが予期しないデータで応答するか、入力データの検証が失敗するすることなどです。

モジュールがシナリオの実行中にエラーをスローし、モジュールにエラー処理ルートがアタッチされていない場合は、デフォルトのエラー処理ロジックが実行されます。詳しくは、「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) でのエラー処理」を参照してください。

エラーハンドラールートをモジュールに追加することで、デフォルトのエラー処理ロジックを独自のエラー処理ロジックに置き換えることができます。[!DNL Adobe Workfront Fusion] では、エラーハンドラールートの最後に挿入できる 5 つの異なるディレクティブを提供しています。

詳しくは、「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md) でのエラー処理のディレクティブ」を参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプやアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md) を参照してください。

## エラーハンドラールート

モジュールにエラーハンドラールートを追加するには、次の手順に従います。

1. モジュールを右クリックし、「**[!UICONTROL エラーハンドラーを追加]**」を選択します。

   ![](assets/error-handler-route.png)

   モジュールには、ディレクティブのリストと、シナリオで使用されているアプリが表示されます。

1. エラーハンドラーを追加したモジュールがルートの最後のモジュールの場合は、ディレクティブの 1 つを選択します。

   または

   1 つ以上のモジュールをエラーハンドラールートに追加します。

   ルートにモジュールをさらに追加した場合、デフォルトでは[!UICONTROL 無視]のディレクティブが適用され、エラーの発生時は、そのルートの後続のモジュールが処理されます。


>[!INFO]
>
>この例では、[!UICONTROL フォルダーを作成]モジュールの実行中にエラーが発生すると、[!UICONTROL 無視]ディレクティブが自動的に適用され、シナリオはエラーハンドラルート上の次のモジュールに移動します。
>
>ただし、エラーが発生していない場合、シナリオは通常のルート上の「[!UICONTROL フォルダーモジュール内のすべてのファイルの一覧表示]」に移動します。
>
>![](assets/if-there-is-no-error-350x234.png)

エラーハンドラルートは透明な円で示され、通常のルートは不透明の円で示されます。

## エラー処理ディレクティブ

ディレクティブについて、以下で簡単に説明します。詳しくは、「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md) でのエラー処理のディレクティブ」を参照してください。

合計 5 つのディレクティブがあり、シナリオの実行を続行するかどうかに応じて、次のカテゴリにグループ化できます。

次のディレクティブを使用して、シナリオの実行が継続されるようにします。

* **[!UICONTROL 再開]**：エラーを含むモジュールの代替出力を指定できます。シナリオの実行ステータスは、成功と表示されます。
* **[!UICONTROL 無視]**：エラーを無視します。シナリオの実行ステータスは、成功と表示されます。
* **[!UICONTROL 一時停止]**：入力を不完全な実行のキューに保存します。シナリオの実行ステータスは、警告と表示されます。詳しくは、「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) での不完全な実行の表示と解決」を参照してください。

エラーが発生したときにシナリオの実行が停止する場合は、次のいずれかのディレクティブを使用します。

* **[!UICONTROL ロールバック]**：シナリオの実行を直ちに停止し、そのステータスをエラーと表示します。
* **[!UICONTROL コミット]**：シナリオの実行を直ちに停止し、そのステータスを成功と表示します

エラー処理について詳しくは、以下を参照してください。

* [ [!DNL Adobe Workfront Fusion] でのエラー処理のディレクティブ](../../workfront-fusion/errors/directives-for-error-handling.md)
* [ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) での高度なエラー処理