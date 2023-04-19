---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 現在利用可能なAdobe Workfront Fusion テンプレート
description: 現在、Adobe Workfront Fusion では、次のパブリックテンプレートを使用できます。
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: f0ab9a14fc397b36c5e3dffe07306ebc43e76500
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 現在利用可能なAdobe Workfront Fusion テンプレート

現在、Adobe Workfront Fusion では、次のパブリックテンプレートを使用できます。

チームまたは組織が他のチーム作成テンプレートを使用できる場合があります。

使用可能なテンプレートを表示するには、 **テンプレート** アイコン ![](assets/fusion-template-icon.png) 」をクリックします。

## Workfrontテンプレート

これらのテンプレートは、Workfrontのプロセスとワークフローを自動化します。

### Workfront — 承認済みの問題をプロジェクトに変換する

このテンプレートは、イシューをプロジェクトに変換します。 組織の標準に合わせて変更できます。

### フィールドの変更に基づくカスタマイズされた通知

このテンプレートは、フィールド値の変更などの一意のイベントに基づいて、Workfrontプロジェクトで作業する個人に対してカスタマイズされた更新（および関連する通知）を作成します。 このシナリオは、指定されたフィールドがタスクまたはイシューで変更されたときにWorkfrontを監視します。 発生した場合、シナリオは関連プロジェクトの情報を評価し、プロジェクトの特定の役割に割り当てられた人物に合わせてカスタマイズされた更新を作成します。

### Workfront — プロジェクト名に一括で付加され、規則が適用されます

この一括更新テンプレートは、検索の条件（ポートフォリオ内に含まれる）を満たすすべてのプロジェクトの名前を変更し、標準形式で名前を変更します。

### Workfront — 命名規則を使用してプロジェクト名を変更する

このテンプレートでは、フィルタの条件を満たすすべてのプロジェクトを検索し（ポートフォリオ内に含まれる）、標準の形式で名前を変更します。

### Workfront — ステータスの変更時にベースラインを作成

このテンプレートは、「切り替え」モジュールに記載されたプロジェクトの状態の変更に基づいて、プロジェクトのベースラインをキャプチャし、ログの更新ストリームに更新を作成します。

### Workfront — 週単位のベースライン作成

このテンプレートは、ポートフォリオでフィルタリングされたプロジェクトに関し、毎週月曜日の午前 6 時に、プロジェクトのベースラインをキャプチャし、更新ストリームでログに記録する更新を作成します。

### ポリシー時間で使用されていないプロジェクトテンプレートを検索して通知

月に 1 回、独自のポリシーを使用してプロジェクトテンプレートを確認します。管理が容易なテンプレートで、ポリシーに違反してテンプレートに関する通知が適切なユーザーに送信されます。

## Workfront - Workfront配達確認テンプレート

これらのテンプレートは、WorkfrontとWorkfrontの配達確認を組み合わせたワークフローを自動化します。

### Workfrontの配達確認/Workfront — 配達確認の決定に対するプロジェクトの更新

プロジェクトに直接追加された配達確認に対して決定がおこなわれると、この自動化では、誰が決定したかなど、配達確認の決定に関する情報が収集され、その進行状況が対応するWorkfrontプロジェクトに更新として反映されます。

### Workfrontの配達確認/Workfront — 配達確認の決定のタスクの更新と完了（承認済みの場合）

個々の配達確認が個々のタスクに関連付けられている場合、このシナリオでは、配達確認の承認が決定されると、関連するタスクが閉じます。 承認された場合は、タスクが完了し、プロジェクトが更新されます。

## HTTP - Workfrontテンプレート

これらのテンプレートは、Web サービスから情報を取得し、その情報をWorkfrontに取り込みます。

>[!NOTE]
>
> この節でテンプレートを使用するには、Workfront Fusion for Work Automation and Integration ライセンスが必要です。

### APILayer / Workfront — 日別為替レート更新 (EUR)

このテンプレートでは、設定された時点での為替レートの更新を自動化するシナリオが作成されます。 このシナリオでは、APIlayers.com API からユーロ (EUR) のレートを米ドル (USD) に取り込み、Workfrontのレートを更新します。

## Workfront — アナプランテンプレート

これらのテンプレートは、Workfrontと Anaplan の統合をサポートし、Workfrontの Anaplan の両方で特定の設定がおこなわれることを想定しています。 これらのテンプレートと必要な設定について詳しくは、個々のテンプレートに関する記事を参照してください。

Workfrontと Anaplan の統合について詳しくは、 [Adobe Workfrontとアナプラン](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> この節でテンプレートを使用するには、Workfront Fusion for Work Automation and Integration ライセンスが必要です。

### 支出の最適化ワークフロー

* [送信 [!DNL Adobe Workfront] プロジェクトの更新 [!DNL Anaplan] リスト項目](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [送信 [!DNL Adobe Workfront] ～への費用 [!DNL Anaplan] リスト項目](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [送信 [!DNL Adobe Workfront] の実際の更新時間 [!DNL Anaplan] リスト項目](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### 予算リクエストをリンクするためのワークフロー

* [の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] 予算リクエスト](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] プロジェクト](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### キャンペーンリクエストをリンクするワークフロー

* [の作成 [!DNL Anaplan] リスト項目 [!DNL Adobe Workfront] キャンペーンリクエスト](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [適用： [!DNL Anaplan] 予算配分 [!DNL Adobe Workfront] キャンペーンリクエストまたはキャンペーンプロジェクト](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
