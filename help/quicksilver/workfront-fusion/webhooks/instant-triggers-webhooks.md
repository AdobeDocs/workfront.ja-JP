---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: のインスタントトリガー（Web フック） [!DNL Adobe Workfront Fusion]
description: 多くのサービスでは、サービスで特定の変更が発生した場合に即座に通知を受け取る Web フックが用意されています。 これらの通知を処理するには、インスタントトリガーを使用することをお勧めします。 この記事では、Adobe Workfront Fusion でのインスタントトリガーの使用と機能について説明します。
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 04191419ab6079cc34576b5a7532cd1596e4b91d
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# のインスタントトリガー（Web フック） [!DNL Adobe Workfront Fusion]

多くのサービスでは、サービスで特定の変更が発生した場合に即座に通知を受け取る Web フックが用意されています。 これらの通知を処理するには、インスタントトリガーを使用することをお勧めします。 これらは、 [!DNL Adobe Workfront Fusion] タグの理由：

![](assets/instant-350x256.png)

Web フックが提供されない場合は、ポーリングトリガーを使用して定期的にサービスをポーリングする必要があります。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## ウェブフックのキューを表示する

受信 Webhook からのメッセージはすべて、Webhook のキューに保存されます。

1. クリック **[!UICONTROL ウェブフック]** をクリックします。
1. キューを表示する Webhook を見つけます。
1. トラックのアイコンと受信したウェブフックの数を含むボタンをクリックします。

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >受信する Webhook データは、オプションの設定方法に関係なく、常にキューに格納されます。 [!UICONTROL データ] は機密情報 ( [のシナリオ設定パネル [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)) をクリックします。 シナリオでデータが処理されるとすぐに、そのデータはシステムから完全に削除されます。

## インスタントトリガーのスケジュール

シナリオにインスタントトリガーが含まれる場合、シナリオが直ちに実行されるようにスケジュールできます。

![](assets/schedule-setting-350x185.png)

この場合、シナリオは、 [!DNL Workfront Fusion] はサービスから新しいデータを受け取ります。 シナリオの実行後、キュー内で待機中の保留中の Webhook の総数がカウントされ、シナリオは保留中の Webhook の数と同じ数のサイクルを実行し、サイクルごとに 1 つの Webhook を処理します。 詳しくは、 [のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* サイクルは、シナリオ実行とは異なります。 1 回のシナリオ実行で複数のサイクルを実行できます。
>* 即時実行がスケジュールされたインスタントトリガーでシナリオを実行する場合、次の例外が適用されます。
   >
   >     * 2 回の実行間隔は、価格設定計画に従って「最小間隔」に従いません。

      >
      >       例えば、シナリオの実行が完了すると、Webhook のキューが再度チェックされます。 保留中の Web フックがある場合は、シナリオが直ちに再実行され、保留中の Web フックがすべて再度処理されます。
   >   
   >     * 「サイクルの最大数」のシナリオ設定は無視され、100 に設定されます。つまり、1 回のシナリオの実行中に、保留中の Web フックが 100 個以下になります（1 サイクルあたり 1 イベント）。
>



他のスケジュール設定を使用する場合は、 [!UICONTROL 即時]の場合、シナリオは指定した間隔で実行されます。 間隔中に複数の Web フックをキューで収集できるので、 [[!UICONTROL 最大サイクル数]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) をデフォルトの 1 より大きい値に設定すると、1 つのシナリオで複数の Web フックが処理されます。

1. 次をクリック： [!UICONTROL シナリオ設定] アイコン ![](assets/gear-icon-settings.png) をクリックします。
1. 内 **[!UICONTROL シナリオ設定]** 表示されるボックスに、 **[!UICONTROL 最大サイクル数]** ボックスに、シナリオを実行するたびに実行するキュー内の Web フック数を示します。

## レート制限

現在のレート制限は、1 秒あたり 5 ウェブフックです。 制限を超えた場合は、429 ステータスコードが返されます。

## 非アクティブなウェブフックの有効期限

120 時間以上どのシナリオにも割り当てられていない Webhook は削除されます。

## Webhook ペイロード

[!DNL Workfront Fusion] は、30 日間、webhook ペイロードを保存します。 作成後 30 日を超える Webhook ペイロードにアクセスすると、「[!UICONTROL ストレージからファイルを読み取れませんでした。]&quot;

## エラー処理

インスタントトリガーでシナリオにエラーが発生した場合は、次のようになります。

* 直ちに停止 — シナリオが実行されるように設定されている場合 [!UICONTROL 即時].
* 3 回の失敗（3 回のエラー）の後に停止します。シナリオがスケジュールどおりに実行されるように設定されている場合です。

シナリオの実行中にエラーが発生した場合、Webhook は、インスタントトリガーのロールバックフェーズ中にキューに戻されます。 このような状況では、シナリオを修正して再実行することができます。 詳しくは、 [ロールバック](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 記事内 [のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

シナリオに Webhook 応答モジュールがある場合、エラーは Webhook 応答に送信されます。 Webhook の応答モジュールは、常に最後に実行されます ( [!UICONTROL 自動コミット] 」オプションが有効になっていない場合にのみ考慮されます )。 詳しくは、 [Web フックへの応答](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) 記事内 [ウェブフック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## カスタムウェブフック

独自の Web フックを作成できます。 詳しくは、 [ウェブフック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook の無効化

次のいずれかに該当する場合、Webhook は自動的に非アクティブ化されます。

* Webhook は 5 日以上どのシナリオにも接続されていません
* Webhook は、非アクティブなシナリオ（30 日以上非アクティブであったシナリオ）でのみ使用されます。

非アクティブ化された Web フックは、シナリオに接続されておらず、30 日以上非アクティブ状態にある場合、自動的に削除され、登録解除されます。


