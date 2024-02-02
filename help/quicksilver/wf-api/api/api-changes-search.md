---
filename: api-changes-search
content-type: api
keywords: オブジェクト、ステータス、検索、ベスト、プラクティス、応答
navigation-topic: api-navigation-topic
title: 「コア API の変更：ステータス検索応答」
description: Workfront でのステータスオブジェクトの保存方法の変更。
feature: Workfront API
role: Developer
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: ht
source-wordcount: '441'
ht-degree: 100%

---

# コア API の変更：ステータス検索応答

Workfront のステータスオブジェクトの保存方法が変更されました。これらの変更は、ステータス検索リクエストの実行方法には影響しませんが、グループのステータスの不完全なリストを返すことにより、ステータスオブジェクトの検索を含む API リクエストによって返される応答には影響します。

## ベストプラクティス

グループに対して使用可能なステータスの完全なリストを確実に取得するために、次のリクエストがベストプラクティスと見なされます。

>[!NOTE]
>
>これらのリクエスト構造は、ステータス検索の変更がクラスターに加えられたかどうかに関係なく、すべてのユーザーに推奨されます。

プロジェクトグループのステータスの場合：

>**例：**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

タスクグループのステータスの場合：

>**例：**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

イシューグループのステータスの場合：

>**例：**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

これら 3 つのエンドポイントはすべて、特定のグループの非表示のプロジェクト、タスク、イシューステータスを取得するために、**includeHidden=true** パラメーターを受け入れます。ステータス検索クエリをこれらのベストプラクティスの例の後にモデリングすると、各応答にすべてのグループステータス情報が確実に含まれます。

システムレベルのロックステータス **Custom_1** とロック解除ステータス **Custom_2** を含むタスクグループに対して行われるステータス検索クエリの例を次に示します。

>**例：**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d286d000004fc8f53942de697a868
```

この形式を使用すると、応答に次のすべてが含まれるようになります。

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

## レガシーステータス検索クエリに加えられた変更の理解

レガシーシステムでは、ステータス検索クエリは、クエリに含まれるすべてのグループに対して使用可能なすべてのシステムステータスをコピーします。レガシー応答には、クエリの各グループで使用できるすべてのシステムステータスとグループレベルのステータスが含まれます。

例えば、このクエリは次のとおりです（現在の推奨ベストプラクティスには従いません）。

>**例：**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

レガシーシステムでは次の応答が返されます。この応答には、すべてのオブジェクトステータスが含まれます。

```
{
    "data": [
        {
            "color": "1C68FF",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "New",
            "objCode": "CSTEM",
            "value": "NEW"
        },
        {
            "color": "39FF39",
            "equatesWith": "INP",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "In Progress",
            "objCode": "CSTEM",
            "value": "INP"
        },
        {
            "color": "FF3939",
            "equatesWith": "CPL",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Complete",
            "objCode": "CSTEM",
            "value": "CPL"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_1",
            "objCode": "CSTEM",
            "value": "JET"
        },
        {
            "color": "8BC34A",
            "equatesWith": "NEW",
            "groupID": "602d27640000bb3b779f770d5fb95d6d",
            "label": "Custom_2",
            "objCode": "CSTEM",
            "value": "OGC"
        }
    ]
}
```

ただし、ステータスの保存および使用方法に対する更新に従って、ステータスはグループに対してコピーされず、システムレベルで各グループに継承されます。結果として、検索 API クエリは、特定のグループに直接関連付けられているステータスのみを読み取るので、応答にはシステムロック済みのステータスとロック解除済みのステータスが含まれますが、問題のステータスが追加された後に作成されたグループのみが対象です。

レガシーシステムが更新された後に、更新されたベストプラクティスの方法を使用してステータス検索クエリを実行しないと、不完全なグループステータスのリストが応答で返されます。

レガシーシステムが更新された後に、この古いリクエスト構造が返す例を次に示します。

>**例：**

```
/attask/api/<VERSION>/CSTEM/search?groupID=602d27640000bb3b779f770d5fb95d6d&enumClass=STATUS_TASK
```

この応答には、グループ固有のステータスのみが含まれ、システムレベルで宣言されたステータスは除外されます。

```
{
  "data": [
    {
      "color": "8BC34A",
      "equatesWith": "NEW",
      "groupID": "602d286d000004fc8f53942de697a868",
      "label": "Custom_2",
      "objCode": "CSTEM",
      "value": "MMI"
    }
  ]
}
```
