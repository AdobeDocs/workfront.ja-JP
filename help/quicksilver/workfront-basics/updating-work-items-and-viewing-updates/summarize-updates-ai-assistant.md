---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: AI アシスタントを使用した更新の要約の作成
description: 更新は、AI アシスタントを使用して更新を要約するボタンを含むオブジェクトの更新です。
author: Becky
feature: Get Started with Workfront
exl-id: d0c26f90-a01b-4226-b6a0-647808f71e08
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 12%

---

# AI アシスタントを使用した更新の要約の作成

WorkfrontのAI アシスタントを使用すると、更新ストリームの内容をまとめて、Workfront オブジェクトに関するコメントや議論をすばやく理解できます。

「コンテンツを要約」ボタンを使用して要約を生成したり、AI アシスタントにプロンプトを入力したりできます。

>[!NOTE]
>
>AI アシスタントの要約の機能は、概要パネルとは異なります。
>
>Workfrontの概要パネルについて詳しくは、[概要](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意のワークフローパッケージ</p>
      </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p>
   </td>
  </tr>

<tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td><p>更新を表示するオブジェクトに対する表示権限</p>
   </td>
  </tr>

</tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>New: Any</p>
       <p>or</p>
       <p>Current: Not available</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>New: Standard</p>
       <p>or</p>
       <p>Current: Not available</p></td>
  </tr> 
 </tbody> 
</table>
-->

## 前提条件

* Workfront管理者は、組織のAI アシスタントを有効にする必要があります。

  詳しくは、「AI アシスタントの概要」の「[AI アシスタントの前提条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)」を参照してください。
* Workfront管理者は、アクセスレベルでAI アシスタントを有効にする必要があります。

  詳しくは、[AI アシスタントの有効化または無効化](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)を参照してください。

## 「コメントを要約」ボタンを使用した要約

1. 更新を要約するオブジェクトに移動します。
1. 左側のパネルで「**更新**」をクリックします。
1. 「**アップデート**」エリアの上部にある「**コメントを要約**」ボタンをクリックします。

   AI アシスタントが開き、更新ストリームに対するコメントの過去7日間の要約を求めるプロンプトが表示されます。

   AI アシスタントは、オブジェクトの大きさや複雑さによっては、概要を生成するのに少し時間がかかることがあります。

1. AI アシスタントパネルでAIの概要を表示します。
1. （オプション）必要な情報が表示されるように、プロンプトを調整します。

   例えば、「コンテンツを要約」プロンプトを調整して、過去7日間ではなく過去14日間のコメントを要約できます。

## AI アシスタントでのオブジェクトの要約

オブジェクトの概要を表示するには：

1. 概要を表示するオブジェクトに移動します。
1. 画面の右上隅付近にある&#x200B;**AI アシスタント** アイコン ![AI アシスタント アイコン ](assets/ai-assistant-icon.png)をクリックします。
1. AI アシスタントパネルに、次のようなプロンプトを入力します。

   * 3つの文章で要約を入力してください
   * これを要約してください

   AI アシスタントは、オブジェクトの大きさや複雑さによっては、概要を生成するのに少し時間がかかることがあります。

1. AI アシスタントパネルでAIの概要を表示します。
