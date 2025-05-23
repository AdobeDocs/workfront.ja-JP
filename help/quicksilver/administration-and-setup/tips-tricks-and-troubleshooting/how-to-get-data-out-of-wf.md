---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfrontからの履歴データの書き出し：長所と短所
description: この記事では、Workfront からの履歴データの書き出しに使用できる 4 つのオプションの長所と短所について説明します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 39%

---

# [!DNL Adobe Workfront] から履歴データを書き出す：長所と短所

<!-- Audited: 5/2025 -->

この記事では、Adobe Workfrontから履歴データを書き出すために使用できる 4 つのオプションの長所と短所について説明します。

## いずれかのパートナーの利用

[!DNL AtAppStore] （[www.atappstore.com](https://www.atappstore.com)）には、データを自分でダウンロードできる使いやすいアプリ（その [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/) ソリューション）があります。 オプションのビューア（[Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/) ソリューション）を使用すると、データをオフラインで簡単に表示できます。

* **長所：** カスタムフィールドやメモを含むすべてのコア [!DNL Workfront] オブジェクトが書き出され、簡単にアクセスできる [!DNL MS Access] データベースに保存されます。 ビューアのインターフェイスは使いやすく、読みやすくなっています。 ドキュメントの抽出はサービスとして個別に利用することもでき、出力は各ドキュメントとその以前のバージョンにマッピングされる論理フォルダー構造に整理されます。

* **短所：** 2GB のデータには技術的な制限がありますが、AtAppStore では必要なもののみを購入できます。

* **料金：** 詳しくは、[https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/) を参照してください。

## データベースチームへの [!DNL Postgres] データダンプファイルの依頼

お客様は、カスタマーサポートチームにリクエストを送信する必要があります。カスタマーサポートチームは、お客様のデータと共にデータベースダンプファイル（.dmp [!DNL Postgres] ファイル）をエクスポートするよう、データベースチームにリクエストを送信します。 追加のリクエストは、NOC チームに送信され、保存されているすべてのドキュメントを取得します。

* **長所**：カスタムフィールドや、システムに保存されているドキュメントを含め、データロード全体を取得します。

* **短所**：このファイルを読み取るには、ファイルを [!DNL Postgres] データベースにアップロードして、テーブル間の関係を再構築する必要があります。 ドキュメントは別のファイルサーバーに保存され、NOC チームによる別のプロセスを使用して個別に抽出する必要があります。 この場合、ドキュメントは組織化されておらず、すべて GUID で参照されます。

* **コスト**：チームがファイルを作成するのにかかる時間に応じて、このダウンロードに関連するコストがあります。 詳しくは、またはこのプロセスを開始するには、AE または CAE に確認してください。

## [!UICONTROL キックスタート]を使用した書き出し

リモートコンサルティング時間があるかどうかにかかわらず、当社のコンサルタントを利用して、レポートまたは[!UICONTROL キックスタート]の形式でデータを書き出すことも、これらのレポートを自分で実行することもできます。

* **長所**：レポートは読みやすく、様々なアプリケーションで読み込むことができます。 必要に応じて、グループ化やビューを含めるようにカスタマイズできます。

* **短所**：ドキュメントは別途ダウンロードする必要があります。

* **料金**：自分でレポートを実行できる場合（必要なのはシステム管理者ログインのみ）、または残りのリモートコンサルティング時間を使用できる場合は無料です。 これに関するリモートコンサルティングの購入に興味がある場合は、AE または CAE にお問い合わせください。

  キックスタートを使用してデータを書き出す方法について詳しくは、[[!UICONTROL キックスタート]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)を使用した [!DNL Adobe Workfront] からのデータの書き出しを参照してください。

## オープン API の使用

組織に適切なリソースがある場合、ユーザーはカスタム API を作成して、Workfront からすべてのデータを取得できます。

* **長所**：システムからの書き出し内容が管理されています。

* **短所**：ユーザー側の時間が費やされ、API をコーディングし書き出しを実行するためのリソースを探す必要があります。

* **コスト**：組織の内部で発生します。
