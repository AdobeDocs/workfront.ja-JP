---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Workfront内でのオブジェクトの環境間での移動
description: 環境プロモーション機能は、設定関連のオブジェクトを環境間で移動する機能を提供することを目的としています。トランザクションオブジェクトを移動する機能はサポートしていません（例外は制限されています）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: bff394325882dae7b447c319db9cad8c196340d3
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 51%

---

# Workfront環境間でのオブジェクトの移動の概要（環境のプロモーション）

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

環境のプロモーション機能を使用すると、オブジェクトをWorkfront環境から別の環境に移動できます。 例えば、テストが組織の実際のデータに影響を与えないことを知りながら、テンプレートを作成してサンドボックス環境で設定できます。 テンプレートを設定およびテストしたら、使用できる状態で実稼動環境に移動できます。

これを「環境促進」といいます。

Workfrontでこのプロセスを実行するには、移動するオブジェクトのパッケージを作成し、そのパッケージを新しい環境にインストールします。

* Workfrontでこのプロセスを実行する具体的な手順については、以下を参照してください。

   * [環境のプロモーションパッケージの作成または編集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [環境のプロモーションパッケージのインストール](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Workfront API を使用してこのプロセスを実行する手順については、[API を使用した  [!DNL Workfront]  環境間でのオブジェクトの移動  [!DNL Workfront]  を参照してください ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md)。

[この機能のデモビデオを見る](https://video.tv.adobe.com/v/3429735/){target=_blank}

## 環境のプロモーションでサポートされるオブジェクト

環境プロモーション機能の目的は、設定関連オブジェクトを環境間で移動する機能を提供することです。 プロジェクト、チーム、カスタムフォームなど、設定できるオブジェクトです。

環境のプロモーションはオブジェクトの設定を扱うので、トランザクションオブジェクト（頻繁に変更されるオブジェクトや、ユースケースに大きく依存するオブジェクト）は含まれません。 トランザクションオブジェクトの例としては、ドキュメント、イシュー、リクエスト、更新、プルーフ決定などがあります。

* [作業オブジェクト](#work-objects)
* [レポートオブジェクト](#reporting-objects)
* [カスタムデータオブジェクト](#custom-data-objects)
* [組織オブジェクト](#organization-objects)
* [その他の設定オブジェクト](#other-configuration-objects)


### 作業オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモーション可能なリンクオブジェクト |
| --- | --- |
| Project（PROJ） | プロジェクト<br>タスク<br>割り当て<br>前任者<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キュー定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Template（TMPL） | テンプレート<br>テンプレートタスク<br>テンプレートタスクの割り当て<br>テンプレートタスクの先行タスク<br>会社情報<br>上書き率<br>グループ化<br>役割<br>チーム<br>承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>スケジュール<br>非稼働日<br>キューの定義<br>トピックグループをキュー<br>トピックをキュー<br>ルーティングルール<br>マイルストーンのパス<br>マイルストーン<br>時間タイプ<br>リソースプール<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメータグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### レポートオブジェクト

| 昇格可能なオブジェクト | 含まれるプロモーション可能なリンクオブジェクト |
| --- | --- |
| レイアウトテンプレート（UITMPL） | レイアウト テンプレート <br> ダッシュボード <br> カレンダー <br> カレンダーセクション <br> 外部ページ <br> レポート <br> フィルター <br> グループ化 <br> ビュー <br> パラメーター <br> グループ |
| ダッシュボード（PTLTAB） | ダッシュボード<br>カレンダー<br>カレンダーセクション<br>外部ページ<br>レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| カレンダー（CALEND） | カレンダー<br>カレンダーセクション |
| 外部ページ（EXTSEC） | 外部ページ |
| レポート（PTLSEC） | レポート<br>フィルター<br>グループ化<br>表示<br>パラメーター |
| Filter（UIFT） | フィルター<br>パラメーター |
| Grouping（UIGB） | グループ化<br>パラメーター |
| View（UIVW） | ビュー<br>パラメーター |

### カスタムデータオブジェクト

| 昇格可能なオブジェクト | 含まれるプロモーション可能なリンクオブジェクト |
| --- | --- |
| Category（CTGY） | カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック<br>グループ |
| Parameter（PARAM） | パラメーター<br>パラメーターオプション |
| Parameter Group（PGRP） | パラメーターグループ |

### 組織オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモーション可能なリンクオブジェクト |
| --- | --- |
| グループ（GROUP） | グループ<br>サブグループ（最大 5 レベル）*<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Role（ROLE） | 役割 |
| Team（TEAM） | チーム<br>グループ |
| Company（CMPY） | 会社<br>レートの上書き<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーター<br>カテゴリの表示ロジック<br>グループ |
| Portfolio（PORT） | ポートフォリオ<br>プログラム<br>グループ<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |
| Program（PRGM） | プログラム<br>ポートフォリオ<br>グループ<br>カテゴリ<br>カテゴリパラメーター<br>パラメーター<br>パラメーターグループ<br>パラメーターオプション<br>カテゴリの表示ロジック |

### その他の設定オブジェクト

| 昇格可能なオブジェクト | 含まれるプロモーション可能なリンクオブジェクト |
| --- | --- |
| Approval Process（ARVPRC） | 承認プロセス<br>承認パス<br>承認ステップ<br>ステップ承認者<br>役割<br>チーム<br>グループ |
| Schedule（SCHED） | スケジュール<br>非稼働日<br>グループ |
| Milestone Path（MPATH） | マイルストーンパス<br>マイルストーン |
| Timesheet Profile（TSPRO） | タイムシートプロファイル<br>時間タイプ |
| Hour Type（HOURT） | 時間タイプ |
| Expense Type（EXPTYP） | 費用タイプ |
| Risk Type（RSKTYP） | リスクタイプ |
| Resource Pool（RSPL） | リソースプール |
| アクセス レベル （ACSLVL） | アクセスレベル |
| <span class="preview"> 評価カード（RTCRD） </span> | <span class="preview"> 評価カード </span> |

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

## 環境のプロモーションステータス

環境プロモーションパッケージは、環境間を移動するために作成および準備されるいくつかのステータスを経て進行します。 これらのステータスは、Workfront内のパッケージのリストや、Workfront API を使用している場合は API 応答で確認できます。

これらのステータスには、次のものが含まれます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>未組み</td> 
   <td><p>このステータスは自動的に割り当てられ、保存されたが、まだ組み立てられていないパッケージを表します。 </p><p>このステータスは、ユーザーが直接設定することはできません。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>このステータスは、オブジェクトの組み立て中に自動的に割り当てられます。 </p><p>アセンブリとは、パッケージに含めるオブジェクトとサブオブジェクトを識別し、それらのオブジェクトとそのデータをパッケージに追加する自動プロセスを指します。</p><p>このステータスは、ユーザーが直接設定することはできません。</p></td> 
  </tr> 
  <tr> 
   <td>DRAFT</td> 
   <td><p>このステータスは、アセンブリプロセスの終了時、または空のプロモーションパッケージの作成時に割り当てられます。</p><p>ユーザーがプロモーションパッケージをこのステータスに戻す可能性があります。</p><p>このステータスの間は、プロモーションパッケージを環境にインストールすることはできません。</p></td> 
  </tr> 
  <tr> 
   <td>TESTING</td> 
   <td><p>このステータスでは、プロモーションパッケージを任意のプレビューサンドボックスまたはカスタム更新サンドボックスにインストールできます。このステータスの間は、パッケージを実稼動環境にインストールできません。</p></td> 
  </tr> 
  <tr> 
   <td>ACTIVE</td> 
   <td><p>このステータスでは、実稼動環境を含む任意の環境にプロモーションパッケージをインストールできます。</p><p>パッケージのステータスが ACTIVE に設定されている場合、<code>publishedAt</code> の日付はリクエストの現在のタイムスタンプに自動的に設定されます。</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>このステータスは、以前に使用したプロモーションパッケージのうち、今後どの環境にもインストールされないものを非表示にするために使用されます。</p><p>このステータスのパッケージは、任意の環境にインストールできません。</p><p>パッケージのステータスが DISABLED に設定されている場合、<code>retiredAt</code> の日付はリクエストの現在のタイムスタンプに自動的に設定されます。</p><p>このステータスは取得でき、インストール履歴はこのパッケージで作成されたすべてのデプロイメントで保持されるので、<code>DELETE /package</code> エンドポイントを使用する場合よりも使用することをお勧めします。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>ASSEMBLING ステージが失敗すると、プロモーションパッケージは自動的にこのステータスになります。</p><p>パッケージをアセンブリステージに戻すには、アセンブリプロセスを再度トリガーする必要があります。</p><p>パッケージのアセンブリについて詳しくは、環境プロモーションパッケージの作成または編集に関する記事の <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package"> 既存のパッケージの編集またはアセンブリ </a> の節を参照してください。</td> 
  </tr> 
  </tbody> 
</table>

