---
product-area: betas
title: コネクテッドオーガナイゼーション機能を使い始める
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1eaa497ba7e446f7fdf978f369205f309bbe231f
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%
---
# 連続性のある組織に関する基本を学ぶ

>[!IMPORTANT]
>
>コネクテッド組織の機能は現在、クローズドベータ段階にあり、少数の顧客に対してオープンです。
>
>ベータ版は2026年末まで続きます。
>
>ご不明な点は、Adobeのベータプログラムマネージャーにお問い合わせください。

コネクテッドオーガナイゼーション機能により、企業とパートナーの両方がAdobe Workfrontを購入した際に、共同作業をおこなうことができます。

例えば、クライアント企業は、プロバイダー企業に対して、タスクの完了を求めるリクエストを送信できます。

各企業は、独自のユーザー、権限、ワークフローを使用して、独自のWorkfrontインスタンスで作業を続けることができます。

作業オブジェクトは2つのインスタンス間でミラーリングされ、共有に同意したデータのみが同期されます。

その結果、追加のゲストログイン、重複ライセンス、長いメールスレッドがなくても、リクエスト、ステータス、決定の共有ビューを利用できます。

## 今日の複数の組織にまたがるワークフローの概要

両社がWorkfrontに投資した場合、一方が2回払うか、もう一方のシステムに移行することなく、共同で作業できるはずです。

今日、両社が2つの個別のシステムで作業する場合、次のようなワークフローがコラボレーションに含まれる可能性があります。

* リクエストやブリーフは、フォローするのが困難なメールスレッドを経由します。

* ハンドオフは手動で行われ、監査可能性はほとんどありません。

* 他社のシステム内で作業するには、ゲストログイン、追加ライセンス、またはその両方が必要です。

* ファイルの複数のコピーが循環し、誰も真実のソースであるとは確信していません。

* ステータスの追跡は難しいため、アカウントマネージャーは、デッキの構築やアップデートミーティングのスケジュール設定に時間を費やします。

## コネクテッド組織ソリューションの概要

コネクテッド組織の機能を使用する場合、2つの企業は2つの個別のシステムで引き続き作業を行い、そのコラボレーションには次のワークフローの一部が含まれます。

* どちらの組織も、相手のインスタンス内のオブジェクトにアクセスしません。
* クライアント組織からのリクエストなどのオブジェクトが複製され、プロバイダーのインスタンスに公開されます。
* 同期用に設定されたメタデータのみが、2つのコピー間で最新の状態に保たれます。
* 各企業は、そのオブジェクトを超えた独自のユーザー、権限、ワークフローを管理します。

この指針は、作業を完了するために必要な最低限の情報を共有し、その他の情報はすべて機密保持することです。

<table>
<tbody>
<tr class="odd">
<td><strong>共有される内容</strong></td>
<td><strong>非公開の維持</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>概要とリクエスト詳細</p></li>
<li><p>合意された期限とマイルストーン</p></li>
<li><p>コメントをレビュー</p></li>
<li><p>承認の決定</p></li>
<li><p>最終承認アセット</p></li>
</ul></td>
<td><ul>
<li><p>他のクライアントや代理店との関係</p></li>
<li><p>財務、レート、およびクライアントに請求されるもの</p></li>
<li><p>リソースプランニングとキャパシティ</p></li>
<li><p>社内プロジェクトの構造、タスク、共有に選択されていないフィールド</p></li>
</ul></td>
</tr>
</tbody>
</table>

## ベータ版で利用可能な機能

ベータプログラムの最初のフェーズでは、2つのインスタンスを接続して作業を開始できます。

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **機能** | **機能** |
| **接続された組織** | 2つの組織間の2つのWorkfront インスタンスをリンクします。 ベータ版では、Adobeが接続を設定します。 セルフサービスの設定は現在開発中です。 |
| **リクエストフォーム** | クライアント企業がリクエストフォームを作成して公開し、フォームの共有設定からプロバイダー企業と共有します。 |
| **AI支援リクエスト受注** | 依頼者は、AIのフォーム入力機能を使用してプロンプトを入力し、長いフォームに入力する代わりにファイルを添付することができます。 システムはそのコンテンツをフォームフィールドにマッピングし、レビュー用のマッピングを表示します。 依頼者は結果を受け入れ、フォームを送信します。 |
| **要求をミラーリング** | 送信されたリクエストは、カスタムフィールド値を含む読み取り専用コピーとして、プロバイダー会社のリクエスト領域に表示されます。 |
| **プロジェクトへのリクエスト変換** | GenStudioは、リクエストをプロジェクトに変換し、作業を開始するためのポートフォリオ、プログラム、テンプレートを選択します。 プロバイダーのインスタンス内の新しいオブジェクトは、クライアントの元のリクエストにリンクされます。 プロバイダー側の実際の作業の詳細は、リクエスト側の企業には表示されません。 |
| **双方向コメント** | リクエストに対するコメントは双方に表示され、ほぼ即座に到着するので、両者は一箇所で合意に向けて作業することができます。 |
| **リクエストの承認** | 双方が同意すると、プロバイダーはリクエストを受け入れ、クライアントはそれを受け入れたことを確認できます。 |
| **AIが作成したステータスの更新** | 依頼者がコメントでステータスを要求すると、プロバイダーはAI コマンドを使用して、迅速かつ一貫性のあるドラフト返信を生成できます。<br> ドラフトには、リクエストに接続されたオブジェクトからの情報（予定完了日、条件、予定時間など）が含まれます。<br> これは、フィールドごとの書き出しではなく、最も重要な情報の要約です。 担当者は、クライアントに返信を送信する前に、それを確認および編集します。 |

## エンドツーエンドのワークフロー

