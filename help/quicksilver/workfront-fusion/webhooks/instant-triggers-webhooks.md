---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: ' [!DNL Adobe Workfront Fusion] のインスタントトリガー（Web フック）'
description: 多くのサービスでは、サービスで特定の変更が発生した場合に即座に通知を受け取る Web フックが用意されています。これらの通知を処理するには、インスタントトリガーを使用することをお勧めします。この記事では、Adobe Workfront Fusion でのインスタントトリガーの使用と機能について説明します。
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 98%

---

# [!DNL Adobe Workfront Fusion] のインスタントトリガー（Web フック）

多くのサービスでは、サービスで特定の変更が発生した場合に即座に通知を受け取る Web フックが用意されています。これらの通知を処理するには、インスタントトリガーを使用することをお勧めします。これらは [!DNL Adobe Workfront Fusion] のタグによって簡単に認識できます。

![](assets/instant-350x256.png)

サービスが Web フックを提供しない場合は、ポーリングトリガーを使用してサービスを定期的にポーリングする必要があります。

Workfront Fusion の Web フックの紹介ビデオについては、以下を参照してください。

* [Web フックの概要](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [中間ウェブフック](https://video.tv.adobe.com/v/3427030/){target=_blank}

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## Web フックのキューを表示する

受信 Web フックからのメッセージはすべて、Web フックのキューに保存されます。

1. 左側のメニューで、「**[!UICONTROL Web フック]**」をクリックします。
1. キューを表示する Webhook を見つけます。
1. トラックのアイコンと受信した Web フックの数を含むボタンをクリックします。

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >「[!UICONTROL データ]は機密情報」オプションの設定に関係なく、受信 Web フックデータは常にキューに保存されます（[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md) のシナリオ設定パネルで説明されています）。シナリオでデータが処理されるとすぐに、そのデータはシステムから完全に削除されます。

## インスタントトリガーをスケジュールする

シナリオにインスタントトリガーが含まれる場合、シナリオが直ちに実行されるようにスケジュールできます。

![](assets/schedule-setting-350x185.png)

この場合、[!DNL Workfront Fusion] がサービスから新しいデータを受信すると、シナリオはすぐに実行されます。シナリオの実行後、キュー内で待機中の保留中の Web フックの総数がカウントされ、シナリオは保留中の Web フックの数と同じ数のサイクルを実行し、サイクルごとに 1 つの Web フックを処理します。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズを参照してください。

>[!NOTE]
>
>* サイクルは、シナリオ実行とは異なります。1 回のシナリオ実行で複数のサイクルを実行できます。
>* 即時実行がスケジュールされたインスタントトリガーでシナリオを実行する場合、次の例外が適用されます。
>
>     * 2 つの実行間の間隔は、料金プランに基づく最小間隔の影響を受けません。
>
>       例えば、シナリオの実行が完了すると、Web フックのキューが再度チェックされます。保留中の Web フックがある場合は、シナリオが直ちに再実行され、保留中の Web フックがすべて再度処理されます。
>   
>     * サイクルの最大数のシナリオ設定は無視され、100 に設定されます。つまり、1 回のシナリオの実行中に処理される保留中の Web フックが 100 個以下になります（1 サイクルあたり 1 イベントの割合で）。
>


[!UICONTROL 即時]以外のスケジュール設定を使用する場合、シナリオは指定した間隔で実行されます。間隔中に複数の Web フックがキューに集まる可能性があるため、1 回のシナリオ実行でより多くの Web フックを処理するには、[[!UICONTROL 最大サイクル数]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum)をデフォルトの 1 よりも大きい値に設定することをお勧めします。

1. シナリオ下部の[!UICONTROL シナリオ設定]アイコン ![](assets/gear-icon-settings.png) をクリックします。
1. 表示される「**[!UICONTROL シナリオ設定]**」ボックスで、「**[!UICONTROL 最大サイクル数]**」ボックスに数値を入力して、シナリオを実行するたびに実行するキューからの Web フックの数を示します。

## レート制限

現在のレート制限は、1 秒あたり 5 Web フックです。制限を超えた場合は、429 ステータスコードが返されます。

## 非アクティブな Web フックの有効期限

120 時間を超えてどのシナリオにも割り当てられていない Web フックは削除されます。

## Web フックペイロード

[!DNL Workfront Fusion] は、30 日間、Web フックペイロードを保存します。作成後 30 日を超える Web フックペイロードにアクセスすると、「[!UICONTROL ストレージからファイルを読み取れませんでした。]」というエラーが発生します。

## エラー処理

インスタントトリガーでシナリオにエラーが発生した場合は、次のようになります。

* 即時停止 - シナリオが[!UICONTROL 即時]に実行されるように設定されている場合。
* 3 回失敗すると停止（エラーが 3 回） - シナリオがスケジュールどおりに実行されるように設定されている場合。

シナリオの実行中にエラーが発生した場合、Web フックは、インスタントトリガーのロールバックフェーズ中にキューに戻されます。このような状況では、シナリオを修正して再実行することができます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズの記事の[ロールバック](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)を参照してください。

シナリオに Web フックの応答モジュールがある場合、エラーは Web フックの応答に送信されます。Webhook の応答モジュールは、常に最後に実行されます（シナリオ設定の「[!UICONTROL 自動コミット]」オプションが有効になっていない場合）。詳しくは、[Web フック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)の記事の [Web フックへの応答](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi)を参照してください。

## カスタム Web フック

独自の Web フックを作成できます。詳しくは、[Web フック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)を参照してください。

## Webhook の無効化

次のいずれかに該当する場合、Web フックは自動的に非アクティブ化されます。

* Web フックが 6 日以上どのシナリオにも接続されていない
* Web フックが、非アクティブなシナリオ（非アクティブになってから 30 日を超えたシナリオ）でのみ使用される。

非アクティブ化された web フックは、いかなるシナリオにも接続されておらず、非アクティブ状態となって 30 日が経過した場合、自動的に削除され、登録解除されます。


