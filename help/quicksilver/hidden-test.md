---
title: 非表示のテストファイル
author: Bob
description: 検索および左のナビゲーションで非表示
hidefromtoc: true
hide: true
exl-id: b6b0f429-b619-4b8e-ab81-ad190dae5a0b
source-git-commit: 1655726151338c47d8f81201db9ef0bb92d9ce9a
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---


# 非表示のテストファイル — 機能分岐テスト

このファイルは検索で非表示 (`hide: yes`) と左側のナビゲーション (`hidefromtoc: yes`) をクリックします。

<span class="preview">このファイルは **非表示** 検索 (`hide: yes`) と左側のナビゲーション (`hidefromtoc: yes`) をクリックします。</span>

<p class="preview">このファイルは検索で**非表示**(「非表示：はい」) と左側のナビゲーション ('hidefromtoc:はい」)。</p>

## 画像テスト

![画像テスト](assets/get-started.png){width="50" align="center"}

## プレビューのハイライトのテスト

**コンポーネントのブロックには DIV を使用します。**

DIV は以下で始まります。

<div class="preview">

DIV の開始。

>[!NOTE]
>
>これはメモです。
>
>メモの背景を強調するリクエストがあります。

![画像](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/assets/add-admin-1.png)

最後にハイライトされた項目。

</div>

DIV は上で終わります。

**段落や語句に SPAN を使用する**

これは段落です。 <span class="preview">私は黄色い文字です。</span> 構文を正しく閉じないでください。閉じないと、ページが異常にレンダリングされる場合があります。

DIV と SPAN は、HTMLテーブルでも便利です。

**その他のサポートされるHTML要素**

また、 `class="preview"` の構文 `<p>`, `<td>`, `<tr>`など。 必ずプレビューでテストしてください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr class="preview"> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a>*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"></td> 
   <td> <p class="preview">計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira アクセス</td> 
   <td> <p><span class="preview">システム管理者のアクセス権</p> <p>重要：ユーザーに付随する可能性のある既存のアカウントを使用するのではなく、Jira とWorkfrontで、この統合専用の個別のシステム管理者アカウントを作成することをお勧めします。 </span></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Workfront管理者である。 Workfront管理者の詳細については、を参照してください。</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

画質= 12 のビデオ

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=12)

画質= 6 のビデオ

>[!VIDEO](https://video.tv.adobe.com/v/3413544/?quality=6)

ビデオのHTML表内

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  </tr> 
  <tr> 
   <td role="rowheader">このビデオは動作しますか？</td> 
   <td>いいえ </td> 
  </tr> 
 </tbody> 
</table>

Markdown テーブル内のビデオ

| 列 1 | 列 2 |
|---|---|
| これは機能しますか？ | また、いいえ |
