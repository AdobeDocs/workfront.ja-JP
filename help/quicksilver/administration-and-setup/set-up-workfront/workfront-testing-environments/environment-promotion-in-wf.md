---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Workfront内のオブジェクトを別の環境に移動する
description: 環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 トランザクションオブジェクトを移動する機能はサポートしていません（例外は制限されています）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
TQID: https://experienceleague.adobe.com/8rHmgTfG96Ca44EffT6BdyM1YwIkYhgRBu9KEvdbuL8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 943
ht-degree: 41%

---

# Workfront環境間でのオブジェクトの移動の概要（環境プロモーション）

環境プロモーション機能を使用すると、オブジェクトを1つのWorkfront環境から別の環境に移動できます。 例えば、テンプレートを作成し、サンドボックス環境で設定することで、テストを行っても組織の実際のデータには影響しないことが分かります。 テンプレートを設定してテストしたら、本番環境に移動して使用する準備が整います。

この過程を「環境推進」と呼びます。

このプロセスをWorkfrontで実行するには、移動するオブジェクトのパッケージを作成し、そのパッケージを新しい環境にインストールします。

* Workfront内でこのプロセスを実行する具体的な手順については、次を参照してください。

   * [環境のプロモーションパッケージの作成または編集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [環境のプロモーションパッケージのインストール](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Workfront APIを使用してこのプロセスを実行する手順については、 [!DNL Workfront] API[&#128279;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md)を使用して [!DNL Workfront] 環境間でオブジェクトを移動するを参照してください。

[この機能のデモ動画を見る](https://video.tv.adobe.com/v/3429735/){target=_blank}

## 環境のプロモーションでサポートされるオブジェクト

環境プロモーション機能は、構成関連オブジェクトを環境から別の環境に移動する機能を提供することを目的としています。 プロジェクト、チーム、カスタムフォームなど、設定できるオブジェクトです。

環境プロモーションではオブジェクト設定を扱うため、トランザクションオブジェクト（頻繁に変更されるオブジェクトや、ユースケースに大きく依存するオブジェクト）は含まれません。 トランザクションオブジェクトの例には、文書、イシュー、リクエスト、更新、プルーフ決定などがあります。

* [作業オブジェクト](#work-objects)
* [レポートオブジェクト](#reporting-objects)
* [カスタムデータオブジェクト](#custom-data-objects)
* [組織オブジェクト](#organization-objects)
* [その他の設定オブジェクト](#other-configuration-objects)


### 作業オブジェクト

| 昇格可能なオブジェクト | 含まれているプロモート可能なリンクされたオブジェクト |
| --- | --- |
| Project（PROJ） | プロジェクト<br>タスク<br>割り当て<br>前任者<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キュー定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Template（TMPL） | テンプレート<br>テンプレートタスク<br>テンプレートタスクの割り当て<br>テンプレートタスクの先行タスク<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キューの定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### レポートオブジェクト

| 昇格可能なオブジェクト | 含まれているプロモート可能なリンクされたオブジェクト |
| --- | --- |
| レイアウトテンプレート（UITMPL） | レイアウトテンプレート <br> ダッシュボード <br> カレンダー<br> カレンダーセクション <br>外部ページ <br> レポート <br> フィルター<br> グループ化<br> ビュー<br> パラメーター<br> グループ |
| ダッシュボード（PTLTAB） | ダッシュボード<br>カレンダー<br>カレンダーセクション<br>外部ページ<br>レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| カレンダー（CALEND） | カレンダー<br>カレンダーセクション |
| 外部ページ（EXTSEC） | 外部ページ |
| レポート（PTLSEC） | レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| Filter（UIFT） | フィルター<br>パラメーター |
| Grouping（UIGB） | グループ化<br>パラメーター |
| View（UIVW） | ビュー<br>パラメーター |

### カスタムデータオブジェクト

| 昇格可能なオブジェクト | 含まれているプロモート可能なリンクされたオブジェクト |
| --- | --- |
| Category（CTGY） | カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック<br>グループ |
| Parameter（PARAM） | パラメーター<br>パラメーターオプション |
| Parameter Group（PGRP） | パラメーターグループ |

### 組織オブジェクト

| 昇格可能なオブジェクト | 含まれているプロモート可能なリンクされたオブジェクト |
| --- | --- |
| グループ（GROUP） | グループ<br>サブグループ（最大 5 レベル）*<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Role（ROLE） | 役割 |
| Team（TEAM） | チーム<br>グループ |
| Company（CMPY） | 会社<br>レートの上書き<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーター<br>カテゴリの表示ロジック<br>グループ |
| Portfolio（PORT） | ポートフォリオ<br>プログラム<br>グループ<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Program（PRGM） | プログラム<br>ポートフォリオ<br>グループ<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### その他の設定オブジェクト

| 昇格可能なオブジェクト | 含まれているプロモート可能なリンクされたオブジェクト |
| --- | --- |
| Approval Process（ARVPRC） | 承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>役割<br>チーム<br>グループ |
| Schedule（SCHED） | スケジュール<br>非稼働日<br>グループ |
| Milestone Path（MPATH） | マイルストーンパス<br>マイルストーン |
| Timesheet Profile（TSPRO） | タイムシートプロファイル<br>時間タイプ |
| Hour Type（HOURT） | 時間タイプ |
| Expense Type（EXPTYP） | 費用タイプ |
| Risk Type（RSKTYP） | リスクタイプ |
| Resource Pool（RSPL） | リソースプール |
| アクセスレベル （ACSLVL） | アクセスレベル |
| レートカード（RTCRD） | レートカード |
| 場所/分類子（CLSF） | 場所/分類子 |
| ビジネスルール（BSNRUL） | ビジネスルール |

\* 現在は利用できません

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## 環境プロモーションのステータス

環境プロモーションパッケージは、環境間で作成および移動する準備ができたときに、いくつかのステータスを通過します。 Workfront APIを使用している場合は、Workfront内のパッケージのリスト、またはAPI レスポンスで、これらのステータスを確認できます。

これらのステータスには、次のものが含まれます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>未構成</td> 
   <td><p>このステータスは自動的に割り当てられ、保存済みだが、まだ組み立てられていないパッケージを表します。 </p><p>このステータスは、ユーザーが直接設定することはできません。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>このステータスは、オブジェクトの組み立て中に自動的に割り当てられます。 </p><p>アセンブリとは、パッケージに含めるオブジェクトとサブオブジェクトを識別し、それらのオブジェクトとそのデータをパッケージに追加する自動プロセスを指します。</p><p>このステータスは、ユーザーが直接設定することはできません。</p></td> 
  </tr> 
  <tr> 
   <td>DRAFT</td> 
   <td><p>このステータスは、アセンブリプロセスの終了時、または空のプロモーションパッケージの作成時に割り当てられます。</p><p>ユーザーは、プロモーションパッケージをこのステータスに戻すことができます。</p><p>このステータスでは、プロモーションパッケージはどの環境にもインストールできません。</p></td> 
  </tr> 
  <tr> 
   <td>TESTING</td> 
   <td><p>このステータスでは、プロモーションパッケージを任意のプレビューサンドボックスまたはカスタム更新サンドボックスにインストールできます。 このステータスでは、パッケージを実稼動環境にインストールすることはできません。</p></td> 
  </tr> 
  <tr> 
   <td>ACTIVE</td> 
   <td><p>このステータスでは、実稼動環境を含む任意の環境にプロモーションパッケージをインストールできます。</p><p>パッケージのステータスが ACTIVE に設定されている場合、<code>publishedAt</code> の日付はリクエストの現在のタイムスタンプに自動的に設定されます。</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>このステータスは、今後任意の環境にインストールされない、以前に使用したプロモーションパッケージを非表示にするために使用されます。</p><p>このステータスのパッケージは、任意の環境にインストールできません。</p><p>パッケージのステータスが DISABLED に設定されている場合、<code>retiredAt</code> の日付はリクエストの現在のタイムスタンプに自動的に設定されます。</p><p>このステータスは取得可能であり、このパッケージで行われたデプロイメントのインストール履歴が保持されるため、<code>DELETE /package</code> エンドポイントを使用するよりも、このステータスを使用することをお勧めします。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>ASSEMBLING ステージが失敗すると、プロモーションパッケージは自動的にこのステータスになります。</p><p>パッケージをアセンブリステージに戻すには、アセンブリプロセスを再度トリガーする必要があります。</p><p>パッケージのアセンブリについて詳しくは、環境プロモーションパッケージの作成または編集の記事<a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">既存のパッケージの編集またはアセンブリ </a>を参照してください。</td> 
  </tr> 
  </tbody> 
</table>

## リソース

* 環境プロモーションに関するFAQについては、[環境プロモーション FAQ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)を参照してください
* トラブルシューティングの推奨事項については、[環境プロモーションのトラブルシューティング &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)を参照してください


