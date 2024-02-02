---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion のシナリオの概要
description: Adobe Workfront Fusion を使用するには、Adobe Workfront ライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: ht
source-wordcount: '395'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] のシナリオの概要

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] には、[!DNL Adobe Workfront license] に加えて [!DNL Adobe Workfront Fusion] ライセンスが必要です。

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] のシナリオと [!DNL Workfront Scenario Planner] のシナリオを混同しないでください。[!DNL Workfront Scenario Planner] のシナリオについては、[ [!DNL Scenario Planner]  の概要](../../scenario-planner/scenario-planner-overview.md)を参照してください。

[!DNL Adobe Workfront Fusion] の役割は、同じタスクを何度も繰り返すのではなく、新しいタスクに集中できるようにプロセスを自動化することです。これは、アプリ内やサービス内、およびそれらの間でアクションをリンクし、データを自動的に転送および変換するシナリオを作成することで機能します。作成するシナリオは、アプリまたはサービス内のデータを監視し、そのデータを処理して必要な結果を提供します。

シナリオは、アプリ内でのデータの変換方法や、アプリと web サービスの間でのデータの転送方法を示す、一連のモジュールで構成されます。

## 例：[!DNL Adobe Workfront] 内でのプロセスの自動化

>[!NOTE]
>
>この機能は、次のライセンスで使用できます。
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation]
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>

[!DNL Workfront Fusion] では、[!DNL Workfront] 内で単純または複雑なワークフローを自動化して時間を節約し、プロセスを一貫して実行することができます。

この例では、指定したフィールドが [!DNL Workfront] のタスクまたはイシューで変更されるとシナリオがトリガーされます。トリガーされると、シナリオは関連プロジェクトの情報を取得し、プロジェクトの特定の役割に割り当てられたユーザーに合わせて更新を作成します。

![](assets/fusion-template-example-350x102.png)

## 例：[!DNL Workfront] を別のアプリまたは Web サービスに接続する

>[!NOTE]
>
>この機能は、次のライセンスで使用できます。
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>

[!DNL Workfront Fusion] は、他のアプリや Web サービスに接続することもできます。他のアプリケーションからデータに対するアクセス、インポート、処理、エクスポートを通じて、Workfront と統合したり、相互に統合したりすることができます。多くのアプリケーションには専用の [!DNL Workfront Fusion] コネクタがあります。アクセスするアプリケーションの専用コネクタがない場合は、[!DNL Workfront Fusion] の [!UICONTROL HTTP] または [!UICONTROL SOAP] モジュールを使用して、その API を介してアプリケーションに接続できます。

この例では、ユーザーが [!DNL Excel] スプレッドシートに追加されるとシナリオがトリガーされます。シナリオでは、ユーザーが [!DNL Workfront] に存在するかどうかが確認されます。存在しない場合は [!DNL Workfront] でユーザーが作成され、その Workfront ユーザー ID がスプレッドシートに追加されます。

![](assets/fusion-integration-example--350x171.png)

専用コネクタのリストについては、[アプリとそのモジュール](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md)を参照してください。

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] は、ほぼすべての Web サービスに接続できます。使用するアプリに専用の [!DNL Workfront Fusion] コネクタがない場合は、次のモジュールを使用して Web サービスに直接接続できます。
>
>* [[!UICONTROL HTTP ]モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP ]モジュール](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON ]モジュール](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
