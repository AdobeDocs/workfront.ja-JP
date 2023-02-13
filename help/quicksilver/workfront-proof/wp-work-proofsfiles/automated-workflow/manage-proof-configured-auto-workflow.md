---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: の自動ワークフローで設定された配達確認の管理 [!DNL Workfront Proof]
description: 自動ワークフローの配達確認の進行状況は、配達確認の詳細ページの「ワークフロー」セクションで簡単に追跡できます。 各ステージでおこなわれた作業を表示し、配達確認のステージを変更、追加、開始およびロックできます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1d0ad905-f3fb-471a-8766-096b978cdf4e
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# の自動ワークフローで設定された配達確認の管理 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

自動ワークフローの配達確認の進行状況を、 [!UICONTROL 配達確認の詳細] ページ。 各ステージでおこなわれた作業を表示し、配達確認のステージを変更、追加、開始およびロックできます。

## 自動ワークフローの表示

自動ワークフローは、主に次の 3 つの方法で表示できます。

* [ステージの詳細を表示](#view-a-stage-in-detail)
* [すべてのステージを表示](#view-all-stages)
* [すべてのステージの詳細を表示](#view-all-stages-in-detail)

### ステージの詳細を表示 {#view-a-stage-in-detail}

1. セクション (1) の上部にあるボタンをクリックします。

   ダイアグラムを使用して、複数のステージを切り替えることができます。 表示中のステージは、グレー (2) でハイライト表示されます。

1. 別のステージを表示するには、ダイアグラム上で選択します。

![View_a_stage_in_detail.png](assets/view-a-stage-in-detail-350x249.png)

### すべてのステージを表示 {#view-all-stages}

自動ワークフローのすべてのステージを表示するには、次の手順に従います。

1. ページ上部の「 」ボタンをクリックします (3)。

   自動ワークフローのすべてのステージが「 」セクションに表示されますが、詳細は非表示になっています。

1. ステージの詳細を表示するには、各ステージの名前の横にあるプラスアイコン (4) をクリックします。

![View_all_stages.png](assets/view-all-stages-350x212.png)

### すべてのステージの詳細を表示 {#view-all-stages-in-detail}

自動ワークフローのすべてのステージの詳細を表示するには：

1. ページ上部の「 」ボタンをクリックします (5)。

   これにより、自動ワークフローのすべてのステージが表示され、各ステージの詳細が展開されます。

   マイナスアイコン (6) をクリックすると、各ステージの詳細を非表示にできます。

![View_all_stages_in_detail.png](assets/view-all-stages-in-detail-350x370.png)

## 自動ワークフローダイアグラムの使用

自動の図 [!UICONTROL ワークフロー] 「ワークフロー」セクションの上部に表示されます。

ダイアグラムを非表示にするには

1. 次をクリック： **[!UICONTROL を隠す]** ボタン (1)

![図__1_.png](assets/diagram--1--350x217.png)

ダイアグラムのステージは、次のようにマークされます。

![dot.png](assets/dot.png) — アクティブなステージ

![gray_dot.png](assets/grey-dot.png) — 非アクティブなステージ\
![sbw-key-icon.png](assets/sbw-key-icon.png)   — 私的な舞台

![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)   — ロックされたステージ

ステージ間の行は、ステージ間の依存関係を表します。 非アクティブなステージに至る線は、ステージがアクティブになるまで点線で表示されます。

ダイアグラムのステージの上にマウスポインターを置くと、ステージの進行状況が表示されます。 ステージがアクティブでなく、ステージ上で編集権限を持っている場合は、 [!UICONTROL 開始ステージ] 」ボタンをクリックします。 同様に、「アクティブなステージをロック」オプションが表示されます。

プログレスバーについて詳しくは、  [配達確認の進行状況とステータスをで表示 [!DNL Workfront] 配達確認](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

![Diagram_-_stage_summary.png](assets/diagram---stage-summary-350x214.png)

## 新しいステージを追加

自動ワークフローに新しいステージを追加するには、 [!UICONTROL 配達確認の詳細] ページ。

1. 次をクリック： **[!UICONTROL 新しいステージ]** ボタン (1)

![Adding_a_new_stage_1.png](assets/adding-a-new-stage-1-350x218.png)

内 **新しいステージ** 表示されるボックスに、ステージの詳細と設定を入力できます。

![Adding_a_new_stage_2.png](assets/adding-a-new-stage-2-350x332.png)

## ステージ設定の管理

ページの詳細で、（編集権限を持っている場合は）各ステージの設定を変更できます。

* ステージ (1) の期限を変更、追加または削除します。
* ステージ (2) をロック — ステージがアクティブな場合、このオプションが表示されます。非アクティブなステージの場合は、「ステージを開始」オプションが表示されます
* インライン編集による設定の変更 (3)
* ステージで必要な決定は 1 つだけ (4)
* ステージのプライバシーの変更 (5)

![Managing_stage_settings.png](assets/managing-stage-settings-350x93.png)

あるステージから別のステージにドラッグするだけで、レビュー担当者をステージ間で移動することもできます。 使用可能なステージが青色でハイライトされ、各ステージのドロップ領域が明確にマークされます。

![Moving_reviewers_between_stages.png](assets/moving-reviewers-between-stages-350x254.png)

## ステージオプション

この [!UICONTROL アクション] 各ステージのメニュー (1) には、次のオプションがあります。

* すべてのメッセージ (2) — ステージ上のすべてのレビュー担当者にリマインダーの E メールを送信できます
* 共有 (3) — ステージに新しいレビュー担当者を追加できます
* ステージを削除 (4) — 配達確認の所有者がそのステージにいる場合は、新しいステージを選択するように求められます。
