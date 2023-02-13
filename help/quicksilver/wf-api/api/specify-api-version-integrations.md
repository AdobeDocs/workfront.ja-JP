---
content-type: api
navigation-topic: api-navigation-topic
title: 統合での API バージョンの指定
description: 統合での API バージョンの指定
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 統合での API バージョンの指定

すべてのAdobe Workfront URI は、URI の「attask/api」部分の後にある特定のバージョンの API を参照するために必要です。 次の例では、バージョン 7.0 を呼び出します。
`attask/api/v7.0/<objectName>/<objectId>` 現在サポートされているすべての統合がWorkfront API を呼び出していることを確認してください。

## Workfront API のリリースおよび廃止スケジュール

この API の新しいバージョンは、6～8 ヶ月ごとに年 2 回リリースされています。 各バージョンは、リリース日から 3 年間サポートされます。また、バージョンは使用可能であるがサポートされていない、非推奨（廃止予定）の状態の年も追加されます。

Workfront API のリリースケイデンスおよび廃止スケジュールについて詳しくは、 [API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md).

Workfrontは、2017 年 7 月に API のデフォルトバージョンを非推奨（廃止予定）となりました。 つまり、Workfrontは、特定のバージョンの API をデフォルトバージョンに指定しなくなりました。 今後のすべての API URI では、有効にするために API のバージョンを指定する必要があります。

>[!IMPORTANT]
>
> デフォルト API バージョンを使用する統合は、2018 年 7 月 1 日までに、サポートされている特定の API バージョンを呼び出すように更新する必要があります。

## 使用している API バージョンの確認

Workfront API に送信された HTTP リクエストの URI を確認することで、使用している API のバージョンを確認できます。 次の例は、API のバージョン 7 を指定するWorkfrontリクエスト URI を示しています。

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

URI でバージョンが指定されていない場合、次の例に示すように、API のデフォルトバージョンが使用されます。

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> URI で API のバージョンを指定しない統合は、自動的に API のデフォルトバージョンにルーティングされ、2018 年 7 月 1 日以降、機能しなくなります。

## サポートされている API バージョンを使用するための統合の更新

Workfront統合を構築または維持する際に、API バージョンおよび変更される可能性のある他のプロパティ（API キーなど）を動的に更新するメソッドを含める必要があります。

統合をより効率的に更新するために、統合値を記録する際には、次の提案を考慮する必要があります。

* 将来の変更の影響を受ける値を、更新し続けるプロパティファイルに保存します
* プロパティをリアルタイムで管理する Web サービスを作成する
* アプリケーションが読み取れるデータストアにプロパティ値を格納します

このことを念頭に置いてWorkfront統合を設計すると、これらの値が必然的に変更される場合に、大規模な開発作業の必要性が軽減されます。
