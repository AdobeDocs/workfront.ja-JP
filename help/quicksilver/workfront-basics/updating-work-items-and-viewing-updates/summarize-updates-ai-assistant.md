---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: AI アシスタントで更新プログラムの要約を作成する
description: '[ 更新 ] は、AI アシスタントを使用して更新を要約するボタンを含むオブジェクトです。'
author: Becky
feature: Get Started with Workfront
exl-id: d0c26f90-a01b-4226-b6a0-647808f71e08
source-git-commit: cf3d5daa739fa6ab413ee82a9f465441ef61ae6d
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 4%

---

# AI アシスタントで更新プログラムの要約を作成する

Workfrontの AI アシスタントは、更新ストリームのコンテンツを要約できるので、Workfront オブジェクトに関するコメントやディスカッションをすばやく理解できます。

[ コンテンツの要約 ] ボタンを使用して要約を生成するか、AI アシスタントにプロンプトを入力します。

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
   <td><p>更新を表示するオブジェクトに対する表示以上の権限</p>
   </td>
  </tr>

</tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
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
</table>-->

## 前提条件

* Workfront管理者が、組織で AI アシスタントを有効にする必要があります。

  詳しくは、「AI アシスタントの概要」の記事の [AI アシスタントの前提条件 &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) を参照してください。
* Workfront管理者が、アクセスレベルに応じて AI アシスタントを有効にする必要があります。

  詳しくは、[AI アシスタントを有効または無効にする &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) を参照してください。

## [ コメントの要約 ] ボタンを使用して要約する

1. 更新を要約するオブジェクトに移動します。
1. 左側のパネルで **更新** をクリックします。
1. **更新** エリアの上部にある「**コメントの要約** ボタンをクリックします。

   AI アシスタントが開き、更新ストリームに対する過去 7 日間のコメントの概要を確認するプロンプトが表示されます。

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
