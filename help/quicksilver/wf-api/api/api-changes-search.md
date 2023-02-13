---
filename: api-changes-search
content-type: api
keywords: オブジェクト，ステータス，検索，ベスト，プラクティス，応答
navigation-topic: api-navigation-topic
title: '''コア API の変更：ステータス検索応答`'
description: Workfrontのステータスオブジェクトの保存方法の変更。
exl-id: 322f1525-d1d5-4845-a590-e34eb94ccdc2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# コア API の変更点は次のとおりです。ステータス検索の応答

Workfrontのステータスオブジェクトの保存方法が変更されました。 これらの変更は、ステータス検索リクエストの実行方法には影響しませんが、グループのステータスの不完全なリストを返すことにより、ステータスオブジェクトの検索を含む API リクエストによって返される応答には影響します。

## ベストプラクティス

グループに対して使用可能なステータスの完全なリストを確実に取得するために、次のリクエストがベストプラクティスと見なされます。

>[!NOTE]
>
>これらのリクエスト構造は、ステータス検索の変更がクラスターに加えられたかどうかに関係なく、すべてのユーザーに推奨されます。

プロジェクトグループのステータス：

>**例:**

```
/attask/api/<VERSION>/CSTEM/projectGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

タスクグループのステータス：

>**例:**

```
/attask/api/<VERSION>/CSTEM/taskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

問題グループのステータスの場合：

>**例:**

```
/attask/api/<VERSION>/CSTEM/opTaskGroupStatuses?groupID=602d27640000bb3b779f770d5fb95d6d
```

これら 3 つのエンドポイントはすべて、 **includeHidden=true** 特定のグループの非表示のプロジェクト/タスク/問題のステータスを取得するためのパラメーター。 ステータス検索クエリをこれらのベストプラクティスの例の後にモデリングすると、各応答にすべてのグループステータス情報が確実に含まれます。

次に、システムレベルのロック済みステータスを含むタスクグループに対して実行されるステータス検索クエリの例を示します **Custom_1** ロック解除済みの状態 **Custom_2**:

>**例:**

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

## 従来のステータス検索クエリに加えられた変更の理解

レガシーシステムでは、ステータス検索クエリは、クエリに含まれるすべてのグループに対して使用可能なすべてのシステムステータスをコピーします。 従来の応答には、クエリの各グループで使用できるすべてのシステムステータスとグループレベルのステータスが含まれます。

例えば、次のクエリを実行します（現在の推奨ベストプラクティスには従いません）。

>**例:**

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

ただし、ステータスの保存および使用方法に対する更新に従って、ステータスはグループに対してコピーされず、システムレベルで各グループに継承されます。 結果として、検索 API クエリは、特定のグループに直接関連付けられているステータスのみを読み取るので、応答にはシステムロック済みのステータスとロック解除済みのステータスが含まれますが、問題のステータスの後に作成されたグループのみが含まれます。

レガシーシステムが更新された後に、更新されたベストプラクティスの方法を使用してステータス検索クエリを実行しないと、不完全なグループステータスのリストが応答で返されます。

レガシーシステムが更新された後に、この古いリクエスト構造が返す例を次に示します。

>**例:**

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
