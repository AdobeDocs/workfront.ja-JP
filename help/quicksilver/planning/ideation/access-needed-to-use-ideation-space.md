---
title: アイデア創出スペースの使用に必要なアクセス
description: Adobe Workfront Planningでは、キャンペーンを開始する前にアイデアを立案するための機能が追加されました。 AIを活用して、データとインプットを具体的な計画に変換し、Adobeのアイデア創出スペースで空白ページを作成するのではなく、情報にもとづいた出発点を提供します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 215b8f1bf28e8df2b95c4f0519ffebcbcaa8df16
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 3%
---

# アイデア創出スペースの利用に必要なアクセス

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 これは、**アイデア創出スペース Beta** プログラムの一部としてのみ使用できます。</span>

<span class="preview">詳細については、[Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。</span>


>[!IMPORTANT]
>
>この記事では、Adobe Workfront Planningを持つWorkfrontのお客様のみが使用できる機能について説明します。 会社は、追加のプランニングパッケージを購入する必要があります。
>
>ここで説明する機能は、組織がスタンドアロン製品としてWorkfront Planningを購入した場合は使用できません。
>
>Workfront計画の一般的な詳細については、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

Adobe Workfront Planningでは、キャンペーンを開始する前にアイデアを立案するための機能が追加されました。

Workfrontのアイデア創出スペースでは、WorkfrontのAdobe Enterprise CX Coworkerの会話機能を活用して、データと入力を具体的な計画に変換し、空白ページではなく情報にもとづいた出発点を提供できます。

ここでは、Workfront Planningからアイデア創出スペースにアクセスするために必要なアクセス権と権限について説明します。

アイデア創出スペースについて詳しくは、[Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)を参照してください。

## 必要な製品

<!--section duplicated here: help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md-->

>[!NOTE]
>
>アイデア創出スペースにアクセスするために個別のログインは必要ありません。 Workfront Planningをお持ちの場合は、Workfrontにログインするとすぐに利用できます。
>
>アイデア出しスペースを使用するために必要なアクセスについて詳しくは、「[ アイデア出しスペースを使用するために必要なアクセス ](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md)」を参照してください。

組織が次のアクセス権を持っている場合は、アイデア創出スペースにアクセスできます。

* クラウドプロバイダー：

  * AWS

    AzureおよびGCP プロバイダーはサポートされていません。

* 導入製品：

  * Adobe WorkfrontとWorkfront計画
  * WorkfrontのCX Enterprise Coworker

    >[!IMPORTANT]
    >
    >CX Enterprise Coworkerは現在、ヘルスケアや金融などの機密性の高いデータを扱う企業では利用できません。 これらの企業ではAI アシスタントを利用できますが、Coworkerを導入していないWorkfrontのお客様はアイデア創出スペースを利用できません。

* Adobe パッケージ：

  * Open Beta リリース（2026年11月12日以降）では、次の要件が満たされている必要があります。

    * Workfront計画パッケージを含むAdobe Workfront Workflow パッケージ

  * 一般提供リリース（2027年2月1日を対象）の後、次のいずれかになる可能性があります。

    * Workfront計画パッケージを含むAdobe Workfront Workflow パッケージ
    * スタンドアロン製品としてのAdobe Workfront計画


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

## システムおよびアクセスレベルの要件

アイデア創出スペースへのアクセスは、Workfrontでシステムレベルとアクセスレベルの設定を組み合わせて有効にすることで設定されます。

Workfrontのアイデア創出スペースにアクセスするには、次の設定が必要です。

* セットアップ <!--check the UI because Becky was going to change it-->のシステム環境設定エリアで、同僚とMCPの環境設定を有効にします

  詳しくは、[ システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

  >[!IMPORTANT]
  >
  >CX Enterprise Coworkerは現在、ヘルスケアや金融などの機密性の高いデータを扱う企業では利用できません。
  >
  >AI アシスタントは、これらの組織で利用できます。
  >
  >Coworkerを搭載していないが、AI アシスタントを搭載している可能性があるWorkfrontのお客様は、アイデア創出スペースを利用できません。

* ユーザーのアクセスレベルの「追加制限の設定」セクションで、次の設定の選択を解除します。

  * Workfrontの CX Coworker パネルを無効にする
  * アイディエーションスペースを無効にする

    >[!TIP]
    >
    >Workfront管理者は、アクセスレベルの「アイデア創出スペースを無効にする」設定を選択解除することで、アイデア創出スペースへのアクセスを特定のユーザーに制限できます。
    >
    > システム管理者は常にアイデア創出スペースにアクセスできます。
    >
    >詳しくは、[ カスタムアクセスレベルの作成と変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。



## ライセンス要件

アイデア創出スペースにアクセスするには、Workfrontのアクセスレベルに次のライセンスタイプが含まれている必要があります。

* 標準ワークフローライセンス。プランニングパッケージに加えてワークフローパッケージを購入した場合。
* Standard Planningのライセンスで、次のいずれかを購入した場合：

  * ワークフローとプランニングパッケージ（オープンベータ版）
  * ワークフローとプランニングパッケージ、またはスタンドアロン製品としてのWorkfrontプランニング（一般公開後）。

## Workfront Planningの権限要件

Workfront Planningのアイデア創出スペースを使用する場合、各プランニングレコードは、アイデア創出スペース内の1つの概要に接続されます。

アイデア創出スペースの概要の権限は、Workfront Planning レコードの権限から継承されます。<!--not sure if this is right, because now you can share the ideation with others??-->

アイデア創出スペースでレコードを作成または編集するには、Planningのレコードタイプに対してContribute以上の権限が必要です。

レコードに対する表示権限を持つプランニングユーザーは、レコードのアイデア創出スペースを表示できます。

次の表は、Workfront Planning レコードの権限とアイデア創出スペースの概要の権限の間の関係を示しています。

| プランニングレコードレベルの権限 | アイデア創出スペースの概要レベルの権限 |
|---|---|
| レコードに対するアクセス許可の貢献度を上げる | レコードのアイデア創出スペースにブリーフを作成し |
| レコードへの権限の表示 | アイデア出しスペース内のレコードの概要を読み取ることはできますが、変更することはできません |

## アイデア創出スペースの権限

<!--this is also duplicated in the intro of the Share an ideation space article-->

計画権限は、レコードのアイデア創出スペースに転送されます。

さらに、他のユーザーにアイデア創出スペースを使用するための権限を付与し、アイデアを追加することもできます。

次の点に注意してください。

* アイデア創出ブリーフの作成者は、常に自身のブリーフに対する編集権限を持っています。

* ブリーフを作成してPlanningまたはファイルに書き出すには、アイデア創出スペースに対するエディター権限が必要です。

アイデア創出スペースの権限とその機能は次のとおりです。

| アイデア創出スペースの権限 | 機能 |
|---|---|
| 編集者 | アイデア創出スペースの編集、ダウンロード、共有が可能 |
| コメンター | アイデア出しスペースの表示とコメントができます |
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
