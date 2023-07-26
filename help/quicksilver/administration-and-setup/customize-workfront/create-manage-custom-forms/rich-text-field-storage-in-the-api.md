---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API のリッチテキストフィールドストレージ
description: プロジェクト、イシュー、タスクなどのオブジェクトにリッチテキストが含まれている場合は、Workfront API を通じてパラメーター値として保存され、アクセスできます。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# API のリッチテキストフィールドストレージ

プロジェクト、イシュー、タスクなどのオブジェクトにリッチテキストが含まれている場合は、Workfront API を通じてパラメーター値として保存され、アクセスできます。

リッチテキストを含むプロジェクトオブジェクトからテキスト情報を要求するには、フィールドを使用します **parameterValues**.

例えば、単純な HTTP リクエストは次のようになります。

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

この例のプロジェクトに、計算フィールド、段落テキスト、リッチ 1 の 3 つのカスタムフィールドを持つカスタムフォームが含まれている場合。 次に、上記のリクエストは、次のような応答を返します。この場合、フィールド「rich 1」はリッチテキストパラメーターフィールドで、テキスト値は「 」です。**こんにちは** *世界！*&quot;:

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

リッチテキスト情報が保存され、Adobe Workfront API で取得できる方法について詳しくは、 [Adobe Workfront API のリッチテキストフィールド](../../../wf-api/general/rich-text-field-api.md).
