---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Adobe Workfrontから履歴データを書き出し：賛否両論'
description: この記事では、Workfrontから履歴データを書き出す 4 つのオプションの長所と短所について説明します。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 次の履歴データを書き出す： [!DNL Adobe Workfron]t:長所と短所

この記事では、履歴データの書き出しに使用できる 4 つのオプションの長所と短所について説明します。 [!DNL Workfront].

## パートナーの 1 人を使用

[!DNL AtAppStore], a [!DNL Workfront] 認定されたパートナーは、使いやすいアプリを使用して、データをダウンロードできます。 また、データを簡単に表示できるビューアも含まれています。

* **長所：** すべての [!DNL Workfront] カスタムフィールドを含むオブジェクトが書き出されます。 Viewer のインターフェイスは、使いやすく、読みやすく、簡単に読み込み可能な [!DNL MS Access] データベース。

* **短所：** ドキュメントは書き出されません。 個別にダウンロードする必要があります。 詳しくは、を参照してください。 [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## リクエスト a [!DNL Postgres] データベースチームからのデータダンプファイル

アカウント担当者は、データベースダンプファイル (.dmp) をエクスポートするリクエストをデータベースチームに送信できます [!DNL Postgres] ファイル ) をデータに置き換えます。 追加の要求が AOS チームに送信され、保存されているすべてのドキュメントが取得されます。

* **長所**:カスタムフィールドや、システムに保存されているドキュメントを含め、データ読み込み全体を取得します。

* **短所**:データベースファイルを読み取るのが困難です：このファイルを読み込むには、 [!DNL Postgres] データベースを作成し、テーブル間のリレーションシップを再確立します。 ドキュメントは、別のファイルサーバーに保存され、AOS チームによる別のプロセスを使用して別々に抽出する必要があります。 この場合、ドキュメントに対する組織はなく、ドキュメントはすべて GUID で参照されます。
* **コスト**:チームがファイルを作成するのにかかる時間に応じて、このダウンロードに関連するコストが発生します。 詳細は AE/CAE にお問い合わせください。また、このプロセスを開始するには、AE/CAE にお問い合わせください。

## 書き出し元 [!UICONTROL キックスタート]

リモートコンサルティング時間があるかどうかにかかわらず、アドビのコンサルタントの 1 人を使用して、データをレポートまたは [!UICONTROL キックスタート]または、次のレポートを自分で実行できます。

* **長所**:レポートは読みやすく、様々なアプリケーションでインポートできます。任意のグループやビューを含めるようにカスタマイズできます。

* **短所**:ドキュメントは別々にダウンロードする必要があります。

* **コスト**:自分でレポートを実行できる場合（システム管理者ログインが必要な場合）、または残りのリモートコンサルティング時間を使用できる場合は、無料です。 このリモートコンサルティングを購入したい場合は、AE/CAE にお問い合わせください。

   Kick-Starts を使用してデータを書き出す方法について詳しくは、 [データのエクスポート元 [!DNL Adobe Workfront] 経由 [!UICONTROL キックスタート]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## オープン API を使用

組織に適切なリソースがある場合、ユーザーはカスタム API を構築して、Workfrontからすべてのデータを取得できます。

* **長所**:システムからの書き出しを制御しています。

* **短所**:この時間はユーザー側で費やされ、API をコーディングして書き出しを実行するためのリソースを見つける必要があります。

* **コスト**:組織の内部。
