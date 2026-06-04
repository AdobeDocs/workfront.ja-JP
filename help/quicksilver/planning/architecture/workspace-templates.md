---
title: ワークスペーステンプレートのリスト
description: ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。 Adobe Workfront Planning には、ワークスペースの作成時に基本的なレコードタイプ、フィールドを使い始められる一連のテンプレートが用意されています。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c4758b87-45dc-4ffd-b086-5e2e907bdf34
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fo6vWjL0XWOPzrBDUC02ES9kgnzmlTGsi050JUfz3zk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 958
ht-degree: 22%

---

# ワークスペーステンプレートのリスト

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースはチームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。

Workfront Planning には、ワークスペースの作成時に基本的なレコードタイプ、フィールドを使い始められる一連のテンプレートが用意されています。 ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

この記事では、Adobe Workfront Plannin で使用できるワークスペーステンプレートについて説明します。

## Adobe Workfront Planning テンプレートに関する考慮事項

* Planning Workspace テンプレートを使用する際に作成するワークスペースの数に応じて、次の種類のテンプレートを使用できます。

   * 単一テンプレート：1つのテンプレートで1つのワークスペースが作成されます。
   * マルチワークスペーステンプレートバンドル：テンプレートバンドルは、相互接続された6つのワークスペースを作成します。
* 各テンプレートには、一連のレコードタイプが用意されています。

  詳しくは、[ レコードタイプの概要](/help/quicksilver/planning/architecture/overview-of-record-types.md)を参照してください。
* 各テンプレートのレコードタイプは、セクションで整理されています。
* レコードタイプには、それぞれに一連のフィールドが用意されています。 これらのフィールドの一部は、他の Workfront Planning レコードタイプとの接続です。
* テンプレートを使用してワークスペースを作成し、作成した後で、テンプレートをカスタマイズしてレコードタイプ、フィールド、レコード、ビューの追加を開始し、他のユーザーと共有できます。
* 各テンプレートのレコードタイプには、サンプルレコードが含まれています。 テンプレートからワークスペースを作成した後に削除できます。
* テンプレートからワークスペースを作成した後、ワークスペースマネージャーはレコードタイプ、フィールド、ビュー、レコードを削除できます。


<!--
 I modeled this article by the "List of available Blueprints" and that articles does not have an Access area

## Access requirements

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--
the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="././administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Planning area in your layout template. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

-->

## 単一のWorkfront計画ワークスペーステンプレート

次に、Workfront Planningのワークスペースのテンプレートと、そのテンプレートに含まれるレコードタイプを示します。

* **Operations Initiative Studio**：統合イニシアチブを計画および実行する方法を示す、完全な、すぐに探索できるOperations イニシアチブモデル（Workfrontの自動SOL リンク）。 イニシアチブからワークストリームへの分類、関連リスク、問題と意思決定、サポートリファレンスリスト（チーム、システム）、タイムライン、テーブル、カレンダーの表示、簡単な労力式が含まれているため、チームはプランニング機能を迅速に学習できます。

  Operations Initiative Studio テンプレートには、次のレコードタイプとそのフィールドが含まれています。

   * イニシアチブ
   * ワークストリーム
   * リスクと課題
   * 決定
   * システム
   * チーム
* **Communications Planning Studio**：通信計画ハブを迅速に設定するためのアイデア。 まず、ロングまたはショートのコミュニケーションプランのテンプレートレコードを複製し、戦術とトラッキング承認チェックポイントを追加してロールアウトを構築します。 オーディエンス、市場、チャネルを参照し、一貫したレポート、フィルタリング、再利用を実現。 サンプルレコードとすぐに使用できるテーブル、タイムライン、カレンダービューが含まれているため、プランニング機能をすぐに確認できます。

  Communications Planning Studio テンプレートには、次のレコードタイプとそのフィールドが含まれます。

   * コミュニケーション
   * オーディエンス
   * 戦術
   * 承認のチェックポイント
   * チャネル
   * 市場
   * 関係者の役割

* **基本：マーケティング管理**：基盤となるマーケティングシステムの基盤を確立する組織に最適です。 テンプレートには、次のレコードタイプと、他のレコードタイプに接続されたフィールドを含むフィールド数が含まれます。

   * Campaign
   * ペルソナ
   * ブランド
   * 製品

