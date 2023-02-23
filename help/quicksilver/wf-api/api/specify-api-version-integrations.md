---
content-type: api
navigation-topic: api-navigation-topic
title: 統合での API バージョンの指定
description: 統合での API バージョンの指定
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 統合での API バージョンの指定

<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、プレビューサンドボックス環境でのみ使用できます。</span>

すべてのAdobe Workfront URI は、URI の「attask/api」部分の後にある特定のバージョンの API を参照するために必要です。 次の例では、バージョン 15.0 を呼び出します。

`attask/api/v15.0/<objectName>/<objectId>`

現在サポートされているすべての統合がWorkfront API を呼び出していることを確認してください。

## Workfront API のリリースおよび廃止スケジュール

この API の新しいバージョンは、通常年に 2 回定期的にリリースされています。 各バージョンは、リリース日から 3 年間サポートされます。また、バージョンは使用可能であるがサポートされていない、非推奨（廃止予定）の状態の年も追加されます。

Workfront API のリリースケイデンスおよび廃止スケジュールについて詳しくは、 [API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* 23.2 リリース以降、API のデフォルトバージョンは最新バージョンに設定されます。 バージョンが指定されていない API 呼び出しでは、デフォルトバージョンが使用されます。 Workfrontが API の新しいバージョンをリリースするたびに、デフォルトのバージョンが最新バージョンに更新されます。 したがって、新しいバージョンのWorkfront API がリリースされた後は、デフォルトバージョンを使用する API 呼び出しをチェックして、機能が引き続きサポートされていることを確認する必要があります。
>
>* お客様の組織が現在デフォルト API を使用している場合、Workfront管理者に、デフォルト API に関する詳細な手順を含むアナウンスセンターのメッセージが届きました。
>
>* <span class="preview">プレビュー環境のデフォルト API は、最新バージョンに設定されています。 実稼動環境のデフォルト API は、23.2 リリース（2023 年 4 月）以降の最新バージョンに設定されます。</span>.
>
>この API の最新バージョンについては、 [API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md).


## 使用している API バージョンの確認

Workfront API に送信された HTTP リクエストの URI を確認することで、使用している API のバージョンを確認できます。 次の例は、API のバージョン 15 を指定するWorkfrontリクエスト URI を示しています。

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

URI でバージョンが指定されていない場合、次の例に示すように、API のデフォルトバージョンが使用されます。

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> URI で API のバージョンを指定しない統合は、自動的に API のデフォルトバージョンにルーティングされます。

## サポートされている API バージョンを使用するための統合の更新

Workfront統合を構築または維持する際に、API バージョンおよび変更される可能性のある他のプロパティ（API キーなど）を動的に更新するメソッドを含める必要があります。

統合をより効率的に更新するために、統合値を記録する際には、次の提案を考慮する必要があります。

* 将来の変更の影響を受ける値を、更新し続けるプロパティファイルに保存します
* プロパティをリアルタイムで管理する Web サービスを作成する
* アプリケーションが読み取れるデータストアにプロパティ値を格納します

このことを念頭に置いてWorkfront統合を設計すると、これらの値が必然的に変更される場合に、大規模な開発作業の必要性が軽減されます。
