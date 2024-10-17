---
title: AI アシスタントを使用して要約する
content-type: reference
description: 「要約」機能を使用すると、作業項目とドキュメントをすばやく要約できます。
author: Becky
feature: Get Started with Workfront
exl-id: b7d4d9a5-cdc5-43a6-a58f-57480f702034
source-git-commit: 59c74b6530df09cb664e146b611d246465cf0116
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 11%

---

# AI アシスタントを使用して要約する

Workfrontの AI アシスタントは、いくつかのオブジェクトをまとめ、オブジェクトの意図や詳細の概要を表示できます。

例えば、AI アシスタントにプロジェクトの要約を依頼すると、プロジェクトの目的とステータスの簡単な説明が返され、完了したタスクとまだ保留中のタスクの例が示され、追加の詳細とメモが提供されます。

AI アシスタントでは、次のオブジェクトをまとめることができます。

* プロジェクト
* タスク
* イシュー
* ドキュメント

>[!NOTE]
>
>AI アシスタントの要約機能は、概要パネルとは異なります。
>
>Workfrontの概要パネルについて詳しくは、[ 概要の概要 ](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md) を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：任意</p>
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

## 前提条件

* Workfront管理者が組織の AI アシスタントを有効にしている必要があります。

  詳しくは、「AI アシスタントの概要」の記事の [AI アシスタントの前提条件 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) を参照してください。
* Workfront管理者が、アクセスレベルに対して AI アシスタントを有効にしている必要があります。

  詳しくは、[AI アシスタントを有効または無効にする ](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

## 要約ボタンを使用した要約

次の領域には、AI アシスタントを使用して要約を生成するボタンがあります。

* プロジェクト ヘッダー：プロジェクトの要約
* [ 更新 ] 領域：コメントの要約

「プロジェクトの要約」または「コメントの要約」ボタンを使用するには、次の手順に従います。

1. ボタンをクリックします。

   AI アシスタントが開き、プロジェクトの概要または更新ストリームに対する過去 7 日間のコメントの概要を確認するプロンプトが表示されます。

   AI アシスタントは、オブジェクトの大きさや複雑さに応じて、概要の生成に数分かかることがあります。

1. AI アシスタント パネルで AI の概要を表示します。
1. （オプション）プロンプトを調整して、必要な情報が提供されるようにします。

   たとえば、Summarize Contents プロンプトを改良して、過去 7 日間ではなく過去 14 日間のコメントを要約することができます。

## AI アシスタントでのオブジェクトの要約

オブジェクトの概要を確認するには：

1. 概要を表示するオブジェクトに移動します。
1. 画面の右上隅付近にある **AI アシスタント** アイコン ![AI アシスタント アイコン ](assets/ai-assistant-icon.png) をクリックします。
1. AI アシスタント パネルで、次のようなプロンプトを入力します。

   * 要約を 3 文で提供する
   * これを要約

   AI アシスタントは、オブジェクトの大きさや複雑さに応じて、概要の生成に数分かかることがあります。

1. AI アシスタント パネルで AI の概要を表示します。

