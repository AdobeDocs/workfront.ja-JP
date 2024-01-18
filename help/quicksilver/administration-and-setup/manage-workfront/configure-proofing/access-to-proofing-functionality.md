---
user-type: administrator
content-type: reference;overview
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Workfrontの校正機能へのアクセス
description: ユーザーが使用できる校正機能は、組織が購入したWorkfrontプランによって異なります。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 30a41ae9-9755-4c7b-9e3b-d4a8b0ad7ee8
source-git-commit: 41a2d58ce00baa6460ee6ca697d4fe06363eee85
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Workfrontの校正機能へのアクセス

ユーザーが使用できる校正機能は、組織が購入したWorkfrontプランによって異なります。

## Workfrontでの校正

現在、Workfrontでの校正に関する 3 つのプランオプションがあります。

* **ニューWorkfrontプラン**：新しいWorkfrontプランのすべてのライセンスに対して、校正が自動的に含まれます。
* **現在のWorkfront Pro+プラン**:Pro、Business、Enterprise Workfrontの各プランをご利用の場合は、Work and Plan ライセンスに対する校正が自動的に含まれます。
* **Workfront Premium レガシープラン**：このオプションは、従来のWorkfrontプラン (Select、Enterprise、Premium) を対象としています。 このプランのライセンスには、校正機能が自動的に含まれていません。 ユーザープロファイル内の特定のユーザーに対して、校正アクセス権を付与する必要があります。

  Workfrontの管理者は、セットアップ/システム/ライセンスに移動して、インスタンスがどのプランにあるかを確認できます。

### Workfrontの校正機能

Workfrontでユーザーの配達確認を作成および表示するためのアクセス権の付与と取り消しについて詳しくは、 [ユーザーの校正アクセスを設定する](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

* 外部に表示される URL およびドキュメントに対して静的な配達確認またはインタラクティブな配達確認を生成します。 詳しくは、 [配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).
* 配達確認に自動ワークフローを含めます。 詳しくは、 [自動ワークフローの概要](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).
* 配達確認のアクセス設定と購読設定を指定します。 詳しくは、 [配達確認のアクセスおよび購読設定を構成する](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md).
* Workfrontでユーザーの校正機能を有効にする際に、カスタム配達確認権限プロファイルを割り当てます。 詳しくは、 [ユーザーの校正を有効または無効にする（レガシープランのみ）](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md#enabling-and-disabling-proofing-for-a-user) in [ユーザーの校正アクセスを設定する](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).
* 配達確認の進行状況およびステータスを追跡します。 詳しくは、 [配達確認の進行状況とステータスの概要](../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).
* Workfront内で校正ユーザーを作成する際に、この節で説明するように、「 Workfront Proof 」権限プロファイルを設定します。

  これらのプロファイルは、Workfrontの配達確認権限でのみ権限に影響し、Workfrontでは影響しません。

* 同じ配達確認の 2 つの配達確認または 2 つのバージョンを比較する。 詳しくは、 [配達確認を比較](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).
* 配達確認の承認レポートを作成します。 詳しくは、  [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* ドキュメントのバージョンレポートで、各ドキュメントのバージョンで現在アクティブな配達確認ステージを表示します。 ステージの名前は、「Active Proof Stages」列に表示されます。 ドキュメントバージョンで現在アクティブなステージがない場合、列は空白になります。 ビューとレポートで使用可能なフィールドについて詳しくは、 [Adobe Workfrontの用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
* 特定のステージに関連付けられているユーザーに対して、自動ワークフローを含む配達確認を表示するタイミングを設定します。 詳しくは、 [ワークフローステージアクティビティに基づく配達確認の表示を設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md#configuring-proof-visibility-based-on-workflow-stage-activity) in  [ユーザーの共有設定を構成します](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).
* Workfrontグローバルナビゲーションバーから直接Workfront Proof にシームレスにアクセス（追加のログインは不要） 詳しくは、 [Adobe WorkfrontからWorkfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

<!--
>[!NOTE]
>
>There are some capabilities included in Workfront Proof standalone that are not included in Proofing in Workfront. To learn more, see [Standalone Workfront Proof to Integrated Proofing in Workfront overview](../../../administration-and-setup/manage-workfront/configure-proofing/move-to-proofing-in-workfront.md)
-->
