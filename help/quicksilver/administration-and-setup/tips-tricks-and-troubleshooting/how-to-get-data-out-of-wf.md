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
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 42%

---

# [!DNL Adobe Workfront]から履歴データを書き出す：長所と短所

<!-- Audited: 5/2025 -->

この記事では、Adobe Workfrontから履歴データを書き出すために使用できる4つのオプションの長所と短所について説明します。

## いずれかのパートナーの利用

[!DNL AtAppStore] （[www.atappstore.com](https://www.atappstore.com)）には、自分でデータをダウンロードできる使いやすいアプリ（[Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/) ソリューション）があります。 オプションのビューア（[Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/) ソリューション）を使用すると、データをオフラインで簡単に表示できます。

* **長所：**&#x200B;すべてのコア [!DNL Workfront] オブジェクトが書き出され、カスタムフィールドとメモが含まれ、簡単にアクセスできる[!DNL MS Access] データベースに保存されます。 ビューアのインターフェイスは使いやすく、読みやすいです。 ドキュメントの抽出はサービスとして個別に利用でき、出力は各ドキュメントと以前のバージョンにマッピングされる論理フォルダー構造に整理されます。

* **短所：** 2GBのデータの技術的な制限がありますが、AtAppStoreでは、必要なものだけを購入できます。

* **コスト：**&#x200B;詳しくは、[https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/)にアクセスしてください。



## [!UICONTROL キックスタート]を使用した書き出し

リモートコンサルティング時間があるかどうかにかかわらず、当社のコンサルタントを利用して、レポートまたは[!UICONTROL キックスタート]の形式でデータを書き出すことも、これらのレポートを自分で実行することもできます。

* **長所**: レポートは読みやすく、さまざまなアプリケーションで読み込むことができます。 必要なグループ化やビューを含めるようにカスタマイズできます。

* **短所**：ドキュメントは別途ダウンロードする必要があります。

* **コスト**：自分でレポートを実行できる場合（必要なのはシステム管理者のログインのみ）、または残りのリモートコンサルティング時間を使用できる場合は無料です。 これに関するリモートコンサルティングの購入に興味がある場合は、AE または CAE にお問い合わせください。

  キックスタートを使用してデータを書き出す方法について詳しくは、[[!UICONTROL キックスタート]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)を使用した [!DNL Adobe Workfront] からのデータの書き出しを参照してください。

## オープン API の使用

組織に適切なリソースがある場合、ユーザーはカスタム API を作成して、Workfront からすべてのデータを取得できます。

* **長所**：システムからの書き出し内容が管理されています。

* **短所**：ユーザー側の時間が費やされ、API をコーディングし書き出しを実行するためのリソースを探す必要があります。

* **コスト**：組織の内部です。
