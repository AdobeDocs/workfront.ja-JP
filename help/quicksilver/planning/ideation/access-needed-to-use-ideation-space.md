---
title: アイデア創出スペースの使用に必要なアクセス
description: Adobe Workfront Planningでは、キャンペーンを開始する前にアイデアを立案するための機能が追加されました。 AIを活用して、データとインプットを具体的な計画に変換し、Adobeのアイデア創出スペースで空白ページを作成するのではなく、情報にもとづいた出発点を提供します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: cf783443d618874e1241d91895bcc78d78db23df
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 2%
---

# アイデア創出スペースの利用に必要なアクセス

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 これは、**アイデア創出スペース Beta** プログラムの一部としてのみ使用できます。</span>

<span class="preview">詳細については、[Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。</span>


{{planning-important-intro}}

Adobe Workfront Planningでは、キャンペーンを開始する前にアイデアを立案するための機能が追加されました。 AIを活用して、データとインプットを具体的な計画に変換し、Adobeのアイデア創出スペースで空白ページを作成するのではなく、情報にもとづいた出発点を提供します。

ここでは、Workfront Planningからアイデア創出スペースにアクセスするために必要なアクセス権と権限について説明します。

アイデア創出スペースについて詳しくは、[Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。

## 必要な製品


アイデア創出スペースは、単独のプロダクトではなく、Adobe Workfrontプランニングの機能を提供します。

組織がアイデア創出スペースにアクセスでき、アイデア創出スペースにアクセスするタイミングに応じて、次のパッケージにアクセスできる場合は、アイデア創出スペースにアクセスできます。

* Open Betaのリリース中は、次の要件を満たしている必要があります。

  * Workfront計画パッケージを含むAdobe Workfront Workflow パッケージ

* 一般提供リリースの後、次のいずれかを実行できます。

  * Workfront計画パッケージを含むAdobe Workfront Workflow パッケージ
  * スタンドアロン製品としてのAdobe Workfront計画

アイデア創出スペースのリリース段階について詳しくは、[Adobe Workfront計画のアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。

>[!NOTE]
>
>アイデア創出スペースには、Adobe WorkfrontのメインメニューまたはWorkfront計画からのみアクセスできます。 アイデア創出スペースにアクセスするために個別のログインは必要ありません。 Workfrontにログインできる場合は、すぐに利用できます。

<!--
No longer the case: 

Your organization must purchase a package for the following products to access the Ideation space: 

* An Adobe Workfront Workflow package in addition to a Planning package

    Or
    
    An Adobe Workfront Planning purchased as a standalone product. 
* An Adobe GenStudio for Performance Marketing license

    >[!TIP]
    >
    >GenStudio for Performance Marketing is needed to have access to the correct font entitlements. 

-->

<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Workfront Planningのアクセスレベル要件

アイデア創出スペースへのアクセスはWorkfrontで設定されます。

アイデア創出スペースにアクセスするには、Workfrontのアクセスレベルに以下を含める必要があります。

* 標準ワークフローライセンス。プランニングパッケージに加えてワークフローパッケージを購入した場合。
* ワークフローとプランニングパッケージ、またはスタンドアロン製品としてのWorkfront Planningを使用して購入した場合のStandard Planning ライセンス。
* アクセスレベルの「追加の制限を設定」セクションの「アイデア出しスペースを無効にする」設定を選択しない必要があります。<!--***********check the UI for this***********-->

## Workfront Planningの権限要件

各プランニングレコードは、アイデア創出スペース内の1つの概要に接続されています。

アイデア創出スペースの概要の権限は、Workfront Planning レコードの権限から継承されます。<!--not sure if this is right, because now you can share the ideation with others??-->

アイデア創出スペースでレコードを作成または編集するには、レコードを作成するには、Planningのレコードタイプに対する管理権限が必要です。

レコードに対する表示権限を持つプランニングユーザーは、レコードのアイデア創出スペースを表示できます。

次の表は、Workfront Planning レコードの権限とアイデア創出スペースの概要の権限の間の関係を示しています。

| プランニングレコードレベルの権限 | アイデア創出スペースの概要レベルの権限 |
|---|---|
| レコードに対する権限の管理 | レコードのアイデア創出スペースにブリーフを作成し |
| レコードへの権限の表示 | アイデア出しスペースでそのレコードの概要を読むことができますが、変更することはできません |

## アイデア創出スペースの権限

<!--this is also duplicated in the intro of the Share an ideation space article-->

計画権限は、レコードのアイデア創出スペースに転送されます。

さらに、他のユーザーにアイデア創出スペースを使用するための権限を付与し、アイデアを追加することもできます。

次の点に注意してください。

* アイデアの作成者は、常に自分のアイデアに対する編集者の権限を持っています。

* ブリーフを作成して他のアプリケーションに書き出すには、アイデア創出スペースに対する編集者権限が必要です。

アイデア創出スペースの権限とその機能は次のとおりです。

| アイデア創出スペースの権限 | 機能 |
|---|---|
| 編集者 | アイデア創出スペースの編集、ダウンロード、共有が可能 |
| コメンター | アイデア創出スペースの表示とコメントを行えます |
| ビューア | アイデア創出スペースを表示できます |

アイデア創出スペースの共有について詳しくは、[ アイデア創出スペースの共有](/help/quicksilver/planning/ideation/share-the-ideation-space.md)を参照してください。

<!--
there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users
-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
