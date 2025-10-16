---
title: AI アシスタントを使用して要約する
content-type: reference
description: 「要約」機能を使用すると、作業項目とドキュメントをすばやく要約できます。
author: Becky
feature: Get Started with Workfront
exl-id: b7d4d9a5-cdc5-43a6-a58f-57480f702034
source-git-commit: e9a9e45720c8b9ad25e3fa9340c813a73989fb4a
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

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
>Workfrontの概要パネルについて詳しくは、[&#x200B; 概要の概要 &#x200B;](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md) を参照してください。



## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* Workfront管理者が組織の AI アシスタントを有効にしている必要があります。

  詳しくは、「AI アシスタントの概要」の記事の [AI アシスタントの前提条件 &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) を参照してください。
* Workfront管理者が、アクセスレベルに対して AI アシスタントを有効にしている必要があります。

  詳しくは、[AI アシスタントを有効または無効にする &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

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
1. 画面の右上隅付近にある **AI アシスタント** アイコン ![AI アシスタント アイコン &#x200B;](assets/ai-assistant-icon.png) をクリックします。
1. AI アシスタント パネルで、次のようなプロンプトを入力します。

   * 要約を 3 文で提供する
   * これを要約

   AI アシスタントは、オブジェクトの大きさや複雑さに応じて、概要の生成に数分かかることがあります。

1. AI アシスタント パネルで AI の概要を表示します。