* **詳細：マーケティング管理**：より詳細なマーケティング戦略を検討する準備ができているチームに適しています。 テンプレートには、次のレコードタイプと、他のレコードタイプに接続されたフィールドを含むフィールド数が含まれます。

   * キャンペーン
   * プログラム
   * 地域
   * 顧客ジャーニーの段階
   * オーディエンス
   * 配信物
   * ブランド

* **エンタープライズ：マーケティング管理**：複雑なマーケティングシステムを持つ大規模または成熟した組織向けに設計されています。 テンプレートには、次のレコードタイプと、他のレコードタイプに接続されたフィールドを含むフィールド数が含まれます。

   * キャンペーン
   * プログラム
   * 戦術
   * アクティビティ
   * 製品
   * 配信物
   * ターゲットオーディエンス
   * 地域
   * サブ領域
   * パートナー
   * ユースケース
   * 顧客ジャーニーの段階

* セールス管理：営業プロセスを合理化し、効率を高める包括的なセールスシステムを構築できます。 テンプレートには、次のレコードタイプと、他のレコードタイプに接続されたフィールドを含むフィールド数が含まれます。

   * Opportunity
   * アクティビティ
   * Campaign
   * アカウント
   * リード
   * 連絡先
   * 領域
   * 業界
   * 購買センター
   * 製品/サービス
   * 他社製品


* 製品管理：このテンプレートを使用して、効率的で構造化された製品管理プロセスを作成できます。 このテンプレートには、次のレコードタイプと、他のレコードタイプに接続されたフィールドを含むフィールド数が含まれます。

   * テーマ
   * イニシアチブ
   * エピック
   * ユーザーストーリー
   * 顧客
   * スプリント
   * 製品チーム
   * 機能リクエスト
   * 業界

## マルチワークスペース Workfront計画ワークスペーステンプレート

ベストプラクティスのマルチワークスペーステンプレートバンドルを使用して、6つのワークスペースを同時に作成できます。

次の点に注意してください。

* このバンドルでテンプレートを1つだけ選択することはできません。
* 6つのワークスペースをすべて一度に作成する必要があります。使用しないワークスペースは削除できます。

マルチワークスペーステンプレートバンドルには、次のテンプレートと、それぞれのレコードタイプが含まれています。

* 1.**グローバル分類と分類**: Fréscopaのコア共有レコードと分類のエンタープライズガバナンスのハブ。 あらゆるシステムやチームをまたいで、一貫性、整合性、標準化が確保されます。

  >[!NOTE]
  >
  >「フレスコパ」という呼び名は、企業の一般的な例としてのみ使っている。


   * カスタマージャーニー
   * 国
   * チャネル
   * 地域
   * 州、県
   * 言語
   * Platform
   * エクスペリエンスタイプ
   * 年
   * 四半期
   * メッセージ戦略
   * ターゲットオーディエンス
   * ペルソナ
   * 製品
   * ブランド
   * 製品カテゴリ
   * 値
   * ビジョンとミッション
   * 柱
   * 主要業績評価指標

* **2.Fréscopa Global Marketing**: Fréscopaのエンタープライズマーケティング戦略と実行を管理するための一元化されたワークスペース。 キャンペーン、コンテンツ、指標をつなぎ合わせ、ブランドの効果を向上できます。

   * キャンペーン
   * チャネル戦術
   * エクスペリエンス
   * イベント

* **3.Fréscopa Social Marketing**: Fréscopaのソーシャルメディアでのプレゼンスとキャンペーンを管理するための専用ワークスペースです。 ソーシャルメディアのプランニング、公開、パフォーマンスの追跡を一元管理できます。

   * インフルエンサー

* **4.Fréscopa Media &amp; PR**：グローバルなマーケティング目標をサポートする活動をメディア チームとPR チームが調整する場所。

   * レポーター
   * Media Outlets
   * Media Engagements

* **5.Fréscopa Global Events**：すべての地域、国、事業部をまたいでFréscopa イベントを計画および追跡するための一元的な場所。

   * イベントタイプ
   * ワークストリームタイプ
   * スピーカー
   * イベントの場所
   * イベントオーディエンスタイプ

* **6.Fréscopa Executive Company Leadership**：戦略的リーダーが企業の目標や目的などの実用的なデータと連携するための一元化されたワークスペースです。

   * 企業の目標
   * 部署の目的
   * チーム目標
   * 主な成果

