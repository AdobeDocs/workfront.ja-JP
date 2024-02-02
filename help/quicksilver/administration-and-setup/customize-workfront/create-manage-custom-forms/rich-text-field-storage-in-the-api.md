---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API のリッチテキストフィールドストレージ
description: プロジェクト、イシュー、タスクなどのオブジェクトにリッチテキストが含まれている場合は、Workfront API を通じてパラメーター値として保存されアクセスできます。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '171'
ht-degree: 100%

---

# API のリッチテキストフィールドストレージ

プロジェクト、イシュー、タスクなどのオブジェクトにリッチテキストが含まれている場合は、Workfront API を通じてパラメーター値として保存されアクセスできます。

リッチテキストを含むプロジェクトオブジェクトからテキスト情報を要求するには、フィールド **parameterValues** を使用します。

例えば、単純な HTTP リクエストは次のようになります。

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

このサンプルプロジェクトに、計算フィールド、段落テキスト、rich 1 の 3 つのカスタムフィールドを持つカスタムフォームが含まれているとすると、上記のリクエストは、次のような応答を返します。フィールド「rich 1」はリッチテキストパラメーターフィールドで、テキスト値は「**Hello** *World!*」です。

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

リッチテキスト情報の保存方法と Adobe Workfront API での取得方法について詳しくは、[Adobe Workfront API のリッチテキストフィールド](../../../wf-api/general/rich-text-field-api.md)を参照してください。
