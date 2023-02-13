---
content-type: api
keywords: API，データ，同期，ジャーナル，エントリ，オブジェクト
navigation-topic: general-api
title: API を使用してプログラムとサービスのデータを同期する
description: API を使用してプログラムとサービスのデータを同期する
author: John
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: e6bad8cbe84d0f116e9679ecaba5178973a2604f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# API を使用したプログラムおよびサービスのデータの同期

API を利用してプログラムやサービスのデータを同期する一般的な方法を次に示します。

## ほぼリアルタイムの更新

Adobe Workfrontは、「イベント購読」（一般的に Web フックとも呼ばれます）を使用して、API を介して、サポートされているオブジェクトやアクションに関するほぼリアルタイムの更新を目的のエンドポイントに送信します。 新しいオブジェクトやアクションに関する更新は 5 秒以内に届くと考えられますが、平均的な更新は約 1 秒で届きます。 サポートされるオブジェクトの種類、サポートされるアクションの種類、技術的な詳細、イベント購読の設定方法の例について詳しくは、 [イベント購読 API](../../wf-api/general/event-subs-api.md) および [イベント購読配信要件](../../wf-api/general/setup-event-sub-endpoint.md).

## 一括更新

バッチ更新を使用すると、Workfrontサーバーに定期的にリクエストを実行して、システムの更新を設定できます。 これをおこなう方法は多数ありますが、通常は、サービスにWorkfront API サーバーにリクエストを送信させ、最後のリクエスト呼び出し以降に作成または変更されたオブジェクトを検索させることです。 潜在的なリクエスト呼び出しと便利なパラメーターについて詳しくは、 [GET動作](../../wf-api/general/api-basics.md#get-behavior) セクション [API の基本](../../wf-api/general/api-basics.md) 記事。

バッチ更新用にサービスを設定する際には、次の点に注意してください。

### 入口日

エントリ日は、ISO 8601 形式で保存されます。 この標準には、日付、時刻、タイムゾーン情報が含まれます。

**例：** ISO 8601 日付フォーマット

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

オブジェクトの作成日と変更日の両方が、それぞれ「entryDate」と「lastUpdateDate」として保存されます。 Workfrontオブジェクト、関連するフィールド、フィールド名について詳しくは、 [API エクスプローラ](../../wf-api/general/api-explorer.md). 特定のWorkfrontオブジェクトの entryDate は変更されません。lastUpdatedDate はオブジェクトが変更されるたびに変更されます。

**例：** GETリクエスト（イシューオブジェクトに対する）、イシューオブジェクトを利用 **lastUpdateDate** フィールドに入力します。 このリクエストを実行すると、指定された日付以降に更新されたすべての問題が返されます。

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v11.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### ジャーナルエントリオブジェクト

オブジェクト上の特定のフィールドに関する変更を取得したい場合は、「ジャーナルエントリ」オブジェクトに対してクエリを実行できます。 Workfront Journal Entry オブジェクトを設定して、特定のオブジェクトフィールドに関する情報を、それらのフィールドが変更されたときに記録することができます。詳しくは、 [システム更新の構成](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) を参照してください。

フィールドをジャーナルエントリオブジェクトの一部としてログに記録するように設定すると、そのフィールドが変更されるたびに対応するジャーナルエントリが作成されます。 その後、次のような API 呼び出しを使用して、ジャーナルエントリオブジェクトに対してクエリを実行できます。

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v11.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>「entryDate」は、変更されたオブジェクト自体を調べるのではなく、変更のジャーナルエントリを調べるために使用されます。
