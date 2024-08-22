---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「Adobe Workfrontからの履歴データのエクスポート：長所と短所」
description: この記事では、Workfront からの履歴データの書き出しに使用できる 4 つのオプションの長所と短所について説明します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 72%

---

# [!DNL Adobe Workfron]t からの履歴データの書き出し：長所と短所

この記事では、[!DNL Workfront] から履歴データを書き出すために使用できる 4 つのオプションの長所と短所を説明します。

## いずれかのパートナーの利用

[!DNL AtAppStore] （[www.atappstore.com](https://www.atappstore.com)）には、データを自分でダウンロードできる使いやすいアプリ（その [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/) ソリューション）があります。 オプションのビューア（[Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/) ソリューション）を使用すると、データをオフラインで簡単に表示できます。

* **長所：** カスタムフィールドやメモを含むすべてのコア [!DNL Workfront] オブジェクトが書き出され、すべてのオブジェクトは簡単にアクセス可能な [!DNL MS Access] データベースに保存されます。 ビューアのインターフェイスは使いやすく、読みやすいです。 ドキュメントの抽出はサービスとして個別に利用することもでき、出力は各ドキュメント（およびオプションで以前のバージョン）にマッピングされる論理フォルダー構造に整理されます。

* **短所：** 2GB のデータには技術的な制限がありますが、AtAppStore では必要なもののみを購入できます。

* **料金：** 詳しくは、[https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/) を参照してください。

## データベースチームへの [!DNL Postgres] データダンプファイルの依頼

アカウント担当者は、データを含んだデータベースダンプファイル（.dmp [!DNL Postgres] ファイル）の書き出し依頼を当社のデータベースチームに送信できます。保存されているすべてのドキュメントを取得するには、追加の依頼を当社の AOS チームに送信します。

* **長所**：カスタムフィールドや、システムに保存されているドキュメントを含め、データロード全体を取得します。

* **短所**：データベースファイルは読み取りが困難です。このファイルを [!DNL Postgres] データベースにアップロードしてテーブル間の関係を再確立しない限り、読み取ることはできません。ドキュメントは、別のファイルサーバーに保存され、AOS チームによる別のプロセスを使用して別途抽出する必要があります。この場合、ドキュメントは組織化されておらず、すべて GUID で参照されます。

* **コスト**：チームがファイルを作成するのにかかる時間に応じて、このダウンロードに関連するコストが発生します。詳しくは、またはこのプロセスを開始するには、AE または CAE に確認してください。

## [!UICONTROL キックスタート]を使用した書き出し

リモートコンサルティング時間があるかどうかにかかわらず、当社のコンサルタントを利用して、レポートまたは[!UICONTROL キックスタート]の形式でデータを書き出すことも、これらのレポートを自分で実行することもできます。

* **長所**：レポートは読みやすく、様々なアプリケーションに読み込めます。レポートは、任意のグループ化やビューを含めるようにカスタマイズできます。

* **短所**：ドキュメントは別途ダウンロードする必要があります。

* **コスト**：レポートを自分で実行できる場合（システム管理者ログインのみが必要）や、残りのリモートコンサルティング時間を使用できる場合は、無料です。これに関するリモートコンサルティングの購入に興味がある場合は、AE または CAE にお問い合わせください。

  キックスタートを使用してデータを書き出す方法について詳しくは、[[!UICONTROL キックスタート]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)を使用した [!DNL Adobe Workfront] からのデータの書き出しを参照してください。

## オープン API の使用

組織に適切なリソースがある場合、ユーザーはカスタム API を作成して、Workfront からすべてのデータを取得できます。

* **長所**：システムからの書き出し内容が管理されています。

* **短所**：ユーザー側の時間が費やされ、API をコーディングし書き出しを実行するためのリソースを探す必要があります。

* **コスト**：組織内で発生します。
