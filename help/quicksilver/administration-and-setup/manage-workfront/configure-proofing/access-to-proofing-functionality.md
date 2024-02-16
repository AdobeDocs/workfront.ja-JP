---
user-type: administrator
content-type: reference;overview
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Workfront のプルーフ機能へのアクセス
description: ユーザーが使用できるプルーフ機能は、組織が購入した Workfront プランによって異なります。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 30a41ae9-9755-4c7b-9e3b-d4a8b0ad7ee8
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 86%

---

# Workfront のプルーフ機能へのアクセス

ユーザーが使用できるプルーフ機能は、組織が購入した Workfront プランによって異なります。

## Workfront のプルーフ

現在、Workfrontでの校正に関する 3 つのプランオプションがあります。

* **ニューWorkfrontプラン**：新しいWorkfrontプランのすべてのライセンスに対して、校正が自動的に含まれます。
* **現在のWorkfront Pro+プラン**:Pro、Business、Enterprise Workfrontの各プランをご利用の場合は、Work and Plan ライセンスに対する校正が自動的に含まれます。
* **従来のWorkfront Premium プラン**：このオプションは、従来のWorkfrontプラン (Select、Enterprise、Premium) を対象としています。 このプランのライセンスには、プルーフ機能が自動的には含まれません。ユーザープロファイル内の特定のユーザーに、プルーフのアクセス権を付与する必要があります。

  Workfront の管理者は、設定／システム／ライセンスに移動して、インスタンスがどのプランにあるかを確認できます。

### Workfront のプルーフ機能

Workfront でユーザーのプルーフを作成および表示するためのアクセス権の付与と取り消しについて詳しくは、[ユーザーのプルーフアクセスの設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)を参照してください。

* 外部に表示される URL およびドキュメントに対して静的なプルーフまたはインタラクティブなプルーフを生成します。詳しくは、[プルーフの作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md)を参照してください。
* プルーフに自動ワークフローを含めます。詳しくは、[自動ワークフローの概要](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)を参照してください。
* プルーフのアクセスと登録を設定します。詳しくは、[プルーフのアクセスおよび登録の設定の指定](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)を参照してください。
* Workfront でユーザーのプルーフ機能を有効にする際に、カスタムのプルーフ権限プロファイルを割り当てます。詳しくは、[ユーザーのプルーフアクセスの設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)の記事の[ユーザーのプルーフを有効または無効にする（従来のプランのみ）](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md#enabling-and-disabling-proofing-for-a-user)を参照してください。
* プルーフの進捗状況およびステータスをトラックします。詳しくは、[プルーフの進捗状況とステータスの概要](../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md)を参照してください。
* Workfront でプルーフユーザーを作成する際に、この節で説明するように、Workfront Proof 権限プロファイルを設定します。

  これらのプロファイルが影響するのは Workfront Proof の権限のみで、Workfront には影響しません。

* 同じプルーフの 2 つのプルーフまたは 2 つのバージョンを比較します。詳しくは、[プルーフの比較](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md)を参照してください。
* プルーフの承認レポートを作成します。詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
* ドキュメントのバージョンレポート内の各ドキュメントのバージョンで、現在アクティブなプルーフのステージを表示します。ステージの名前は、「アクティブなプルーフステージ」列に表示されます。ドキュメントのバージョンで現在アクティブなステージがない場合、列は空白になります。ビューとレポートで使用可能なフィールドについて詳しくは、[Adobe Workfront の用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。
* 特定のステージに関連付けられているユーザーに対して、自動ワークフローを含むプルーフを表示するタイミングを設定します。詳しくは、[ユーザーの共有設定を指定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md)の記事の[ワークフローのステージアクティビティに基づくプルーフの表示の設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md#configuring-proof-visibility-based-on-workflow-stage-activity)を参照してください。
* Workfront グローバルナビゲーションバーから直接 Workfront Proof にシームレスにアクセスします（追加のログインは不要）。詳しくは、[Adobe Workfront から Workfront Proof にアクセス](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)を参照してください。

<!--
>[!NOTE]
>
>There are some capabilities included in Workfront Proof standalone that are not included in Proofing in Workfront. To learn more, see [Standalone Workfront Proof to Integrated Proofing in Workfront overview](../../../administration-and-setup/manage-workfront/configure-proofing/move-to-proofing-in-workfront.md)
-->
