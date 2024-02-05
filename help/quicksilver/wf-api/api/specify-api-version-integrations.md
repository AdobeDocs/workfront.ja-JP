---
content-type: api
navigation-topic: api-navigation-topic
title: 統合での API バージョンを指定
description: 統合での API バージョンを指定
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 100%

---

# 統合での API バージョンを指定

すべての Adobe Workfront URI は、URI の「attask/api」部分の後にある特定のバージョンの API を参照する必要があります。次の例では、バージョン 15.0 を呼び出します。

`attask/api/v15.0/<objectName>/<objectId>`

すべての統合が現在サポートされている Workfront API を呼び出すことを確認してください。

## Workfront API のリリースおよび廃止スケジュール

API の新しいバージョンは、通常年に 2 回、定期的にリリースされています。各バージョンは、リリース日から 3 年間サポートされます。また、使用可能であるがサポートされていない、廃止予定の状態のバージョンには、1 年が追加されます。

Workfront API のリリース頻度および廃止スケジュールに関して詳しくは、[API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md)を参照してください。

>[!IMPORTANT]
>
>* API のデフォルトバージョンは、最新バージョンに設定されています。バージョンが指定されていない API 呼び出しでは、デフォルトバージョンが使用されます。Workfront が API の新しいバージョンをリリースするたびに、デフォルトのバージョンが最新バージョンにアップデートされます。**したがって、新しいバージョンの Workfront API がリリースされた後は、すべてのデフォルトバージョンを使用する API 呼び出しをチェックして、機能が引き続きサポートされていることを確認する必要があります。**
>
>* 組織が現在デフォルト API を使用している場合、Workfront 管理者に、デフォルト API に関する詳細な手順を含む、お知らせセンターのメッセージが届いています。
>
>API の最新バージョンについては、[API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md)を参照してください。


## 使用している API バージョンの特定

Workfront API に送信された HTTP リクエストの URI を確認することで、使用している API のバージョンを確認することができます。次の例は、API のバージョン 15 を指定する Workfront リクエスト URI を示しています。

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

URI でバージョンが指定されていない場合、次の例に示すように、API のデフォルトバージョンが使用されています。

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> URI で API のバージョンを指定しない統合は、自動的に API のデフォルトバージョンにルーティングされます。

## サポートされている API バージョンを使用するための統合の更新

Workfront 統合を作成または維持する際に、API バージョンや変更される可能性のある（API キーなどの）他のプロパティを動的にアップデートするメソッドを含める必要があります。

統合をより効率的にアップデートするために、統合値を録画する際には、以下の提案を考慮する必要があります。

* 将来的に変更され得る値を、常にアップデートされるプロパティファイルに保存します
* プロパティをリアルタイムで管理する web サービスを作成
* アプリケーションが読み取れるデータストアに、プロパティ値を格納します

このことを念頭に置いて Workfront 統合を設計すると、これらの値が必然的に変更される場合に、大規模な開発作業の必要性が軽減されます。