このセクションでは、この統合に関与する2つの関係者が、それぞれの関連する組織のWorkfront インスタンスが接続された後のワークフローについて説明します。

クライアントとプロバイダーのワークフローを例として使用しています。

### 顧客のワークフロー

クライアントの組織の依頼者として、次の操作を行うことができます。

1. リクエストフォームを作成して公開し、接続されているプロバイダーの組織と共有するように管理者に依頼するか、作成します。

2. 「要求」領域から公開されたフォームを開き、プロンプトを入力してファイルを添付します。

3. コンテンツがフォームフィールドにどのようにマッピングされるかを確認し、承認および送信します。

### プロバイダーのワークフロー

プロバイダーの組織の作業マネージャーとして、次の操作を行います。

1. リクエストを読み取り専用コピーとしてリクエスト領域に受け取ります。

2. 双方が足並みを揃えるまでコメントを通して要求について話し合い、受け入れる。

3. 必要に応じて、ポートフォリオ、プログラム、テンプレートを選択して、リクエストをプロジェクトに変換します。

4. クライアントのリクエストにミラーリングするプロジェクトフィールドを選択します。

5. コメントでステータスに関する質問に答えたり、ステータスのドラフトを生成して更新し、レビューして、リクエストに公開したりできます。 また、クライアントの元のリクエストにも表示されます。

   この時点から、プロバイダー側のリクエストは、クライアントの当初のリクエストのレプリカとして機能するため、コメントと合意されたデータは同期したままになります。

## セキュリティとガバナンス

各組織のデータを保護することは、設計上の重要な要件です。

ベータ版が確立すべきベースラインの1つは、IT部門とセキュリティ部門がインスタンス間の接続を簡単に承認および管理できることです。

コネクテッド組織ワークフローの利点は次のとおりです。

* **クロスインスタンスアクセスなし**: インスタンスにパートナー組織のユーザーは必要ないため、ゲストログインや追加ライセンスはありません。

* **最低限必要な共有**：同期に設定されたデータのみが共有されます。 それ以外はすべて元のインスタンスに残ります。

* **独立したコントロール**：各組織は、独自のユーザー、権限、ワークフローを保持します。

* **チームレベルのスコープ**：リクエストは、既存のWorkfront アクセス制御を使用して、そのクライアントと連携するように設定された代理店チームにのみリーチすることを目的としています。

## ロードマップ見通し

以下のフェーズでは、現在の開発とリリースプランについて説明します。 シーケンスは、ベータ段階で学習した内容に応じて変更される場合があります。 後のフェーズはコミットメントではありません。

<table>
<tbody>
<tr class="odd">
<td><strong>フェーズ</strong></td>
<td><strong>集中力と計画的な能力</strong></td>
<td><strong>ステータス</strong></td>
</tr>
<tr class="even">
<td><strong>フェーズ 1</strong></td>
<td>インスタンスを接続して作業を開始：リクエストフォーム、AIを活用した受け入れ、ミラーリクエスト、プロジェクトコンバージョン、コメント、ステータスの作成。</td>
<td>ベータ版</td>
</tr>
<tr class="odd">
<td><strong>フェーズ 2</strong></td>
<td><ul>
<li><p>Frameと統一されたレビューおよび承認エクスペリエンスを使用したレビューと承認</p></li>
<li><p>関係者が作業する場所にかかわらず、WorkfrontまたはFrameに保留中のレビューが表示されます</p></li>
<li><p>注釈は作業ファイルに関連付けられるので、クリエイティブチームはフィードバックを1か所で確認できます</p></li>
</ul></td>
<td>予定</td>
</tr>
<tr class="even">
<td><strong>フェーズ 3</strong></td>
<td><ul>
<li><p>リクエストに加えた、タスクベースの作業の割り当て</p></li>
<li><p>共有フィールドと非共有フィールドにもとづく、より自動化されたステータス</p></li>
<li><p>ブリーフィング中にメタデータが定義され、最終的に承認されたアセットによって継承される、新しい成果物タイプ</p></li>
<li><p>承認された最終アセットをブランドのAEMに直接配信し、手作業によるメタデータ入力を削減</p></li>
</ul></td>
<td>予定</td>
</tr>
<tr class="odd">
<td><strong>フェーズ 4</strong></td>
<td><ul>
<li><p>パートナー間で共有されるコンテキスト</p></li>
<li><p>レビュー前にAdobe Brand Intelligence <!--by the agency-->を使用しており、アクセスはチームによって制御されています</p></li>
<li><p>コンテクストに基づいた見積もり機能</p></li>
</ul></td>
<td>長期的</td>
</tr>
</tbody>
</table>

## Beta に参加する

ベータ版に参加するには、Adobeのベータプログラムマネージャーにお問い合わせください。

### 参加者に何を求めるか

* 毎週のフィードバックコールに参加してください。

* 1週間に1時間ほどを確保し、自分で実践テストを行います。 電話でのライブワーキングセッションはオプションです。

* 可能な限り、パートナーの両方の視点をミーティングに取り入れる。

* 接続するWorkfront環境を特定し、少数のAdobe エンジニアの管理者アカウントをプロビジョニングして、接続を検証できるようにします。

### 学習したいこと

* オブジェクトをミラーリングし、選択したデータのみを同期することは、適切な共有モデルですか？ それぞれの側面に対して十分な柔軟性を持っているか？

* フェーズの順序付けは正しいか、それとも後の機能がもっと早く来るべきか？

* コラボレーションに欠けているタッチポイントは何か？

* 2つのインスタンス間のフィールドの命名とマッピングはどのように機能しますか？

  現在、フォームとリクエストはクライアントが所有しており、プロバイダーはクライアントのフィールド名を使用して読み取り専用で表示しています。

* 接続を承認および管理するためにIT部門が必要とするものは何ですか？




<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->