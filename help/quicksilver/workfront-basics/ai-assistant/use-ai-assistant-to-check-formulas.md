---
title: AI アシスタントで計算フィールドの数式を修正する
content-type: reference
description: AI アシスタントを使用して、計算フィールドの無効なカスタム式に含まれるエラーを解決できます。
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# AI アシスタントで計算フィールドの数式を修正する

AI アシスタントを使用して、計算フィールドの無効なカスタム式に含まれるエラーを解決できます。

カスタムフォームビルダーで計算フィールドを作成すると、式が無効な場合に、そのフィールドの下にエラーメッセージが表示されます。

![ 無効な式エラー ](assets/invalid-expression.png)

AI アシスタントは、数式を有効な計算フィールド式に修正するのに役立ちます。

## 計算フィールドの式の変更

無効な計算フィールド式を変更するには：

1. 画面の右上隅付近にある **AI アシスタント** アイコン ![AI アシスタント アイコン ](assets/ai-assistant-icon.png) をクリックします。
1. [AI アシスタント ] パネルの下部付近のプロンプト領域で、次のようなプロンプトを入力します。
   `Rewrite this formula to remove the invalid expression error`
1. 無効な式をカスタムフォームビルダーからコピーし、プロンプト領域に貼り付けます。
1. **Enter** キーを押します。

   AI アシスタントは、数式の大きさや複雑さに応じて、修正された数式を生成するのにしばらく時間がかかる場合があります。
1. 改訂された式を AI アシスタント パネルに表示します。
1. （任意）変更した数式を AI アシスタント パネルからコピーし、カスタムフォームビルダーの計算フィールドに貼り付けます。

>[!NOTE]
>
>計算フィールドをテストして、期待される結果が取得されることを確認することをお勧めします。

Workfrontの計算フィールドについて詳しくは、「[ フォームに計算フィールドを追加する ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)」を参照してください。
