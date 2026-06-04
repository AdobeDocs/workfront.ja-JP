---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: APIでのリッチテキストフィールドストレージ
description: プロジェクト、イシュー、タスクなどのオブジェクトにリッチテキストが含まれている場合は、Workfront API を通じてパラメーター値として保存されアクセスできます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
TQID: https://experienceleague.adobe.com/lLZZugNI5odziqyz7uBMnkiVoOdGcT-jKb90j9TUG1Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 95%

---

# API のリッチテキストフィールドストレージ

プロジェクト、イシュー、タスクなどのオブジェクトにリッチテキストが含まれている場合は、Workfront API を通じてパラメーター値として保存されアクセスできます。

リッチテキストを含むプロジェクトオブジェクトからテキスト情報を要求するには、フィールド **parameterValues** を使用します。

例えば、単純な HTTP リクエストは次のようになります。

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

このサンプルプロジェクトに、計算フィールド、段落テキスト、rich 1 の 3 つのカスタムフィールドを持つカスタムフォームが含まれているとすると、 上記のリクエストは、次のような応答を返します。フィールド「rich 1」はリッチテキストパラメーターフィールドで、テキスト値は「**Hello** *World!*」です。

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
