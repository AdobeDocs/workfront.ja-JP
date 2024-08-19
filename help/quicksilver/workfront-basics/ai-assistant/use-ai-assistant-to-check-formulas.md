---
title: AI アシスタントで計算フィールドの数式を修正する
content-type: reference
description: AI アシスタントを使用して、計算フィールドの無効なカスタム式に含まれるエラーを解決できます。
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 513d33c653901394f35c342d8dbf89906017fb3f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 14%

---

# AI アシスタントで計算フィールドの数式を生成または変更する

AI アシスタントを使用して、指定したプロンプトに基づいて数式を生成できます。 また、計算フィールドでの無効なカスタム式のエラーを解決することもできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：Prime または Ultimate</p>
       <p>または</p>
       <p>現在：使用できません</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：使用できません</p></td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 計算フィールドの式の生成

## 計算フィールドの式の変更

カスタムフォームビルダーで計算フィールドを作成すると、式が無効な場合に、そのフィールドの下にエラーメッセージが表示されます。

![ 無効な式エラー ](assets/invalid-expression.png)

AI アシスタントは、数式を有効な計算フィールド式に修正するのに役立ちます。

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
