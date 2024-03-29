---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Workfront内でのオブジェクトの移動
description: 環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 トランザクションオブジェクトを移動する機能はサポートしていません（例外は制限されています）。
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: b44c83314a06592e21ab3c4316e2574b75e85715
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 3%

---

# Workfront環境間でのオブジェクトの移動の概要（環境の昇格）

環境プロモーション機能は、あるWorkfront環境から別の環境にオブジェクトを移動する機能を提供することを目的としています。 例えば、テンプレートを作成し、サンドボックス環境で設定する場合、テストが組織の実際のデータに影響を与えないことを確認できます。 テンプレートの設定とテストが完了したら、実稼動環境に移動して、すぐに使用できる状態にすることができます。

このプロセスを「環境プロモーション」と呼びます。

移動するオブジェクトのパッケージを作成し、そのパッケージを新しい環境にインストールすることで、Workfrontでこのプロセスを実行できます。

* Workfront内でこのプロセスを実行する手順について詳しくは、以下を参照してください。

   * [環境プロモーションパッケージの作成または編集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [環境プロモーションパッケージのインストール](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Workfront API を使用してこのプロセスを実行する手順については、 [オブジェクトの移動間隔： [!DNL Workfront] 環境の使用 [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## 環境の昇格でサポートされるオブジェクト

環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。 トランザクションオブジェクトを移動する機能はサポートしていません（例外は制限されています）。

* [作業オブジェクト](#work-objects)
* [レポートオブジェクト](#reporting-objects)
* [カスタムデータオブジェクト](#custom-data-objects)
* [組織オブジェクト](#organization-objects)
* [その他の設定オブジェクト](#other-configuration-objects)


### 作業オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| Project（PROJ） | プロジェクト<br>タスク<br>割り当て<br>前任者<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キューの定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Template（TMPL） | テンプレート<br>テンプレートタスク<br>テンプレートタスクの割り当て<br>テンプレートタスクの先行タスク<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キューの定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### レポートオブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| レイアウトテンプレート (UITMPL) | レイアウトテンプレート<br>ダッシュボード<br>カレンダー<br>カレンダーセクション<br>外部ページ<br>レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| ダッシュボード (PTLTAB) | ダッシュボード<br>カレンダー<br>カレンダーセクション<br>外部ページ<br>レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| カレンダー (CALEND) | カレンダー<br>カレンダーセクション |
| 外部ページ (EXTSEC) | 外部ページ |
| レポート (PTLSEC) | レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| フィルター (UIFT) | フィルター<br>パラメーター |
| グループ化 (UIGB) | グループ化<br>パラメーター |
| 表示 (UIVW) | 表示<br>パラメーター |

### カスタムデータオブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| Category（CTGY） | カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック<br>グループ化 |
| Parameter（PARAM） | パラメーター<br>パラメーターオプション |
| パラメータグループ (PGRP) | パラメーターグループ |

### 組織オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| グループ（GROUP） | グループ化 <br>サブグループ（最大 5 レベル） *<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Role（ROLE） | 役割 |
| チーム（チーム） | チーム<br>グループ化 |
| 会社 (CMPY) | 会社情報<br>上書き率<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーター <br>カテゴリの表示ロジック<br>グループ化 |
| Portfolio（PORT） | Portfolio<br>プログラム<br>グループ化<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Program（PRGM） | プログラム<br>Portfolio<br>グループ化<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### その他の設定オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモート可能なサブオブジェクト |
| --- | --- |
| 承認プロセス (ARVPRC) | 承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>役割<br>チーム<br>グループ化 |
| スケジュール (SCHED) | スケジュール<br>非稼働日<br>グループ化 |
| マイルストーンパス (MPATH) | マイルストーンのパス<br>マイルストーン |
| タイムシートプロファイル (TSPRO) | タイムシートプロファイル<br>時間タイプ |
| 時間のタイプ (HOURT) | 時間タイプ |
| 費用タイプ (EXPTYP) | 費用タイプ |
| リスクタイプ (RSKTYP) | リスクタイプ |
| リソースプール (RSPL) | リソースプール |

\*現在は利用できません


## 環境の昇格ステータス

環境プロモーションパッケージは、作成され、環境間を移動するための準備が整うたびに、複数のステータスを処理します。 これらのステータスは、Workfront内のパッケージのリスト、またはWorkfront API を使用している場合は API 応答で確認できます。

これらのステータスには、次のものが含まれます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>組み立て</td> 
   <td><p>このステータスは、オブジェクトのアセンブリ中に自動的に割り当てられます。 </p><p>アセンブリとは、パッケージに含めるオブジェクトとサブオブジェクトを識別し、それらのオブジェクトとそのデータをパッケージに追加する自動プロセスを指します。</p><p>このステータスは、顧客が直接設定することはできません。</p></td> 
  </tr> 
  <tr> 
   <td>ドラフト</td> 
   <td><p>このステータスは、アセンブリプロセスの終了時、または空のプロモーションパッケージの作成時に割り当てられます。</p><p>顧客は、プロモーションパッケージをこのステータスに戻すことができます。</p><p>このステータスの場合、どの環境にもプロモーションパッケージをインストールすることはできません。</p></td> 
  </tr> 
  <tr> 
   <td>テスト</td> 
   <td><p>このステータスにより、任意のプレビューまたはカスタム更新サンドボックスにプロモーションパッケージをインストールできます。 このステータスの場合、パッケージを実稼動環境にインストールすることはできません。</p></td> 
  </tr> 
  <tr> 
   <td>アクティブ</td> 
   <td><p>このステータスにより、プロモーションパッケージを実稼動環境を含む任意の環境にインストールできます。</p><p>パッケージのステータスがアクティブに設定されている場合、 <code>publishedAt</code> 日付は、リクエストの現在のタイムスタンプに自動的に設定されます。</p></td> 
  </tr> 
  <tr> 
   <td>無効</td> 
   <td><p>このステータスは、以前使用したプロモーションパッケージを非表示にするために使用されます。このパッケージは、今後どの環境にもインストールされなくなります。</p><p>このステータスのパッケージは、どの環境にもインストールできません。</p><p>パッケージのステータスが DISABLED に設定されている場合、 <code>retiredAt</code> 日付は、リクエストの現在のタイムスタンプに自動的に設定されます。</p><p>このステータスの使用は、<code>DELETE /package</code> エンドポイントを設定する必要があります。このパッケージを使用して作成されたデプロイメントでは、このエンドポイントが取得可能で、インストール履歴が保持されるからです。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>ASSEMBLING ステージに障害が発生すると、プロモーションパッケージは自動的にこのステータスに入ります。</p><p>パッケージを ASSEMBLING ステージに戻すには、抽出プロセスを再びトリガーする必要があります。</p></td> 
  </tr> 
  </tbody> 
</table>


