---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion のシナリオの概要
description: Adobe Workfront Fusion には、Adobe Workfrontライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] シナリオの概要

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] にはが必要です [!DNL Adobe Workfront Fusion] に加えてライセンス [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] シナリオを [!DNL Workfront Scenario Planner] シナリオ。 詳しくは、 [!DNL Workfront Scenario Planner] シナリオ， 「 [この [!DNL Scenario Planner] 概要](../../scenario-planner/scenario-planner-overview.md).

の役割 [!DNL Adobe Workfront Fusion] は、同じタスクを何度も繰り返す代わりに、新しいタスクに集中できるように、プロセスを自動化するためのものです。 アプリやサービス内でアクションをリンクして、データを自動的に転送および変換するシナリオを作成できます。 アプリまたはサービスのデータを監視し、そのデータを処理して目的の結果を提供するシナリオです。

シナリオは、アプリ内でのデータの変換方法や、アプリと Web サービスの間での転送方法を示す一連のモジュールで構成されます。

## 例：内でのプロセスの自動化 [!DNL Adobe Workfront]

>[!NOTE]
>
>この機能は、次のライセンスで使用できます。
>
>* [!UICONTROL [!DNL Workfront Fusion] 自動化作業用]
>* [!UICONTROL [!DNL Workfront Fusion] 作業の自動化と統合]
>


[!DNL Workfront Fusion] では、 [!DNL Workfront]を使用することで、時間を節約し、プロセスを一貫して実行できるようにします。

この例では、シナリオは、指定したフィールドが Task または Issue in の [!DNL Workfront]. トリガーされると、シナリオは関連プロジェクトの情報を取得し、プロジェクトの特定の役割に割り当てられた個人に対してカスタマイズされた更新を作成します。

![](assets/fusion-template-example-350x102.png)

## 例：接続中 [!DNL Workfront] 別のアプリまたは Web サービスへ

>[!NOTE]
>
>この機能は、次のライセンスで使用できます。
>
>* [!UICONTROL [!DNL Workfront Fusion] 作業の自動化と統合]
>


[!DNL Workfront Fusion] は、他のアプリや web サービスに接続することもできます。 他のアプリケーションからのデータへのアクセス、インポート、操作またはエクスポートを行い、Workfrontとの統合や相互の統合をおこなうことができます。 多くのアプリケーションに専用の [!DNL Workfront Fusion] コネクタ。 アクセスするアプリケーション専用のコネクタがない場合は、 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] または [!UICONTROL SOAP] API を介してアプリケーションに接続するモジュール。

この例では、ユーザーが [!DNL Excel] スプレッドシート。 シナリオは、ユーザーが [!DNL Workfront]. そうでない場合、シナリオはでユーザーを作成します。 [!DNL Workfront] を追加して、Workfrontユーザー ID をスプレッドシートに戻します。

![](assets/fusion-integration-example--350x171.png)

専用コネクタの一覧については、 [アプリとそのモジュール](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] は、ほとんどすべての web サービスに接続できます。 を使用するアプリに、専用の [!DNL Workfront Fusion] コネクタを使用すると、次のモジュールを使用して Web サービスに直接接続できます。
>
>* [[!UICONTROL HTTP] モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] モジュール](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] モジュール](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

